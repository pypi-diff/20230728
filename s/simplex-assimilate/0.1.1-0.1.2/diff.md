# Comparing `tmp/simplex_assimilate-0.1.1.tar.gz` & `tmp/simplex_assimilate-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplex_assimilate-0.1.1.tar", max compression
+gzip compressed data, was "simplex_assimilate-0.1.2.tar", max compression
```

## Comparing `simplex_assimilate-0.1.1.tar` & `simplex_assimilate-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      892 2023-06-14 18:19:15.322493 simplex_assimilate-0.1.1/README.md
--rw-r--r--   0        0        0      660 2023-06-30 07:53:44.002764 simplex_assimilate-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       66 2023-06-14 19:41:47.172366 simplex_assimilate-0.1.1/simplex_assimilate/__init__.py
--rw-r--r--   0        0        0    10063 2023-06-14 20:28:19.516095 simplex_assimilate-0.1.1/simplex_assimilate/cdf.py
--rw-r--r--   0        0        0     4196 2023-06-14 17:08:51.038465 simplex_assimilate-0.1.1/simplex_assimilate/dirichlet.py
--rw-r--r--   0        0        0     1407 2023-06-14 16:59:00.153456 simplex_assimilate-0.1.1/simplex_assimilate/quantize.py
--rw-r--r--   0        0        0     1153 2023-06-14 19:49:43.938700 simplex_assimilate-0.1.1/simplex_assimilate/transport.py
--rw-r--r--   0        0        0     1367 1970-01-01 00:00:00.000000 simplex_assimilate-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      892 2023-06-14 18:19:15.322493 simplex_assimilate-0.1.2/README.md
+-rw-r--r--   0        0        0      660 2023-07-28 17:09:20.562794 simplex_assimilate-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-06-14 19:41:47.172366 simplex_assimilate-0.1.2/simplex_assimilate/__init__.py
+-rw-r--r--   0        0        0    10155 2023-07-28 17:09:11.799602 simplex_assimilate-0.1.2/simplex_assimilate/cdf.py
+-rw-r--r--   0        0        0     4183 2023-06-30 13:20:38.308580 simplex_assimilate-0.1.2/simplex_assimilate/dirichlet.py
+-rw-r--r--   0        0        0     1407 2023-06-14 16:59:00.153456 simplex_assimilate-0.1.2/simplex_assimilate/quantize.py
+-rw-r--r--   0        0        0     1153 2023-06-14 19:49:43.938700 simplex_assimilate-0.1.2/simplex_assimilate/transport.py
+-rw-r--r--   0        0        0     1367 1970-01-01 00:00:00.000000 simplex_assimilate-0.1.2/PKG-INFO
```

### Comparing `simplex_assimilate-0.1.1/README.md` & `simplex_assimilate-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `simplex_assimilate-0.1.1/pyproject.toml` & `simplex_assimilate-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simplex-assimilate"
-version = "0.1.1"
+version = "0.1.2"
 description = "Perform Data Assimilation on the Simplex. Models an ensemble as a mixture of Dirichlet distributions."
 authors = ["Oscar Laird <olaird25@gmail.com>"]
 readme = "README.md"
 packages = [{include = "simplex_assimilate"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

### Comparing `simplex_assimilate-0.1.1/simplex_assimilate/cdf.py` & `simplex_assimilate-0.1.2/simplex_assimilate/cdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,9 +182,12 @@
     assert np.all(0 < X) and np.all(X < ONE)
     # check the values on either side of X
     three = np.column_stack((X - DELTA, X, X + DELTA))  # X and the two values on either side
     X = three[
         np.arange(len(X)), np.argmin(np.abs(np.column_stack(tuple(f(COL) for COL in three.T)) - Y[:, None]), axis=1)]
     if np.any(X == 0) or np.any(X == ONE):
         warnings.warn("Binary search selected a value on the bounds of [0,1]."
-                      "This could cause a sample to shift to an incompatible class.")
-    return X
+                      "This could cause a sample to shift to an incompatible class."
+                      "0 will be rounded up to 1 epsilon")
+        X[X == 0] = 1
+        # 
+    return X
```

### Comparing `simplex_assimilate-0.1.1/simplex_assimilate/dirichlet.py` & `simplex_assimilate-0.1.2/simplex_assimilate/dirichlet.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         return
 
     def __repr__(self):
         return f'MixedDirichlet(full_alpha={self.full_alpha}, mixture_weights={self.mixture_weights})'
 
     @classmethod
     def est_from_samples(cls, samples: NDArray[np.float64]):
-        pass
         classes = np.unique(samples > 0, axis=0)
         alphas = []
         s_determined = []
         mixture_weights = []
         for c in classes:
             class_rows = ((samples > 0) == c).all(axis=1)  # rows of samples which agree with class c
             class_samples = samples[class_rows][:, c]  # nonzero components
```

### Comparing `simplex_assimilate-0.1.1/simplex_assimilate/quantize.py` & `simplex_assimilate-0.1.2/simplex_assimilate/quantize.py`

 * *Files identical despite different names*

### Comparing `simplex_assimilate-0.1.1/simplex_assimilate/transport.py` & `simplex_assimilate-0.1.2/simplex_assimilate/transport.py`

 * *Files identical despite different names*

### Comparing `simplex_assimilate-0.1.1/PKG-INFO` & `simplex_assimilate-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplex-assimilate
-Version: 0.1.1
+Version: 0.1.2
 Summary: Perform Data Assimilation on the Simplex. Models an ensemble as a mixture of Dirichlet distributions.
 Author: Oscar Laird
 Author-email: olaird25@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
```

