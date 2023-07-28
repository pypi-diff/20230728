# Comparing `tmp/VN-transformer-0.0.2.tar.gz` & `tmp/VN-transformer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VN-transformer-0.0.2.tar", last modified: Fri Jul 28 17:26:14 2023, max compression
+gzip compressed data, was "VN-transformer-0.0.3.tar", last modified: Fri Jul 28 17:56:31 2023, max compression
```

## Comparing `VN-transformer-0.0.2.tar` & `VN-transformer-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:26:14.981051 VN-transformer-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 17:26:04.000000 VN-transformer-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 17:26:14.981051 VN-transformer-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-28 17:26:04.000000 VN-transformer-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:26:14.981051 VN-transformer-0.0.2/VN_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-07-28 17:26:04.000000 VN-transformer-0.0.2/VN_transformer/VN_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-28 17:26:04.000000 VN-transformer-0.0.2/VN_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 17:26:04.000000 VN-transformer-0.0.2/VN_transformer/rotations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:26:14.981051 VN-transformer-0.0.2/VN_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 17:26:14.000000 VN-transformer-0.0.2/VN_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 17:26:14.000000 VN-transformer-0.0.2/VN_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:26:14.000000 VN-transformer-0.0.2/VN_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 17:26:14.000000 VN-transformer-0.0.2/VN_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 17:26:14.000000 VN-transformer-0.0.2/VN_transformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 17:26:14.981051 VN-transformer-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-28 17:26:04.000000 VN-transformer-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:26:14.981051 VN-transformer-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-28 17:26:04.000000 VN-transformer-0.0.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:56:31.107891 VN-transformer-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 17:56:20.000000 VN-transformer-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 17:56:31.107891 VN-transformer-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-28 17:56:20.000000 VN-transformer-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:56:31.107891 VN-transformer-0.0.3/VN_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-07-28 17:56:20.000000 VN-transformer-0.0.3/VN_transformer/VN_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-28 17:56:20.000000 VN-transformer-0.0.3/VN_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 17:56:20.000000 VN-transformer-0.0.3/VN_transformer/rotations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:56:31.107891 VN-transformer-0.0.3/VN_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 17:56:31.000000 VN-transformer-0.0.3/VN_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 17:56:31.000000 VN-transformer-0.0.3/VN_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:56:31.000000 VN-transformer-0.0.3/VN_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 17:56:31.000000 VN-transformer-0.0.3/VN_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 17:56:31.000000 VN-transformer-0.0.3/VN_transformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 17:56:31.107891 VN-transformer-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-28 17:56:20.000000 VN-transformer-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:56:31.107891 VN-transformer-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-28 17:56:20.000000 VN-transformer-0.0.3/tests/test.py
```

### Comparing `VN-transformer-0.0.2/LICENSE` & `VN-transformer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `VN-transformer-0.0.2/PKG-INFO` & `VN-transformer-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VN-transformer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Vector Neuron Transformer (VN-Transformer)
 Home-page: https://github.com/lucidrains/VN-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,vector neurons,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VN-transformer-0.0.2/README.md` & `VN-transformer-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -18,19 +18,20 @@
 import torch
 from VN_transformer import VNTransformer
 
 model = VNTransformer(
     dim = 64,
     depth = 2,
     dim_head = 64,
-    heads = 8
+    heads = 8,
+    beta_epsilon = 1e-6  # in this paper, they propose breaking equivariance with a tiny bit of bias noise in the VN linear. they claim this leads to improved stability. setting this to 0 would turn off the epsilon approximate equivariance
 )
 
 feats = torch.randn(1, 32, 64)
-coors = torch.randn(1, 32, 3)
+coors = torch.randn(1, 32, 3)    # (batch, sequence, spatial coordinates)
 
 feats, coors = model(feats, coors)
 ```
 
 ## Tests
 
 Confidence in equivariance
