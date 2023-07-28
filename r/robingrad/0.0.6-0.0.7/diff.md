# Comparing `tmp/robingrad-0.0.6.tar.gz` & `tmp/robingrad-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robingrad-0.0.6.tar", last modified: Sat Jul 22 12:47:57 2023, max compression
+gzip compressed data, was "robingrad-0.0.7.tar", last modified: Fri Jul 28 16:36:28 2023, max compression
```

## Comparing `robingrad-0.0.6.tar` & `robingrad-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-22 12:47:57.817217 robingrad-0.0.6/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-07-11 17:52:34.000000 robingrad-0.0.6/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2950 2023-07-22 12:47:57.816946 robingrad-0.0.6/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1289 2023-07-22 12:47:33.000000 robingrad-0.0.6/README.md
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      694 2023-07-22 12:47:24.000000 robingrad-0.0.6/pyproject.toml
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-22 12:47:57.814193 robingrad-0.0.6/robingrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-07-22 12:47:28.000000 robingrad-0.0.6/robingrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-07-12 20:52:44.000000 robingrad-0.0.6/robingrad/graph.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3030 2023-07-22 10:30:14.000000 robingrad-0.0.6/robingrad/lab.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-22 12:47:57.816241 robingrad-0.0.6/robingrad/nn/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      423 2023-07-13 16:36:34.000000 robingrad-0.0.6/robingrad/nn/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1564 2023-07-20 13:31:06.000000 robingrad-0.0.6/robingrad/optim.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1384 2023-07-15 12:31:49.000000 robingrad-0.0.6/robingrad/state.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11131 2023-07-22 10:23:56.000000 robingrad-0.0.6/robingrad/tensor.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-22 12:47:57.815930 robingrad-0.0.6/robingrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2950 2023-07-22 12:47:57.000000 robingrad-0.0.6/robingrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      358 2023-07-22 12:47:57.000000 robingrad-0.0.6/robingrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-07-22 12:47:57.000000 robingrad-0.0.6/robingrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       15 2023-07-22 12:47:57.000000 robingrad-0.0.6/robingrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       10 2023-07-22 12:47:57.000000 robingrad-0.0.6/robingrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-07-22 12:47:57.817295 robingrad-0.0.6/setup.cfg
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-22 12:47:57.816537 robingrad-0.0.6/tests/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     6291 2023-07-22 10:35:08.000000 robingrad-0.0.6/tests/test_tensor.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-28 16:36:28.741640 robingrad-0.0.7/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-07-11 17:52:34.000000 robingrad-0.0.7/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2950 2023-07-28 16:36:28.741373 robingrad-0.0.7/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1289 2023-07-28 10:49:50.000000 robingrad-0.0.7/README.md
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      694 2023-07-28 10:49:39.000000 robingrad-0.0.7/pyproject.toml
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-28 16:36:28.736558 robingrad-0.0.7/robingrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-07-28 10:49:45.000000 robingrad-0.0.7/robingrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-07-12 20:52:44.000000 robingrad-0.0.7/robingrad/graph.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     6324 2023-07-28 16:35:35.000000 robingrad-0.0.7/robingrad/lab.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-28 16:36:28.739935 robingrad-0.0.7/robingrad/nn/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      448 2023-07-24 22:02:33.000000 robingrad-0.0.7/robingrad/nn/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      244 2023-07-24 22:08:46.000000 robingrad-0.0.7/robingrad/nn/loss.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1564 2023-07-20 13:31:06.000000 robingrad-0.0.7/robingrad/optim.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1384 2023-07-15 12:31:49.000000 robingrad-0.0.7/robingrad/state.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11792 2023-07-28 16:35:53.000000 robingrad-0.0.7/robingrad/tensor.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-28 16:36:28.738452 robingrad-0.0.7/robingrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2950 2023-07-28 16:36:28.000000 robingrad-0.0.7/robingrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      379 2023-07-28 16:36:28.000000 robingrad-0.0.7/robingrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-07-28 16:36:28.000000 robingrad-0.0.7/robingrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       15 2023-07-28 16:36:28.000000 robingrad-0.0.7/robingrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       10 2023-07-28 16:36:28.000000 robingrad-0.0.7/robingrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-07-28 16:36:28.741718 robingrad-0.0.7/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-28 16:36:28.740817 robingrad-0.0.7/tests/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9043 2023-07-28 13:50:02.000000 robingrad-0.0.7/tests/test_tensor.py
```

### Comparing `robingrad-0.0.6/LICENSE` & `robingrad-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.6/PKG-INFO` & `robingrad-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robingrad
-Version: 0.0.6
+Version: 0.0.7
 Summary: Something between Tinygrad and Micrograd
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2023 Marco Salvalaggio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -32,15 +32,15 @@
 
 
 ## Installation
 
 To install the current release,
 
 ```console
-pip install robingrad==0.0.6
+pip install robingrad==0.0.7
 ```
 
 From source
 
 ```console
 git clone https://github.com/marcosalvalaggio/robingrad.git
 cd robingrad
```

