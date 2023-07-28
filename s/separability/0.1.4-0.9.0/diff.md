# Comparing `tmp/separability-0.1.4.tar.gz` & `tmp/separability-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "separability-0.1.4.tar", max compression
+gzip compressed data, was "separability-0.9.0.tar", max compression
```

## Comparing `separability-0.1.4.tar` & `separability-0.9.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     2484 2023-02-26 22:57:03.671779 separability-0.1.4/README.md
--rw-r--r--   0        0        0     1114 2023-02-26 22:57:14.075881 separability-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       97 2023-02-23 01:38:19.170502 separability-0.1.4/src/separability/__init__.py
--rw-r--r--   0        0        0    28493 2023-02-23 01:38:19.170502 separability-0.1.4/src/separability/activations.py
--rw-r--r--   0        0        0     8535 2023-02-23 01:38:19.170502 separability-0.1.4/src/separability/data_classes.py
--rw-r--r--   0        0        0    37728 2023-02-23 01:38:19.170502 separability-0.1.4/src/separability/model.py
--rw-r--r--   0        0        0     3296 2023-02-23 01:38:19.170502 separability-0.1.4/src/separability/model_maps.py
--rw-r--r--   0        0        0      715 2023-02-23 01:38:19.170502 separability-0.1.4/src/separability/model_repos.py
--rw-r--r--   0        0        0     5162 2023-02-23 01:38:19.170502 separability-0.1.4/src/separability/nn.py
--rw-r--r--   0        0        0     2814 2023-02-23 01:38:19.170502 separability-0.1.4/src/separability/texts.py
--rw-r--r--   0        0        0     3755 1970-01-01 00:00:00.000000 separability-0.1.4/setup.py
--rw-r--r--   0        0        0     3942 1970-01-01 00:00:00.000000 separability-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2513 2023-07-19 11:39:42.458790 separability-0.9.0/README.md
+-rw-r--r--   0        0        0     1255 2023-07-28 13:25:49.369400 separability-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-07-19 11:39:42.478791 separability-0.9.0/src/separability/__init__.py
+-rw-r--r--   0        0        0    17621 2023-07-27 19:11:40.028590 separability-0.9.0/src/separability/activations.py
+-rw-r--r--   0        0        0    13461 2023-07-27 17:43:19.180107 separability-0.9.0/src/separability/data_classes.py
+-rw-r--r--   0        0        0     6359 2023-07-27 18:09:57.978819 separability-0.9.0/src/separability/eval.py
+-rw-r--r--   0        0        0    44439 2023-07-27 18:08:51.106310 separability-0.9.0/src/separability/model.py
+-rw-r--r--   0        0        0    27253 2023-07-28 10:57:43.099254 separability-0.9.0/src/separability/model_maps.py
+-rw-r--r--   0        0        0      715 2023-07-19 11:39:42.478791 separability-0.9.0/src/separability/model_repos.py
+-rw-r--r--   0        0        0    13504 2023-07-27 18:08:30.414151 separability-0.9.0/src/separability/nn.py
+-rw-r--r--   0        0        0     2027 2023-07-19 11:39:42.478791 separability-0.9.0/src/separability/parser.py
+-rw-r--r--   0        0        0     9692 2023-07-27 18:08:15.914040 separability-0.9.0/src/separability/prune.py
+-rw-r--r--   0        0        0     5763 2023-07-27 19:16:27.675463 separability-0.9.0/src/separability/scoring.py
+-rw-r--r--   0        0        0     4185 2023-07-19 11:39:42.478791 separability-0.9.0/src/separability/texts.py
+-rw-r--r--   0        0        0     4115 1970-01-01 00:00:00.000000 separability-0.9.0/PKG-INFO
```

### Comparing `separability-0.1.4/README.md` & `separability-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 ## Pruning based on Capabilities
 
 For a full example, see `src/separability.ipynb`.
 
 The simple example is:
 ```
 from model import Model
-from activations import prune_and_evaluate, evaluate_all
+from activations import prune_and_evaluate
+from separability.eval import evaluate_all
 
 # Load and Evaluate Model on Pile and Code
 
 opt = Model('125m', limit=1000)
 eval_data = evaluate_all(opt, 1e5)
 print(eval_data)
```

### Comparing `separability-0.1.4/pyproject.toml` & `separability-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 [tool.poetry]
 name = "separability"