```

#### html2text {}

```diff
@@ -1,16 +1,20 @@
 [./vn-transformer.png] ## VN (Vector Neuron) Transformer (wip) A Transformer
 made_of_Rotation-equivariant_Attention using Vector_Neurons Open_Review ##
 Install ```bash $ pip install VN-transformer ``` ## Usage ```python import
 torch from VN_transformer import VNTransformer model = VNTransformer( dim = 64,
-depth = 2, dim_head = 64, heads = 8 ) feats = torch.randn(1, 32, 64) coors =
-torch.randn(1, 32, 3) feats, coors = model(feats, coors) ``` ## Tests
-Confidence in equivariance ```bash $ python setup.py test ``` ## Citations
-```bibtex @inproceedings{Assaad2022VNTransformerRA, title = {VN-Transformer:
-Rotation-Equivariant Attention for Vector Neurons}, author = {Serge Assaad and
-C. Downey and Rami Al-Rfou and Nigamaa Nayakanti and Benjamin Sapp}, year =
-{2022} } ``` ```bibtex @article{Deng2021VectorNA, title = {Vector Neurons: A
-General Framework for SO(3)-Equivariant Networks}, author = {Congyue Deng and
-Or Litany and Yueqi Duan and Adrien Poulenard and Andrea Tagliasacchi and
-Leonidas J. Guibas}, journal = {2021 IEEE/CVF International Conference on
-Computer Vision (ICCV)}, year = {2021}, pages = {12180-12189}, url = {https://
-api.semanticscholar.org/CorpusID:233394028} } ```
+depth = 2, dim_head = 64, heads = 8, beta_epsilon = 1e-6 # in this paper, they
+propose breaking equivariance with a tiny bit of bias noise in the VN linear.
+they claim this leads to improved stability. setting this to 0 would turn off
+the epsilon approximate equivariance ) feats = torch.randn(1, 32, 64) coors =
+torch.randn(1, 32, 3) # (batch, sequence, spatial coordinates) feats, coors =
+model(feats, coors) ``` ## Tests Confidence in equivariance ```bash $ python
+setup.py test ``` ## Citations ```bibtex @inproceedings
+{Assaad2022VNTransformerRA, title = {VN-Transformer: Rotation-Equivariant
+Attention for Vector Neurons}, author = {Serge Assaad and C. Downey and Rami
+Al-Rfou and Nigamaa Nayakanti and Benjamin Sapp}, year = {2022} } ``` ```bibtex
+@article{Deng2021VectorNA, title = {Vector Neurons: A General Framework for SO
+(3)-Equivariant Networks}, author = {Congyue Deng and Or Litany and Yueqi Duan
+and Adrien Poulenard and Andrea Tagliasacchi and Leonidas J. Guibas}, journal =
+{2021 IEEE/CVF International Conference on Computer Vision (ICCV)}, year =
+{2021}, pages = {12180-12189}, url = {https://api.semanticscholar.org/CorpusID:
+233394028} } ```
```

### Comparing `VN-transformer-0.0.2/VN_transformer/VN_transformer.py` & `VN-transformer-0.0.3/VN_transformer/VN_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         self.scale = (dim_coor * dim_head) ** -0.5
         dim_inner = dim_head * heads
         self.heads = heads
 
         self.to_qkv = VNLinear(dim, dim_inner * 3, bias_epsilon = bias_epsilon)
         self.to_out = VNLinear(dim_inner, dim, bias_epsilon = bias_epsilon)
 
-    def forward(self, x):
+    def forward(self, x, mask = None):
         """
         einstein notation
         b - batch
         n - sequence
         h - heads
         d - feature dimension (channels)
         c - coordinate dimension (3 for 3d space)
@@ -111,14 +111,18 @@
         q, k, v = self.to_qkv(x).chunk(3, dim = -2)
         q, k, v = map(lambda t: rearrange(t, 'b n (h d) c -> b h n d c', h = self.heads), (q, k, v))
 
         q = q * self.scale
 
         sim = einsum('b h i d c, b h j d c -> b h i j', q, k)
 
+        if exists(mask):
+            mask = rearrange(mask, 'b j -> b 1 1 j')
+            sim = sim.masked_fill(~mask, -torch.finfo(sim.dtype).max)
+
         attn = sim.softmax(dim = -1)
 
         out = einsum('b h i j, b h j d c -> b h i d c', attn, v)
 
         out = rearrange(out, 'b h n d c -> b n (h d) c')
         return self.to_out(out)
 
@@ -179,15 +183,15 @@
         mask = None
     ):
         *_, d, c = x.shape
 
         assert x.ndim == 4 and d == self.dim and c == self.dim_coor, 'input needs to be in the shape of (batch, seq, dim ({self.dim}), coordinate dim ({self.dim_coor}))'
 
         for attn, attn_post_ln, ff, ff_post_ln in self.layers:
-            x = attn_post_ln(attn(x)) + x
+            x = attn_post_ln(attn(x, mask = mask)) + x
             x = ff_post_ln(ff(x)) + x
 
         return self.norm(x)
 
 # invariant layers
 
 class VNInvariant(nn.Module):
@@ -247,10 +251,10 @@
     def forward(
         self,
         feats,
         coors,
         mask = None
     ):
         coors = self.vn_proj_in(coors)
-        coors = self.encoder(coors)
+        coors = self.encoder(coors, mask = mask)
         coors = self.vn_proj_out(coors)
         return feats, coors
```

### Comparing `VN-transformer-0.0.2/VN_transformer.egg-info/PKG-INFO` & `VN-transformer-0.0.3/VN_transformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VN-transformer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Vector Neuron Transformer (VN-Transformer)
 Home-page: https://github.com/lucidrains/VN-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,vector neurons,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VN-transformer-0.0.2/setup.py` & `VN-transformer-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'VN-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'Vector Neuron Transformer (VN-Transformer)',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/VN-transformer',
   keywords = [
```

### Comparing `VN-transformer-0.0.2/tests/test.py` & `VN-transformer-0.0.3/tests/test.py`

 * *Files identical despite different names*