### Comparing `robingrad-0.0.6/README.md` & `robingrad-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 ## Installation
 
 To install the current release,
 
 ```console
-pip install robingrad==0.0.6
+pip install robingrad==0.0.7
 ```
 
 From source
 
 ```console
 git clone https://github.com/marcosalvalaggio/robingrad.git
 cd robingrad
```

### Comparing `robingrad-0.0.6/pyproject.toml` & `robingrad-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robingrad"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Something between Tinygrad and Micrograd"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `robingrad-0.0.6/robingrad/graph.py` & `robingrad-0.0.7/robingrad/graph.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.6/robingrad/optim.py` & `robingrad-0.0.7/robingrad/optim.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.6/robingrad/state.py` & `robingrad-0.0.7/robingrad/state.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.6/robingrad/tensor.py` & `robingrad-0.0.7/robingrad/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,28 +131,30 @@
         return out
     
     def __add__(self, other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor":
         other = other if isinstance(other, Tensor) else Tensor.broadcast(self, other, dtype=self.data.dtype, requires_grad=self.requires_grad)
         out = Tensor(self.data + other.data, dtype=self.data.dtype, _children=(self, other), _op='+', _origin="__add__", requires_grad=self.requires_grad)
         
         def _backward():
-            self.grad += out.grad
+            self.grad += np.sum(out.grad, axis=0) if self.data.shape != out.data.shape else out.grad
             # other.grad += out.grad
-            other.grad += np.sum(out.grad, axis=0) if len(other.data.shape) > 1 else out.grad
+            other.grad += np.sum(out.grad, axis=0) if other.data.shape != out.data.shape else out.grad
         out._backward = _backward
 
         return out
     
     def __mul__(self, other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor":
         other = other if isinstance(other, Tensor) else Tensor.broadcast(self, other, dtype=self.data.dtype, requires_grad=self.requires_grad)
         out = Tensor(self.data * other.data, dtype=self.data.dtype, _children=(self, other), _op='*', _origin="__mul__", requires_grad=self.requires_grad)
 
         def _backward():
-            self.grad += other.data * out.grad
-            other.grad += self.data * out.grad
+            # self.grad += other.data * out.grad
+            self.grad += np.sum(other.data * out.grad, axis=0) if self.data.shape != out.data.shape else (other.data * out.grad)
+            # other.grad += self.data * out.grad
+            other.grad += np.sum(self.data * out.grad, axis=0) if other.data.shape != out.data.shape else (self.data * out.grad)
         out._backward = _backward
 
         return out
     
     def __pow__(self, other: Union[int, float]) -> "Tensor":
         assert isinstance(other, (int, float)), "only supporting int/float powers for now"
         out = Tensor(self.data ** other, dtype=self.data.dtype, _children=(self,), _op=f'**{other}', _origin="__pow__", requires_grad=self.requires_grad)
@@ -257,8 +259,17 @@
         return out
 
     @property
     def T(self) -> "Tensor": return self.transpose()  
     
     def linear(self, weight: "Tensor", bias: Optional["Tensor"] = None) -> "Tensor":
         x = self * weight if len(weight.shape) == 1 else self @ weight
-        return x + bias if bias is not None else x
+        return x + bias if bias is not None else x
+
+    def flatten(self) -> "Tensor":
+        out = Tensor(self.data.flatten(), dtype=self.data.dtype, _children=(self,), _op="flatten", _origin="flatten", requires_grad=self.requires_grad)
+
+        def _backward():
+            self.grad = out.grad.reshape(self.shape)
+        out._backward = _backward
+
+        return out
```

### Comparing `robingrad-0.0.6/robingrad.egg-info/PKG-INFO` & `robingrad-0.0.7/robingrad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robingrad
-Version: 0.0.6
+Version: 0.0.7
 Summary: Something between Tinygrad and Micrograd
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2023 Marco Salvalaggio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -32,15 +32,15 @@
 
 
 ## Installation
 
 To install the current release,
 
 ```console
-pip install robingrad==0.0.6
+pip install robingrad==0.0.7
 ```
 
 From source
 
 ```console
 git clone https://github.com/marcosalvalaggio/robingrad.git
 cd robingrad
```

### Comparing `robingrad-0.0.6/tests/test_tensor.py` & `robingrad-0.0.7/tests/test_tensor.py`

 * *Files 23% similar despite different names*

```diff
@@ -172,30 +172,108 @@
         loss = f.sum()
         loss.backward()
         res_torch_1 = a.grad.numpy().tolist()
         # test 
         self.assertAlmostEqual(res_robin_1, res_torch_1)
 
     def test_new_add(self):
-        # robin
+        # robin 1
         a = Tensor.full((5,1), 3., requires_grad=True)
         b = Tensor.full((1,1), 2., requires_grad=True)
         c = a + b
         loss = c.mean()
         loss.backward()
         res_robin_1 = a.grad.tolist()
         res_robin_2 = b.grad.tolist()
-        # torch
+        # torch 1
         a = torch.full((5,1), 3., requires_grad=True)
         b = torch.full((1,1), 2., requires_grad=True)
         c = a + b
         loss = c.mean()
         loss.backward()
         res_torch_1 = a.grad.tolist()
         res_torch_2 = b.grad.tolist()
-        #test
+        #test 1
         self.assertEqual(res_robin_1, res_torch_1)
         self.assertEqual(res_robin_2, res_torch_2)
+        # robin 2
+        a = Tensor.full((5,1), 3., requires_grad=True)
+        b = Tensor.full((1,1), 2., requires_grad=True)
+        c =  b + a
+        loss = c.mean()
+        loss.backward()
+        res_robin_3 = a.grad.tolist()
+        res_robin_4 = b.grad.tolist()
+        # torch 2
+        a = torch.full((5,1), 3., requires_grad=True)
+        b = torch.full((1,1), 2., requires_grad=True)
+        c = b + a
+        loss = c.mean()
+        loss.backward()
+        res_torch_3 = a.grad.tolist()
+        res_torch_4 = b.grad.tolist()
+        #test 2
+        self.assertEqual(res_robin_3, res_torch_3)
+        self.assertEqual(res_robin_4, res_torch_4)
 
+    def test_flatten(self):
+        # robin 
+        a = Tensor.ones((2,3), requires_grad=True)
+        b = Tensor.full((3,2), 3., requires_grad=True)
+        c = a @ b
+        d = c.flatten()
+        loss = d.mean()
+        loss.backward()
+        res_robin_1 = a.grad.tolist()
+        res_robin_2 = b.grad.tolist()
+        # torch
+        a = torch.ones((2,3), requires_grad=True)
+        b = torch.full((3,2), 3., requires_grad=True)
+        c = a @ b
+        d = c.flatten()
+        loss = d.mean()
+        loss.backward()
+        res_torch_1 = a.grad.numpy().tolist()
+        res_torch_2 = b.grad.numpy().tolist()
+        # test 
+        self.assertEqual(res_robin_1, res_torch_1)
+        self.assertEqual(res_robin_2, res_torch_2)
 
-
-
+    def test_new_mul(self):
+        # robin 1
+        a = Tensor.full((5,1), 3., requires_grad=True)
+        b = Tensor.ones((1,1), requires_grad=True)
+        c = a * b
+        loss = c.sum()
+        loss.backward()
+        res_robin_1 = a.grad.tolist()
+        res_robin_2 = b.grad.tolist()
+        # torch 1
+        a = torch.full((5,1), 3., requires_grad=True)
+        b = torch.ones((1,1), requires_grad=True)
+        c = a * b
+        loss = c.sum()
+        loss.backward()
+        res_torch_1 = a.grad.numpy().tolist()
+        res_torch_2 = b.grad.numpy().tolist()
+        # test 1
+        self.assertEqual(res_robin_1, res_torch_1)
+        self.assertEqual(res_robin_2, res_torch_2)
+        # robin 2
+        a = Tensor.full((5,1), 3., requires_grad=True)
+        b = Tensor.ones((1,1), requires_grad=True)
+        c = b * a
+        loss = c.sum()
+        loss.backward()
+        res_robin_3 = a.grad.tolist()
+        res_robin_4 = b.grad.tolist()
+        # torch 2
+        a = torch.full((5,1), 3., requires_grad=True)
+        b = torch.ones((1,1), requires_grad=True)
+        c = b * a
+        loss = c.sum()
+        loss.backward()
+        res_torch_3 = a.grad.numpy().tolist()
+        res_torch_4 = b.grad.numpy().tolist()
+        # test 2
+        self.assertEqual(res_robin_3, res_torch_3)
+        self.assertEqual(res_robin_4, res_torch_4)
```

