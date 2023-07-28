# Comparing `tmp/torch_choice-1.0.3.tar.gz` & `tmp/torch_choice-1.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_choice-1.0.3.tar", last modified: Wed Jul 19 02:36:56 2023, max compression
+gzip compressed data, was "torch_choice-1.0.4a0.tar", last modified: Fri Jul 28 21:53:25 2023, max compression
```

## Comparing `torch_choice-1.0.3.tar` & `torch_choice-1.0.4a0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:36:56.030014 torch_choice-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-19 02:36:41.000000 torch_choice-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15688 2023-07-19 02:36:56.030014 torch_choice-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-07-19 02:36:41.000000 torch_choice-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 02:36:56.030014 torch_choice-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-19 02:36:41.000000 torch_choice-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:36:56.030014 torch_choice-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-19 02:36:41.000000 torch_choice-1.0.3/tests/test_choice_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-19 02:36:41.000000 torch_choice-1.0.3/tests/test_conditional_logit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-07-19 02:36:41.000000 torch_choice-1.0.3/tests/test_nested_logit_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:36:56.030014 torch_choice-1.0.3/torch_choice/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:36:56.030014 torch_choice-1.0.3/torch_choice/data/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23807 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/data/choice_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/data/example_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/data/joint_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:36:56.030014 torch_choice-1.0.3/torch_choice/model/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/model/coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/model/conditional_logit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/model/formula_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23066 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/model/nested_logit_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:36:56.030014 torch_choice-1.0.3/torch_choice/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23594 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/utils/easy_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/utils/run_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/utils/run_helper_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/utils/std.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:36:56.030014 torch_choice-1.0.3/torch_choice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15688 2023-07-19 02:36:56.000000 torch_choice-1.0.3/torch_choice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-19 02:36:56.000000 torch_choice-1.0.3/torch_choice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:36:56.000000 torch_choice-1.0.3/torch_choice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-19 02:36:56.000000 torch_choice-1.0.3/torch_choice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-19 02:36:56.000000 torch_choice-1.0.3/torch_choice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:53:25.125344 torch_choice-1.0.4a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15690 2023-07-28 21:53:25.121344 torch_choice-1.0.4a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 21:53:25.125344 torch_choice-1.0.4a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:53:25.121344 torch_choice-1.0.4a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/tests/test_choice_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/tests/test_conditional_logit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/tests/test_nested_logit_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:53:25.121344 torch_choice-1.0.4a0/torch_choice/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:53:25.121344 torch_choice-1.0.4a0/torch_choice/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23807 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/data/choice_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/data/example_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/data/joint_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:53:25.121344 torch_choice-1.0.4a0/torch_choice/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/model/coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18464 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/model/conditional_logit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/model/formula_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24480 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/model/nested_logit_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:53:25.121344 torch_choice-1.0.4a0/torch_choice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23594 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/utils/easy_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/utils/run_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/utils/run_helper_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-28 21:53:15.000000 torch_choice-1.0.4a0/torch_choice/utils/std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:53:25.121344 torch_choice-1.0.4a0/torch_choice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15690 2023-07-28 21:53:25.000000 torch_choice-1.0.4a0/torch_choice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-28 21:53:25.000000 torch_choice-1.0.4a0/torch_choice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 21:53:25.000000 torch_choice-1.0.4a0/torch_choice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-28 21:53:25.000000 torch_choice-1.0.4a0/torch_choice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 21:53:25.000000 torch_choice-1.0.4a0/torch_choice.egg-info/top_level.txt
```

### Comparing `torch_choice-1.0.3/LICENSE` & `torch_choice-1.0.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.3/PKG-INFO` & `torch_choice-1.0.4a0/torch_choice.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: torch_choice
-Version: 1.0.3
+Name: torch-choice
+Version: 1.0.4a0
 Summary: A Pytorch Backend Library for Choice Modelling
 Home-page: https://gsbdbi.github.io/torch-choice/
 Author: Tianyu Du, Ayush Kanodia, and Susan Athey
 Author-email: tianyudu@stanford.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_choice-1.0.3/README.md` & `torch_choice-1.0.4a0/README.md`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.3/setup.py` & `torch_choice-1.0.4a0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="torch_choice",
-    version="1.0.3",
+    version="1.0.4a",
     description="A Pytorch Backend Library for Choice Modelling",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://gsbdbi.github.io/torch-choice/",
     author="Tianyu Du, Ayush Kanodia, and Susan Athey",
     author_email="tianyudu@stanford.edu",
     license="MIT",
```

