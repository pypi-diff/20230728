# Comparing `tmp/hedges-0.0.1a2.tar.gz` & `tmp/hedges-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hedges-0.0.1a2.tar", last modified: Sun Jul 23 20:18:06 2023, max compression
+gzip compressed data, was "hedges-0.0.1a3.tar", last modified: Thu Jul 27 23:10:03 2023, max compression
```

## Comparing `hedges-0.0.1a2.tar` & `hedges-0.0.1a3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1004)        0 2023-07-23 20:18:06.067686 hedges-0.0.1a2/
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)       99 2023-07-19 18:52:52.000000 hedges-0.0.1a2/.gitignore
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)      246 2023-07-23 20:16:02.000000 hedges-0.0.1a2/Makefile
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     8554 2023-07-23 20:18:06.067686 hedges-0.0.1a2/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     7403 2023-07-23 19:49:50.000000 hedges-0.0.1a2/README.md
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1004)        0 2023-07-23 20:18:06.067686 hedges-0.0.1a2/hedges/
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)        0 2023-07-11 06:47:01.000000 hedges-0.0.1a2/hedges/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)      162 2023-07-23 20:18:06.000000 hedges-0.0.1a2/hedges/_version.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     1519 2023-07-19 18:59:37.000000 hedges-0.0.1a2/hedges/bc.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)      679 2023-07-15 21:50:14.000000 hedges-0.0.1a2/hedges/fluxes.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)    15144 2023-07-19 18:59:52.000000 hedges-0.0.1a2/hedges/hyperbolic_solver_1d.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     4976 2023-07-19 18:59:56.000000 hedges-0.0.1a2/hedges/quadrature.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     2993 2023-07-11 06:47:01.000000 hedges-0.0.1a2/hedges/rk.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     4367 2023-07-23 19:31:03.000000 hedges-0.0.1a2/hedges/simulation.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)    10270 2023-07-19 19:00:09.000000 hedges-0.0.1a2/hedges/swe_1d.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1004)        0 2023-07-23 20:18:06.067686 hedges-0.0.1a2/hedges.egg-info/
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     8554 2023-07-23 20:18:06.000000 hedges-0.0.1a2/hedges.egg-info/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)      400 2023-07-23 20:18:06.000000 hedges-0.0.1a2/hedges.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)        1 2023-07-23 20:18:06.000000 hedges-0.0.1a2/hedges.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)       23 2023-07-23 20:18:06.000000 hedges-0.0.1a2/hedges.egg-info/requires.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)       12 2023-07-23 20:18:06.000000 hedges-0.0.1a2/hedges.egg-info/top_level.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)   183756 2023-07-23 19:47:59.000000 hedges-0.0.1a2/main.ipynb
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     3391 2023-07-23 19:41:03.000000 hedges-0.0.1a2/main.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     1465 2023-07-19 18:54:57.000000 hedges-0.0.1a2/pyproject.toml
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)       46 2023-07-19 18:10:56.000000 hedges-0.0.1a2/requirements.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)       38 2023-07-23 20:18:06.067686 hedges-0.0.1a2/setup.cfg
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1004)        0 2023-07-27 23:10:03.460245 hedges-0.0.1a3/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)       99 2023-07-19 18:52:52.000000 hedges-0.0.1a3/.gitignore
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)      246 2023-07-23 20:16:02.000000 hedges-0.0.1a3/Makefile
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     8690 2023-07-27 23:10:03.460245 hedges-0.0.1a3/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     7539 2023-07-27 23:08:35.000000 hedges-0.0.1a3/README.md
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1004)        0 2023-07-27 23:10:03.460245 hedges-0.0.1a3/hedges/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)        0 2023-07-27 22:35:03.000000 hedges-0.0.1a3/hedges/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)      162 2023-07-27 23:10:03.000000 hedges-0.0.1a3/hedges/_version.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     3046 2023-07-25 08:44:31.000000 hedges-0.0.1a3/hedges/bc.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)      679 2023-07-15 21:50:14.000000 hedges-0.0.1a3/hedges/fluxes.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)    15144 2023-07-19 18:59:52.000000 hedges-0.0.1a3/hedges/hyperbolic_solver_1d.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     4976 2023-07-19 18:59:56.000000 hedges-0.0.1a3/hedges/quadrature.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     2993 2023-07-11 06:47:01.000000 hedges-0.0.1a3/hedges/rk.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1004)        0 2023-07-27 23:10:03.460245 hedges-0.0.1a3/hedges/swe_1d/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)        0 2023-07-27 22:32:56.000000 hedges-0.0.1a3/hedges/swe_1d/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)    10353 2023-07-27 22:43:29.000000 hedges-0.0.1a3/hedges/swe_1d/pde.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)      827 2023-07-26 08:41:33.000000 hedges-0.0.1a3/hedges/swe_1d/steady.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1004)        0 2023-07-27 23:10:03.460245 hedges-0.0.1a3/hedges.egg-info/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     8690 2023-07-27 23:10:03.000000 hedges-0.0.1a3/hedges.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)      433 2023-07-27 23:10:03.000000 hedges-0.0.1a3/hedges.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)        1 2023-07-27 23:10:03.000000 hedges-0.0.1a3/hedges.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)       23 2023-07-27 23:10:03.000000 hedges-0.0.1a3/hedges.egg-info/requires.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)       12 2023-07-27 23:10:03.000000 hedges-0.0.1a3/hedges.egg-info/top_level.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     7804 2023-07-27 23:07:03.000000 hedges-0.0.1a3/main.ipynb
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     4335 2023-07-27 23:06:15.000000 hedges-0.0.1a3/main.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     1465 2023-07-19 18:54:57.000000 hedges-0.0.1a3/pyproject.toml
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)       46 2023-07-19 18:10:56.000000 hedges-0.0.1a3/requirements.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)       38 2023-07-27 23:10:03.460245 hedges-0.0.1a3/setup.cfg
```

### Comparing `hedges-0.0.1a2/PKG-INFO` & `hedges-0.0.1a3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedges
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: A Discontinuous Galerkin solver oriented toward prototyping and education
 Author-email: schrodingersket <schrodingersket@gmail.com>
 License: LGPL-2.1
 Project-URL: Homepage, https://github.com/schrodingersket/hedges
 Project-URL: Bug Tracker, https://github.com/schrodingersket/hedges/issues
 Keywords: Partial differential equations,Hyperbolic,Scientific computing,Scientific machine learning,Discontinuous Galerkin
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -49,35 +49,38 @@
 The main script (`main.py`) instantiates several instances of `simulation.SWEFlowRunner`, which is
 configured specifically for running simultaneous simulations for prescribed inflow and transmissive 
 outflow for the Shallow Water Equations. While that class may be useful as a reference 
 implementation for running several simulations, the following is a full example of 
 running a single simulation for the purpose of experimentation/modification:
 
 ```python
-#!/usr/bin/env python3
+#!/usr/bin/env python
 # coding: utf-8
 
 # # 1D Discontinuous Galerkin Shallow Water Solver
-# 
+#
 # We solve the 1D Shallow Water Equations in conservative form:
-# 
+#
 # \begin{align*}
 #     h_t + q_x &= 0 \\
 #     q_t + \left[ \frac{q^2}{h} + \frac{1}{2} g h^2 \right]_x &= -g h b_x - C_f \left(\frac{q}{h}\right)^2
 # \end{align*}
-# 
+#
+# We neglect friction so that $C_f = 0$.
+#
+
 import numpy as np
 import matplotlib.pyplot as plt
 
 
 import hedges.bc as bc
 import hedges.fluxes as fluxes
 import hedges.quadrature as quadrature
 import hedges.rk as rk
-import hedges.swe_1d as swe_1d
+import hedges.swe_1d.pde as pde
 
 
 # Physical parameters
 #
 g = 1.0  # gravity
 
 # Domain
@@ -85,15 +88,15 @@
 tspan = (0.0, 4.0)
 xspan = (-1, 1)
 
 # Bathymetry parameters
 #
 b_smoothness = 0.1
 b_amplitude = 0.02
-b_slope = -0.05
+b_slope = 0.05
 assert(b_smoothness > 0)
 
 # Inflow parameters
 #
 inflow_amplitude = 0.05
 inflow_smoothness = 1.0
 inflow_peak_time = 2.0
@@ -105,57 +108,64 @@
 assert(h0 > 0)
 
 
 def swe_bathymetry(x):
     """
     Describes bathymetry with an upslope which is perturbed by a hyperbolic tangent function.
     """
-    return b_slope * x + b_amplitude * np.arctan(x/b_smoothness)
+    return b_slope * x + b_amplitude * np.arctan(x / b_smoothness)
 
 
 def swe_bathymetry_derivative(x):
     """
     Derivative of swe_bathymetry
     """
-    return b_slope * np.ones(x.shape) + b_amplitude * b_smoothness/(1 + np.square(b_smoothness*x)) * np.exp(-np.square(b_smoothness*x))
+    return b_slope + b_amplitude / (
+            b_smoothness * (1 + np.square(x / b_smoothness))
+    )
 
 
 def q_bc(t):
     """
     Describes a Gaussian inflow, where the function transitions to a constant value upon attaining
     its maximum value.
 
     :param t: Time
     :return:
     """
-    tt = np.array(t)
-    return inflow_amplitude * np.exp( -np.square(np.minimum(tt, inflow_peak_time * np.ones(tt.shape)) - inflow_peak_time) / (2 * np.square(inflow_smoothness)) )
+    t_np = np.array(t)
+    return inflow_amplitude * np.exp(
+        -np.square(
+            np.minimum(t_np, inflow_peak_time * np.ones(t_np.shape)) - inflow_peak_time
+        ) / (2 * np.square(inflow_smoothness))
+    )
 
 
 def initial_condition(x):
     """
     Creates initial conditions for (h, uh).
 
     :param x: Computational domain
     :return:
     """
     initial_height = h0 * np.ones(x.shape) - swe_bathymetry(x)  # horizontal water surface
-    initial_flow = q_bc(0) * np.ones(x.shape)  # Start with whatever flow is prescribed by our inflow BC
+    initial_flow = q_bc(0) * np.ones(x.shape)  # Start with inflow BC
 
-    ic = np.array((
+    initial_values = np.array((
         initial_height,
         initial_flow,
     ))
 
     # Verify consistency of initial condition
     #
-    if not np.allclose(ic[1][0], q_bc(0)):
+    if not np.allclose(initial_values[1][0], q_bc(0)):
         raise ValueError('Initial flow condition must match prescribed inflow.')
 
-    return ic
+    return initial_values
+
 
 # Plot bathymetry and ICs
 #
 xl, xr = xspan
 t0, tf = tspan
 
 xx = np.linspace(xl, xr, num=100)
@@ -184,15 +194,15 @@
 q_bc_ax.set_title('Boundary flow rate $q({}, t)$'.format(xl))
 
 plt.tight_layout()
 plt.show()
 
 # Instantiate solver with bathymetry
 #
-solver = swe_1d.ShallowWater1D(
+solver = pde.ShallowWater1D(
     b=swe_bathymetry,
     b_x=swe_bathymetry_derivative,
     gravity=g
 )
 
 
 t_interval_ms = 20
@@ -202,16 +212,23 @@
 solution = solver.solve(
     tspan=tspan,
     xspan=xspan,
     cell_count=16,
     polydeg=4,
     initial_condition=initial_condition,
     intercell_flux=surface_flux,
-    left_boundary_flux=swe_1d.ShallowWater1D.bc_prescribed_inflow(q_bc, gravity=g, surface_flux=surface_flux),
-    right_boundary_flux=bc.transmissive_outflow(surface_flux=surface_flux),
+    left_boundary_flux=pde.ShallowWater1D.bc_prescribed_inflow(
+        q_bc,
+        gravity=g,
+        surface_flux=surface_flux,
+    ),
+    right_boundary_flux=bc.transmissive_boundary(
+        surface_flux=surface_flux,
+        direction=bc.Direction.DOWNSTREAM,
+    ),
     quad_rule=quadrature.gll,
     **{
         'method': rk.SSPRK33,
         't_eval': np.arange(tspan[0], tspan[1], dt),
         'max_step': dt,  # max time step for ODE solver
         'rtol': 1.0e-6,
         'atol': 1.0e-6,
```

