# Comparing `tmp/tedeous-0.3.0.tar.gz` & `tmp/tedeous-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tedeous-0.3.0.tar", last modified: Wed Jul 26 10:35:39 2023, max compression
+gzip compressed data, was "tedeous-0.3.1.tar", last modified: Fri Jul 28 14:31:58 2023, max compression
```

## Comparing `tedeous-0.3.0.tar` & `tedeous-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:35:39.254169 tedeous-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-26 10:35:32.000000 tedeous-0.3.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-26 10:35:39.254169 tedeous-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-26 10:35:32.000000 tedeous-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 10:35:39.254169 tedeous-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-26 10:35:32.000000 tedeous-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:35:39.254169 tedeous-0.3.0/tedeous/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/derivative.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    10749 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/finite_diffs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25476 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/input_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/points_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    17556 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:35:39.254169 tedeous-0.3.0/tedeous.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-26 10:35:39.000000 tedeous-0.3.0/tedeous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-26 10:35:39.000000 tedeous-0.3.0/tedeous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 10:35:39.000000 tedeous-0.3.0/tedeous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 10:35:39.000000 tedeous-0.3.0/tedeous.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:31:58.854523 tedeous-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-28 14:31:53.000000 tedeous-0.3.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-28 14:31:58.854523 tedeous-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-28 14:31:53.000000 tedeous-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 14:31:58.854523 tedeous-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-28 14:31:53.000000 tedeous-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:31:58.854523 tedeous-0.3.1/tedeous/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 14:31:53.000000 tedeous-0.3.1/tedeous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17875 2023-07-28 14:31:53.000000 tedeous-0.3.1/tedeous/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-28 14:31:53.000000 tedeous-0.3.1/tedeous/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-07-28 14:31:53.000000 tedeous-0.3.1/tedeous/derivative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-28 14:31:53.000000 tedeous-0.3.1/tedeous/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10749 2023-07-28 14:31:53.000000 tedeous-0.3.1/tedeous/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-07-28 14:31:53.000000 tedeous-0.3.1/tedeous/finite_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25476 2023-07-28 14:31:53.000000 tedeous-0.3.1/tedeous/input_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-28 14:31:53.000000 tedeous-0.3.1/tedeous/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-28 14:31:53.000000 tedeous-0.3.1/tedeous/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-28 14:31:53.000000 tedeous-0.3.1/tedeous/points_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-28 14:31:53.000000 tedeous-0.3.1/tedeous/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17749 2023-07-28 14:31:53.000000 tedeous-0.3.1/tedeous/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-28 14:31:53.000000 tedeous-0.3.1/tedeous/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:31:58.854523 tedeous-0.3.1/tedeous.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-28 14:31:58.000000 tedeous-0.3.1/tedeous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-28 14:31:58.000000 tedeous-0.3.1/tedeous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:31:58.000000 tedeous-0.3.1/tedeous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 14:31:58.000000 tedeous-0.3.1/tedeous.egg-info/top_level.txt
```

### Comparing `tedeous-0.3.0/LICENCE` & `tedeous-0.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `tedeous-0.3.0/PKG-INFO` & `tedeous-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tedeous
-Version: 0.3.0
+Version: 0.3.1
 Summary: TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library
 Author: Alexander Hvatov
 Author-email: itmo.nss.team@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tedeous-0.3.0/README.rst` & `tedeous-0.3.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 
 The purpose of the project
 --------------------------
 
 1. Make equation discovery more transparent and illustrative
-2. Combine power of pytorch, numerical methods and math overall to conquer and solve ALL {O,P}DEs. There are some examples to provide a little insight to an operator form
+2. Combine power of pytorch, numerical methods and math overall to conquer and solve ALL XDEs(X={O,P}). There are some examples to provide a little insight to an operator form
 
 Table of Contents
 --------------------
 
 - `Core features <Core features_>`_
 - `Installation <Installation_>`_
 - `Examples <Examples_>`_
```

