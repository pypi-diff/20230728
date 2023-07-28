# Comparing `tmp/audio-diffusion-pytorch-fork-0.0.103.tar.gz` & `tmp/audio-diffusion-pytorch-fork-0.0.104.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio-diffusion-pytorch-fork-0.0.103.tar", last modified: Mon Jul 17 20:36:21 2023, max compression
+gzip compressed data, was "audio-diffusion-pytorch-fork-0.0.104.tar", last modified: Fri Jul 28 19:44:59 2023, max compression
```

## Comparing `audio-diffusion-pytorch-fork-0.0.103.tar` & `audio-diffusion-pytorch-fork-0.0.104.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-17 20:36:21.000000 audio-diffusion-pytorch-fork-0.0.103/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1068 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.103/LICENSE
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      626 2023-07-17 20:36:21.000000 audio-diffusion-pytorch-fork-0.0.103/PKG-INFO
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    12252 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.103/README.md
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-17 20:36:21.000000 audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      832 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    22680 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork/diffusion.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    15989 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork/model.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    47073 2023-07-17 20:35:21.000000 audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork/modules.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3609 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork/utils.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-17 20:36:21.000000 audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork.egg-info/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      626 2023-07-17 20:36:21.000000 audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork.egg-info/PKG-INFO
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      499 2023-07-17 20:36:21.000000 audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork.egg-info/SOURCES.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        1 2023-07-17 20:36:21.000000 audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork.egg-info/dependency_links.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      115 2023-07-17 20:36:21.000000 audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork.egg-info/requires.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       29 2023-07-17 20:36:21.000000 audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork.egg-info/top_level.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       80 2023-07-13 19:38:47.000000 audio-diffusion-pytorch-fork-0.0.103/pyproject.toml
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       38 2023-07-17 20:36:21.000000 audio-diffusion-pytorch-fork-0.0.103/setup.cfg
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      976 2023-07-17 20:35:18.000000 audio-diffusion-pytorch-fork-0.0.103/setup.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-28 19:44:59.000000 audio-diffusion-pytorch-fork-0.0.104/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1068 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.104/LICENSE
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      626 2023-07-28 19:44:59.000000 audio-diffusion-pytorch-fork-0.0.104/PKG-INFO
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    12252 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.104/README.md
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-28 19:44:59.000000 audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      832 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    22680 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork/diffusion.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    15989 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork/model.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    47856 2023-07-21 04:40:14.000000 audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork/modules.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3609 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork/utils.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-28 19:44:59.000000 audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork.egg-info/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      626 2023-07-28 19:44:59.000000 audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork.egg-info/PKG-INFO
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      499 2023-07-28 19:44:59.000000 audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        1 2023-07-28 19:44:59.000000 audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      115 2023-07-28 19:44:59.000000 audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork.egg-info/requires.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       29 2023-07-28 19:44:59.000000 audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork.egg-info/top_level.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       80 2023-07-13 19:38:47.000000 audio-diffusion-pytorch-fork-0.0.104/pyproject.toml
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       38 2023-07-28 19:44:59.000000 audio-diffusion-pytorch-fork-0.0.104/setup.cfg
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      976 2023-07-28 19:44:05.000000 audio-diffusion-pytorch-fork-0.0.104/setup.py
```

### Comparing `audio-diffusion-pytorch-fork-0.0.103/LICENSE` & `audio-diffusion-pytorch-fork-0.0.104/LICENSE`

 * *Files identical despite different names*

### Comparing `audio-diffusion-pytorch-fork-0.0.103/PKG-INFO` & `audio-diffusion-pytorch-fork-0.0.104/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-diffusion-pytorch-fork
-Version: 0.0.103
+Version: 0.0.104
 Summary: A fork of Flavio Schneider's Audio Diffusion - PyTorch
 Home-page: https://github.com/harmonai-org/audio-diffusion-pytorch-fork
 Author: Harmonai
 License: MIT
 Keywords: artificial intelligence,deep learning,audio generation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `audio-diffusion-pytorch-fork-0.0.103/README.md` & `audio-diffusion-pytorch-fork-0.0.104/README.md`

 * *Files identical despite different names*

### Comparing `audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork/__init__.py` & `audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork/__init__.py`

 * *Files identical despite different names*

### Comparing `audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork/diffusion.py` & `audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork/diffusion.py`

 * *Files identical despite different names*