### Comparing `torch_choice-1.0.3/tests/test_choice_dataset.py` & `torch_choice-1.0.4a0/tests/test_choice_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.3/tests/test_conditional_logit_model.py` & `torch_choice-1.0.4a0/tests/test_conditional_logit_model.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.3/tests/test_nested_logit_model.py` & `torch_choice-1.0.4a0/tests/test_nested_logit_model.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.3/torch_choice/data/choice_dataset.py` & `torch_choice-1.0.4a0/torch_choice/data/choice_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.3/torch_choice/data/example_datasets.py` & `torch_choice-1.0.4a0/torch_choice/data/example_datasets.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.3/torch_choice/data/joint_dataset.py` & `torch_choice-1.0.4a0/torch_choice/data/joint_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.3/torch_choice/data/utils.py` & `torch_choice-1.0.4a0/torch_choice/data/utils.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.3/torch_choice/model/coefficient.py` & `torch_choice-1.0.4a0/torch_choice/model/coefficient.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 
 class Coefficient(nn.Module):
     def __init__(self,
                  variation: str,
                  num_params: int,
                  num_items: Optional[int]=None,
-                 num_users: Optional[int]=None
+                 num_users: Optional[int]=None,
+                 init: Optional[str]=None
                  ) -> None:
         """A generic coefficient object storing trainable parameters. This class corresponds to those variables typically
         in Greek letters in the model's utility representation.
 
         Args:
             variation (str): the degree of variation of this coefficient. For example, the coefficient can vary by users or items.
                 Currently, we support variations 'constant', 'item', 'item-full', 'user', 'user-item', 'user-item-full'.
@@ -34,55 +35,67 @@
                 an user-specific coefficient called `theta_user`. The coefficient enters the utility form while being multiplied
                 with some K-dimension observables. Then, for each user, there are K parameters to be multiplied with the K-dimensional
                 observable. However, the total number of parameters is K * U (K for each of U users). In this case, `num_params` should
                 be set to `K`, NOT `K*U`.
             num_items (int): the number of items in the prediction problem, this is required to reshape the parameter correctly.
             num_users (Optional[int], optional): number of users, this is only necessary if the coefficient varies by users.
                 Defaults to None.
+            init (Optional[str], optional): the initialization method for the coefficient. Currently, we support zero initialization, standard normal distribution, and uniform distribution. By default, the coefficient is initialized using standard normal distribution.
         """
         super(Coefficient, self).__init__()
         self.variation = variation
         self.num_items = num_items
         self.num_users = num_users
         self.num_params = num_params
+        self.init = init
+        # create initialization function.
+        str_to_init_func = {'zero': torch.zeros,
+                            'uniform': torch.rand,
+                            'normal': torch.randn,
+                            None: torch.randn # default initialization is standard normal distribution.
+                            }
+        if self.init in str_to_init_func:
+            init_func = str_to_init_func[self.init]  # retrieve the initialization function.
+        else:
+            raise ValueError(f"Unsupported initialization method: {self.init}, supported methods are {list(str_to_init_func.keys())}")
 
         # construct the trainable.
         if self.variation == 'constant':
             # constant for all users and items.
-            self.coef = nn.Parameter(torch.randn(num_params), requires_grad=True)
+            self.coef = nn.Parameter(init_func(num_params), requires_grad=True)
         elif self.variation == 'item':
             # coef depends on item j but not on user i.
             # force coefficients for the first item class to be zero.
-            self.coef = nn.Parameter(torch.zeros(num_items - 1, num_params), requires_grad=True)
+            self.coef = nn.Parameter(init_func(num_items - 1, num_params), requires_grad=True)
         elif self.variation == 'item-full':
             # coef depends on item j but not on user i.
             # model coefficient for every item.
-            self.coef = nn.Parameter(torch.zeros(num_items, num_params), requires_grad=True)
+            self.coef = nn.Parameter(init_func(num_items, num_params), requires_grad=True)
         elif self.variation == 'user':
             # coef depends on the user.
             # we always model coefficient for all users.
-            self.coef = nn.Parameter(torch.zeros(num_users, num_params), requires_grad=True)
+            self.coef = nn.Parameter(init_func(num_users, num_params), requires_grad=True)
         elif self.variation == 'user-item':
             # coefficients of the first item is forced to be zero, model coefficients for N - 1 items only.