### Comparing `tedeous-0.3.0/setup.py` & `tedeous-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def get_requirements():
     requirements = extract_requirements('requirements.txt')
     return requirements
 
 setup(
     name = 'tedeous',
-    version= '0.3.0' ,
+    version= '0.3.1' ,
     description = 'TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library',
     long_description = 'Combine power of pytorch, numerical methods and math overall to conquer and solve ALL {O,P}DEs. There are some examples to provide a little insight to an operator form',
     author = 'Alexander Hvatov',
     author_email = 'itmo.nss.team@gmail.com', # add email
     classifiers = [      
               'Development Status :: 3 - Alpha',
               'Programming Language :: Python :: 3',
```

### Comparing `tedeous-0.3.0/tedeous/cache.py` & `tedeous-0.3.1/tedeous/cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         except:
             init_model = init_model.model
         
         return init_model, model
         
 
     def cache_lookup(self, lambda_operator: float = 1., lambda_bound: float = 0.001,
-                nmodels: Union[int, None] = None, save_graph: bool = False, cache_verbose: bool = False) -> Tuple[dict, torch.Tensor]:
+                nmodels: Union[int, None] = None, save_graph: bool = False, cache_verbose: bool = False, return_normalized_loss: bool = False) -> Tuple[dict, torch.Tensor]:
         """
         Looking for a saved cache.
         Args:
             lambda_bound: an arbitrary chosen constant, influence only convergence speed.
             save_graph: boolean constant, responsible for saving the computational graph.
             cache_dir: directory where saved cache in.
             nmodels: maximal number of models that are looked before optimization
@@ -189,15 +189,17 @@
                 best_checkpoint['optimizer_state_dict'] = \
                     checkpoint['optimizer_state_dict']
                 if cache_verbose:
                     print('best_model_num={} , normalized_loss={}'.format(i, min_norm_loss))
         if best_checkpoint == {}:
             best_checkpoint = None
             min_loss = np.inf
-        return best_checkpoint, min_norm_loss
+        if return_normalized_loss:
+            min_loss=min_norm_loss
+        return best_checkpoint, min_loss
 
     def save_model(self, prep_model: Any, state: dict, optimizer_state: dict, name: Union[str, None] = None):
         """
         Saved model in a cache (uses for 'NN' and 'autograd' methods).
         Args:
             prep_model: model to save.
             state: a dict holding current model state (i.e., dictionary that maps each layer to its parameter tensor).
@@ -322,15 +324,15 @@
             cache_model.eval()
             self.model, optimizer_state = self.scheme_interp(
                 cache_model, cache_verbose=cache_verbose)
         return self.model, optimizer_state
 
     def cache_nn(self, cache_dir: str, nmodels: Union[int, None], lambda_operator: float, lambda_bound: float,
               cache_verbose: bool,model_randomize_parameter: Union[float, None],
-              cache_model: torch.nn.Sequential, ):
+              cache_model: torch.nn.Sequential, return_normalized_loss: bool = False):
         """
        Restores the model from the cache and uses it for retraining.
        Args:
            cache_dir: a directory where saved cache in.
            nmodels: smth
            lambda_bound: an arbitrary chosen constant, influence only convergence speed.
            cache_verbose: more detailed info about models in cache.
@@ -341,26 +343,27 @@
            * **model** -- NN.\n
            * **min_loss** -- min loss as is.
        """
         r = create_random_fn(model_randomize_parameter)
         cache_checkpoint, min_loss = self.cache_lookup(nmodels=nmodels,
                                                        cache_verbose=cache_verbose,
                                                        lambda_operator= lambda_operator,
-                                                       lambda_bound=lambda_bound)
+                                                       lambda_bound=lambda_bound, 
+                                                       return_normalized_loss = return_normalized_loss)
         
         self.model, optimizer_state = self.cache_retrain(cache_checkpoint,
                                                          cache_verbose=cache_verbose)
 
         self.model.apply(r)
 
         return self.model, min_loss
 
     def cache_mat(self, nmodels: Union[int, None],lambda_operator: float, lambda_bound: float,
               cache_verbose: bool,model_randomize_parameter: Union[float, None],
-              cache_model: torch.nn.Sequential):
+              cache_model: torch.nn.Sequential, return_normalized_loss: bool = False):
         """
        Restores the model from the cache and uses it for retraining.
        Args:
            cache_dir: a directory where saved cache in.
            nmodels: smth
            lambda_bound: an arbitrary chosen constant, influence only convergence speed.
            cache_verbose: more detailed info about models in cache.
@@ -385,15 +388,16 @@
         r = create_random_fn(model_randomize_parameter)
         eq = Equation(NN_grid, operator, bconds).set_strategy('NN')
         model_cls = Model_prepare(NN_grid, eq, cache_model, 'NN', self.weak_form)
         cache_checkpoint, min_loss = model_cls.cache_lookup(
             cache_dir=self.cache_dir,
             nmodels=nmodels,
             cache_verbose=cache_verbose,
-            lambda_bound=lambda_bound)
+            lambda_bound=lambda_bound, 
+            return_normalized_loss=return_normalized_loss)
         prepared_model, optimizer_state = model_cls.cache_retrain(
             cache_checkpoint,
             cache_verbose=cache_verbose)
 
         prepared_model.apply(r)
 
         if len(self.grid.shape) == 2:
@@ -407,15 +411,16 @@
                                       self.model, self.mode, self.weak_form,
                                       lambda_operator, lambda_bound).evaluate()
 
         return self.model, min_loss
 
     def cache(self, nmodels: Union[int, None],lambda_operator, lambda_bound: float,
               cache_verbose: bool,model_randomize_parameter: Union[float, None],
-              cache_model: torch.nn.Sequential, ):
+              cache_model: torch.nn.Sequential, 
+              return_normalized_loss: bool = False):
         """
         Restores the model from the cache and uses it for retraining.
         Args:
             cache_dir: a directory where saved cache in.
             nmodels: number cached models.
             lambda_bound: an arbitrary chosen constant, influence only convergence speed.
             cache_verbose: more detailed info about models in cache.