-version = "0.1.4"
-description = "separability of LLM Capabilities"
+version = "0.9.0"
+description = "LLM Tools for looking at separability of LLM Capabilities"
 authors = ["Nicky Pochinkov"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 repository = "https://github.com/pesvut/separability"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.9,<3.13"
 ipykernel = "^6.21.1"
 ipywidgets = "^8.0.4"
 numpy = "^1.23"
 numexpr = "^2.7.0"
-torch = "^1.13.0"
+torch = "^2.0.1"
 tensorboardx = "^2.5.1"
 tensorboard = "^2.11.2"
 dict-deep = "^4.1.2"
 pandas = "^1.5.3"
-transformers = "^4.26.0"
+transformers = "^4.30.0"
+tokenizers = "^0.13.3"
+sentencepiece = "^0.1.99"
+bitsandbytes = "^0.40.2"
+scipy = "^1.11.1"
 datasets = "^2.9.0"
 evaluate = "^0.4.0"
 zstandard = "^0.19.0"
 welford-torch = "^0.1.2"
 einops = "^0.6.0"
 matplotlib = "^3.6.3"
 wandb = "^0.13.9"
-accelerate = "^0.16.0"
+accelerate = "^0.21.0"
+celery = "^5.3.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 mypy = "^0.991"
 autopep8 = "^2.0.1"
 sphinx = "^6.1.3"
```

### Comparing `separability-0.1.4/src/separability/model.py` & `separability-0.9.0/src/separability/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 """ Defines the 'Model' class which wraps the Meta OPT model,
 with additional methods for inspecting the activations of the model.
 """
 
 # import types for typed python
-from typing import Optional, List, Tuple, Union
+from typing import Optional, List, Tuple, Callable
 import warnings
+import time
 from torch import Tensor
 from accelerate import Accelerator
 from datasets import Dataset
-from transformers.models.opt.modeling_opt import OPTAttention
 
 from transformers import AutoTokenizer, AutoModelForCausalLM
 import torch
+import torch.nn.functional as F
 import numpy as np
 from welford_torch import Welford
 from tqdm import tqdm
 
+# Import matplotlib and set dpi to 300
+import matplotlib as mpl
+
 # Import from inside module
 from .model_repos import supported_model_repos
-from .nn import InverseLinear, mlp_delete_rows, mlp_adjust_biases, mlp_delete_columns
+from .nn import InverseLinear, mlp_delete_rows, mlp_delete_rows_raw, mlp_adjust_biases, \
+    mlp_delete_columns, mlp_svd_two_layer_raw, mlp_delete_columns_raw
+from .model_maps import convert_hf_model_config, ModelMap
+from .data_classes import DtypeMap
 
-# Import matplotlib and set dpi to 300
-import matplotlib as mpl
 mpl.rcParams['figure.dpi'] = 300
 
 # Return with the output tensors detached from gpu
 def detached( output ):
     """ Recursively detach Tensor or List of Tensors """
 
     if isinstance(output, tuple):
@@ -48,40 +53,50 @@
 
     def __init__( self,
             model_repo: str  = "facebook/opt-125m",
             limit: int = None,
             model_device: str = None,
             output_device: str = None,
             use_accelerator: bool = True,
-            dtype: torch.dtype = torch.float32,
+            dtype: Optional[str] = None,
+            torch_dtype: Optional[torch.dtype] = None,
+            svd_attn: bool = False,
         ):
         """
         OPT Model with functions for extracting activations.
         facebook/opt-{model_size}
         model_size : 125m, 350m, 1.3b, 2.7b, 6.7b, 13b, 30b, 66b, 175b
 
         facebook/galactica-{model_size}
         model_size : 125m, 1.3b, 6.7b, 30b, 120b
         """
 
         # Initialize model differently depending on accelerator use
         self.use_accelerator = use_accelerator and torch.cuda.device_count() > 1
         self.dtype = dtype
+        self.svd_attn = svd_attn
+
+        # Handle dtype
+        if dtype is None and torch_dtype is None:
+            dtype = "fp16"
+        self.dtype_map = DtypeMap(dtype, torch_dtype)
+        self.dtype = self.dtype_map._dtype
+        self.dtype_args = self.dtype_map._dtype_args
 
         if self.use_accelerator:
             self.accelerator = Accelerator()
             self.device = self.accelerator.device
             self.output_device = output_device if output_device else 'cuda:1'
 
         else:
             self.device = 'cuda' if torch.cuda.is_available() else 'cpu'
             self.device = model_device if model_device else self.device
             self.output_device = output_device if output_device else self.device
 
-        self.init_model( model_repo ).to( self.device )
+        self.init_model( model_repo )
         self.limit = limit
 
         # Indices of outputs for reference
         self.layer_index     = -3
         self.token_index     = -2
         self.dimension_index = -1
 
@@ -92,52 +107,60 @@
 
         self.model_size = model_repo.split('-')[-1]
         self.model_repo = model_repo
 
     # pylint: disable=attribute-defined-outside-init
     def init_model( self, model_repo: Optional[str] = None ):
         if not model_repo is None:
-            self.set_repo( model_repo )
-        self.tokenizer = AutoTokenizer.from_pretrained(self.model_repo)
-
+            self.set_repo(model_repo)
         # Initialize model (with or without accelerator)
         device_map = "auto" if self.use_accelerator else None
-        #self.predictor = OPTForCausalLM.from_pretrained(self.repo, dtype=self.dtype)
+
+        # Import model config
+        self.cfg = convert_hf_model_config(self.model_repo)
+        self.cfg.is_low_precision = self.dtype_map.is_low_precision
+
+        # Import model components
+        self.tokenizer = AutoTokenizer.from_pretrained(self.model_repo)
         self.predictor = AutoModelForCausalLM.from_pretrained(
-            self.model_repo, torch_dtype=self.dtype, device_map=device_map)
-        self.model = self.predictor.model
+            self.model_repo, device_map=device_map, **self.dtype_args)
 
-        print(f'- Loaded {self.model_repo}')
-        self.activations = {}
+        # Build map for working with model
+        self.map = ModelMap(self.predictor, self.cfg)
+        self.model  = self.map["model"]
+        self.layers = self.map.layers
 
-        attn0 = self.model.decoder.layers[0].self_attn
-        self.d_model = attn0.embed_dim
-        self.d_head  = attn0.head_dim
-        self.n_heads = attn0.num_heads
-        self.n_layers = len(self.model.decoder.layers)
+        #self.predictor = OPTForCausalLM.from_pretrained(self.repo, dtype=self.dtype)
+        self.to(self.device)
 
-        self.d_ff = 4 * self.d_model
+        print(f'- Loaded {self.model_repo}')
+        self.activations = {}
 
         self.register_activations()
-        self.register_inverse_out_proj()
+        if self.svd_attn:
+            self.svd_attention_layers()
+        else:
+            self.register_inverse_out_proj()
 
         return self
 
     def show_details( self, verbose=True ):
         if verbose:
-            print( " - n_layers :", self.n_layers )
-            print( " - d_model  :", self.d_model  )
-            print( " - n_heads  :", self.n_heads  )
-            print( " - d_head   :", self.d_head   )
+            print( " - n_layers :", self.cfg.n_layers )
+            print( " - d_model  :", self.cfg.d_model  )
+            print( " - n_heads  :", self.cfg.n_heads  )
+            print( " - d_head   :", self.cfg.d_head   )
         else:
-            print( f" - n_layers, d_model = {self.n_layers}, {self.d_model}" )
+            print( f" - n_layers, d_model = {self.cfg.n_layers}, {self.cfg.d_model}" )
 
     def to( self, device ):
         if self.use_accelerator: # If using accelerator, init handles multi-device
             return
+        if self.dtype_map.is_low_precision: # 8bit & 4bit mode handled by accelerator
+            return
         self.device = device
         self.predictor.to( device )
         self.model.to( device )
 
     def out_stack(self, tensor_list: List[Tensor]) -> Tensor:
         if self.use_accelerator or self.device != self.output_device:
             tensor_list = [ t.to(self.output_device) for t in tensor_list ]
@@ -150,37 +173,67 @@
                 return
             self.activations[name] = detached( output )
         return hook
 
     def register_activations( self ):
         # register the forward hook
         attention_index = 0
-        for module in self.model.decoder.layers.modules():
-            if isinstance(module, OPTAttention):
-                name = pad_zeros( attention_index ) + "-attention"
-                # print( f"registering : ({name}), OPTAttention layer" )
-                module.register_forward_hook( self.get_activation_of( name ) )
-                attention_index += 1
-                continue
-        print( f" - Registered {attention_index} OPT Attention Layers" )
+        for layer_index, layer in enumerate(self.layers):
+            attn = layer["attn"]
+            name = pad_zeros( layer_index ) + "-attention"
+            # print( f"registering : ({name}), OPTAttention layer" )
+            attn.register_forward_hook( self.get_activation_of( name ) )
+            attention_index += 1
+            continue
+        print( f" - Registered {attention_index} Attention Layers" )
 
     def register_inverse_out_proj( self ):
         # Make it possible to get the output right before out_proj
-        for layer in self.model.decoder.layers:
-            inv_out_proj = InverseLinear(layer.self_attn.out_proj)
+        for layer in self.layers:
+            #print(layer["attn.W_O"].shape)
+            inv_out_proj = InverseLinear(
+                original_weights=layer["attn.W_O"],
+                original_biases=layer["attn.b_O"],
+                n_heads=self.cfg.n_heads,
+            )
             inv_out_proj = inv_out_proj.to(dtype=self.dtype)
 
             if self.use_accelerator:
                 inv_out_proj = self.accelerator.prepare(inv_out_proj)
             else:
                 # Use self.output_device since that is where the output will be stored
                 inv_out_proj = inv_out_proj.to(self.output_device)
 
-            layer.self_attn.inv_out_proj = inv_out_proj
+            layer["attn.inv_out_proj"] = inv_out_proj
 
+    def svd_attention_layers( self ):
+        # Rewrite the v_proj and out_proj matrices using SVD
+        t0 = time.time()
+        for layer in self.layers:
+            with torch.no_grad():
+                W_in,  b_in  = layer["attn.W_V"], layer["attn.b_V"]
+                W_out, b_out = layer["attn.W_O"], layer["attn.b_O"]
+
+                inv_out_proj, updated_weights = \
+                    mlp_svd_two_layer_raw(W_in, W_out, b_in, b_out)
+
+                layer["attn.W_V"] = updated_weights["W_in"]
+                layer["attn.W_O"] = updated_weights["W_out"]
+                layer["attn.b_V"] = updated_weights["b_in"]
+                layer["attn.b_O"] = updated_weights["b_out"]
+
+                layer["attn.inv_out_proj"] = inv_out_proj.to(self.output_device)
+
+        t = time.time() - t0
+        print( f" - SVD Attention Layers in {t:.1f} seconds" )
+
+    def delete_residual_biases( self ):
+        for layer in self.layers:
+            layer["attn.b_O"] = torch.zeros_like( layer["attn.b_O"] )
+            layer["mlp.b_out"] = torch.zeros_like( layer["mlp.b_out"] )
 
     def get_ids( self, text:str, limit:Optional[int]=None ):
         limit = self.limit if (limit is None) else limit
         input_ids = self.tokenizer( text, return_tensors='pt').input_ids
         if not limit is None:
             input_ids = torch.stack([ input_ids[0][:limit] ])
         return input_ids.to( self.device )
@@ -189,22 +242,22 @@
                 text: Optional[str] = None,
                 input_ids: Optional[Tensor] = None,
                 limit: Optional[int] = None
             ):
         if input_ids is None:
             input_ids = self.get_ids( text, limit )
 
-        inputs_embeds = self.model.decoder.embed_tokens( input_ids )
+        inputs_embeds = self.map["embed"]( input_ids )
 
         return inputs_embeds
 
     def get_recent_activations( self ) -> List[ Tuple[str, Tensor, Tensor, Tensor] ]:
         """
         Returns a list of output tuples \
-        ( "##-attention", output, key_values, attention_output ) \
+        ( "##-attention", output, attn_weights, key_values ) \
         from each attention block
         """
         layers = []
         for key, value in self.activations.items():
             layer = []
             layer.append( key )
             for out in value:
@@ -279,15 +332,15 @@
 
         # get attention outputs
         attention_out = self.out_stack([a[1] for a in self.get_recent_activations()])
         attention_out = attention_out.squeeze().detach()
 
         # get ff outputs
         ff_out =  []
-        for i in range(self.n_layers):
+        for i in range(self.cfg.n_layers):
             ff_out.append( hidden_states[i+1] - attention_out[i] - hidden_states[i] )
         ff_out = self.out_stack( ff_out ).squeeze().detach().detach()
 
         # get the final output
         output: Tensor = outputs.last_hidden_state[0].detach()
 
         return inpt, attention_out, ff_out, output
