# Comparing `tmp/froog-0.1.7.tar.gz` & `tmp/froog-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froog-0.1.7.tar", last modified: Wed Jul 26 06:37:17 2023, max compression
+gzip compressed data, was "froog-0.1.8.tar", last modified: Fri Jul 28 04:16:39 2023, max compression
```

## Comparing `froog-0.1.7.tar` & `froog-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-26 06:37:17.079475 froog-0.1.7/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-07-16 20:10:22.000000 froog-0.1.7/LICENSE
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2451 2023-07-26 06:37:17.079350 froog-0.1.7/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2125 2023-07-26 06:32:22.000000 froog-0.1.7/README.md
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-26 06:37:17.077371 froog-0.1.7/froog/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       57 2023-07-26 06:32:22.000000 froog-0.1.7/froog/__init__.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2107 2023-07-26 06:32:22.000000 froog-0.1.7/froog/gradcheck.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)    10300 2023-07-26 06:32:22.000000 froog-0.1.7/froog/ops.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2016 2023-07-19 05:23:59.000000 froog-0.1.7/froog/optim.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     3803 2023-07-26 06:32:22.000000 froog-0.1.7/froog/tensor.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2685 2023-07-23 19:46:48.000000 froog-0.1.7/froog/utils.py
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-26 06:37:17.077931 froog-0.1.7/froog.egg-info/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2451 2023-07-26 06:37:17.000000 froog-0.1.7/froog.egg-info/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      350 2023-07-26 06:37:17.000000 froog-0.1.7/froog.egg-info/SOURCES.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-07-26 06:37:17.000000 froog-0.1.7/froog.egg-info/dependency_links.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       15 2023-07-26 06:37:17.000000 froog-0.1.7/froog.egg-info/requires.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        6 2023-07-26 06:37:17.000000 froog-0.1.7/froog.egg-info/top_level.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-07-26 06:37:17.079508 froog-0.1.7/setup.cfg
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      852 2023-07-26 06:36:29.000000 froog-0.1.7/setup.py
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-26 06:37:17.079074 froog-0.1.7/tests/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     3184 2023-07-26 06:32:22.000000 froog-0.1.7/tests/test_conv_speed.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     4256 2023-07-26 06:32:22.000000 froog-0.1.7/tests/test_mnist.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2949 2023-07-26 06:32:22.000000 froog-0.1.7/tests/test_ops.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2604 2023-07-26 06:32:22.000000 froog-0.1.7/tests/test_tensor.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-28 04:16:39.246644 froog-0.1.8/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-07-16 20:10:22.000000 froog-0.1.8/LICENSE
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2640 2023-07-28 04:16:39.246517 froog-0.1.8/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2315 2023-07-28 03:27:43.000000 froog-0.1.8/README.md
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-28 04:16:39.244341 froog-0.1.8/froog/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       57 2023-07-26 06:32:22.000000 froog-0.1.8/froog/__init__.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2104 2023-07-28 03:55:03.000000 froog-0.1.8/froog/gradcheck.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     1259 2023-07-28 03:37:44.000000 froog-0.1.8/froog/nn.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)    12095 2023-07-28 03:42:14.000000 froog-0.1.8/froog/ops.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     1986 2023-07-27 02:41:00.000000 froog-0.1.8/froog/optim.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     4114 2023-07-28 03:49:20.000000 froog-0.1.8/froog/tensor.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2710 2023-07-28 02:45:00.000000 froog-0.1.8/froog/utils.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-28 04:16:39.245040 froog-0.1.8/froog.egg-info/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2640 2023-07-28 04:16:39.000000 froog-0.1.8/froog.egg-info/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      382 2023-07-28 04:16:39.000000 froog-0.1.8/froog.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-07-28 04:16:39.000000 froog-0.1.8/froog.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       15 2023-07-28 04:16:39.000000 froog-0.1.8/froog.egg-info/requires.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        6 2023-07-28 04:16:39.000000 froog-0.1.8/froog.egg-info/top_level.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-07-28 04:16:39.246683 froog-0.1.8/setup.cfg
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      851 2023-07-28 04:16:31.000000 froog-0.1.8/setup.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-28 04:16:39.246210 froog-0.1.8/tests/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     3172 2023-07-28 03:44:46.000000 froog-0.1.8/tests/test_conv_speed.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     4256 2023-07-28 03:41:52.000000 froog-0.1.8/tests/test_mnist.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     3556 2023-07-28 03:26:43.000000 froog-0.1.8/tests/test_ops.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     1987 2023-07-27 02:40:39.000000 froog-0.1.8/tests/test_optim.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2604 2023-07-27 02:41:36.000000 froog-0.1.8/tests/test_tensor.py
```

### Comparing `froog-0.1.7/froog/gradcheck.py` & `froog-0.1.8/froog/gradcheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
   ji = input.data.reshape(-1).shape[-1]  # jacobian of input
   jo = output.data.reshape(-1).shape[-1] # jacobian of output
   J = np.zeros((jo, ji), dtype=np.float32)
 
   for o in range(jo):
     o_scalar = Tensor(mask_like(output.data, o, 1.)).mul(output).sum()
     o_scalar.backward()
