# Comparing `tmp/siren-pytorch-0.1.6.tar.gz` & `tmp/siren-pytorch-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siren-pytorch-0.1.6.tar", last modified: Fri Dec  3 18:59:26 2021, max compression
+gzip compressed data, was "siren-pytorch-0.1.7.tar", last modified: Fri Jul 28 14:59:34 2023, max compression
```

## Comparing `siren-pytorch-0.1.6.tar` & `siren-pytorch-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-03 18:59:26.171754 siren-pytorch-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2021-12-03 18:59:17.000000 siren-pytorch-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      611 2021-12-03 18:59:26.171754 siren-pytorch-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4368 2021-12-03 18:59:17.000000 siren-pytorch-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-03 18:59:26.171754 siren-pytorch-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      733 2021-12-03 18:59:17.000000 siren-pytorch-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-03 18:59:26.171754 siren-pytorch-0.1.6/siren_pytorch/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-12-03 18:59:17.000000 siren-pytorch-0.1.6/siren_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4748 2021-12-03 18:59:17.000000 siren-pytorch-0.1.6/siren_pytorch/siren_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-03 18:59:26.171754 siren-pytorch-0.1.6/siren_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      611 2021-12-03 18:59:25.000000 siren-pytorch-0.1.6/siren_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      267 2021-12-03 18:59:26.000000 siren-pytorch-0.1.6/siren_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-03 18:59:25.000000 siren-pytorch-0.1.6/siren_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-12-03 18:59:25.000000 siren-pytorch-0.1.6/siren_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-12-03 18:59:25.000000 siren-pytorch-0.1.6/siren_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:59:34.148167 siren-pytorch-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 14:59:24.000000 siren-pytorch-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-28 14:59:34.148167 siren-pytorch-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-28 14:59:24.000000 siren-pytorch-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 14:59:34.148167 siren-pytorch-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-28 14:59:24.000000 siren-pytorch-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:59:34.148167 siren-pytorch-0.1.7/siren_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 14:59:24.000000 siren-pytorch-0.1.7/siren_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-07-28 14:59:24.000000 siren-pytorch-0.1.7/siren_pytorch/siren_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:59:34.148167 siren-pytorch-0.1.7/siren_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-28 14:59:34.000000 siren-pytorch-0.1.7/siren_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-28 14:59:34.000000 siren-pytorch-0.1.7/siren_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:59:34.000000 siren-pytorch-0.1.7/siren_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 14:59:34.000000 siren-pytorch-0.1.7/siren_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 14:59:34.000000 siren-pytorch-0.1.7/siren_pytorch.egg-info/top_level.txt
```

### Comparing `siren-pytorch-0.1.6/LICENSE` & `siren-pytorch-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `siren-pytorch-0.1.6/PKG-INFO` & `siren-pytorch-0.1.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: siren-pytorch
-Version: 0.1.6
+Version: 0.1.7
 Summary: Implicit Neural Representations with Periodic Activation Functions
 Home-page: https://github.com/lucidrains/siren-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `siren-pytorch-0.1.6/README.md` & `siren-pytorch-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `siren-pytorch-0.1.6/setup.py` & `siren-pytorch-0.1.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'siren-pytorch',
   packages = find_packages(),
-  version = '0.1.6',
+  version = '0.1.7',
   license='MIT',
   description = 'Implicit Neural Representations with Periodic Activation Functions',
+  long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/siren-pytorch',
   keywords = ['artificial intelligence', 'deep learning'],
   install_requires=[
       'einops',
       'torch'
```

### Comparing `siren-pytorch-0.1.6/siren_pytorch/siren_pytorch.py` & `siren-pytorch-0.1.7/siren_pytorch/siren_pytorch.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,62 +20,88 @@
         self.w0 = w0
     def forward(self, x):
         return torch.sin(self.w0 * x)
 
 # siren layer
 
 class Siren(nn.Module):
-    def __init__(self, dim_in, dim_out, w0 = 1., c = 6., is_first = False, use_bias = True, activation = None):
+    def __init__(
+        self,
+        dim_in,
+        dim_out,
+        w0 = 1.,
+        c = 6.,
+        is_first = False,
+        use_bias = True,
+        activation = None,
+        dropout = 0.
+    ):
         super().__init__()
         self.dim_in = dim_in
         self.is_first = is_first
 
         weight = torch.zeros(dim_out, dim_in)
         bias = torch.zeros(dim_out) if use_bias else None
         self.init_(weight, bias, c = c, w0 = w0)
 
         self.weight = nn.Parameter(weight)
         self.bias = nn.Parameter(bias) if use_bias else None
         self.activation = Sine(w0) if activation is None else activation
+        self.dropout = nn.Dropout(dropout)
 
     def init_(self, weight, bias, c, w0):
         dim = self.dim_in
 
         w_std = (1 / dim) if self.is_first else (math.sqrt(c / dim) / w0)
         weight.uniform_(-w_std, w_std)
 
         if exists(bias):
             bias.uniform_(-w_std, w_std)
 
     def forward(self, x):
         out =  F.linear(x, self.weight, self.bias)
         out = self.activation(out)
+        out = self.dropout(out)
         return out
 
 # siren network
 
 class SirenNet(nn.Module):
-    def __init__(self, dim_in, dim_hidden, dim_out, num_layers, w0 = 1., w0_initial = 30., use_bias = True, final_activation = None):
+    def __init__(
+        self,
+        dim_in,
+        dim_hidden,
+        dim_out,
+        num_layers,
+        w0 = 1.,
+        w0_initial = 30.,
+        use_bias = True,
+        final_activation = None,
+        dropout = 0.
+    ):
         super().__init__()
         self.num_layers = num_layers
         self.dim_hidden = dim_hidden
 
         self.layers = nn.ModuleList([])
         for ind in range(num_layers):
             is_first = ind == 0
             layer_w0 = w0_initial if is_first else w0
             layer_dim_in = dim_in if is_first else dim_hidden
 
-            self.layers.append(Siren(
+            layer = Siren(
                 dim_in = layer_dim_in,
                 dim_out = dim_hidden,
                 w0 = layer_w0,
                 use_bias = use_bias,
-                is_first = is_first
-            ))
+                is_first = is_first,
+                dropout = dropout
+            )
+
+            self.layers.append(layer)
 
         final_activation = nn.Identity() if not exists(final_activation) else final_activation
         self.last_layer = Siren(dim_in = dim_hidden, dim_out = dim_out, w0 = w0, use_bias = use_bias, activation = final_activation)
 
     def forward(self, x, mods = None):
         mods = cast_tuple(mods, self.num_layers)
```

### Comparing `siren-pytorch-0.1.6/siren_pytorch.egg-info/PKG-INFO` & `siren-pytorch-0.1.7/siren_pytorch.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: siren-pytorch
-Version: 0.1.6
+Version: 0.1.7
 Summary: Implicit Neural Representations with Periodic Activation Functions
 Home-page: https://github.com/lucidrains/siren-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
-
-UNKNOWN
-
```