@@ -302,18 +355,18 @@
             ) -> Tensor:
 
         if text_activations is None:
             text_activations = self.get_text_activations( text,
                 input_ids, inputs_embeds, limit, **kwargs )
         inpt, attention_out, ff_out, _output = text_activations
 
-        assert len(attention_out) == self.n_layers
-        assert len(ff_out) == self.n_layers
+        assert len(attention_out) == self.cfg.n_layers
+        assert len(ff_out) == self.cfg.n_layers
 
-        adjustments = [0]*(2*self.n_layers)
+        adjustments = [0]*(2*self.cfg.n_layers)
         adjustments[0::2] = attention_out
         adjustments[1::2] = ff_out
 
 
         residual_stream = []
         residual_stream.append( inpt )
 
@@ -358,27 +411,45 @@
 
         [ _inpt, attn_out, _ff_out, _output ] = text_activations
         pre_outs = self.calculate_attn_pre_out(
             attn_out.to(self.device), reshape, transpose )
 
         return pre_outs
 
+    def get_attn_value_activations( self,
+                text: Optional[str] = None,
+                input_ids: Optional[Tensor] = None,
+                inputs_embeds: Optional[Tensor] = None,
+                text_activations: Optional[List[Tensor]] = None,
+                residual_stream: Optional[Tensor] = None,
+                limit: Optional[int] = None,
+                **kwargs
+            ) -> Tensor:
+        if residual_stream is None:
+            residual_stream = self.get_residual_stream( text, input_ids,
+                inputs_embeds, text_activations, limit, **kwargs )
+
+        attn_inputs = residual_stream[0:-1:2]
+        attn_values = self.calculate_attn_value( attn_inputs.to(self.device) )
+        return attn_values
+
     # Functions for calculating attention
     # Brief description of attention mechanism with OPTAttention reference:
     # input: x_i
     # then: x_i -> k_i, q_i, v_i
     # then: k_i, q_j            -> attention a_ij  "attn_weights"
-    # then: sum_i( a_ij * v_j ) ->                 "attn_pre_out"
+    # then: sum_j( a_ij * v_j ) ->                 "attn_pre_out"
     # then: W_o * pre_out       -> output          "attn_out"
     # output: attn_out, attn_weights, (k_i, v_i)
 
     def get_attn_layers(self):
-        return [ l.self_attn for l in self.model.decoder.layers ]
+        return [ l["attn"] for l in self.layers ]
 
     def prepare_attention_mask( self, inpt: Tensor ):