-
     for i, grad in enumerate(input.grad.reshape(-1)):
       J[o,i] = grad
   return J
 
 def numerical_jacobian(model, input, eps = 1e-6):
 #     """
 #     https://timvieira.github.io/blog/post/2017/04/21/how-to-test-gradient-implementations/
@@ -31,18 +30,18 @@
 #     """
   output = model(input)
 
   ji = input.data.reshape(-1).shape[-1]
   jo = output.data.reshape(-1).shape[-1]
   NJ = np.zeros((jo, ji), dtype=np.float32)
 
-  for o in range(jo):
-    for i in range(ji):
+  for i in range(ji):
+    eps_perturb = mask_like(input.data, i, mask_value = eps)
+    for o in range(jo):
 
-      eps_perturb = mask_like(input.data, i, mask_value = eps)
       output_perturb_add = model(Tensor(input.data + eps_perturb)).data.reshape(-1)[o]
       output_perturb_sub = model(Tensor(input.data - eps_perturb)).data.reshape(-1)[o]
 
       grad_approx = ((output_perturb_add) - (output_perturb_sub)) / (2*eps) # CDM: (f(x + h) - f(x - h)) / (2 * h)
 
       NJ[o][i] = grad_approx
   return NJ
```

### Comparing `froog-0.1.7/froog/ops.py` & `froog-0.1.8/froog/ops.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,26 +14,47 @@
     return x + y
   
   @staticmethod
   def backward(ctx, grad_output):
     return grad_output, grad_output 
 register("add", Add)
 
+class Sub(Function): # x.sub(y)
+  @staticmethod
+  def forward(ctx, x, y):
+    return x-y
+
+  @staticmethod
+  def backward(ctx, grad_output):
+    return grad_output, -grad_output
+register('sub', Sub)
+
 class Mul(Function): # x.mul(y)
   @staticmethod
   def forward(ctx, x, y):
     ctx.save_for_backward(x, y)
     return x * y
 
   @staticmethod
   def backward(ctx, grad_output):
     x, y = ctx.saved_tensors
     return y * grad_output, x * grad_output
 register("mul", Mul)
 
+class Pow(Function): # x.pow(y)
+  @staticmethod
+  def forward(ctx, x, y):
+    ctx.save_for_backward(x, y)
+    return x ** y
+  
+  @staticmethod
+  def backward(ctx, grad_output):
+    x, y = ctx.saved_tensors
+    return y * (x**(y-1.0)) * grad_output, (x**y) * np.log(x) * grad_output # power rule, d/dx (y^x)
+register("pow", Pow)
 
 class Dot(Function):  # x.dot(y)
   @staticmethod
   def forward(ctx, input, weight):
     ctx.save_for_backward(input, weight)
     return input.dot(weight)
 
@@ -59,39 +80,68 @@
   def backward(ctx, grad_output):
     (input,) = ctx.saved_tensors
     return grad_output * np.ones_like(input)
 register("sum", Sum)
 
 # ******* nn ops *******
 
