# Comparing `tmp/separability-0.9.0.tar.gz` & `tmp/separability-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "separability-0.9.0.tar", max compression
+gzip compressed data, was "separability-0.9.1.tar", max compression
```

## Comparing `separability-0.9.0.tar` & `separability-0.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2513 2023-07-19 11:39:42.458790 separability-0.9.0/README.md
--rw-r--r--   0        0        0     1255 2023-07-28 13:25:49.369400 separability-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       24 2023-07-19 11:39:42.478791 separability-0.9.0/src/separability/__init__.py
--rw-r--r--   0        0        0    17621 2023-07-27 19:11:40.028590 separability-0.9.0/src/separability/activations.py
--rw-r--r--   0        0        0    13461 2023-07-27 17:43:19.180107 separability-0.9.0/src/separability/data_classes.py
--rw-r--r--   0        0        0     6359 2023-07-27 18:09:57.978819 separability-0.9.0/src/separability/eval.py
--rw-r--r--   0        0        0    44439 2023-07-27 18:08:51.106310 separability-0.9.0/src/separability/model.py
--rw-r--r--   0        0        0    27253 2023-07-28 10:57:43.099254 separability-0.9.0/src/separability/model_maps.py
--rw-r--r--   0        0        0      715 2023-07-19 11:39:42.478791 separability-0.9.0/src/separability/model_repos.py
--rw-r--r--   0        0        0    13504 2023-07-27 18:08:30.414151 separability-0.9.0/src/separability/nn.py
--rw-r--r--   0        0        0     2027 2023-07-19 11:39:42.478791 separability-0.9.0/src/separability/parser.py
--rw-r--r--   0        0        0     9692 2023-07-27 18:08:15.914040 separability-0.9.0/src/separability/prune.py
--rw-r--r--   0        0        0     5763 2023-07-27 19:16:27.675463 separability-0.9.0/src/separability/scoring.py
--rw-r--r--   0        0        0     4185 2023-07-19 11:39:42.478791 separability-0.9.0/src/separability/texts.py
--rw-r--r--   0        0        0     4115 1970-01-01 00:00:00.000000 separability-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2910 2023-07-28 13:39:41.284479 separability-0.9.1/README.md
+-rw-r--r--   0        0        0     1255 2023-07-28 15:44:50.750369 separability-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-07-19 11:39:42.478791 separability-0.9.1/src/separability/__init__.py
+-rw-r--r--   0        0        0    17621 2023-07-27 19:11:40.028590 separability-0.9.1/src/separability/activations.py
+-rw-r--r--   0        0        0    13461 2023-07-27 17:43:19.180107 separability-0.9.1/src/separability/data_classes.py
+-rw-r--r--   0        0        0     6359 2023-07-27 18:09:57.978819 separability-0.9.1/src/separability/eval.py
+-rw-r--r--   0        0        0    44439 2023-07-27 18:08:51.106310 separability-0.9.1/src/separability/model.py
+-rw-r--r--   0        0        0    27253 2023-07-28 10:57:43.099254 separability-0.9.1/src/separability/model_maps.py
+-rw-r--r--   0        0        0      715 2023-07-19 11:39:42.478791 separability-0.9.1/src/separability/model_repos.py
+-rw-r--r--   0        0        0    13504 2023-07-27 18:08:30.414151 separability-0.9.1/src/separability/nn.py
+-rw-r--r--   0        0        0     2027 2023-07-19 11:39:42.478791 separability-0.9.1/src/separability/parser.py
+-rw-r--r--   0        0        0     9692 2023-07-27 18:08:15.914040 separability-0.9.1/src/separability/prune.py
+-rw-r--r--   0        0        0     5763 2023-07-27 19:16:27.675463 separability-0.9.1/src/separability/scoring.py
+-rw-r--r--   0        0        0     4185 2023-07-19 11:39:42.478791 separability-0.9.1/src/separability/texts.py
+-rw-r--r--   0        0        0     4512 1970-01-01 00:00:00.000000 separability-0.9.1/PKG-INFO
```

### Comparing `separability-0.9.0/README.md` & `separability-0.9.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,68 @@
 # separability
 
-My basic library for studying LLMs (currently, only the Meta OPT models).
-This includes functions for analysing the activations of the models for different inputs, and for pruning different parts of the model based on those activations.
+My basic library for studying LLMs, with support for Multi-GPU inference and
+editing, as well as quantilised inference (not editing yet).
+This includes functions for analysing the activations of the models for
+different inputs, and for pruning different parts of the model based on those
+activations.
+
+The currently tested list of models is:
+- GPT2
+- EleutherAI's Pythia
+- Meta Opt
+- Meta Galactica
 
 ## Pruning based on Capabilities
 
