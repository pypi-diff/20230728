# Comparing `tmp/ssfm-gpu-0.1.0.tar.gz` & `tmp/ssfm-gpu-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssfm-gpu-0.1.0.tar", last modified: Thu Jan 19 16:20:22 2023, max compression
+gzip compressed data, was "ssfm-gpu-0.1.1.tar", last modified: Fri Jul 28 14:02:02 2023, max compression
```

## Comparing `ssfm-gpu-0.1.0.tar` & `ssfm-gpu-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-01-19 16:20:22.031046 ssfm-gpu-0.1.0/
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     1067 2022-08-15 17:08:04.000000 ssfm-gpu-0.1.0/LICENSE
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     2035 2023-01-19 16:20:22.031046 ssfm-gpu-0.1.0/PKG-INFO
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      138 2022-11-10 15:39:27.000000 ssfm-gpu-0.1.0/README.md
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      743 2023-01-19 16:20:02.000000 ssfm-gpu-0.1.0/pyproject.toml
--rw-rw-r--   0 esf0      (1000) esf0      (1000)       38 2023-01-19 16:20:22.031046 ssfm-gpu-0.1.0/setup.cfg
-drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-01-19 16:20:22.031046 ssfm-gpu-0.1.0/ssfm_gpu/
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      140 2022-12-13 15:48:24.000000 ssfm-gpu-0.1.0/ssfm_gpu/__init__.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)        0 2022-11-23 11:11:09.000000 ssfm-gpu-0.1.0/ssfm_gpu/channel.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     2593 2022-12-14 13:48:45.000000 ssfm-gpu-0.1.0/ssfm_gpu/conversion.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     4675 2022-12-13 16:00:17.000000 ssfm-gpu-0.1.0/ssfm_gpu/examples.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    14951 2023-01-19 16:20:02.000000 ssfm-gpu-0.1.0/ssfm_gpu/propagation.py
-drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-01-19 16:20:22.031046 ssfm-gpu-0.1.0/ssfm_gpu.egg-info/
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     2035 2023-01-19 16:20:22.000000 ssfm-gpu-0.1.0/ssfm_gpu.egg-info/PKG-INFO
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      269 2023-01-19 16:20:22.000000 ssfm-gpu-0.1.0/ssfm_gpu.egg-info/SOURCES.txt
--rw-rw-r--   0 esf0      (1000) esf0      (1000)        1 2023-01-19 16:20:22.000000 ssfm-gpu-0.1.0/ssfm_gpu.egg-info/dependency_links.txt
--rw-rw-r--   0 esf0      (1000) esf0      (1000)        9 2023-01-19 16:20:22.000000 ssfm-gpu-0.1.0/ssfm_gpu.egg-info/top_level.txt
+drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-28 14:02:02.406231 ssfm-gpu-0.1.1/
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     1067 2022-08-15 17:08:04.000000 ssfm-gpu-0.1.1/LICENSE
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     2035 2023-07-28 14:02:02.406231 ssfm-gpu-0.1.1/PKG-INFO
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      138 2022-11-10 15:39:27.000000 ssfm-gpu-0.1.1/README.md
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      743 2023-07-28 14:00:26.000000 ssfm-gpu-0.1.1/pyproject.toml
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)       38 2023-07-28 14:02:02.406231 ssfm-gpu-0.1.1/setup.cfg
+drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-28 14:02:02.406231 ssfm-gpu-0.1.1/ssfm_gpu/
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      140 2022-12-13 15:48:24.000000 ssfm-gpu-0.1.1/ssfm_gpu/__init__.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)        0 2022-11-23 11:11:09.000000 ssfm-gpu-0.1.1/ssfm_gpu/channel.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     3098 2023-05-16 16:10:15.000000 ssfm-gpu-0.1.1/ssfm_gpu/conversion.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     4675 2022-12-13 16:00:17.000000 ssfm-gpu-0.1.1/ssfm_gpu/examples.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    14939 2023-07-28 14:00:26.000000 ssfm-gpu-0.1.1/ssfm_gpu/propagation.py
+drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-28 14:02:02.406231 ssfm-gpu-0.1.1/ssfm_gpu.egg-info/
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     2035 2023-07-28 14:02:02.000000 ssfm-gpu-0.1.1/ssfm_gpu.egg-info/PKG-INFO
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      269 2023-07-28 14:02:02.000000 ssfm-gpu-0.1.1/ssfm_gpu.egg-info/SOURCES.txt
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)        1 2023-07-28 14:02:02.000000 ssfm-gpu-0.1.1/ssfm_gpu.egg-info/dependency_links.txt
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)        9 2023-07-28 14:02:02.000000 ssfm-gpu-0.1.1/ssfm_gpu.egg-info/top_level.txt
```

### Comparing `ssfm-gpu-0.1.0/LICENSE` & `ssfm-gpu-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ssfm-gpu-0.1.0/PKG-INFO` & `ssfm-gpu-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssfm-gpu
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tensorflow GPU version of split-step Fourier method for Nonlinear Schrodinger and Manakov equations
 Author-email: Egor Sedov <e.sedov@g.nsu.ru>
 License: MIT License
         
         Copyright (c) 2022 Egor Sedov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ssfm-gpu-0.1.0/pyproject.toml` & `ssfm-gpu-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssfm-gpu"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Egor Sedov", email="e.sedov@g.nsu.ru" },
 ]
 description = "Tensorflow GPU version of split-step Fourier method for Nonlinear Schrodinger and Manakov equations"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `ssfm-gpu-0.1.0/ssfm_gpu/conversion.py` & `ssfm-gpu-0.1.1/ssfm_gpu/conversion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import numpy as np
 
-# convert NLSE equation
-# dimensionless form iq_z +- 1/2 q_tt + |q|^2 * q = 0
-# dimension form iQ_Z - beta2 / 2 Q_TT + gamma |Q|^2 * Q = 0
+# convert
+# NLSE equation
+# dimensionless form
+# iq_z +- 1/2 q_tt + |q|^2 * q = 0
+
+# dimension form
+# iQ_Z - beta2 / 2 Q_TT + gamma |Q|^2 * Q = 0
 #
 # T = T_0 * t
 # Z = L * z
 # L = T_0 ^ 2 / |beta2|
 # Q = C * q
 # C = 1 / (gamma * L) ^ (1/2) = |beta2| ^ (1/2) / (gamma ^ (1/2) * T_0)
 
@@ -20,71 +24,86 @@
 # i Q1_Z - beta2 / 2 * Q1_TT + 8/9 * gamma * (|Q1|^2 + |Q2|^2) * Q1 = 0
 # i Q2_Z - beta2 / 2 * Q2_TT + 8/9 * gamma * (|Q1|^2 + |Q2|^2) * Q2 = 0
 #
 # T = T_0 * t
 # Z = L * z
 # L = 2 * T_0 ^ 2 / |beta2|
 # Q = C * q
-# [2 / (8/9 * gamma * L)] ^ (1/2) = |beta2| ^ (1/2) / [(8/9 * gamma * L) ^ (1/2) * T_0]
+# C = [2 / (8/9 * gamma * L)] ^ (1/2) = |beta2| ^ (1/2) / [(8/9 * gamma * L) ^ (1/2) * T_0]
 
 # to run dimensionless form of NLSE solver
 # beta2 = -+ 1
 # gamma = 1
 
 # to run dimensionless form of Manakov solver
 # beta2 = -2
 # gamma = +- 2 * 9/8 -> "+" focus / "-" defocus
 
+# Additional for Manakov equation
+# dimensionless form
+# i q1_z +- 1/2 q1_tt + (|q1|^2 + |q2|^2) q1 = 0
+# i q2_z +- 1/2 q2_tt + (|q1|^2 + |q2|^2) q2 = 0
+# -1/+1 -> defocus / focus
+#
+# T = T_0 * t
+# Z = L * z
+# L = T_0 ^ 2 / |beta2|
+# Q = C * q
+# C = [1 / (8/9 * gamma * L)] ^ (1/2) = |beta2| ^ (1/2) / [(8/9 * gamma * L) ^ (1/2) * T_0]
+
 
 def get_convert_coefficients_nlse(beta2, gamma, t0):
 
     coefficients = {}
     coefficients['T0'] = t0
     coefficients['L'] = t0 * t0 / abs(beta2)
     coefficients['C'] = 1.0 / (gamma * coefficients['L']) ** 0.5
 
     return coefficients
 
 
-def get_convert_coefficients_manakov(beta2, gamma, t0):
+def get_convert_coefficients_manakov(beta2, gamma, t0, manakov_type=0):
     coefficients = {}
     coefficients['T0'] = t0
-    coefficients['L'] = 2 * t0 * t0 / abs(beta2)
-    coefficients['C'] = (2.0 / (8. / 9. * gamma * coefficients['L'])) ** 0.5
+    if manakov_type == 0:
+        coefficients['L'] = 2 * t0 * t0 / abs(beta2)
+    else:
+        coefficients['L'] = t0 * t0 / abs(beta2)
+    coefficients['C'] = (abs(beta2) / (8. / 9. * gamma)) ** 0.5 / t0
 
     return coefficients
 
 
-def convert_forward(q, t, z, beta2, gamma, t0, type='nlse'):
+def convert_forward(q, t, z, beta2, gamma, t0, type='nlse', manakov_type=0):
     # convert from dimensionless to dimension form
     result = {}
     if type == 'nlse':
         coefficients = get_convert_coefficients_nlse(beta2, gamma, t0)
         result['Q'] = coefficients['C'] * q
     else:
         # manakov
-        coefficients = get_convert_coefficients_manakov(beta2, gamma, t0)
+        coefficients = get_convert_coefficients_manakov(beta2, gamma, t0, manakov_type)
         result['Q1'] = coefficients['C'] * q[0]
         result['Q2'] = coefficients['C'] * q[1]
 
     result['T'] = coefficients['T0'] * t
     result['Z'] = coefficients['L'] * z
 
     return result
 
 
-def convert_inverse(q, t, z, beta2, gamma, t0, type='nlse'):
+def convert_inverse(q, t, z, beta2, gamma, t0, type='nlse', manakov_type=0):
     # convert from dimension to dimensionless form
     result = {}
     if type == 'nlse':
         coefficients = get_convert_coefficients_nlse(beta2, gamma, t0)
         result['q'] = q / coefficients['C']
     else:
         # manakov
-        coefficients = get_convert_coefficients_manakov(beta2, gamma, t0)
+        coefficients = get_convert_coefficients_manakov(beta2, gamma, t0, manakov_type)
         result['q1'] = q[0] / coefficients['C']
         result['q2'] = q[1] / coefficients['C']
 
     result['t'] = t / coefficients['T0']
     result['z'] = z / coefficients['L']
 
     return result
```