### Comparing `hedges-0.0.1a2/README.md` & `hedges-0.0.1a3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,35 +25,38 @@
 The main script (`main.py`) instantiates several instances of `simulation.SWEFlowRunner`, which is
 configured specifically for running simultaneous simulations for prescribed inflow and transmissive 
 outflow for the Shallow Water Equations. While that class may be useful as a reference 
 implementation for running several simulations, the following is a full example of 
 running a single simulation for the purpose of experimentation/modification:
 
 ```python
-#!/usr/bin/env python3
+#!/usr/bin/env python
 # coding: utf-8
 
 # # 1D Discontinuous Galerkin Shallow Water Solver
-# 
+#
 # We solve the 1D Shallow Water Equations in conservative form:
-# 
+#
 # \begin{align*}
 #     h_t + q_x &= 0 \\
 #     q_t + \left[ \frac{q^2}{h} + \frac{1}{2} g h^2 \right]_x &= -g h b_x - C_f \left(\frac{q}{h}\right)^2
 # \end{align*}
-# 
+#
+# We neglect friction so that $C_f = 0$.
+#
+
 import numpy as np
 import matplotlib.pyplot as plt
 
 
 import hedges.bc as bc
 import hedges.fluxes as fluxes
 import hedges.quadrature as quadrature
 import hedges.rk as rk
-import hedges.swe_1d as swe_1d
+import hedges.swe_1d.pde as pde
 
 
 # Physical parameters
 #
 g = 1.0  # gravity
 
 # Domain
@@ -61,15 +64,15 @@
 tspan = (0.0, 4.0)
 xspan = (-1, 1)
 
 # Bathymetry parameters
 #
 b_smoothness = 0.1
 b_amplitude = 0.02
-b_slope = -0.05
+b_slope = 0.05
 assert(b_smoothness > 0)
 
 # Inflow parameters
 #
 inflow_amplitude = 0.05
 inflow_smoothness = 1.0
 inflow_peak_time = 2.0
@@ -81,57 +84,64 @@
 assert(h0 > 0)
 
 
 def swe_bathymetry(x):
     """
     Describes bathymetry with an upslope which is perturbed by a hyperbolic tangent function.
     """
-    return b_slope * x + b_amplitude * np.arctan(x/b_smoothness)
+    return b_slope * x + b_amplitude * np.arctan(x / b_smoothness)
 
 
 def swe_bathymetry_derivative(x):
     """
     Derivative of swe_bathymetry
     """
-    return b_slope * np.ones(x.shape) + b_amplitude * b_smoothness/(1 + np.square(b_smoothness*x)) * np.exp(-np.square(b_smoothness*x))
+    return b_slope + b_amplitude / (
+            b_smoothness * (1 + np.square(x / b_smoothness))
+    )
 
 
 def q_bc(t):
     """
     Describes a Gaussian inflow, where the function transitions to a constant value upon attaining
     its maximum value.
 
     :param t: Time
     :return:
     """
-    tt = np.array(t)
-    return inflow_amplitude * np.exp( -np.square(np.minimum(tt, inflow_peak_time * np.ones(tt.shape)) - inflow_peak_time) / (2 * np.square(inflow_smoothness)) )
+    t_np = np.array(t)
+    return inflow_amplitude * np.exp(
+        -np.square(
+            np.minimum(t_np, inflow_peak_time * np.ones(t_np.shape)) - inflow_peak_time
+        ) / (2 * np.square(inflow_smoothness))
+    )
 
 
 def initial_condition(x):
     """
     Creates initial conditions for (h, uh).
 
     :param x: Computational domain
     :return:
     """
     initial_height = h0 * np.ones(x.shape) - swe_bathymetry(x)  # horizontal water surface
-    initial_flow = q_bc(0) * np.ones(x.shape)  # Start with whatever flow is prescribed by our inflow BC
+    initial_flow = q_bc(0) * np.ones(x.shape)  # Start with inflow BC
 
-    ic = np.array((
+    initial_values = np.array((
         initial_height,
         initial_flow,
     ))
 
     # Verify consistency of initial condition
     #
-    if not np.allclose(ic[1][0], q_bc(0)):
+    if not np.allclose(initial_values[1][0], q_bc(0)):
         raise ValueError('Initial flow condition must match prescribed inflow.')
 
-    return ic
+    return initial_values
+
 
 # Plot bathymetry and ICs
 #
 xl, xr = xspan
 t0, tf = tspan
 
 xx = np.linspace(xl, xr, num=100)
@@ -160,15 +170,15 @@
 q_bc_ax.set_title('Boundary flow rate $q({}, t)$'.format(xl))
 
 plt.tight_layout()
 plt.show()
 
 # Instantiate solver with bathymetry
 #
-solver = swe_1d.ShallowWater1D(
+solver = pde.ShallowWater1D(
     b=swe_bathymetry,
     b_x=swe_bathymetry_derivative,
     gravity=g
 )
 
 
 t_interval_ms = 20
@@ -178,16 +188,23 @@
 solution = solver.solve(
     tspan=tspan,
     xspan=xspan,
     cell_count=16,
     polydeg=4,
     initial_condition=initial_condition,
     intercell_flux=surface_flux,
-    left_boundary_flux=swe_1d.ShallowWater1D.bc_prescribed_inflow(q_bc, gravity=g, surface_flux=surface_flux),
-    right_boundary_flux=bc.transmissive_outflow(surface_flux=surface_flux),
+    left_boundary_flux=pde.ShallowWater1D.bc_prescribed_inflow(
+        q_bc,
+        gravity=g,
+        surface_flux=surface_flux,
+    ),
+    right_boundary_flux=bc.transmissive_boundary(
+        surface_flux=surface_flux,
+        direction=bc.Direction.DOWNSTREAM,
+    ),
     quad_rule=quadrature.gll,
     **{
         'method': rk.SSPRK33,
         't_eval': np.arange(tspan[0], tspan[1], dt),
         'max_step': dt,  # max time step for ODE solver
         'rtol': 1.0e-6,
         'atol': 1.0e-6,
```