-class ReLU(Function): # max(0,x)
+class ReLU(Function): 
   @staticmethod
   def forward(ctx, input):
     ctx.save_for_backward(input)
-    return np.maximum(input, 0)
+    return np.maximum(input, 0) # relu(x) = max(0,x)
 
   @staticmethod
   def backward(ctx, grad_output):
-    (input,) = ctx.saved_tensors
+    input, = ctx.saved_tensors
     grad_input = grad_output * (input >= 0)
     return grad_input
 register("relu", ReLU)
 
+class Sigmoid(Function): 
+  @staticmethod
+  def forward(ctx, input):
+    ctx.save_for_backward(input)
+    with np.warnings.catch_warnings():           # TODO: stable sigmoid? does the overflow matter?
+      np.warnings.filterwarnings('ignore')
+      ret = 1/(1 + np.exp(-input))               # sigmoid(x) = 1 / (1 + exp(-x))
+    return ret 
+
+  @staticmethod
+  def backward(ctx, grad_output):
+    ret, = ctx.saved_tensors
+    grad_input = grad_output * (ret * (1 - ret)) # just take the derivative of sigmoid
+    return grad_input
+register("sigmoid", Sigmoid)
+
 class Reshape(Function):
   @staticmethod
   def forward(ctx, x, shape):
     ctx.save_for_backward(x.shape)
     return x.reshape(shape)
 
   @staticmethod
   def backward(ctx, grad_output):
     in_shape, = ctx.saved_tensors
-    return grad_output.reshape(in_shape), None
+    return grad_output.reshape(in_shape)
 register('reshape', Reshape)
 
+class Pad2D(Function):
+  """
+  The first element (0,0) corresponds to padding along the batch dimension, which indicates no padding on both sides (0 elements added).
+  """
+  @staticmethod
+  def forward(ctx, x, padding=None): 
+    return np.pad(x, ((0,0), (0,0), (padding[0], padding[1]), (padding[2], padding[3]))) # (top, bottom, left, right)
+
+  @staticmethod
+  def backward(ctx, grad_output):
+    raise Exception("write this")
+register('pad2d', Pad2D)
+
 class LogSoftmax(Function):
   """
   converts a vector of numbers into a vector of probabilities
   probabilities of each value are proportional to the scale of each value 
   """
   @staticmethod
   def forward(ctx, input):
@@ -109,15 +159,15 @@
     return grad_output - np.exp(output) * grad_output.sum(axis=1).reshape((-1, 1))
 register("logsoftmax", LogSoftmax)
 
 # ************* conv ops *************
 
 class Conv2D(Function): 
   @staticmethod
-  def forward(ctx, x, w, stride=1):
+  def forward(ctx, x, w, stride=1, groups=1):
     """
     https://github.com/vdumoulin/conv_arithmetic/blob/master/README.md
     WARNING: doesn't handle padding or strides yet
     Args:
       x.shape[0] 									  --> number of input examples (batch size)
       cout 			 								    --> number of output channels
       x.shape[2]-(H-1)					 	  --> non-padded height of conv output, need to subtract because this is an unpadded conv
@@ -126,14 +176,18 @@
       (a, b, c, d)(e, f, g, h)      --> (a, e, c-(g-1), d-(h-1)) 
       in general, output x and y = [(W−K+2P)/S]+1
     """
     if type(ctx.stride) == int:                                                          # ctx stores function params
       ctx.stride = (ctx.stride, ctx.stride)
 
     cout, cin, H, W = w.shape
+
+    if groups > 1:                                                                       # allows grouped convolutions 
+      w = np.repeat(w, groups, axis=1) / groups                                          # TODO: why does this work?
+
     tw = w.reshape(cout, -1).T                                                           # slice of kernel 
     y_stride, x_stride = ctx.stride
     bs, oy, ox = x.shape[0], (x.shape[2]-(H-y_stride))//y_stride, (x.shape[3]-(W-x_stride))//x_stride
     ctx.save_for_backward(x, w)
 
     ret = np.zeros((bs, cout, oy, ox), dtype=w.dtype)