+        # TODO: change to ModelMap
         decoder = self.model.decoder
         input_shape = input.size()[:-1]
 
         # embed positions
         attention_mask = torch.ones( input_shape, dtype=torch.bool,
             device=input.device )
         attention_mask = decoder._prepare_decoder_attention_mask(
@@ -387,17 +458,17 @@
         return attention_mask
 
     def calculate_attn_out_layer( self,
                 attn_in: Tensor,
                 layer: int,
                 attention_mask: Tensor
             ):
-        u = self.model.decoder.layers[ layer ]
-        x = u.self_attn_layer_norm( attn_in )
-        x = u.self_attn( x, attention_mask=attention_mask )[0]
+        u = self.layers[ layer ]
+        x = u["ln1"]( attn_in )
+        x = u["attn"]( x, attention_mask=attention_mask )[0]
         return x
 
     def calculate_attn_out( self, attn_in: Tensor, add_residual: bool = False ):
         """
         Calculate the output of each attention layer.
 
         inputs:
@@ -422,23 +493,23 @@
     def calculate_attn_pre_out_layer( self,
             attn_out: Tensor,
             layer: int,
             reshape: bool,
             transpose: bool
             ):
         # ie: turns attn_out into attn_pre_out
-        self_attn = self.model.decoder.layers[layer].self_attn
-
-        # Calculate the layer before
-        pre_out = self_attn.inv_out_proj( attn_out )
+        layer = self.layers[layer]
+        pre_out = layer["attn.inv_out_proj"]( attn_out )
 
         # reshape into the shape it was before W_out
         if reshape:
+            if len(attn_out.shape) == 1: # fix for single token inputs
+                attn_out = attn_out.reshape(1, -1)
             [ tgt_len, _embed_dim ] = attn_out.size() # see OPTAttention
-            pre_out = pre_out.view(tgt_len, self.n_heads, self.d_head)
+            pre_out = pre_out.view(tgt_len, self.cfg.n_heads, self.cfg.d_head)
 
         # whether to transpose the output to what it originally looked like
         if reshape and transpose:
             pre_out = pre_out.transpose( 0, 1 )
 
         return pre_out
 
@@ -455,145 +526,199 @@
             layer (int): The layer to calculate the pre_out for.
             reshape (bool): Whether to reshape the output into heads.
             transpose (bool, optional): Whether to transpose the output to original
                 format used in OPT. Only done if reshape is True.
         """
 
         out = []
-        assert len(attn_out) == self.n_layers
-        for layer in range(self.n_layers):
+        assert len(attn_out) == self.cfg.n_layers
+        for layer in range(self.cfg.n_layers):
             pre_out = self.calculate_attn_pre_out_layer(
                 attn_out[layer], layer, reshape, transpose )
             out.append( pre_out)
         return self.out_stack( out )
 
+
+    def calculate_attn_value_layer( self,
+                attn_in_layer: Tensor,
+                layer_index: int,
+            ):
+        layer = self.layers[layer_index]
+        if "attn.v_proj" in layer and layer["attn.v_proj"] is not None:
+            return layer["attn.v_proj"]( attn_in_layer )
+
+        # TODO: Make more general (ie: work on multiple GPUs)
+        W_V, b_V = layer["attn.W_V"], layer["attn.b_V"]
+        return F.linear(input=attn_in_layer, weight=W_V, bias=b_V)
+
+    def calculate_attn_value(self, attn_in: Tensor):
+        """Given the inputs to the attention layers, calculate the values
+        """
+        out = []
+        assert len(attn_in) == self.cfg.n_layers
+        for layer in range(self.cfg.n_layers):
+            values = self.calculate_attn_value_layer(attn_in[layer], layer)
+            out.append(values)
+        return self.out_stack(out)
+
     def delete_attn_pre_out_layer( self,
             layer_index: int,
             remove_indices: Tensor,
-            mean_values: Optional[Tensor] = None
+            mean_activation: Optional[Tensor] = None
             ):
         """
         A function that deletes the impact that the pre_out layer has on the model
 
         Args:
             layer_index (int): Layer of attention in which out_proj is being pruned.
             indices (Tensor): a tensor of size (d_model) or (n_heads, d_head) which
                 has value True at each index which will be pruned.
-            mean_values (Optional[Tensor], optional): The value to offset the output
+            mean_activation (Optional[Tensor], optional): The value to offset the output
                 by to compensate for the fact it is no longer in service.
                 Defaults to None.
         """
         if isinstance(remove_indices, np.ndarray):
             remove_indices = torch.tensor(remove_indices, dtype=torch.bool)
-        if isinstance(mean_values,    np.ndarray):
-            mean_values = torch.tensor(mean_values, dtype=torch.float32)
+        if isinstance(mean_activation,    np.ndarray):
+            mean_activation = torch.tensor(mean_activation, dtype=torch.float32)
 
         # NOTE: in this case, we need to modify both the input and the output
         #       of the attention pre_out (ie: v_proj and out_proj) layers
         #       since we have the option of offset by the mean value
 
         with torch.no_grad():
-            # check tensor sizes are correct
             size = remove_indices.size()
-            if size[-1] == self.d_head:
-                remove_indices = remove_indices.reshape( (*size[:-2], -1) )
-                size = remove_indices.size()
-            assert remove_indices.size() == torch.Size([self.d_model])
-
-            # get the attention that we are changing.
-            # We change both (1) the inputs and (2) the outputs of the pre_out layer
-            out_proj = self.model.decoder.layers[layer_index].self_attn.out_proj
-            v_proj   = self.model.decoder.layers[layer_index].self_attn.v_proj
-
-            # 1. Adjust the biases out of the out_proj layer to compensate for
-            #    the deletion of the weights
-            if not remove_indices is None:
-                mlp_adjust_biases( out_proj, remove_indices, mean_values )
 
-            # Optionally, delete the weights going out of a neuron
-            # more of a sanity check than actually being useful
+            # Get flat remove indices, needed for out weight changing
+            flat_remove_indices = remove_indices
+            if size[-1] == self.cfg.d_head:
+                flat_remove_indices = remove_indices.reshape( (*size[:-2], -1) )
+
+            # check tensor sizes are correct
+            assert flat_remove_indices.size() == torch.Size([self.cfg.d_model])
+
+            # We change both the inputs and the outputs of the pre_out layer
+            layer = self.layers[layer_index]
+
+            # 1. Optionally, adjust the biases out of the out_proj layer to
+            #    compensate for the deletion of the weights
+            #if (mean_activation is not None):
+            #    # TODO: Make compatible with ModelMap
+            #    out_proj = layer["attn.out_proj"]
+            #    mlp_adjust_biases( out_proj, remove_indices, mean_activation )
+
+
+            # 2. Optionally, delete the weights going out of a neuron
+            #    ( more of a sanity check. )
             if not self.use_accelerator:
-                mlp_delete_columns( out_proj, remove_indices )
+                W_O = layer["attn.W_O"]
+                W_O = mlp_delete_columns_raw( W_O, flat_remove_indices )
+                layer["attn.W_O"] = W_O
+
+            # Additionally, delete inv_out_proj weights (to better keep track)
+            params = layer["attn.inv_out_proj"].state_dict()
+            W_inv = params["weight"]
+            W_inv, _ = mlp_delete_rows_raw(flat_remove_indices, W_inv)
+            params["weight"] = W_inv
+            layer["attn.inv_out_proj"].load_state_dict(params)
+
+
+            # 3. Delete the weights and biases going into neuron (v_proj)
+            #    so it never activates in the first place
+            W_V, b_V = layer["attn.W_V"], layer["attn.b_V"]
+            for i_head in range(self.cfg.n_heads):
+                for i_row in range(self.cfg.d_head):
+                    if not remove_indices[i_head][i_row]:
+                        continue
+                    W_V[i_head][i_row] = torch.zeros_like(W_V[i_head][i_row])
+                    b_V[i_head][i_row] = torch.zeros_like(b_V[i_head][i_row])
+            layer["attn.W_V"], layer["attn.b_V"] = W_V, b_V
+
 
-            # 2. Delete the weights and biases going into neuron (v_proj)
-            #  so it never activates in the first place
-            mlp_delete_rows(v_proj, remove_indices)
 
     def delete_attn_pre_out( self,
             remove_indices: Tensor,
-            mean_values: Tensor = None,
+            mean_activation: Tensor = None,
         ):
         """Delete effect of attn_pre_out for neurons at indices {remove_indices}.
-        Optionally offset the output my some mean activation {mean_values}.
+        Optionally offset the output my some mean activation {mean_activation}.
 
         Args:
             remove_indices (Tensor): Tensor of type [n_layer, n_heads, d_head] or
                 [n_layer, d_model] with value True for nodes of attn_pre_out to
                 prune / make inactive.
-            mean_values (Tensor, optional): Mean activation to adjust the bias to
+            mean_activation (Tensor, optional): Mean activation to adjust the bias to
                 compensate for the deletion of the attn_pre_out interactions.
                 Defaults to None.
 
         Returns:
             self (Model)
         """
-        use_means = not (mean_values is None)
+        use_means = not (mean_activation is None)
         if use_means:
-            assert mean_values.size() == remove_indices.size()
+            # TODO: test this is fine?
+            assert torch.tensor(mean_activation.size()).prod() \
+                == torch.tensor(remove_indices.size()).prod()
 
-        for layer_index in range(self.n_layers):
-            mean_values_layer = mean_values[layer_index] if use_means else None
+        for layer_index in range(self.cfg.n_layers):
+            layer_mean_activation = mean_activation[layer_index] if use_means else None
             self.delete_attn_pre_out_layer( layer_index,
-                remove_indices[layer_index], mean_values_layer )
+                remove_indices[layer_index], layer_mean_activation )
 
         return self
 