### Comparing `ssfm-gpu-0.1.0/ssfm_gpu/examples.py` & `ssfm-gpu-0.1.1/ssfm_gpu/examples.py`

 * *Files identical despite different names*

### Comparing `ssfm-gpu-0.1.0/ssfm_gpu/propagation.py` & `ssfm-gpu-0.1.1/ssfm_gpu/propagation.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     if abs(fiber_length) < 1e-15:
         return initial_signal
 
     dz = fiber_length / n_span
 
     n = len(initial_signal)
-    w = fftshift(np.array([(i - n / 2) * (2. * np.pi / t_span) for i in range(n)], dtype=np.complex))
+    w = fftshift(np.array([(i - n / 2) * (2. * np.pi / t_span) for i in range(n)], dtype=complex))
     w2 = tf.math.pow(w, 2)
     w3 = tf.math.pow(w, 3)
 
     dispersion = tf.math.exp((0.5j * beta2 * w2 + 1. / 6. * beta3 * w3 - alpha / 2.) * dz)
     dispersion_half = tf.math.exp((0.5j * beta2 * w2 + 1. / 6. * beta3 * w3 - alpha / 2.) * dz / 2.)
     dispersion_mhalf = tf.math.exp((0.5j * beta2 * w2 + 1. / 6. * beta3 * w3 - alpha / 2.) * -dz / 2.)
 