-            self.coef = nn.Parameter(torch.zeros(num_users, num_items - 1, num_params), requires_grad=True)
+            self.coef = nn.Parameter(init_func(num_users, num_items - 1, num_params), requires_grad=True)
         elif self.variation == 'user-item-full':
             # construct coefficients for every items.
-            self.coef = nn.Parameter(torch.zeros(num_users, num_items, num_params), requires_grad=True)
+            self.coef = nn.Parameter(init_func(num_users, num_items, num_params), requires_grad=True)
         else:
             raise ValueError(f'Unsupported type of variation: {self.variation}.')
 
     def __repr__(self) -> str:
         """Returns a string representation of the coefficient.
 
         Returns:
             str: the string representation of the coefficient.
         """
         return f'Coefficient(variation={self.variation}, num_items={self.num_items},' \
                + f' num_users={self.num_users}, num_params={self.num_params},' \
-               + f' {self.coef.numel()} trainable parameters in total, device={self.device}).'
+               + f" {self.coef.numel()} trainable parameters in total, initialization={self.init if self.init is not None else 'normal'}, device={self.device})."
 
     @property
     def device(self) ->torch.device:
         """Returns the device of the coefficient.
 
         Returns:
             torch.device: the device of the coefficient.
```

### Comparing `torch_choice-1.0.3/torch_choice/model/conditional_logit_model.py` & `torch_choice-1.0.4a0/torch_choice/model/conditional_logit_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Conditional Logit Model.
 
 Author: Tianyu Du
 Update: Apr. 10, 2023
 """
 import warnings
 from copy import deepcopy
-from typing import Dict, Optional
+from typing import Dict, Optional, Union
 
 import torch
 import torch.nn as nn
 
 from torch_choice.data.choice_dataset import ChoiceDataset
 from torch_choice.model.coefficient import Coefficient
 from torch_choice.model.formula_parser import parse_formula
@@ -43,15 +43,16 @@
                  formula: Optional[str]=None,
                  dataset: Optional[ChoiceDataset]=None,
                  coef_variation_dict: Optional[Dict[str, str]]=None,
                  num_param_dict: Optional[Dict[str, int]]=None,
                  num_items: Optional[int]=None,
                  num_users: Optional[int]=None,
                  regularization: Optional[str]=None,
-                 regularization_weight: Optional[float]=None
+                 regularization_weight: Optional[float]=None,
+                 weight_initialization: Optional[Union[str, Dict[str, str]]]=None
                  ) -> None:
         """
         Args:
             formula (str): a string representing the utility formula.
                 The formula consists of '(variable_name|variation)'s separated by '+', for example:
                 "(var1|item) + (var2|user) + (var3|constant)"
                 where the first part of each term is the name of the variable
@@ -96,14 +97,19 @@
                 - 'L2' will subtract regularization_weight * 2-norm of parameters from the log-likelihood.
                 - None does not modify the log-likelihood.
                 Defaults to None.
             regularization_weight (Optional[float]): the weight of parameter norm subtracted from the log-likelihood.
                 This term controls the strength of regularization. This argument is required if and only if regularization
                 is not None.
                 Defaults to None.
+            weight_initialization (Optional[Union[str, Dict[str, str]]]): controls for how coefficients are initialized;
+                users can pass a string from {'normal', 'uniform', 'zero'} to initialize all coefficients in the same way.
+                Alternatively, users can pass a dictionary with keys exactly the same as the `coef_variation_dict` dictionary,
+                and values from {'normal', 'uniform', 'zero'} to initialize coefficients of different types of variables differently.
+                By default, all coefficients are initialized following a standard normal distribution.
         """
         # ==============================================================================================================
         # Check that the model received a valid combination of inputs so that it can be initialized.
         # ==============================================================================================================
         if coef_variation_dict is None and formula is None:
             raise ValueError("Either coef_variation_dict or formula should be provided to specify the model.")
 
@@ -144,15 +150,15 @@
 
         self.coef_variation_dict = deepcopy(coef_variation_dict)
         self.num_param_dict = deepcopy(num_param_dict)
 
         self.num_items = num_items
         self.num_users = num_users
 
-        self.regularization = regularization
+        self.regularization = deepcopy(regularization)
         assert self.regularization in ['L1', 'L2', None], f"Provided regularization={self.regularization} is not allowed, allowed values are ['L1', 'L2', None]."
         self.regularization_weight = regularization_weight
         if (self.regularization is not None) and (self.regularization_weight is None):
             raise ValueError(f'You specified regularization type {self.regularization} without providing regularization_weight.')
         if (self.regularization is None) and (self.regularization_weight is not None):
             raise ValueError(f'You specified no regularization but you provide regularization_weight={self.regularization_weight}, you should leave regularization_weight as None if you do not want to regularize the model.')
 