+    def delete_attn_values( self, remove_indices, mean_activation ):
+        """Does the same thing as delete_attn_pre_out"""
+        return self.delete_attn_pre_out( remove_indices, mean_activation )
+
+    def expand_remove_heads_to_remove_indices( self, remove_heads ):
+        # Check that the size for remove_heads is correct
+        if remove_heads.size() != torch.Size([ self.cfg.n_layers, self.cfg.n_heads ]):
+            raise ValueError( "Removals must have dimension [n_layers, n_heads]" )
+        remove_indices = remove_heads.unsqueeze(-1).expand([
+            self.cfg.n_layers, self.cfg.n_heads, self.cfg.d_head])
+        return remove_indices
+
     def delete_attn_pre_out_heads( self,
             remove_heads: Tensor,
             means: Tensor = None,
         ):
         """remove specific attention heads from model, and optionally offset
         activation by some mean activation
 
         Args:
             remove_heads (Tensor): tensor of model heads to remove of size
                 [n_layers, n_heads], with value True if you want to remove it
             means (Tensor, optional): tensor of means to offset activations by.
                 Defaults to None.
         """
-        # Check that the size for remove_heads is correct
-        if remove_heads.size() != torch.Size([ self.n_layers, self.n_heads ]):
-            raise ValueError( "Removals must have dimension [n_layers, n_heads]" )
-
-        # Convert 'heads' tensor into 'individual neurons' tensor
-        remove_indices = remove_heads.unsqueeze(-1).expand([
-            self.n_layers, self.n_heads, self.d_head])
+        remove_indices = self.expand_remove_heads_to_remove_indices(remove_heads)
 
         # delete heads in each layer
-        for layer in range(self.n_layers):
+        for layer in range(self.cfg.n_layers):
             # if using means, get means for current layer
             if means is None:
                 means_i = None
             else:
                 means_i = means[layer].flatten()
-                assert means_i.size() == torch.Size([ self.d_model ])
+                assert means_i.size() == torch.Size([ self.cfg.d_model ])
 
             self.delete_attn_pre_out_layer( layer, remove_indices[layer], means_i )
 
     # Functions for calculating feed-forward fully connected layer activations
     def calculate_ff_keys_layer( self,
             ff_in: Tensor,
             layer: int,
             use_activation_function: bool = True,
         ):
-        u = self.model.decoder.layers[ layer ]
-        x = u.final_layer_norm( ff_in )
-        x = u.fc1( x )
+        u = self.layers[ layer ]
+        x = u["ln2"]( ff_in )
+        x = u["fc1"]( x )
         if use_activation_function:
-            x = u.activation_fn( x )
+            x = u["activation_fn"]( x )
         return x
 
     def calculate_ff_keys( self,
             ff_in: Tensor,
             use_activation_function: bool = True
         ):
         out = []
@@ -601,36 +726,39 @@
             out.append(
                 self.calculate_ff_keys_layer( ff_in_layer, layer_index,
                     use_activation_function=use_activation_function )
             )
         return self.out_stack( out )
 
     def calculate_ff_out_layer( self, ff_in: Tensor, layer: int):
-        u = self.model.decoder.layers[ layer ]
-        x = u.final_layer_norm( ff_in )
-        x = u.fc1( x )
-        x = u.activation_fn( x )
-        x = u.fc2( x )
+        u = self.layers[ layer ]
+        x = u["ln2"]( ff_in )
+        x = u["fc1"]( x )
+        x = u["activation_fn"]( x )
+        x = u["fc2"]( x )
         return x
 
     def calculate_ff_out( self, ff_in: Tensor, add_residual: bool = False ):
         out = []
         for layer_index, ff_in_layer in enumerate(ff_in):
             ff_out = self.calculate_ff_out_layer( ff_in_layer, layer_index )
             if add_residual:
                 ff_out += ff_in[layer_index]
             out.append( ff_out )
         return self.out_stack( out )
 
     # functions for 'deleting' neurons from the MLP mid layers
     def delete_ff_keys( self, layer_key_map: Tensor ):