### Comparing `audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork/model.py` & `audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork/model.py`

 * *Files identical despite different names*

### Comparing `audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork/modules.py` & `audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,15 +313,27 @@
         mid_features = head_features * num_heads
         out_features = default(out_features, features)
 
         self.to_out = nn.Linear(
             in_features=mid_features, out_features=out_features
         )
 
-        self.use_flash = version.parse(torch.__version__) >= version.parse('2.0.0')
+        self.use_flash = torch.cuda.is_available() and version.parse(torch.__version__) >= version.parse('2.0.0')
+
+        if not self.use_flash:
+            return
+
+        device_properties = torch.cuda.get_device_properties(torch.device('cuda'))
+
+        if device_properties.major == 8 and device_properties.minor == 0:
+            # Use flash attention for A100 GPUs
+            self.sdp_kernel_config = (True, False, False)
+        else:
+            # Don't use flash attention for other GPUs
+            self.sdp_kernel_config = (False, True, True)
 
     def forward(
         self, q: Tensor, k: Tensor, v: Tensor, mask: Optional[Tensor] = None
     ) -> Tensor:
         # Split heads
         q, k, v = rearrange_many((q, k, v), "b n (h d) -> b h n d", h=self.num_heads)
 
@@ -332,15 +344,15 @@
 
             # Get attention matrix with softmax
             attn = sim.softmax(dim=-1, dtype=torch.float32)
 
             # Compute values
             out = einsum("... n m, ... m d -> ... n d", attn, v)
         else:
-            with sdp_kernel(enable_flash = True, enable_math=False, enable_mem_efficient= False):
+            with sdp_kernel(*self.sdp_kernel_config):
                 out = F.scaled_dot_product_attention(q, k, v, is_causal=False)
 
         out = rearrange(out, "b h n d -> b n (h d)")
         return self.to_out(out)
 
 class Attention(nn.Module):
     def __init__(
@@ -1178,16 +1190,23 @@
                     batch_mask = torch.cat([embedding_mask, embedding_mask], dim=0)
 
                 batch_features = None
                 features = kwargs.pop("features", None)
                 if self.use_context_features:
                     batch_features = torch.cat([features, features], dim=0)
 
+                batch_channels = None
+                channels_list = kwargs.pop("channels_list", None)
+                if self.use_context_channels:
+                    batch_channels = []
+                    for channels in channels_list:
+                        batch_channels += [torch.cat([channels, channels], dim=0)]
+
                 # Compute both normal and fixed embedding outputs
-                batch_out = super().forward(batch_x, batch_time, embedding=batch_embed, embedding_mask=batch_mask, features=batch_features, **kwargs)
+                batch_out = super().forward(batch_x, batch_time, embedding=batch_embed, embedding_mask=batch_mask, features=batch_features, channels_list=batch_channels, **kwargs)
                 out, out_masked = batch_out.chunk(2, dim=0)
            
             else:
                 # Compute both normal and fixed embedding outputs
                 out = super().forward(x, time, embedding=embedding, embedding_mask=embedding_mask, **kwargs)
                 out_masked = super().forward(x, time, embedding=fixed_embedding, embedding_mask=embedding_mask, **kwargs)
```

### Comparing `audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork/utils.py` & `audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork/utils.py`

 * *Files identical despite different names*

### Comparing `audio-diffusion-pytorch-fork-0.0.103/audio_diffusion_pytorch_fork.egg-info/PKG-INFO` & `audio-diffusion-pytorch-fork-0.0.104/audio_diffusion_pytorch_fork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-diffusion-pytorch-fork
-Version: 0.0.103
+Version: 0.0.104
 Summary: A fork of Flavio Schneider's Audio Diffusion - PyTorch
 Home-page: https://github.com/harmonai-org/audio-diffusion-pytorch-fork
 Author: Harmonai
 License: MIT
 Keywords: artificial intelligence,deep learning,audio generation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `audio-diffusion-pytorch-fork-0.0.103/setup.py` & `audio-diffusion-pytorch-fork-0.0.104/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name="audio-diffusion-pytorch-fork",
     packages=find_packages(exclude=[]),
-    version="0.0.103",
+    version="0.0.104",
     license="MIT",
     description="A fork of Flavio Schneider's Audio Diffusion - PyTorch",
     long_description_content_type="text/markdown",
     author="Harmonai",
     url="https://github.com/harmonai-org/audio-diffusion-pytorch-fork",
     keywords=["artificial intelligence", "deep learning", "audio generation"],
     install_requires=[
```