### Comparing `hedges-0.0.1a2/hedges/fluxes.py` & `hedges-0.0.1a3/hedges/fluxes.py`

 * *Files identical despite different names*

### Comparing `hedges-0.0.1a2/hedges/hyperbolic_solver_1d.py` & `hedges-0.0.1a3/hedges/hyperbolic_solver_1d.py`

 * *Files identical despite different names*

### Comparing `hedges-0.0.1a2/hedges/quadrature.py` & `hedges-0.0.1a3/hedges/quadrature.py`

 * *Files identical despite different names*

### Comparing `hedges-0.0.1a2/hedges/rk.py` & `hedges-0.0.1a3/hedges/rk.py`

 * *Files identical despite different names*

### Comparing `hedges-0.0.1a2/hedges/swe_1d.py` & `hedges-0.0.1a3/hedges/swe_1d/pde.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 from scipy import optimize
 
-from . import fluxes
-from . import hyperbolic_solver_1d
+from hedges import bc
+from hedges import fluxes
+from hedges import hyperbolic_solver_1d
 
 
 class ShallowWater1D(hyperbolic_solver_1d.Hyperbolic1DSolver):
     solution_vars = 2
 
     def __init__(self, b=None, b_x=None, gravity=9.81):
         """
@@ -267,41 +268,45 @@
 
             return np.array((f1, f2))
         return _flux_function
 
     @staticmethod
     def bc_prescribed_inflow(q_in, gravity=9.81, surface_flux=fluxes.lax_friedrichs_flux):
         """