-        for layer, key_map in enumerate(layer_key_map):
-            # 2. Delete the weights going into ff key so it never activates
-            ff_in = self.model.decoder.layers[ layer ].fc1
-            mlp_delete_rows(ff_in, key_map)
+        with torch.no_grad():
+            for layer_index, key_map in enumerate(layer_key_map):
+                # Delete the weights going into ff key so it never activates
+                layer = self.layers[layer_index]
+                W_in, b_in = layer["mlp.W_in"], layer["mlp.b_in"]
+                W_in, b_in = mlp_delete_rows_raw(key_map, W_in, b_in)
+                layer["mlp.W_in"], layer["mlp.b_in"] = W_in, b_in
 
         return self
 
     def delete_ff_keys_from_files( self, files: List[str] ):
         """Delete ff mid layer neurons from list of numpy files
         pointing to which neurons to delete.
 
@@ -648,34 +776,67 @@
             criteria += ff_criterion
 
             sums = [ x.sum() for x in ff_criterion ]
             print( f"%5d - {sums}" % np.sum(sums) )
 
         self.delete_ff_keys( criteria )
 
-    # Next token prediction, show tokens
-    def predict( self, text : str, num: int = 10, limit: Optional[int] = None ):
+    def generate(self,
+            text: str,
+            num: int = 10,
+            do_sample: bool = True,
+            temperature: float = 0.7,
+            limit: int = None,
+            **kwargs,
+        ):
         """ Predict the next {num} tokens from an input {text}."""
 
         inputs = self.tokenizer( text, return_tensors="pt" )
         input_ids = inputs.input_ids.to( self.device )
 
         if limit:
             input_ids = input_ids[0][:limit].reshape(1, -1)
 
+        attn_mask = None
+        if hasattr(self.tokenizer, "pad_token_id"):
+            attn_mask = torch.ones_like(input_ids).bool()
+            for index, _id in enumerate(attn_mask[0]):
+                if _id == self.tokenizer.pad_token_id:
+                    attn_mask[index] = 0
+
+        # Hard code GPT2 Tokeniser pad_token_id to avoid warnings
+        if self.cfg.architecture == "GPT2LMHeadModel":
+            if not "pad_token_id" in kwargs:
+                kwargs["pad_token_id"] = 50256
+
         new_len = len(input_ids[0])+num
-        generate_ids = self.predictor.generate( input_ids, max_length=new_len )
+        generate_ids = self.predictor.generate( input_ids, max_length=new_len,
+            do_sample=do_sample, temperature=temperature,
+            attention_mask=attn_mask, **kwargs)
+        #import inspect
+        #print(inspect.getsource(self.predictor.generate))
+        #print(temperature)
 
         before = self.tokenizer.batch_decode( input_ids,
             skip_special_tokens=True, clean_up_tokenization_spaces=False )[0]
         after  = self.tokenizer.batch_decode( generate_ids,
             skip_special_tokens=True, clean_up_tokenization_spaces=False )[0]
         after = after[ len(before): ]
         return before, after
 
+    # Next token prediction, show tokens
+    def predict(self,
+            text: str,
+            num: int = 10,
+            limit: int = None,
+            ):
+        """ Predict the next {num} tokens from an input {text}."""
+
+        return self.generate( text, num, do_sample=False, limit=limit )
+
     def get_kth_tokens( self, output: Tensor, k: int = 16 ):
         n_tokens = output.size()[self.token_index]
         indices = torch.tensor( list(range( k-1, n_tokens, k )) )
 
         return torch.index_select( output, self.token_index, indices )
 
     def unembed( self, embedded_outputs: Tensor ):
@@ -705,15 +866,15 @@
             logits: Optional[Tensor] = None,
             start_index: int = 1,
             skip_strings: Optional[List[str]] = None,
         ):
         """Evaluates performance with top-1 and top-k token predictions.
 
         Args:
-            text (str, optional): The text to evaluat.
+            text (str, optional): The text to evaluate.
             input_ids (Tensor, optional): The input IDs from text to evaluate.
             logits (Tensor, optional): The pre-computed logits from text to evaluate.
             k (int): the number of tokens to consider.
             start_index (int, optional): The starting index from which to count.
                 Defaults to 1.
             skip_strings (List[str], optional): Tokens to skip when evaluating.
                 Defaults to [].
@@ -737,14 +898,17 @@
         skip_strings = [] if (skip_strings is None) else skip_strings
         for skip_string in skip_strings:
             skip_id = int( self.get_ids( skip_string ).squeeze(dim=0)[-1] )
             skip_ids.add( skip_id )
 
         # Count top-k prediction accuracy
         input_ids = input_ids.squeeze()
+        # Edge case: if input_ids is a single token, convert it back into a list
+        if len(input_ids.size()) == 0:
+            input_ids = torch.tensor([ input_ids ])
         num_predictions = 0
         num_accurate = 0
         num_topk_accurate = 0
         num_skip_predictions = 0
         num_skip_accurate = 0
         num_topk_skip_accurate = 0
         for i in range( start_index, len(input_ids) ):
@@ -763,14 +927,16 @@
             num_skip_predictions   += 1
             num_skip_accurate      += is_accurate
             num_topk_skip_accurate += is_topk_accurate
 
         # Keep track of most used tokens
         token_counts = np.zeros( token_dictionary_size )
         for input_id in input_ids:
+            if input_id > token_dictionary_size:
+                continue # Not sure why I need this, but for some reason I do
             token_counts[input_id] += 1
 
         output = {
             'num_predictions'  : num_predictions,
             'num_accurate'     : num_accurate,
             'num_topk_accurate': num_topk_accurate,
             'num_skip_predictions'  : num_skip_predictions,
@@ -788,15 +954,15 @@
             text: Optional[str] = None,
             input_ids: Optional[Tensor] = None,
             logits: Optional[Tensor] = None
         ):
         """Cross entropy loss for predicting the next token
 
         Args:
-            text (str, optional): The text to evaluat.
+            text (str, optional): The text to evaluate.
             input_ids (Tensor, optional): The input IDs from text to evaluate.
             logits (Tensor, optional): The pre-computed logits from text to evaluate.
 
         Returns:
             loss: Mean Cross-Entropy loss over tokens
         """
         if text is None and input_ids is None:
@@ -829,35 +995,44 @@
             "base"      : (100 * out["num_accurate"] / pred),
             "skip"      : (100 * out["num_skip_accurate"] / skip_pred),
         }
         if string:
             percent = { k: ( "%.2f" % v ) for k, v in percent.items() }
         return percent
 