@@ -97,15 +97,15 @@
             signal_cdc (tf_tensor): signal with compensated dispersion
 
     """
 
     #  Dispersion compensation #
     nt_cdc = len(signal)
     t_span = nt_cdc * dt
-    w = fftshift(np.array([(i - nt_cdc / 2) * (2. * np.pi / t_span) for i in range(nt_cdc)], dtype=np.complex))
+    w = fftshift(np.array([(i - nt_cdc / 2) * (2. * np.pi / t_span) for i in range(nt_cdc)], dtype=complex))
     w2 = tf.math.pow(w, 2)
     w3 = tf.math.pow(w, 3)
     dispersion = tf.math.exp((0.5j * channel['beta2'] * w2 + 1. / 6. * channel['beta3'] * w3) *
                              (-channel['z_span'] * channel['n_spans']))
     signal_cdc = tf_ssfm_dispersive_step(tf.cast(signal, tf.complex128), dispersion)
 
     return signal_cdc
@@ -138,15 +138,15 @@
     dz = fiber_length / n_steps
 
     if len(initial_first) != len(initial_second):
         print('[tf_manakov_fiber_propogate] Error: sizes of first and second polarisation have to be the same!')
         return initial_first, initial_second
 
     n = len(initial_first)
-    w = tf.signal.fftshift(np.array([(i - n / 2) * (2. * np.pi / t_span) for i in range(n)], dtype=np.complex))
+    w = tf.signal.fftshift(np.array([(i - n / 2) * (2. * np.pi / t_span) for i in range(n)], dtype=complex))
     w2 = tf.math.pow(w, 2)
     w3 = tf.math.pow(w, 3)
 
     dispersion = tf.math.exp((0.5j * beta2 * w2 + 1. / 6. * beta3 * w3 - alpha / 2.) * dz)
     dispersion_half = tf.math.exp((0.5j * beta2 * w2 + 1. / 6. * beta3 * w3 - alpha / 2.) * dz / 2.)
     dispersion_mhalf = tf.math.exp((0.5j * beta2 * w2 + 1. / 6. * beta3 * w3 - alpha / 2.) * -dz / 2.)
 
@@ -260,15 +260,15 @@
             signal_cdc_y (tf_tensor): signal on the second (y) polarisation with compensated dispersion
 
     """
 
     #  Dispersion compensation #
     nt_cdc = len(signal_x)
     t_span = nt_cdc * dt