-        Maintains a (possibly time-dependent) prescribed rate of flow at the inflow boundary by setting
-        backward characteristics for upwinded values and cell values equal at the leftmost boundary.
+        Maintains a (possibly time-dependent) prescribed rate of flow at the inflow boundary by
+        setting backward characteristics for upwinded values and cell values equal at the leftmost
+        boundary.
 
-        :param q_in: A function with time as its single parameter, which should return the rate of flow
-                     at a particular time.
+        :param q_in: A function with time as its single parameter which should return the rate of
+                     flow at a particular time.
         :param gravity: Gravitational constant.
         :param surface_flux: Function used to compute numerical flux between adjacent cell states.
         :return:
         """
-        def _flux_function(u_l, u_r, xx, t, f, f_prime):
+        def qbc(t, u_l, u_r):
             h_r, q_r = u_r
 
             # Backward characteristic
             #
             w_b = q_r / h_r - 2 * np.sqrt(gravity * h_r)
 
             # Evaluate prescribed bathymetry value at t
             #
             q = q_in(t)
 
-            # We solve for the square root of h to avoid numerical issues with Newton's method
+            # We solve for the square root of h to mitigate numerical issues with Newton's method
             #
             sqrt_h = optimize.newton(
                 lambda hh: q / np.square(hh) - 2 * np.sqrt(gravity) * hh - w_b,
                 x0=np.square(h_r),
                 # fprime=lambda hh: -2 * q / hh ** 3 - 2 * np.sqrt(g),
                 maxiter=500
             )
-
             h = np.square(sqrt_h)
 
-            return surface_flux(np.array((h, q)), u_r, xx, t, f, f_prime)
+            return h, q
 
-        return _flux_function
+        return bc.dirichlet_boundary(
+            qbc,
+            surface_flux=surface_flux,
+            direction=bc.Direction.UPSTREAM,
+        )
```

### Comparing `hedges-0.0.1a2/hedges.egg-info/PKG-INFO` & `hedges-0.0.1a3/hedges.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedges
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: A Discontinuous Galerkin solver oriented toward prototyping and education
 Author-email: schrodingersket <schrodingersket@gmail.com>
 License: LGPL-2.1
 Project-URL: Homepage, https://github.com/schrodingersket/hedges
 Project-URL: Bug Tracker, https://github.com/schrodingersket/hedges/issues
 Keywords: Partial differential equations,Hyperbolic,Scientific computing,Scientific machine learning,Discontinuous Galerkin
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -49,35 +49,38 @@
 The main script (`main.py`) instantiates several instances of `simulation.SWEFlowRunner`, which is
 configured specifically for running simultaneous simulations for prescribed inflow and transmissive 
 outflow for the Shallow Water Equations. While that class may be useful as a reference 
 implementation for running several simulations, the following is a full example of 
 running a single simulation for the purpose of experimentation/modification:
 
 ```python
-#!/usr/bin/env python3
+#!/usr/bin/env python
 # coding: utf-8
 
 # # 1D Discontinuous Galerkin Shallow Water Solver
-# 
+#
 # We solve the 1D Shallow Water Equations in conservative form:
-# 
+#
 # \begin{align*}
 #     h_t + q_x &= 0 \\
 #     q_t + \left[ \frac{q^2}{h} + \frac{1}{2} g h^2 \right]_x &= -g h b_x - C_f \left(\frac{q}{h}\right)^2
 # \end{align*}
-# 
+#
+# We neglect friction so that $C_f = 0$.
+#
+
 import numpy as np
 import matplotlib.pyplot as plt
 
 
 import hedges.bc as bc
 import hedges.fluxes as fluxes
 import hedges.quadrature as quadrature
 import hedges.rk as rk
-import hedges.swe_1d as swe_1d
+import hedges.swe_1d.pde as pde
 
 
 # Physical parameters
 #
 g = 1.0  # gravity
 
 # Domain
@@ -85,15 +88,15 @@
 tspan = (0.0, 4.0)
 xspan = (-1, 1)
 
 # Bathymetry parameters
 #
 b_smoothness = 0.1
 b_amplitude = 0.02
-b_slope = -0.05
+b_slope = 0.05
 assert(b_smoothness > 0)
 
 # Inflow parameters
 #
 inflow_amplitude = 0.05
 inflow_smoothness = 1.0
 inflow_peak_time = 2.0
@@ -105,57 +108,64 @@
 assert(h0 > 0)
 
 
 def swe_bathymetry(x):
     """
     Describes bathymetry with an upslope which is perturbed by a hyperbolic tangent function.
     """
-    return b_slope * x + b_amplitude * np.arctan(x/b_smoothness)
+    return b_slope * x + b_amplitude * np.arctan(x / b_smoothness)
 
 
 def swe_bathymetry_derivative(x):
     """
     Derivative of swe_bathymetry
     """
-    return b_slope * np.ones(x.shape) + b_amplitude * b_smoothness/(1 + np.square(b_smoothness*x)) * np.exp(-np.square(b_smoothness*x))
+    return b_slope + b_amplitude / (
+            b_smoothness * (1 + np.square(x / b_smoothness))
+    )
 
 
 def q_bc(t):
     """
     Describes a Gaussian inflow, where the function transitions to a constant value upon attaining
     its maximum value.
 
     :param t: Time
     :return:
     """
-    tt = np.array(t)
-    return inflow_amplitude * np.exp( -np.square(np.minimum(tt, inflow_peak_time * np.ones(tt.shape)) - inflow_peak_time) / (2 * np.square(inflow_smoothness)) )
+    t_np = np.array(t)
+    return inflow_amplitude * np.exp(
+        -np.square(
+            np.minimum(t_np, inflow_peak_time * np.ones(t_np.shape)) - inflow_peak_time
+        ) / (2 * np.square(inflow_smoothness))
+    )
 
 
 def initial_condition(x):
     """
     Creates initial conditions for (h, uh).
 
     :param x: Computational domain
     :return:
     """
     initial_height = h0 * np.ones(x.shape) - swe_bathymetry(x)  # horizontal water surface
-    initial_flow = q_bc(0) * np.ones(x.shape)  # Start with whatever flow is prescribed by our inflow BC
+    initial_flow = q_bc(0) * np.ones(x.shape)  # Start with inflow BC
 
-    ic = np.array((
+    initial_values = np.array((
         initial_height,
         initial_flow,
     ))
 
     # Verify consistency of initial condition
     #
-    if not np.allclose(ic[1][0], q_bc(0)):
+    if not np.allclose(initial_values[1][0], q_bc(0)):
         raise ValueError('Initial flow condition must match prescribed inflow.')
 
-    return ic
+    return initial_values
+
 
 # Plot bathymetry and ICs
 #
 xl, xr = xspan
 t0, tf = tspan
 
 xx = np.linspace(xl, xr, num=100)
@@ -184,15 +194,15 @@
 q_bc_ax.set_title('Boundary flow rate $q({}, t)$'.format(xl))
 
 plt.tight_layout()
 plt.show()
 
 # Instantiate solver with bathymetry
 #
-solver = swe_1d.ShallowWater1D(
+solver = pde.ShallowWater1D(
     b=swe_bathymetry,
     b_x=swe_bathymetry_derivative,
     gravity=g
 )
 
 
 t_interval_ms = 20
@@ -202,16 +212,23 @@
 solution = solver.solve(
     tspan=tspan,
     xspan=xspan,
     cell_count=16,
     polydeg=4,
     initial_condition=initial_condition,
     intercell_flux=surface_flux,
-    left_boundary_flux=swe_1d.ShallowWater1D.bc_prescribed_inflow(q_bc, gravity=g, surface_flux=surface_flux),
-    right_boundary_flux=bc.transmissive_outflow(surface_flux=surface_flux),
+    left_boundary_flux=pde.ShallowWater1D.bc_prescribed_inflow(
+        q_bc,
+        gravity=g,
+        surface_flux=surface_flux,
+    ),
+    right_boundary_flux=bc.transmissive_boundary(
+        surface_flux=surface_flux,
+        direction=bc.Direction.DOWNSTREAM,
+    ),
     quad_rule=quadrature.gll,
     **{
         'method': rk.SSPRK33,
         't_eval': np.arange(tspan[0], tspan[1], dt),
         'max_step': dt,  # max time step for ODE solver
         'rtol': 1.0e-6,
         'atol': 1.0e-6,
```

### Comparing `hedges-0.0.1a2/pyproject.toml` & `hedges-0.0.1a3/pyproject.toml`

 * *Files identical despite different names*