+    def default_generator(self, dataset, dataset_text_label):
+        token_limit = self.limit
+        for data in dataset:
+            # predict next token from text
+            text = data[ dataset_text_label ]
+            with torch.no_grad():
+                input_ids = self.get_ids( text, token_limit )
+                logits = self.get_all_logits( input_ids )
+
+            yield (input_ids, logits)
+
     def evaluate_dataset( self,
-            dataset: Dataset,
-            dataset_text_label: str = 'content',
+            generator: Callable,
             k: int = 10,
             start_index: int = 1,
             skip_eval: Optional[List[str]] = None,
             sample_size: int = 1e5,
-            token_limit: Optional[int] = None,
             count_tokens: bool = False,
             num_top_tokens: int = 50,
             loading_bar_desc: str = "Acc",
             ):
         """An evaluation of next-token prediction accuracy for an iterable Dataset,
         which includes options for topk evaluation as well as skipping the most
-        commonly occuring tokens.
+        commonly occurring tokens.
 
         Args:
             dataset (datasets.Dataset): the Datset object to iterate over.
             dataset_text_label (str, optional): The label for the dataset text.
                 eg: 'text'. 'content'. Defaults to 'content'.
-            k (int, optional): Number of topk tokens to look at when asessing
+            k (int, optional): Number of topk tokens to look at when assessing
                 the accuracy of the model (in addition to top1). Defaults to 10.
             start_index (int, optional): The index of the first token to evaluate.
                 Defaults to 1.
             skip_eval (list, optional): A list of token IDs to skip when evaluating.
                 Defaults to [].
             sample_size (int, optional): The number of tokens to evaluate.
                 Defaults to 1e5.
@@ -866,15 +1041,15 @@
             count_tokens (bool, optional): . Defaults to False.
             num_top_tokens (int, optional): If count_tokens is true, this number
                 determines the number of top most-common accurate token predictions
                 to output when counting tokens. Defaults to 50.
 
         Returns:
             dict: A dictionary which contains counts of #predictions and #accurate
-                accross various the various possible combinations of outputs,
+                across various the various possible combinations of outputs,
                 as well as a sub dict 'percent' which contains percentage accuracy.
         """
 
         # Initialize variables
         token_counts = None
         out = {
             "num_predictions": 0,
@@ -887,21 +1062,15 @@
         }
         loss_tracker = Welford()
 
         # Set up approx stopping index
         with tqdm(total=sample_size) as pbar:
 
             # Loop over the dataset
-            for data in dataset:
-                # predict next token from text
-                text = data[ dataset_text_label ]
-                with torch.no_grad():
-                    input_ids = self.get_ids( text, token_limit )
-                    logits = self.get_all_logits( input_ids )
-
+            for (input_ids, logits) in generator:
                 # perform evaluations
                 topk =  self.evaluate_top_k_performance( k, input_ids=input_ids,
                     logits=logits, start_index=start_index, skip_strings=skip_eval )
                 loss = self.evaluate_ce_loss( input_ids=input_ids, logits=logits )
 
                 # Record performance
                 loss_tracker.add( loss.detach() )
```

### Comparing `separability-0.1.4/src/separability/model_repos.py` & `separability-0.9.0/src/separability/model_repos.py`

 * *Files identical despite different names*

### Comparing `separability-0.1.4/PKG-INFO` & `separability-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: separability
-Version: 0.1.4
-Summary: separability of LLM Capabilities
+Version: 0.9.0
+Summary: LLM Tools for looking at separability of LLM Capabilities
 Home-page: https://github.com/pesvut/separability
 Author: Nicky Pochinkov
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: accelerate (>=0.16.0,<0.17.0)
+Requires-Dist: accelerate (>=0.21.0,<0.22.0)
+Requires-Dist: bitsandbytes (>=0.40.2,<0.41.0)
+Requires-Dist: celery (>=5.3.1,<6.0.0)
 Requires-Dist: datasets (>=2.9.0,<3.0.0)
 Requires-Dist: dict-deep (>=4.1.2,<5.0.0)
 Requires-Dist: einops (>=0.6.0,<0.7.0)
 Requires-Dist: evaluate (>=0.4.0,<0.5.0)
 Requires-Dist: ipykernel (>=6.21.1,<7.0.0)
 Requires-Dist: ipywidgets (>=8.0.4,<9.0.0)
 Requires-Dist: matplotlib (>=3.6.3,<4.0.0)
 Requires-Dist: numexpr (>=2.7.0,<3.0.0)
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: scipy (>=1.11.1,<2.0.0)
+Requires-Dist: sentencepiece (>=0.1.99,<0.2.0)
 Requires-Dist: tensorboard (>=2.11.2,<3.0.0)
 Requires-Dist: tensorboardx (>=2.5.1,<3.0.0)
-Requires-Dist: torch (>=1.13.0,<2.0.0)
-Requires-Dist: transformers (>=4.26.0,<5.0.0)
+Requires-Dist: tokenizers (>=0.13.3,<0.14.0)
+Requires-Dist: torch (>=2.0.1,<3.0.0)
+Requires-Dist: transformers (>=4.30.0,<5.0.0)
 Requires-Dist: wandb (>=0.13.9,<0.14.0)
 Requires-Dist: welford-torch (>=0.1.2,<0.2.0)
 Requires-Dist: zstandard (>=0.19.0,<0.20.0)
 Project-URL: Repository, https://github.com/pesvut/separability
 Description-Content-Type: text/markdown
 
 # separability
@@ -42,15 +45,16 @@
 ## Pruning based on Capabilities
 
 For a full example, see `src/separability.ipynb`.
 
 The simple example is:
 ```
 from model import Model
-from activations import prune_and_evaluate, evaluate_all
+from activations import prune_and_evaluate
+from separability.eval import evaluate_all
 
 # Load and Evaluate Model on Pile and Code
 
 opt = Model('125m', limit=1000)
 eval_data = evaluate_all(opt, 1e5)
 print(eval_data)
```