-    w = fftshift(np.array([(i - nt_cdc / 2) * (2. * np.pi / t_span) for i in range(nt_cdc)], dtype=np.complex))
+    w = fftshift(np.array([(i - nt_cdc / 2) * (2. * np.pi / t_span) for i in range(nt_cdc)], dtype=complex))
     w2 = tf.math.pow(w, 2)
     w3 = tf.math.pow(w, 3)
     dispersion = tf.math.exp((0.5j * channel['beta2'] * w2 + 1. / 6. * channel['beta3'] * w3) *
                              (-channel['z_span'] * channel['n_spans']))
     signal_cdc_x, signal_cdc_y = tf_ssfm_manakov_dispersive_step(tf.cast(signal_x, tf.complex128),
                                                                  tf.cast(signal_y, tf.complex128),
                                                                  dispersion)
```

### Comparing `ssfm-gpu-0.1.0/ssfm_gpu.egg-info/PKG-INFO` & `ssfm-gpu-0.1.1/ssfm_gpu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssfm-gpu
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tensorflow GPU version of split-step Fourier method for Nonlinear Schrodinger and Manakov equations
 Author-email: Egor Sedov <e.sedov@g.nsu.ru>
 License: MIT License
         
         Copyright (c) 2022 Egor Sedov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