-For a full example, see `src/separability.ipynb`.
+For a full example, see `src/examples/prune_30.py`.
 
 The simple example is:
 ```
-from model import Model
-from activations import prune_and_evaluate
-from separability.eval import evaluate_all
+from separability.data_classes import PruningConfig
+from separability.parser import cli_parser
+from separability.prune import run_pruning
+
+# Configure initial model and tests
+c = PruningConfig(
+    wandb_project = "testing",
+    model_repo   = "facebook/opt-125m",
+    token_limit  = 1000,
+    run_pre_test = True,
+
+    # Removals parameters
+    ff_scoring = "abs"
+    ff_frac   = 0.02,
+    ff_eps    = 0.001,
+    attn_scoring = "abs",
+    attn_frac = 0.00,
+    attn_eps  = 1e-4,
+
+    # Eval
+    focus     = "pile_codeless",
+    cripple   = "code",
+    additional_datasets=tuple(),
+)
 
-# Load and Evaluate Model on Pile and Code
+# optionally, use parser to get CLI arguments.
+# c, args = cli_parser(c)
 
-opt = Model('125m', limit=1000)
-eval_data = evaluate_all(opt, 1e5)
-print(eval_data)
+# Run the iterated pruning
+model, history = run_pruning(c)
 
-# Prune Model, Removing coding capabilities (compared to pile), and evaluate
-
-eval_data = prune_and_evaluate(opt, ff_prune_frac=0.05, attn_prune_frac=0.05,
-    ff_eps=1e-3, sample_size=1e5, eval_size=1e5, cripple='code', focus='pile')
-print(eval_data)
 ```
 
 ## model.py
 This defines a wrapper function that encapsulates the HuggingFace implementation of Meta OPT.
 To get the model, simply run:
 
 ```
-from model import Model
+from separability import Model
 
-opt = Model('125m', limit=1000)
+m = Model("facebook/opt-125m", limit=1000)
 ```
 
 Where you can provide any of the model sizes that are pre-trained for OPT, and the token limit must be smaller than the max token length that the model is able to handle.
 
 Next, you can run the model to do 2 tokens of predictions, by, for example, running:
 ```
 text = 'Hello, my name is'
@@ -65,13 +90,13 @@
 ```
 
 To get the activations for the input text at all of the MLP mid layers, we can look at:
 `opt.get_ff_key_activations( text )` or `opt.get_ff_key_activations( residual_stream=residual_stream )`.
 
 ## texts.py
 Has some basic tools for loading the two text datasets I am using:
-- 'the_pile' ( validation set of The Pile )
-- 'codeparrot-clean-valid' ( validation set of codeparrot )
+- 'pile', ( EleutherAI's 'The Pile' dataset)
+- 'code' (CodeParrot's 'github-code' dataset)
 
 ## activations.py
-Has code specific to the two datasets I am using to analyze and attempt to remove capabilities from the OPT.
+Has code specific to the two datasets I am using to analyze and attempt to remove capabilities from the models.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `separability-0.9.0/pyproject.toml` & `separability-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "separability"
-version = "0.9.0"
+version = "0.9.1"
 description = "LLM Tools for looking at separability of LLM Capabilities"
 authors = ["Nicky Pochinkov"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `separability-0.9.0/src/separability/activations.py` & `separability-0.9.1/src/separability/activations.py`

 * *Files identical despite different names*

### Comparing `separability-0.9.0/src/separability/data_classes.py` & `separability-0.9.1/src/separability/data_classes.py`

 * *Files identical despite different names*

### Comparing `separability-0.9.0/src/separability/eval.py` & `separability-0.9.1/src/separability/eval.py`

 * *Files identical despite different names*

### Comparing `separability-0.9.0/src/separability/model.py` & `separability-0.9.1/src/separability/model.py`

 * *Files identical despite different names*

### Comparing `separability-0.9.0/src/separability/model_maps.py` & `separability-0.9.1/src/separability/model_maps.py`

 * *Files identical despite different names*

### Comparing `separability-0.9.0/src/separability/model_repos.py` & `separability-0.9.1/src/separability/model_repos.py`

 * *Files identical despite different names*

### Comparing `separability-0.9.0/src/separability/nn.py` & `separability-0.9.1/src/separability/nn.py`

 * *Files identical despite different names*

### Comparing `separability-0.9.0/src/separability/parser.py` & `separability-0.9.1/src/separability/parser.py`

 * *Files identical despite different names*

### Comparing `separability-0.9.0/src/separability/prune.py` & `separability-0.9.1/src/separability/prune.py`

 * *Files identical despite different names*

### Comparing `separability-0.9.0/src/separability/scoring.py` & `separability-0.9.1/src/separability/scoring.py`

 * *Files identical despite different names*

### Comparing `separability-0.9.0/src/separability/texts.py` & `separability-0.9.1/src/separability/texts.py`

 * *Files identical despite different names*

### Comparing `separability-0.9.0/PKG-INFO` & `separability-0.9.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: separability
-Version: 0.9.0
+Version: 0.9.1
 Summary: LLM Tools for looking at separability of LLM Capabilities
 Home-page: https://github.com/pesvut/separability
 Author: Nicky Pochinkov
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -35,48 +35,73 @@
 Requires-Dist: welford-torch (>=0.1.2,<0.2.0)
 Requires-Dist: zstandard (>=0.19.0,<0.20.0)
 Project-URL: Repository, https://github.com/pesvut/separability
 Description-Content-Type: text/markdown
 
 # separability
 
-My basic library for studying LLMs (currently, only the Meta OPT models).
-This includes functions for analysing the activations of the models for different inputs, and for pruning different parts of the model based on those activations.
+My basic library for studying LLMs, with support for Multi-GPU inference and
+editing, as well as quantilised inference (not editing yet).
+This includes functions for analysing the activations of the models for
+different inputs, and for pruning different parts of the model based on those
+activations.
+
+The currently tested list of models is:
+- GPT2
+- EleutherAI's Pythia
+- Meta Opt
+- Meta Galactica
 
 ## Pruning based on Capabilities
 
-For a full example, see `src/separability.ipynb`.
+For a full example, see `src/examples/prune_30.py`.
 
 The simple example is:
 ```
-from model import Model
-from activations import prune_and_evaluate
-from separability.eval import evaluate_all
+from separability.data_classes import PruningConfig
+from separability.parser import cli_parser
+from separability.prune import run_pruning
+
+# Configure initial model and tests
+c = PruningConfig(
+    wandb_project = "testing",
+    model_repo   = "facebook/opt-125m",
+    token_limit  = 1000,
+    run_pre_test = True,
+
+    # Removals parameters
+    ff_scoring = "abs"
+    ff_frac   = 0.02,
+    ff_eps    = 0.001,
+    attn_scoring = "abs",
+    attn_frac = 0.00,
+    attn_eps  = 1e-4,
+
+    # Eval
+    focus     = "pile_codeless",
+    cripple   = "code",
+    additional_datasets=tuple(),
+)
 
-# Load and Evaluate Model on Pile and Code
+# optionally, use parser to get CLI arguments.
+# c, args = cli_parser(c)
 
-opt = Model('125m', limit=1000)
-eval_data = evaluate_all(opt, 1e5)
-print(eval_data)
+# Run the iterated pruning
+model, history = run_pruning(c)
 
-# Prune Model, Removing coding capabilities (compared to pile), and evaluate
-
-eval_data = prune_and_evaluate(opt, ff_prune_frac=0.05, attn_prune_frac=0.05,
-    ff_eps=1e-3, sample_size=1e5, eval_size=1e5, cripple='code', focus='pile')
-print(eval_data)
 ```
 
 ## model.py
 This defines a wrapper function that encapsulates the HuggingFace implementation of Meta OPT.
 To get the model, simply run:
 
 ```
-from model import Model
+from separability import Model
 
-opt = Model('125m', limit=1000)
+m = Model("facebook/opt-125m", limit=1000)
 ```
 
 Where you can provide any of the model sizes that are pre-trained for OPT, and the token limit must be smaller than the max token length that the model is able to handle.
 
 Next, you can run the model to do 2 tokens of predictions, by, for example, running:
 ```
 text = 'Hello, my name is'
@@ -104,14 +129,14 @@
 ```
 
 To get the activations for the input text at all of the MLP mid layers, we can look at:
 `opt.get_ff_key_activations( text )` or `opt.get_ff_key_activations( residual_stream=residual_stream )`.
 
 ## texts.py
 Has some basic tools for loading the two text datasets I am using:
-- 'the_pile' ( validation set of The Pile )
-- 'codeparrot-clean-valid' ( validation set of codeparrot )
+- 'pile', ( EleutherAI's 'The Pile' dataset)
+- 'code' (CodeParrot's 'github-code' dataset)
 
 ## activations.py
-Has code specific to the two datasets I am using to analyze and attempt to remove capabilities from the OPT.
+Has code specific to the two datasets I am using to analyze and attempt to remove capabilities from the models.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