@@ -426,13 +431,13 @@
         Returns:
             cache.cache_nn or cache.cache_mat
         """
 
         if self.mode != 'mat':
             return self.cache_nn(self.cache_dir, nmodels,lambda_operator, lambda_bound,
                                  cache_verbose, model_randomize_parameter,
-                                 cache_model)
+                                 cache_model,return_normalized_loss=return_normalized_loss)
         elif self.mode == 'mat':
             return self.cache_mat(self.cache_dir, nmodels, lambda_operator, lambda_bound,
                                   cache_verbose, model_randomize_parameter,
-                                  cache_model)
+                                  cache_model,return_normalized_loss=return_normalized_loss)
```

### Comparing `tedeous-0.3.0/tedeous/config.py` & `tedeous-0.3.1/tedeous/config.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.3.0/tedeous/derivative.py` & `tedeous-0.3.1/tedeous/derivative.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.3.0/tedeous/device.py` & `tedeous-0.3.1/tedeous/device.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.3.0/tedeous/eval.py` & `tedeous-0.3.1/tedeous/eval.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.3.0/tedeous/finite_diffs.py` & `tedeous-0.3.1/tedeous/finite_diffs.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.3.0/tedeous/input_preprocessing.py` & `tedeous-0.3.1/tedeous/input_preprocessing.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.3.0/tedeous/losses.py` & `tedeous-0.3.1/tedeous/losses.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.3.0/tedeous/models.py` & `tedeous-0.3.1/tedeous/models.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.3.0/tedeous/points_type.py` & `tedeous-0.3.1/tedeous/points_type.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.3.0/tedeous/solution.py` & `tedeous-0.3.1/tedeous/solution.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.3.0/tedeous/solver.py` & `tedeous-0.3.1/tedeous/solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -218,15 +218,16 @@
               abs_loss: Union[None, float] = None, use_cache: bool = True,
               cache_dir: str = '../cache/', cache_verbose: bool = False,
               save_always: bool = False, print_every: Union[int, None] = 100,
               cache_model: Union[torch.nn.Sequential, None] = None,
               patience: int = 5, loss_oscillation_window: int = 100,
               no_improvement_patience: int = 1000, model_randomize_parameter: Union[int, float] = 0,
               optimizer_mode: str = 'Adam', step_plot_print: Union[bool, int] = False,
-              step_plot_save: Union[bool, int] = False, image_save_dir: Union[str, None] = None, tol: float = 0,clear_cache: bool =False) -> Any:
+              step_plot_save: Union[bool, int] = False, image_save_dir: Union[str, None] = None, tol: float = 0,
+              clear_cache: bool  =False, normalized_loss_stop: bool = False) -> Any:
         """
         High-level interface for solving equations.
 
         Args:
             lambda_operator: coeff for operator part in loss.
             lambda_bound: coeff for boundary part in loss.
             lambda_update: enable lambda update.
@@ -273,15 +274,15 @@
         if use_cache:
             self.model, min_loss = Cache_class.cache(nmodels,
                                                      lambda_operator,
                                                      lambda_bound,
                                                      cache_verbose,
                                                      model_randomize_parameter,
                                                      cache_model,
-                                                    )
+                                                    return_normalized_loss=normalized_loss_stop)
 
             Solution_class = Solution(self.grid, self.equal_cls,
                                       self.model, self.mode, self.weak_form,
                                       lambda_operator, lambda_bound)
         else:
             Solution_class = Solution(self.grid, self.equal_cls,
                                       self.model, self.mode, self.weak_form,
@@ -311,15 +312,18 @@
             optimizer.zero_grad()
             loss, loss_normalized = Solution_class.evaluate(second_order_interactions=second_order_interactions,
                                            sampling_N=sampling_N,
                                            lambda_update=lambda_update,
                                            tol=tol)
 
             loss.backward()
-            cur_loss = loss_normalized.item()
+            if normalized_loss_stop:
+                cur_loss = loss_normalized.item()
+            else:
+                cur_loss = loss.item()
             return loss
 
         stop_dings = 0
         t_imp_start = 0
         # to stop train proceduce we fit the line in the loss data
         # if line is flat enough "patience" times, we stop the procedure
         cur_loss = min_loss
```

### Comparing `tedeous-0.3.0/tedeous/utils.py` & `tedeous-0.3.1/tedeous/utils.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.3.0/tedeous.egg-info/PKG-INFO` & `tedeous-0.3.1/tedeous.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tedeous
-Version: 0.3.0
+Version: 0.3.1
 Summary: TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library
 Author: Alexander Hvatov
 Author-email: itmo.nss.team@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