@@ -162,21 +168,36 @@
 
         # infer the number of parameters for intercept if the researcher forgets.
         for variable in self.coef_variation_dict.keys():
             if self.is_intercept_term(variable) and variable not in self.num_param_dict.keys():
                 warnings.warn(f"`{variable}` key found in coef_variation_dict but not in num_param_dict, num_param_dict['{variable}'] has been set to 1.")
                 self.num_param_dict[variable] = 1
 
+        # inform coefficients their ways of being initialized.
+        self.weight_initialization = deepcopy(weight_initialization)
+
         # construct trainable parameters.
         coef_dict = dict()
         for var_type, variation in self.coef_variation_dict.items():
+            if isinstance(self.weight_initialization, dict):
+                if var_type.split('[')[0] in self.weight_initialization.keys():
+                    # use the variable-specific initialization if provided.
+                    init = self.weight_initialization[var_type.split('[')[0]]
+                else:
+                    # use default initialization.
+                    init = None
+            else:
+                # initialize all coefficients in the same way.
+                init = self.weight_initialization
+
             coef_dict[var_type] = Coefficient(variation=variation,
                                               num_items=self.num_items,
                                               num_users=self.num_users,
-                                              num_params=self.num_param_dict[var_type])
+                                              num_params=self.num_param_dict[var_type],
+                                              init=init)
         # A ModuleDict is required to properly register all trainable parameters.
         # self.parameter() will fail if a python dictionary is used instead.
         self.coef_dict = nn.ModuleDict(coef_dict)
 
     def __repr__(self) -> str:
         """Return a string representation of the model.
```

### Comparing `torch_choice-1.0.3/torch_choice/model/formula_parser.py` & `torch_choice-1.0.4a0/torch_choice/model/formula_parser.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.3/torch_choice/model/nested_logit_model.py` & `torch_choice-1.0.4a0/torch_choice/model/nested_logit_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Implementation of the nested logit model, see page 86 of the book
 "discrete choice methods with simulation" by Train. for more details.
 
 Author: Tianyu Du
 Update; Apr. 7, 2023
 """
-from typing import Dict, List, Optional
+from copy import deepcopy
+from typing import Dict, List, Optional, Union
 
 import torch
 import torch.nn as nn
 
 from torch_choice.data.choice_dataset import ChoiceDataset
 from torch_choice.data.joint_dataset import JointDataset
 from torch_choice.model.coefficient import Coefficient
@@ -27,15 +28,17 @@
                  # method 2: specify formula and dataset.
                  item_formula: Optional[str]=None,
                  nest_formula: Optional[str]=None,
                  dataset: Optional[JointDataset]=None,
                  num_users: Optional[int]=None,
                  shared_lambda: bool=False,
                  regularization: Optional[str]=None,
-                 regularization_weight: Optional[float]=None
+                 regularization_weight: Optional[float]=None,
+                 nest_weight_initialization: Optional[Union[str, Dict[str, str]]]=None,
+                 item_weight_initialization: Optional[Union[str, Dict[str, str]]]=None
                  ) -> None:
         """Initialization method of the nested logit model.
 
         Args:
             nest_to_item (Dict[object, List[int]]): a dictionary maps a nest ID to a list
                 of items IDs of the queried nest.
 
@@ -81,14 +84,17 @@
                 - None does not modify the log-likelihood.
                 Defaults to None.
 
             regularization_weight (Optional[float]): the weight of parameter norm subtracted from the log-likelihood.
                 This term controls the strength of regularization. This argument is required if and only if regularization
                 is not None.
                 Defaults to None.
+
+            {nest, item}_weight_initialization (Optional[Union[str, Dict[str, str]]]): methods to initialize the weights of
+                coefficients for {nest, item} level model. Please refer to the `weight_initialization` keyword in ConditionalLogitModel's documentation for more details.
         """
         # handle nest level model.
         using_formula_to_initiate = (item_formula is not None) and (nest_formula is not None)
         if using_formula_to_initiate:
             # make sure that the research does not specify duplicated information, which might cause conflict.
             if (nest_coef_variation_dict is not None) or (item_coef_variation_dict is not None):
                 raise ValueError('You specify the {item, nest}_formula to initiate the model, you should not specify the {item, nest}_coef_variation_dict at the same time.')