```

### Comparing `froog-0.1.7/froog/optim.py` & `froog-0.1.8/froog/optim.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,33 +15,32 @@
 
 class Adam(Optimizer):  
   """
   Default ADAM opimizer from https://arxiv.org/pdf/1412.6980.pdf algorithm
   """
   def __init__(self, params, lr=0.001, b1=0.9, b2=0.999, eps=10e-8):
     super(Adam, self).__init__(params)
-    # self.params = params
-
-    self.alpha = lr
+    self.lr = lr
     self.b1 = b1
     self.b2 = b2
     self.eps = eps # should be 1e-8?
     self.t = 0
 
     self.m = [np.zeros_like(t.data) for t in self.params]
     self.v = [np.zeros_like(t.data) for t in self.params]
 
   def step(self):
     self.t += 1
-    for i, t in enumerate(self.params):
+    a = self.lr * (
+      np.sqrt(1 - np.power(self.b2, self.t)) /
+      (1 - np.power(self.b1, self.t)))
+    for i,t in enumerate(self.params):
       self.m[i] = self.b1 * self.m[i] + (1 - self.b1) * t.grad
-      self.v[i] = self.b2 * self.v[i] + (1 - self.b1) * np.square(t.grad)
-      m_hat = self.m[i] / (1. - self.b1 ** self.t)
-      v_hat = self.v[i] / (1. - self.b2 ** self.t)
-      t.data -=  self.alpha * m_hat / (np.sqrt(v_hat) + self.eps)
+      self.v[i] = self.b2 * self.v[i] + (1 - self.b2) * np.square(t.grad)
+      t.data -= a * self.m[i] / (np.sqrt(self.v[i]) + self.eps)
 
 class RMSprop(Optimizer):
   """
   This version has epsilon
   https://optimization.cbe.cornell.edu/index.php?title=RMSProp
   RMSprop divides the learning rate by an exponentially decaying average of squared gradients.
```

### Comparing `froog-0.1.7/froog/tensor.py` & `froog-0.1.8/froog/tensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 
 # *********** Main Classes ***********
 # ********* Tensor, Function *********
 class Tensor:
   def __init__(self, data):
     if type(data) == list:
       data = np.array(data, dtype=np.float32)
-    if type(data) != np.ndarray:
+    elif type(data) != np.ndarray:
       print(f"error constructing tensor with {data}")
       assert False
-    if data.dtype == np.float64:
-      # print(f"sure you want to use float64 with {data}")
+    
+    if data.dtype != np.float32:
+      # warning? float64 needed for numerical jacobian
+      # TODO: set env flag to print all warnings
       pass
+
     self.data = data
-    self.grad = None
 
     # internal variables used for autograd graph construction
-    # these are where the backward gradient computation are saved
-    self._ctx = None
+    self.grad = None
+    self._ctx = None # these are where the backward gradient computation are saved
 
   def __repr__(self):
       return f"Tensor data: {self.data}, gradients: {self.grad}" 
 
   @property
   def shape(self):
     return self.data.shape
@@ -68,17 +70,27 @@
         continue
       if g.shape != t.data.shape:
         print(f"grad shape must match tensor shape in {self._ctx}, {g.shape} != {t.data.shape}")
         assert False
       t.grad = g
       t.backward(False) # what does inputting False do???
 
+  # ****** basic ops ******
+
   def mean(self):
     div = Tensor(np.array([1 / self.data.size], dtype=self.data.dtype))
     return self.sum().mul(div)
+  
+  def sqrt(self):
+    root = Tensor(np.zeros(self.shape, dtype=self.data.dtype)+0.5)
+    return self.pow(root)
+
+  def div(self, y):
+    root = Tensor(np.zeros(self.shape, dtype=self.data.dtype)-1)
+    return self.mul(y.pow(root))
 
 class Function:
   """
   An instantiation of the Function class includes the context
   """
   def __init__(self, *tensors):
     self.parents = tensors
```

### Comparing `froog-0.1.7/froog/utils.py` & `froog-0.1.8/froog/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,27 @@
 from functools import lru_cache
 
 def dense_layer(*tensor_size):
   # TODO: why dividing by sqrt?
   ret = np.random.uniform(-1., 1., size=tensor_size)/np.sqrt(np.prod(tensor_size)) # random init weights
   return ret.astype(np.float32)
 
+def fetch(url):
+  print(f"fetching {url}...")
+  import requests, os, hashlib
+  fp = os.path.join("/tmp", hashlib.md5(url.encode('utf-8')).hexdigest())
+  if os.path.isfile(fp):
+    with open(fp, "rb") as f:
+      dat = f.read()
+  else:
+    with open(fp, "wb") as f:
+      dat = requests.get(url).content
+      f.write(dat)
+  return dat
+
 def mask_like(like, mask_inx, mask_value=1.0):
   mask = np.zeros_like(like).reshape(-1) # flatten
   mask[mask_inx] = mask_value            # fill 
   return mask.reshape(like.shape)
 
 @lru_cache
 def get_im2col_index(oy, ox, cin, H, W):
@@ -49,26 +62,14 @@
 
   ridx = rearrange_col2im_index(oy, ox, channels_in, H, W)
   # -1 has to be 0s
   x = np.pad(tx.reshape(bs, -1), ((0,0),(0,1)))[:, ridx].sum(axis=2)
   return x.reshape(bs, channels_in, OY, OX)
 
 def fetch_mnist():
-  def fetch(url):
-    import requests, gzip, os, hashlib, numpy
-    fp = os.path.join("/tmp", hashlib.md5(url.encode('utf-8')).hexdigest())
-    if os.path.isfile(fp):
-      with open(fp, "rb") as f:
-        dat = f.read()
-    else:
-      with open(fp, "wb") as f:
-        dat = requests.get(url).content
-        f.write(dat)
-    return numpy.frombuffer(gzip.decompress(dat), dtype=numpy.uint8).copy()
-  
-  print("loading mnist...")
-  X_train = fetch("http://yann.lecun.com/exdb/mnist/train-images-idx3-ubyte.gz")[0x10:].reshape((-1, 28, 28))
-  Y_train = fetch("http://yann.lecun.com/exdb/mnist/train-labels-idx1-ubyte.gz")[8:]
-  X_test = fetch("http://yann.lecun.com/exdb/mnist/t10k-images-idx3-ubyte.gz")[0x10:].reshape((-1, 28, 28))
-  Y_test = fetch("http://yann.lecun.com/exdb/mnist/t10k-labels-idx1-ubyte.gz")[8:]
-  return X_train, Y_train, X_test, Y_test
-
+  import gzip
+  parse = lambda dat: np.frombuffer(gzip.decompress(dat), dtype=np.uint8).copy()
+  X_train = parse(fetch("http://yann.lecun.com/exdb/mnist/train-images-idx3-ubyte.gz"))[0x10:].reshape((-1, 28, 28))
+  Y_train = parse(fetch("http://yann.lecun.com/exdb/mnist/train-labels-idx1-ubyte.gz"))[8:]
+  X_test = parse(fetch("http://yann.lecun.com/exdb/mnist/t10k-images-idx3-ubyte.gz"))[0x10:].reshape((-1, 28, 28))
+  Y_test = parse(fetch("http://yann.lecun.com/exdb/mnist/t10k-labels-idx1-ubyte.gz"))[8:]
+  return X_train, Y_train, X_test, Y_test
```

### Comparing `froog-0.1.7/setup.py` & `froog-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from setuptools import setup
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 setup(name='froog',
-      version='0.1.7',
-      description='FROOG: Fast Real-time Optimization Of Gradients',
+      version='0.1.8',
+      description='a beautifully compact machine-learning library',
       author='Kevin Buhler',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages = ['froog'],
       classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `froog-0.1.7/tests/test_conv_speed.py` & `froog-0.1.8/tests/test_conv_speed.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     cnt = num_time
     fpt, bpt = 0.0, 0.0
     for i in range(1+cnt):
       et0 = time.time()
       x = Tensor.randn(128, 1, 28, 28)
       x = x.conv2d(c1).relu().avg_pool2d()
       x = x.conv2d(c2).relu().max_pool2d()
-      x = x.reshape(Tensor(np.array((x.shape[0], -1))))
+      x = x.reshape(shape=(x.shape[0], -1))
       out = x.dot(l1).logsoftmax()
       out = out.mean()
       et1 = time.time()
       out.backward()
       et2 = time.time()
       if i == 0:
         pr = start_profile()
```

### Comparing `froog-0.1.7/tests/test_mnist.py` & `froog-0.1.8/tests/test_mnist.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     self.c2 = Tensor(dense_layer(out_chan,inter_chan,conv,conv))        # (28-conv+1)(28-conv+1) since kernel isn't padded
     self.l1 = Tensor(dense_layer(out_chan*5*5, 10))                     # MNIST output is 10 classes
 
   def forward(self, x):
     x.data = x.data.reshape((-1, 1, 28, 28))                            # get however many number of imgs in batch
     x = x.conv2d(self.c1).relu().max_pool2d()                           # pass through layer 1 first
     x = x.conv2d(self.c2).relu().max_pool2d()                           # pass through layer 2
-    x = x.reshape(Tensor(np.array((x.shape[0], -1))))                   # then go down to mlp
+    x = x.reshape(shape=[x.shape[0], -1])                               # then go down to mlp
     return x.dot(self.l1).logsoftmax()                                  # softmax to get probs   
 
   def parameters(self):
     return [self.l1, self.c1, self.c2]  
 
 def train(model, optimizer, steps, BS=128):
   # ********* training the model *********
```

### Comparing `froog-0.1.7/tests/test_ops.py` & `froog-0.1.8/tests/test_ops.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import torch
 import numpy as np
-import unittest
 from froog.tensor import Tensor
+import torch
+import unittest
 import timeit
 import functools
 
 def helper_test_op(shape, torch_func, froog_func, atol=1e-7, grad_atol=1e-7):
   torch_tensors = [torch.rand(x, requires_grad=True) for x in shape]
   froog_tensors = [Tensor(x.detach().numpy()) for x in torch_tensors]
 
@@ -29,14 +29,28 @@
   torch_fbp = timeit.Timer(functools.partial(lambda f,x: f(*x).mean().backward(), torch_func, torch_tensors)).timeit(5) * 1000/5
   froog_fbp = timeit.Timer(functools.partial(lambda f,x: f(*x).mean().backward(), froog_func, froog_tensors)).timeit(5) * 1000/5
 
   print(f"shape: {repr(shape) : >32} torch/froog fwd: {torch_fwd:.2f}/{froog_fwd:.2f} ms ({float(froog_fwd/torch_fwd):.2f}x slower) bp: {torch_fbp - torch_fwd:.2f}/{froog_fbp - froog_fwd:.2f} ms ({float((froog_fbp - froog_fwd)/(torch_fbp - torch_fwd)):.2f}x slower)")
 
 
 class TestOps(unittest.TestCase):
+  def test_add(self):
+    helper_test_op([(45,65), (45,65)], lambda x,y: x+y, Tensor.add)
+  def test_sub(self):
+    helper_test_op([(45,65), (45,65)], lambda x,y: x-y, Tensor.sub)
+  def test_mul(self):
+    helper_test_op([(45,65), (45,65)], lambda x,y: x*y, Tensor.mul)
+  def test_div(self):
+    # TODO: why needs more tolerance?
+    helper_test_op([(45,65), (45,65)], lambda x,y: x/y, Tensor.div, atol=5e-5, grad_atol=2e-5)
+  def test_pow(self):
+    helper_test_op([(45,65), (45,65)], lambda x,y: x**y, Tensor.pow)
+  def test_sqrt(self):
+    helper_test_op([(45,65)], lambda x: x.sqrt(), Tensor.sqrt)
+    
   def test_conv2d(self):
     for bs in [1,8]:
       for cin in [1,2,3]:
         for H in [2,3,5]:
           for W in [2,3,5]:
             helper_test_op([(bs,cin,10,7), (4,cin,H,W)], 
                     lambda x,w: torch.nn.functional.conv2d(x,w).relu(),
```

### Comparing `froog-0.1.7/tests/test_tensor.py` & `froog-0.1.8/tests/test_tensor.py`

 * *Files identical despite different names*