@@ -121,20 +127,22 @@
         self.nests = list(nest_to_item.keys())
         self.num_nests = len(self.nests)
         self.num_items = sum(len(items) for items in nest_to_item.values())
 
         # nest coefficients.
         self.nest_coef_dict = self._build_coef_dict(self.nest_coef_variation_dict,
                                                     self.nest_num_param_dict,
-                                                    self.num_nests)
+                                                    self.num_nests,
+                                                    weight_initialization=deepcopy(nest_weight_initialization))
 
         # item coefficients.
         self.item_coef_dict = self._build_coef_dict(self.item_coef_variation_dict,
                                                     self.item_num_param_dict,
-                                                    self.num_items)
+                                                    self.num_items,
+                                                    weight_initialization=deepcopy(item_weight_initialization))
 
         self.shared_lambda = shared_lambda
         if self.shared_lambda:
             self.lambda_weight = nn.Parameter(torch.ones(1), requires_grad=True)
         else:
             self.lambda_weight = nn.Parameter(torch.ones(self.num_nests) / 2, requires_grad=True)
         # breakpoint()
@@ -160,15 +168,17 @@
             int: the total number of learnable parameters.
         """
         return sum(w.numel() for w in self.parameters())
 
     def _build_coef_dict(self,
                          coef_variation_dict: Dict[str, str],
                          num_param_dict: Dict[str, int],
-                         num_items: int) -> nn.ModuleDict:
+                         num_items: int,
+                         weight_initialization: Optional[Union[str, Dict[str, str]]]=None
+                         ) -> nn.ModuleDict:
         """Builds a coefficient dictionary containing all trainable components of the model, mapping coefficient names
             to the corresponding Coefficient Module.
             num_items could be the actual number of items or the number of nests depends on the use case.
             NOTE: torch-choice users don't directly interact with this method.
 
         Args:
             coef_variation_dict (Dict[str, str]): a dictionary mapping coefficient names (e.g., theta_user) to the level
@@ -180,18 +190,31 @@
 
         Returns:
             nn.ModuleDict: a PyTorch ModuleDict object mapping from coefficient names to training Coefficient.
         """
         coef_dict = dict()
         for var_type, variation in coef_variation_dict.items():
             num_params = num_param_dict[var_type]
+
+            if isinstance(weight_initialization, dict):
+                if var_type.split('[')[0] in weight_initialization.keys():
+                    # use the variable-specific initialization if provided.
+                    init = weight_initialization[var_type.split('[')[0]]
+                else:
+                    # use default initialization.
+                    init = None
+            else:
+                # initialize all coefficients in the same way.
+                init = weight_initialization
+
             coef_dict[var_type] = Coefficient(variation=variation,
                                               num_items=num_items,
                                               num_users=self.num_users,
-                                              num_params=num_params)
+                                              num_params=num_params,
+                                              init=init)
         return nn.ModuleDict(coef_dict)
 
 
     def forward(self, batch: ChoiceDataset) -> torch.Tensor:
         """An standard forward method for the model, the user feeds a ChoiceDataset batch and the model returns the
             predicted log-likelihood tensor. The main forward passing happens in the _forward() method, but we provide
             this wrapper forward() method for a cleaner API, as forward() only requires a single batch argument.
```

### Comparing `torch_choice-1.0.3/torch_choice/utils/easy_data_wrapper.py` & `torch_choice-1.0.4a0/torch_choice/utils/easy_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.3/torch_choice/utils/run_helper.py` & `torch_choice-1.0.4a0/torch_choice/utils/run_helper.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.3/torch_choice/utils/run_helper_lightning.py` & `torch_choice-1.0.4a0/torch_choice/utils/run_helper_lightning.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.3/torch_choice/utils/std.py` & `torch_choice-1.0.4a0/torch_choice/utils/std.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.3/torch_choice.egg-info/PKG-INFO` & `torch_choice-1.0.4a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: torch-choice
-Version: 1.0.3
+Name: torch_choice
+Version: 1.0.4a0
 Summary: A Pytorch Backend Library for Choice Modelling
 Home-page: https://gsbdbi.github.io/torch-choice/
 Author: Tianyu Du, Ayush Kanodia, and Susan Athey
 Author-email: tianyudu@stanford.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_choice-1.0.3/torch_choice.egg-info/SOURCES.txt` & `torch_choice-1.0.4a0/torch_choice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

