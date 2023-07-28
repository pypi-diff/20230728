# Comparing `tmp/GQCConstraints-1.0.0.tar.gz` & `tmp/GQCConstraints-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GQCConstraints-1.0.0.tar", last modified: Tue Jul 25 15:59:01 2023, max compression
+gzip compressed data, was "GQCConstraints-1.1.0.tar", last modified: Fri Jul 28 19:44:25 2023, max compression
```

## Comparing `GQCConstraints-1.0.0.tar` & `GQCConstraints-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:59:01.542950 GQCConstraints-1.0.0/GQCC/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/GQCC/Methods/
--rw-r--r--   0 runner    (1001) docker     (122)    14754 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Methods/EntanglementStudy.py
--rw-r--r--   0 runner    (1001) docker     (122)    10437 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Methods/ExpectationValueSearch.py
--rw-r--r--   0 runner    (1001) docker     (122)     4808 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Methods/MultiplierScan.py
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Methods/PotentialEnergySurface.py
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/GQCC/Optimization/
--rw-r--r--   0 runner    (1001) docker     (122)     9917 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Optimization/SpinResolvedOptimizationFunctions.py
--rw-r--r--   0 runner    (1001) docker     (122)     6573 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Optimization/SpinResolvedOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11825 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Optimization/SpinUnresolvedOptimizationFunctions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5066 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Optimization/SpinUnresolvedOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Optimization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/
--rw-r--r--   0 runner    (1001) docker     (122)     8314 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/FCI.py
--rw-r--r--   0 runner    (1001) docker     (122)     6196 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/HubbardFCI.py
--rw-r--r--   0 runner    (1001) docker     (122)    11662 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/UHF.py
--rw-r--r--   0 runner    (1001) docker     (122)     8580 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/UNOCI.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/
--rw-r--r--   0 runner    (1001) docker     (122)     7797 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/FCI.py
--rw-r--r--   0 runner    (1001) docker     (122)     9889 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/GHF.py
--rw-r--r--   0 runner    (1001) docker     (122)     6505 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/GNOCI.py
--rw-r--r--   0 runner    (1001) docker     (122)     5929 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/HubbardFCI.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/GQCConstraints.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-07-25 15:59:01.000000 GQCConstraints-1.0.0/GQCConstraints.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-07-25 15:59:01.000000 GQCConstraints-1.0.0/GQCConstraints.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 15:59:01.000000 GQCConstraints-1.0.0/GQCConstraints.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-25 15:59:01.000000 GQCConstraints-1.0.0/GQCConstraints.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-25 15:59:01.000000 GQCConstraints-1.0.0/GQCConstraints.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 19:44:25.287660 GQCConstraints-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 19:44:25.287660 GQCConstraints-1.1.0/GQCC/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 19:44:25.287660 GQCConstraints-1.1.0/GQCC/Methods/
+-rw-r--r--   0 runner    (1001) docker     (122)    14704 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/Methods/EntanglementStudy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10637 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/Methods/ExpectationValueSearch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/Methods/MultiplierScan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6460 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/Methods/PotentialEnergySurface.py
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/Methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 19:44:25.287660 GQCConstraints-1.1.0/GQCC/Optimization/
+-rw-r--r--   0 runner    (1001) docker     (122)     9867 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/Optimization/SpinResolvedOptimizationFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7567 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/Optimization/SpinResolvedOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11774 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/Optimization/SpinUnresolvedOptimizationFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5825 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/Optimization/SpinUnresolvedOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/Optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 19:44:25.287660 GQCConstraints-1.1.0/GQCC/SpinResolvedConstraints/
+-rw-r--r--   0 runner    (1001) docker     (122)    10191 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/SpinResolvedConstraints/FCI.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9296 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/SpinResolvedConstraints/HubbardFCI.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14926 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/SpinResolvedConstraints/UHF.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10980 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/SpinResolvedConstraints/UNOCI.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/SpinResolvedConstraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 19:44:25.287660 GQCConstraints-1.1.0/GQCC/SpinUnresolvedConstraints/
+-rw-r--r--   0 runner    (1001) docker     (122)    10778 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/SpinUnresolvedConstraints/FCI.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12966 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/SpinUnresolvedConstraints/GHF.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9502 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/SpinUnresolvedConstraints/GNOCI.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9073 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/SpinUnresolvedConstraints/HubbardFCI.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15884 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/SpinUnresolvedConstraints/UHF.py
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/SpinUnresolvedConstraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/GQCC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 19:44:25.287660 GQCConstraints-1.1.0/GQCConstraints.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-07-28 19:44:25.000000 GQCConstraints-1.1.0/GQCConstraints.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1066 2023-07-28 19:44:25.000000 GQCConstraints-1.1.0/GQCConstraints.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 19:44:25.000000 GQCConstraints-1.1.0/GQCConstraints.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-28 19:44:25.000000 GQCConstraints-1.1.0/GQCConstraints.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-28 19:44:25.000000 GQCConstraints-1.1.0/GQCConstraints.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-07-28 19:44:25.287660 GQCConstraints-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1760 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-28 19:44:25.287660 GQCConstraints-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-07-28 19:44:15.000000 GQCConstraints-1.1.0/setup.py
```

### Comparing `GQCConstraints-1.0.0/GQCC/Methods/EntanglementStudy.py` & `GQCConstraints-1.1.0/GQCC/Methods/EntanglementStudy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 """
-Entanglement study
+Entanglement Study
 ------------------
 
-Pre-defined methods that can be used to study the entanglement between subsystems and the environment.
+.. warning::
+
+    The entanglement study method is only implemented for constrained calculations applied to the **Hubbard Model**. 
+
+A pre-defined methods that can be used to study the entanglement between subsystems and the environment.
+
+.. note::
+
+    Examples on how to use our pre-defined methods can be found in the Jupyter notebook examples on our `GitHub page <https://github.com/GQCG-res/GQCConstraints/tree/develop/examples>`_.
 
 """
 
-# Import dependancies
+# Import dependencies
 import pandas as pd
 import GQCC.Methods.MultiplierScan as scan
 import GQCC.Methods.ExpectationValueSearch as search
 
 
 def ofSpinResolvedExpectationValueSearch(constrained_object, optimization_function, expectation_value_grid, domain_partition_p, domain_partition_q, domain_partition_pq, initial_alpha_guesses=None, initial_beta_guesses=None, return_parameters=False, threshold=1e-5, verbose=0, **options):
     """
     An optimization that optimizes the multiplier at each one of the provided expectation values, for the given constrained object.
 
-    Note: Entanglement studies are only active for objects in the 'ConstrainedHubbard' module.
-
     :param constrained_object:          The GQCC constrained object that will be used for the calculations.
     :param optimization_function:       The optimization function that will be used to optimize the multipliers. Can be a pre-defined function by GQCC or a self-implemented function that adheres to the same form.
     :param expectation_value_grid:      The series of expectation values at which the multiplier will be optimized.
     :param domain_partition_p:          The domain partition for the first domain.
     :param domain_partition_q:          The domain partition for the second domains.
     :param domain_partition_pq:         The domain partition of the first and second domain combined.
     :param initial_alpha_guesses:       The series of initial guesses for the optimization, if required.
@@ -65,16 +71,14 @@
         return resolved_search_output
 
 
 def ofSpinResolvedMultiplierScan(constrained_object, multiplier_grid, domain_partition_p, domain_partition_q, domain_partition_pq, return_parameters=False, verbose=0):
     """
     An entanglement study of a multiplier scan for unresolved constrained Hubbard methods.
 
-    Note: Entanglement studies are only active for objects in the 'ConstrainedHubbard' module.
-
     :param constrained_object:      The constrained object on which the multipliers will be applied.
     :param multiplier_grid:         The provided grid of multipliers.
     :param domain_partition_p:      The domain partition for the first domain.
     :param domain_partition_q:      The domain partition for the second domains.
     :param domain_partition_pq:     The domain partition of the first and second domain combined.
     :param return_parameters:       A boolean flag to indicate whether only the wavefunction parameters should also be returned.
     :param verbose:                 An integer representing the amount of output that will be printed.
@@ -108,16 +112,14 @@
         return resolved_scan_output
 
 
 def ofSpinUnresolvedExpectationValueSearch(constrained_object, optimization_function, expectation_values, domain_partition_p, domain_partition_q, domain_partition_pq, initial_guesses=None, return_parameters=False, threshold=1e-5, verbose=0, **options):
     """
     An optimization that optimizes the multiplier at each one of the provided expectation values, for the given constrained object.
 
-    Note: Entanglement studies are only active for objects in the 'ConstrainedHubbard' module.
-
     :param constrained_object:          The GQCC constrained object that will be used for the calculations.
     :param optimization_function:       The optimization function that will be used to optimize the multipliers. Can be a pre-defined function by GQCC or a self-implemented function that adheres to the same form.
     :param expectation_values:          The series of expectation values at which the multiplier will be optimized.
     :param domain_partition_p:          The domain partition for the first domain.
     :param domain_partition_q:          The domain partition for the second domains.
     :param domain_partition_pq:         The domain partition of the first and second domain combined.
     :param initial_guesses:             The series of initial guesses for the optimization, if required.
@@ -158,16 +160,14 @@
         return unresolved_search_output
 
 
 def ofSpinUnresolvedMultiplierScan(constrained_object, multipliers, domain_partition_p, domain_partition_q, domain_partition_pq, return_parameters=False, verbose=0):
     """
     An entanglement study of a multiplier scan for unresolved constrained Hubbard methods.
 
-    Note: Entanglement studies are only active for objects in the 'ConstrainedHubbard' module.
-
     :param constrained_object:      The constrained object on which the multipliers will be applied.
     :param multipliers:             The provided range of multipliers.
     :param domain_partition_p:      The domain partition for the first domain.
     :param domain_partition_q:      The domain partition for the second domains.
     :param domain_partition_pq:     The domain partition of the first and second domain combined.
     :param return_parameters:       A boolean flag to indicate whether only the wavefunction parameters should also be returned.
     :param verbose:                 An integer representing the amount of output that will be printed.
```

### Comparing `GQCConstraints-1.0.0/GQCC/Methods/ExpectationValueSearch.py` & `GQCConstraints-1.1.0/GQCC/Methods/ExpectationValueSearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
-Expectation value search
+Expectation Value Search
 ------------------------
 
-Pre-defined methods that take a series of expectation values and optimize the multiplier for the constrained method at each one of them.
+A pre-defined methods that take a series of expectation values and optimize the multiplier for the constrained method at each one of them.
 
+.. note::
+
+    Examples on how to use our pre-defined methods can be found in the Jupyter notebook examples on our `GitHub page <https://github.com/GQCG-res/GQCConstraints/tree/develop/examples>`_.
 """
 
-# Import dependancies
+# Import dependencies
 import pandas as pd
 
 
 def spinResolved(constrained_object, optimization_function, expectation_value_grid, initial_alpha_guesses=None, initial_beta_guesses=None, return_parameters=False, threshold=1e-5, verbose=0, **options):
     """
     An optimization that optimizes the multiplier at each one of the provided expectation values, for the given constrained object.
```

### Comparing `GQCConstraints-1.0.0/GQCC/Methods/MultiplierScan.py` & `GQCConstraints-1.1.0/GQCC/Methods/MultiplierScan.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """
-Multiplier scan
+Multiplier Scan
 ----------------
 
 A pre-defined method that scans over a given range of multipliers and applies each of them to the constrained object provided.
 
+.. note::
+
+    Examples on how to use our pre-defined methods can be found in the Jupyter notebook examples on our `GitHub page <https://github.com/GQCG-res/GQCConstraints/tree/develop/examples>`_.
 """
 
 # Import dependencies
 import pandas as pd
 
 
 def spinResolved(constrained_object, multiplier_grid, return_parameters=False, verbose=0):
```

### Comparing `GQCConstraints-1.0.0/GQCC/Methods/PotentialEnergySurface.py` & `GQCConstraints-1.1.0/GQCC/Methods/PotentialEnergySurface.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 Potential Energy Surface
 -------------------------
 
 A pre-defined method that takes a series of constrained objects, each from a different internuclear distance & calculates the energies and parameters for each one of them.
 
 Each calculation happens at the same constraint.
 
+.. note::
+
+    Examples on how to use our pre-defined methods can be found in the Jupyter notebook examples on our `GitHub page <https://github.com/GQCG-res/GQCConstraints/tree/develop/examples>`_.
 """
 
 # Import dependencies
 import pandas as pd
 import numpy as np
```

### Comparing `GQCConstraints-1.0.0/GQCC/Optimization/SpinResolvedOptimizationFunctions.py` & `GQCConstraints-1.1.0/GQCC/Optimization/SpinResolvedOptimizationFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Optimization Functions for Optimizing a Spin Resolved Parameter
----------------------------------------------------------------
+Optimization Functions - Spin Resolved
+--------------------------------------
 
 The pre-defined optimization functions for a expectation value search calculation in a spin resolved constrained quantum chemical method framework.
 
 If the user does not want to use these predefined functions, the possibility to add a self-defined optimization function is also provided within the library.
 
 """
 
@@ -184,11 +184,11 @@
         _, spinResolved_W, _ = constrained_method_setup.calculateEnergyAndExpectationValue([mua, mub])
 
         # Create a delta N array. Squares are used to make the function more well behaved.  
         delta_N = np.array([(spinResolved_W[0] - expected_expectation_value_array[0]) ** 2, (spinResolved_W[1] - expected_expectation_value_array[1]) ** 2])
                     
         return delta_N.T @ delta_N
                 
-    # Use the global optimization algorithm `brute` in order to find the minimim.
+    # Use the global optimization algorithm `brute` in order to find the minimum.
     optimized = optimize.basinhopping(objective_function, x0=initial_guess, **options)
     
     return optimized.x
```

### Comparing `GQCConstraints-1.0.0/GQCC/Optimization/SpinResolvedOptimizer.py` & `GQCConstraints-1.1.0/GQCC/Optimization/SpinResolvedOptimizer.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,14 +26,26 @@
 
         :param value_array:              The expectation value for which we want to find the multiplier.
         :param optimize_function:        The optimize function used for finding the mu value.
         :param initial_guess:            The initial guess for the optimization. If `None` a guess is chosen for you (default). 
         :param options:                  The possible options that can be passed to the optimization function.
         
         :returns:                        The optimized mu values for alpha and beta.
+
+        To optimize a set of Lagrange multipliers to yield a certain expectation value for alpha and beta (0.5 and 0.0) we can all this method.
+
+        .. code-block:: python
+
+            optimized_mu = Constrained_object.optimizeMultiplier([0.5, 0.0], GQCC.SpinResolvedOptimizationFunctions.GlobalBrute, ranges=((-1, 1), (-1, 1)), Ns=100)
+
+        .. note::
+
+            `optimized_mu` is an array that looks like this: `[optimized_alpha_mu, optimized_beta_mu]`.
+
+        This can be done with any spin-resolved optimization function and the preferred options associated with that function.
         """
         # Raise an exception if the multiplier is not conform with the requirements.
         if type(value_array) is float or len(value_array) != 2:
              raise ValueError("Value_array must be of dimension 2 as it must contain both an alpha and beta value.")
 
         if initial_guess is not None and (type(initial_guess) is float or len(value_array) != 2):
              raise ValueError("Initial guess must be None or must be of dimension 2 as it must contain both an alpha and beta value.")
@@ -51,14 +63,20 @@
         :param optimized_mu:                       The optimized mu found with an optimization function.
         :param expected_value_array:               The expectation values values expected at the optimized mu values for both alpha and beta.
         :return_parameters:                        A boolean flag that specifies whether the wavefunction parameters are also returned.
         :param threshold:                          The threshold at which the calculated and expected values are compared.
         :param verbose:                            An integer representing the amount of output that will be printed.
 
         :returns:                                  The energy belonging to the multiplier/expectation value combination. If the expected and calculated values don't match, None is returned.
+
+        If you ran an optimization calculation, it is imperative to check whether or not your optimization was successful and does indeed result in the wanted expectation values, i.e. 0.5 and 0.0. To do so call this method with your optimized multiplier.
+
+        .. code-block:: python
+
+            energy = Constrained_object.verifyCombination([optimized_alpha_mu, optimized_beta_mu], [0.5, 0.0])
         """
         # Raise an exception if the multiplier is not conform with the requirements.
         if type(expected_value_array) is float or len(expected_value_array) != 2:
              raise ValueError("Expected_value_array must be of dimension 2 as it must contain both an alpha and beta value.")
 
         if return_parameters:
             E, spinResolved_W, _, par = self.calculateEnergyAndExpectationValue(optimized_mu, return_parameters)
```

### Comparing `GQCConstraints-1.0.0/GQCC/Optimization/SpinUnresolvedOptimizationFunctions.py` & `GQCConstraints-1.1.0/GQCC/Optimization/SpinUnresolvedOptimizationFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Optimization Functions for Optimizing a Spin Unresolved Parameter
------------------------------------------------------------------
+Optimization Functions - Spin Unresolved
+----------------------------------------
 
 The pre-defined optimization functions for a expectation value search calculation in a spin unresolved constrained quantum chemical method framework.
 
 If the user does not want to use these predefined functions, the possibility to add a self-defined optimization function is also provided within the library.
 
 """
 
@@ -161,15 +161,15 @@
     :param options:                         The options contain a bracket, the maximum_iterations, the tolerance and a boolean log parameter.
 
     :returns:                               An optimized multiplier belonging to the estimated expectation value.
     """
 
     # Define the bisection algorithm
     def _bisection_algorithm(objective_function, target_value, bracket=None, maximum_iterations=10000, tolerance=1e-4, log=False):
-        # Timling for the calculation.
+        # Timing for the calculation.
         start = time.time()
 
         # dictionary containing information about the optimization.
         infodict = {}
 
         # Number of iterations
         iter = 1
```

### Comparing `GQCConstraints-1.0.0/GQCC/Optimization/SpinUnresolvedOptimizer.py` & `GQCConstraints-1.1.0/GQCC/Optimization/SpinUnresolvedOptimizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,22 @@
         Note:                            It is possible to write an optimize function that takes an initial guess.
 
         :param expectation value:        The expectation value value for which we want to find the multiplier.
         :param optimize_function:        The optimize function used for finding the mu value. 
         :param options:                  The possible options that can be passed to the optimization function.
         
         :returns:                        The optimized mu value.
+
+        To optimize a Lagrange multiplier to yield a certain expectation value (0.5) we can all this method.
+
+        .. code-block:: python
+
+            optimized_mu = Constrained_object.optimizeMultiplier(0.5, GQCC.SpinUnresolvedOptimizationFunctions.GoldenLineSearch)
+
+        This can be done with any spin-unresolved optimization function and the preferred options associated with that function.
         """
         # We can modify the optimize_function at will, as long as it takes the same arguments and returns an optimized mu value
         optimized_mu = optimize_function(expectation_value, self, initial_guess, **options)
        
         return optimized_mu
         
         
@@ -48,14 +56,20 @@
         :param expected_value:          The expectation value expected at the optimized mu value.
         :param return_parameters:       A boolean flag to indicate whether only the wavefunction parameters should also be returned.
         :param threshold:               The threshold at which the calculated and expected value are compared.
         :param verbose:                 An integer representing the amount of output that will be printed.
 
         :returns:                       The energy belonging to the multiplier/expectation value combination. If the expected and calculated expectation values don't match, None is returned.
         :returns:                       The ground state parameters belonging to the multiplier/expectation value combination. If the expected and calculated expectation values don't match, None is returned (only if return_parameters is set to True).
+
+        If you ran an optimization calculation, it is imperative to check whether or not your optimization was successful and does indeed result in the wanted expectation value, i.e. 0.5. To do so call this method with your optimized multiplier.
+
+        .. code-block:: python
+
+            energy = Constrained_object.verifyCombination(optimized_mu, 0.5)
         """
         if return_parameters:
             E, W, par = self.calculateEnergyAndExpectationValue(optimized_mu, return_parameters)
         else:
             E, W = self.calculateEnergyAndExpectationValue(optimized_mu, return_parameters)
     
         if m.isclose(W, expected_value, abs_tol=threshold):
```

### Comparing `GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/FCI.py` & `GQCConstraints-1.1.0/GQCC/SpinUnresolvedConstraints/GNOCI.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,139 +1,167 @@
 """
-Spin resolved constraints applied to full configuration interaction calculations
---------------------------------------------------------------------------------
+Spin Unresolved Constraints - GNOCI
+-----------------------------------
 
-This class sets up everything needed for a spin resolved constrained CI calculation. The required variables (Hamiltonian, ONV-Basis,...), as well as the required methods. 
+This module is used for constraining spin-unresolved operators in non-orthogonal configuration interaction calculations, carried out in a basis of generalized states. By setting up the constrained GNOCI object, the module prepares the basic functionalities to run constrained calculations for single values or to be used in one of the pre-set methods offered by GQCC.
 
 """
 
 # Import statements
 import gqcpy
 import numpy as np
 
-from GQCC.Optimization.SpinResolvedOptimizer import SpinResolvedOptimizer
+from GQCC.Optimization.SpinUnresolvedOptimizer import SpinUnresolvedOptimizer
 
-class FCI(SpinResolvedOptimizer):
+
+class GNOCI(SpinUnresolvedOptimizer):
     """
-    A constructor that sets up everything needed for spin resolved constrained CI calculations.
+    A constructor that sets up everything needed for constrained NOCI calculations in a generalized basis.
 
     :param molecule:                    The GQCP molecule used for the calculations.
     :param SQ_basis:                    The second quantized GQCP basis set used for the calculations, defined for a molecule in a certain basis set. Make sure it is the same basis as in which the operator is defined.
-    :param operator:                    The GQCP operator that will be constrained.        
+    :param basis_state_vector:          A vector of non-orthogonal states that will serve as a basis for NOCI.
+    :param operator:                    The GQCP operator that will be constrained.    
     :param constrained_observable:      The name of the observable being constrained.
 
-    :returns:                 An object which contains all required data (basis, Hamiltonian,... ) and possesses the necessary methods to perform calculations.
+    :returns:                       An object which contains all required data (basis, Hamiltonian,... ) and possesses the necessary methods to perform calculations.
+
+    First we need to set up some basic variables with GQCP.
+
+    .. code-block:: python
+
+        H3 =  gqcpy.Molecule.HRingFromDistance(3, 1.88972, 0)   # The molecule.
+        basis = gqcpy.GSpinorBasis_d(H3, "STO-3G")              # The spinor basis.
+
+    And an operator (:math:`S_z`).
+
+    .. code-block:: python
+
+        Sz = basis.quantize(gqcpy.ElectronicSpin_zOperator())
+
+    For GNOCI we need a vector of basis states consisting of generalized states, `basis_vector`. One way to generate such states is by running several constrained GHF calculations. 
+
+    .. note:: 
+    
+        For info on generating states with constrained GHF see the `Constrained Hartree-Fock <https://gqcg-res.github.io/GQCConstraints/ConstrainedHartreeFock.html>`_ section or look at our `examples on github <https://github.com/GQCG-res/GQCConstraints/tree/develop/examples>`_.
+
+    Once we have a everything, the constrained NOCI object can be created with GQCC.
+
+    .. code-block:: python
+
+        Constrained_object = GQCC.SpinUnresolvedConstraints.GNOCI(H3, basis, basis_vector, Sz, "Sz value")
     """
-    def __init__(self, molecule, SQ_basis, operator, constrained_observable): 
-        # Check compatibility of the operator type based on the used basis_type.
-        if type(SQ_basis) is gqcpy.gqcpy.USpinOrbitalBasis_d:
-            compatible_operators = [gqcpy.gqcpy.ScalarUSQOneElectronOperator_d, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_d]
-        elif type(SQ_basis) is gqcpy.gqcpy.USpinOrbitalBasis_cd:
-            compatible_operators = [gqcpy.gqcpy.ScalarUSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_cd]
+    def __init__(self, molecule, SQ_basis, basis_state_vector, operator, constrained_observable):
+        # Check compatibility of the operator type based on the used basis type.
+        if type(SQ_basis) is gqcpy.gqcpy.GSpinorBasis_d:
+            compatible_operators = [gqcpy.gqcpy.ScalarGSQOneElectronOperator_d, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_d]
+        elif type(SQ_basis) is gqcpy.gqcpy.GSpinorBasis_cd:
+            compatible_operators = [gqcpy.gqcpy.ScalarGSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_cd, gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_cd]
         else:
-            raise ValueError("the chosen `SQ_basis` is not compatible with this type of calculation. Use `gqcpy.USpinOrbitalBasis_(c)d`instead.")
-        
-        assert (type(operator) in compatible_operators), "Only `ScalarUSQOneElectronOperator_(c)d` or `ScalarUSQTwoElectronOperator_(c)d` can be constrained with this method."     
+            raise ValueError("the chosen `SQ_basis` or `solver` is not compatible with this type of calculation. Use `gqcpy.GSpinorBasis_(c)d`instead.")
+        assert (type(operator) in compatible_operators), "Only `ScalarGSQOneElectronOperator_(c)d` or `ScalarGSQTwoElectronOperator_(c)d` can be constrained with this method."     
 
-        # We can now create a first quantized hamiltonian and use the spin orbital basis to "quantize" it to second quantization.
-        # The SQHamiltonian is stored in the class object.
-        fq_hamiltonian = gqcpy.FQMolecularHamiltonian(molecule)
-        self._sq_hamiltonian = SQ_basis.quantize(fq_hamiltonian)
-
-        # Since we are going to do full CI calculations, we need an ONV-basis.
-        # From the total number of orbitals and total number of electrons we can set up an ONV basis.
-        K = int(SQ_basis.numberOfSpinors() / 2)
-        N_total = molecule.numberOfElectrons()
-
-        if N_total % 2 == 0:
-            N_a = int(N_total / 2)
-            N_b = int(N_total / 2)
-        else:
-            N_a = int(np.ceil(N_total / 2))
-            N_b = int(np.floor(N_total / 2))
+        # Here, a molecule does need to be saved as it is needed to construct the NOCI Hamiltonian.
+        self._molecule = molecule
+
+        # Save the number of electrons.
+        self._N = molecule.numberOfElectrons()
 
-        # The ONV basis gets stored within the class object.
-        self._onv_basis = gqcpy.SpinResolvedONVBasis(K, N_a, N_b)
+        # Quantize the Hamiltonian in the spinor basis.
+        self._sq_hamiltonian = SQ_basis.quantize(gqcpy.FQMolecularHamiltonian(molecule))
 
-        # Calculate the nuclear repulsion term and store it in the class object.
-        self._nuclear_repulsion = gqcpy.NuclearRepulsionOperator(molecule.nuclearFramework()).value()
+        # Save the overlap operator.
+        self._overlap = SQ_basis.quantize(gqcpy.OverlapOperator())
 
-        # Store the operator.
+        # Generate a Non-orthogonal state basis.
+        self._NOCIBasis = gqcpy.GNonOrthogonalStateBasis_d(basis_state_vector, self._overlap, self._N)
+
+        # Save the operator you want to constrain.
         self._operator = operator
-        
         self._constrained_observable = constrained_observable
-        self._constrained_alpha_observable = "alpha " + self._constrained_observable
-        self._constrained_beta_observable = "beta " + self._constrained_observable
-    
 
-    def _solveCIEigenproblem(self, hamiltonian):
+
+    # A solver for the NOCI problem.
+    def _solveNOCIEigenproblem(self, hamiltonian):
         """
-        A method used to solve an unrestricted CI eigenproblem.
+        A method used to solve a NOCI eigenproblem.
 
-        :param hamiltonian:      The USQHamiltonian used for the calculation.
+        :param hamiltonian:      The SQHamiltonian used for the calculation.
 
         :returns:                The ground state energy.
         :returns:                The ground state parameters
         """
-        # Use GQCP to set up a full CI calculation.
-        if type(hamiltonian) is gqcpy.gqcpy.USQHamiltonian_d:
-            CIsolver = gqcpy.EigenproblemSolver.Dense_d()
-            CIenvironment = gqcpy.CIEnvironment.Dense(hamiltonian, self._onv_basis)
-            qc_structure = gqcpy.CI(self._onv_basis).optimize(CIsolver, CIenvironment)
+        if type(hamiltonian) is gqcpy.gqcpy.GSQHamiltonian_d:
+            environment = gqcpy.NOCIEnvironment.Dense_d(hamiltonian, self._NOCIBasis, self._molecule)
+            solver = gqcpy.GeneralizedEigenproblemSolver.Dense_d()
+            qc_structure = gqcpy.NOCI_d(self._NOCIBasis).optimize(solver, environment)
         else:
-            CIsolver = gqcpy.EigenproblemSolver.Dense_cd()
-            CIenvironment = gqcpy.CIEnvironment.Dense_cd(hamiltonian, self._onv_basis)
-            qc_structure = gqcpy.CI_cd(self._onv_basis).optimize(CIsolver, CIenvironment)
+            environment = gqcpy.NOCIEnvironment.Dense_cd(hamiltonian, self._NOCIBasis, self._molecule)
+            solver = gqcpy.GeneralizedEigenproblemSolver.Dense_cd()
+            qc_structure = gqcpy.NOCI_cd(self._NOCIBasis).optimize(solver, environment)
 
         return qc_structure.groundStateEnergy(), qc_structure.groundStateParameters()
-        
 
-    def calculateEnergyAndExpectationValue(self, multiplier_array, return_parameters=False, verbose=0):
+     
+    # A function to calculate the energy and expectation value of NOCI at a certain multiplier. 
+    def calculateEnergyAndExpectationValue(self, multiplier, return_parameters=False, verbose=0):
         """
         A method used to calculate the energy and the expectation value at a given multiplier `mu`.
 
-        :param multiplier_array:      The multiplier used to modify the Hamiltonian. Must be an array/list that contains an alpha and beta value.
+        :param multiplier_array:      The multiplier used to modify the Hamiltonian.
         :param verbose:               An integer representing the amount of output that will be printed.
         :return_parameters:           A boolean flag that specifies whether the wavefunction parameters are also returned.
 
         :returns:                     The energy at the given `mu` values.
-        :returns:                     The alpha/beta expectation values at the given `mu` values.
-        :returns:                     The total spin unresolved expectation value at the given `mu`.
+        :returns:                     The expectation value of the operator at the given `mu` value.
         :returns:                     The wavefunction parameters (only if `return_parameters` is set to `True`).
+
+        In order to calculate the energy and expectation value of your operator, associated with a certain Lagrange multiplier (let's say -1).
+
+        .. code-block:: python
+
+            energy, expval = Constrained_object.calculateEnergyAndExpectationValue(-1)
+        
         """
-        # Raise an exception if the multiplier is not conform with the requirements.
-        if type(multiplier_array) is float or len(multiplier_array) != 2:
-             raise ValueError("Multiplier_array must be of dimension 2 as it must contain both an alpha and beta value.")
-
-        # Modify the Hamiltonian with the given multiplier. Do this respectively for the alpha and beta parts.
-        # This is done differently when the operator is a one electron operator.
-        if type(self._operator) in [gqcpy.gqcpy.ScalarUSQOneElectronOperator_d, gqcpy.gqcpy.ScalarUSQOneElectronOperator_cd]:
-            unrestricted_operator = type(self._operator)((self._operator.alpha * multiplier_array[0]), (self._operator.beta * multiplier_array[1]))
-            modified_hamiltonian = self._sq_hamiltonian - unrestricted_operator
-        # Or a two electron operator.
-        elif type(self._operator) in [gqcpy.gqcpy.ScalarUSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_cd]:
-            raise NotImplementedError("This is to be implemented after the general refactor is done.")
+        # Modify the Hamiltonian with the given multiplier.
+        # For a one- or two- electron operator this happens in the same way.
+        # Note that the one-electron operator modifies the one-electron intergrals, and the two-electron operator modifies the two-electron integrals.
+        if type(self._operator) in [gqcpy.gqcpy.ScalarGSQOneElectronOperator_d, gqcpy.gqcpy.ScalarGSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_cd]:
+            modified_hamiltonian = self._sq_hamiltonian - multiplier * self._operator
+        # For an operator product.
+        elif type(self._operator) in [gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_d, gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_cd]:
+            modified_hamiltonian = self._sq_hamiltonian - (multiplier * self._operator.oneElectron()) - (multiplier * self._operator.twoElectron())
         else:
-            raise ValueError("Something went wrong with the operator type.")
-
-        # Use the private method to solve the full CI eigenproblem.
-        gs_energy, gs_parameters = self._solveCIEigenproblem(modified_hamiltonian)
+            raise ValueError("Something went wrong with the operator type.") 
 
-        # Use the ground state parameters to calculate the 1DM and use it to calculate the expectation value of the Mulliken operator.
-        # The separate alpha and beta expectation values are calculated as well.
-        D = gs_parameters.calculateSpinResolved1DM()
+        gs_energy, gs_parameters = self._solveNOCIEigenproblem(modified_hamiltonian)
 
-        total_expectation_value = self._operator.calculateExpectationValue(D)[0]
-        alpha_expectation_value = self._operator.alpha.calculateExpectationValue(D.alpha)[0]
-        beta_expectation_value = self._operator.beta.calculateExpectationValue(D.beta)[0]
+        # Calculate the density matrices.
+        D = gs_parameters.calculate1DM()
+        #d = gs_parameters.calculate2DM()
+
+        # Calculate the expectation value of the constrained operator.
+        # This differs depending on which kind of operator is being used.
+        # For a one electron operator.
+        if type(self._operator) in [gqcpy.gqcpy.ScalarGSQOneElectronOperator_d, gqcpy.gqcpy.ScalarGSQOneElectronOperator_cd]:
+            expectation_value = self._operator.calculateExpectationValue(D)[0]
+        # For a two electron operator.
+        elif type(self._operator) in [gqcpy.gqcpy.ScalarGSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_cd]:
+            raise NotImplementedError("The NOCI 2DM is not yet implemented in GQCP. As such this functionality is not yet available.")
+            #expectation_value = self._operator.calculateExpectationValue(d)[0]
+        # For an operator product.
+        elif type(self._operator) in [gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_d, gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_cd]:
+            raise NotImplementedError("The NOCI 2DM is not yet implemented in GQCP. As such this functionality is not yet available.")
+            #expectation_value = self._operator.calculateExpectationValue(D, d)
 
-        # Calculate the energy by correcting the ground state energy of the modified Hamiltonian.
-        energy = gs_energy + (multiplier_array[0] * alpha_expectation_value) + (multiplier_array[1] * beta_expectation_value) + self._nuclear_repulsion
+        # Perform the energy correction.
+        energy = gs_energy  + (multiplier * expectation_value)
 
         # Print the progress of which mu values have been completed if verbose >= 2.
         if verbose >= 2:
             print("--------------------------------------------------------")
-            print("Mu combo: alpha = " + str(np.around(multiplier_array[0], 2)) + " , beta = " + str(np.around(multiplier_array[1], 2)) + " done.")
+            print("Mu = " + str(np.around(multiplier, 2)) + " done.")
+
         if return_parameters:
-            return energy, [alpha_expectation_value, beta_expectation_value], total_expectation_value, gs_parameters
+            return energy, expectation_value, gs_parameters
         else:
-            return energy, [alpha_expectation_value, beta_expectation_value], total_expectation_value
+            return energy, expectation_value
```

### Comparing `GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/HubbardFCI.py` & `GQCConstraints-1.1.0/GQCC/SpinResolvedConstraints/HubbardFCI.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-Spin resolved constraints applied to FCI calculations on the Hubbard model.
----------------------------------------------------------------------------
+Spin Resolved Constraints - Hubbard FCI
+---------------------------------------
 
-This class sets up everything needed for a resolved constrained FCI calculation on the Hubbard model. The required variables (Hamiltonian, ONV-Basis,...), as well as the required methods. 
+This module is used for constraining spin-resolved operators in full configuration interaction calculations on the Hubbard model. By setting up the constrained Hubbard FCI object, the module prepares the basic functionalities to run constrained calculations for single values or to be used in one of the pre-set methods offered by GQCC.
 
 """
 
 # Import statements
 import gqcpy
 import numpy as np
 
@@ -18,14 +18,45 @@
 
     
     :param hubbard_hamiltonian:              The GQCP Hubbard Hamiltonian defining the Hubbard model.
     :param operator:                         The GQCP operator that will be constrained.        
     :param constrained_observable:           The name of the observable being constrained.
 
     :returns:                       An object which contains all required data (basis, Hamiltonian,... ) and possesses the necessary methods to perform calculations.
+
+    To initialize a Hubbard FCI object we need a Hubbard Hamiltonian and an operator from GQCP. The Hubbard Hamiltonian can be constructed.
+
+    .. code-block:: python
+
+        L = 3       # number of sites
+        t = 1e-4    # hopping parameter
+        U = 1.0     # on-site repulsion
+        
+        adjacency_matrix = gqcpy.AdjacencyMatrix.Linear(L)
+        hopping_matrix = gqcpy.HoppingMatrix.Homogeneous(adjacency_matrix, t)
+        unmodified_hubbard_chain = gqcpy.HubbardHamiltonian(hopping_matrix, U)
+
+    .. note::
+
+        The Hubbard Hamiltonian does not need to be Homogeneous. Any GQCP Hubbard Hamiltonian will work.
+    
+    and an operator (e.g. number operator) can be made with the following code.
+
+    .. code-block:: python
+
+        P = np.zeros((L, L))
+        P[0, 0] = 1
+        operator_component = gqcpy.ScalarUSQOneElectronOperatorComponent_d(P)
+        number_operator = gqcpy.ScalarUSQOneElectronOperator_d(operator_component, operator_component)
+
+    A constrained Hubbard FCI object can then be constructed.
+
+    .. code-block:: python
+
+        Constrained_object = GQCC.SpinResolvedConstraints.HubbardFCI(unmodified_hubbard_chain, number_operator, "population")
     """
     def __init__(self, hubbard_hamiltonian, operator, constrained_observable):
         # Check compatibility of the operator type based on the used basis_type.
         compatible_operators = [gqcpy.gqcpy.ScalarUSQOneElectronOperator_d, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_d]        
         assert (type(operator) in compatible_operators), "Only `ScalarUSQOneElectronOperator_d` or `ScalarUSQTwoElectronOperator_d` can be constrained with this method."
 
         # Hopping matrix of the defined Hubbard model.
@@ -57,14 +88,32 @@
         """
         A method to calculate the von Neumann entropy of a certain partition within the Hubbard model.
 
         :param domain_partition:              The partition of the universe into "system" and "environment" for which the entropic relations will be calculated.
         :param wavefunction_parameters:       The parameters of the final wavefunction for which the entropic measures will be calculated.
 
         :returns:                             The Von Neumann entropy calculated according to eq. 6 in the following paper by Rissler et. al.: https://doi.org/10.1016/j.chemphys.2005.10.018.
+
+        The Hubbard module can also look at the entanglement between different **domain partitions**. To do so we need to define certain domain partitions.
+
+        .. code-block:: python
+
+            domain_partition_p = gqcpy.DiscreteDomainPartition([0, 1, 1])
+            domain_partition_q = gqcpy.DiscreteDomainPartition([1, 0, 1])
+
+        .. note::
+
+            To calculate entanglement you need the wavefunction parameters. To get them, set **return_parameters** to **True** in the `calculateEnergyAndExpectationValue()` or the `verifyCombination()` method.
+
+        Using these partitions along with the wavefunction parameters, we can calculate the von Neumann entropy.
+
+        .. code-block:: python
+
+            Sp = Constrained_object.vonNeumannEntropy(domain_partition_p, parameters)
+            Sq = Constrained_object.vonNeumannEntropy(domain_partition_q, parameters)
         """
         # Sometimes, the result will not fullfil the constraint. If this is the case, no parameters are saved.
         # This clause circumvents the error that would arise if the type of the saved wavefunction parameters is wrong.
         if type(wavefunction_parameters) is not gqcpy.gqcpy.LinearExpansion_SpinResolved:
             return None
 
         # Calculate the orbital RDM.
@@ -87,14 +136,33 @@
 
         :param domain_partition_p:               The partition of the universe into "system" and "environment" for which the first domain.
         :param domain_partition_q:               The partition of the universe into "system" and "environment" for which the second domain.
         :param domain_partition_pq:              The partition of the universe into "system" and "environment" for which the domain containing domain one and two.
         :param wavefunction_parameters:          The parameters of the final wavefunction for which the entropic measures will be calculated.
 
         :returns:                                The mutual information of site one and two calculated according to eq. 8 in the following paper by Rissler et. al.: https://doi.org/10.1016/j.chemphys.2005.10.018.
+
+        The mutual information is an entanglement measure that elucidates how much two domains know about one another. To use this we need domain partitions for the two single site von Neumann entropies and one of the two site entropy.
+
+        .. code-block:: python
+
+            domain_partition_pq = gqcpy.DiscreteDomainPartition([0, 0, 1])
+            domain_partition_p = gqcpy.DiscreteDomainPartition([0, 1, 1])
+            domain_partition_q = gqcpy.DiscreteDomainPartition([1, 0, 1])
+
+        Now we can call the mutual information.
+
+        .. note::
+
+            To calculate mutual information you need the wavefunction parameters. To get them, set **return_parameters** to **True** in the `calculateEnergyAndExpectationValue()` or the `verifyCombination()` method.
+
+        .. code-block:: python
+
+            I_pq = Constrained_object.mutualInformation(domain_partition_p, domain_partition_q, domain_partition_pq, parameters)
+
         """
         # Sometimes, the result will not fullfil the constraint. If this is the case, no parameters are saved.
         # This clause circumvents the error that would arise if the type of the saved wavefunction parameters is wrong.
         if type(wavefunction_parameters) is not gqcpy.gqcpy.LinearExpansion_SpinResolved:
             return None
         
         S_p = self.vonNeumannEntropy(domain_partition_p, wavefunction_parameters)
```

### Comparing `GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/UHF.py` & `GQCConstraints-1.1.0/GQCC/SpinUnresolvedConstraints/GHF.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,191 +1,227 @@
 """
-Spin Resolved Constraints applied to unrestricted Hartree-Fock
---------------------------------------------------------------
+Spin Unresolved Constraints - GHF
+---------------------------------
 
-This class sets up everything needed for a spin resolved Constrained UHF calculation. The required variables (Hamiltonian, Basis,...), as well as the required methods. 
+This module is used for constraining spin-unresolved operators in generalized Hartree-Fock calculations. By setting up the constrained GHF object, the module prepares the basic functionalities to run constrained calculations for single values or to be used in one of the pre-set methods offered by GQCC.
 
 """
 
 # Import statements
 import gqcpy
 import numpy as np
 import numpy.random as rand
 
-from GQCC.Optimization.SpinResolvedOptimizer import SpinResolvedOptimizer
+from GQCC.Optimization.SpinUnresolvedOptimizer import SpinUnresolvedOptimizer
 
 
-class UHF(SpinResolvedOptimizer):
+class GHF(SpinUnresolvedOptimizer):
     """
-    A constructor that sets up everything needed for constrained UHF calculations.
+    A constructor that sets up everything needed for constrained GHF calculations.
 
     :param molecule:                    The GQCP molecule used for the calculations.
-    :param electrons:                   The amount of alpha and beta electrons in the molecule as an array.
     :param SQ_basis:                    The second quantized GQCP basis set used for the calculations, defined for a molecule in a certain basis set. Make sure it is the same basis as in which the operator is defined.
     :param solver:                      The solver used for the UHF calculations.
     :param initial_guess:               The initial guess for the UHF calculation.
     :param operator:                    The GQCP operator that will be constrained.     
     :param constrained_observable:      The name of the observable being constrained.
     :param stability_analysis:          Boolean flag denoting whether stability analysis is performed. Default is `True`.
 
-    :returns:                           An object which contains all required data (basis, Hamiltonian,... ) and possesses the necessary methods to perform calculations.
+
+    :returns:                An object which contains all required data (basis, Hamiltonian,... ) and possesses the necessary methods to perform calculations.
+
+    In order to set up a GHF calculation with spin unresolved constraints we need several GQCP elements. First, set up some basic variables.
+
+    .. code-block:: python
+
+        H3 =  gqcpy.Molecule.HRingFromDistance(3, 1.88972, 0)                                       # The molecule.
+        basis = gqcpy.GSpinorBasis_d(H3, "STO-3G")                                                  # The spinor basis.
+        solver = gqcpy.GHFSCFSolver_d.Plain(threshold=1e-8, maximum_number_of_iterations=250000)    # The solver for the Hartree-Fock algorithm.
+
+    We also need to give the object an initial guess for the SCF procedure. In this case, let's generate a random symmetric guess.
+
+    .. code-block:: python
+
+        import numpy.random as rand
+
+        rand.seed(2)
+        random_matrix = np.random.rand(basis.numberOfSpinors(), basis.numberOfSpinors())
+        random_matrix_transpose = random_matrix.T
+        symmetric_random_matrix = random_matrix + random_matrix_transpose
+        _, guess = np.linalg.eigh(symmetric_random_matrix)
+        init_guess = gqcpy.GTransformation_d(guess)
+
+    Now we choose an operator to constrain. Let's take the :math:`S_z` operator.
+
+    .. code-block:: python
+
+        Sz = basis.quantize(gqcpy.ElectronicSpin_zOperator())
+
+    Finally we can construct the constrained object using GQCC.
+
+    .. code-block:: python
+
+        Constrained_object = GQCC.SpinUnresolvedConstraints.GHF(H3, basis, solver, init_guess, Sz, "Sz value")
+
     """
-    def __init__(self, molecule, electrons, SQ_basis, solver, initial_guess, operator, constrained_observable, stability_analysis=True):
-        # Raise an exception if the electrons array is not conform with the requirements.
-        if type(electrons[0]) is float or type(electrons[1]) is float or len(electrons) != 2:
-            raise ValueError("Electrons must be of dimension 2 and must contain two ìnt`s as it must contain the number of alpha and beta electrons.")
-        
+    def __init__ (self, molecule, SQ_basis, solver, initial_guess, operator, constrained_observable, stability_analysis=True):
         # Check compatibility of the operator type based on the used basis type.
-        if type(SQ_basis) is gqcpy.gqcpy.USpinOrbitalBasis_d:
-            compatible_operators = [gqcpy.gqcpy.ScalarUSQOneElectronOperator_d, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_d]
-            assert (type(solver) is gqcpy.gqcpy.IterativeAlgorithm_UHFSCFEnvironment)
-
-        elif type(SQ_basis) is gqcpy.gqcpy.USpinOrbitalBasis_cd:
-            compatible_operators = [gqcpy.gqcpy.ScalarUSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_cd]
-            assert (type(solver) is gqcpy.gqcpy.IterativeAlgorithm_UHFSCFEnvironment_cd)
+        if type(SQ_basis) is gqcpy.gqcpy.GSpinorBasis_d:
+            compatible_operators = [gqcpy.gqcpy.ScalarGSQOneElectronOperator_d, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_d]
+            assert (type(solver) is gqcpy.gqcpy.IterativeAlgorithm_GHFSCFEnvironment_d)
+
+        elif type(SQ_basis) is gqcpy.gqcpy.GSpinorBasis_cd:
+            compatible_operators = [gqcpy.gqcpy.ScalarGSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_cd, gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_cd]
+            assert (type(solver) is gqcpy.gqcpy.IterativeAlgorithm_GHFSCFEnvironment_cd)
 
         else:
-            raise ValueError("the chosen `SQ_basis` or `solver` is not compatible with this type of calculation. Use `gqcpy.USpinOrbitalBasis_(c)d`instead.")
-        assert (type(operator) in compatible_operators), "Only `ScalarUSQOneElectronOperator_(c)d` or `ScalarUSQTwoElectronOperator_(c)d` can be constrained with this method."     
+            raise ValueError("the chosen `SQ_basis` or `solver` is not compatible with this type of calculation. Use `gqcpy.GSpinorBasis_(c)d`instead.")
+        assert (type(operator) in compatible_operators), "Only `ScalarGSQOneElectronOperator_(c)d` or `ScalarGSQTwoElectronOperator_(c)d` can be constrained with this method."     
 
         # This basis can now quantize the Hamiltonian.
         self._sq_hamiltonian = SQ_basis.quantize(gqcpy.FQMolecularHamiltonian(molecule))
 
         # We will need the number of electrons, as well as the total number of Spinors later on.        
-        self._Ka = SQ_basis.numberOfSpinors() // 2
-        self._Kb = SQ_basis.numberOfSpinors() // 2
-
-        self._Na = electrons[0]
-        self._Nb = electrons[1]
+        self._K = SQ_basis.numberOfSpinors()
+        self._N = molecule.numberOfElectrons()
 
         # Save the overlap and nuclear repulsion operators. 
         self._nuclear_repulsion = gqcpy.NuclearRepulsionOperator(molecule.nuclearFramework()).value()
         self._overlap = SQ_basis.quantize(gqcpy.OverlapOperator())
 
         # Save the operator you want to constrain.
         self._operator = operator
-
         self._constrained_observable = constrained_observable
-        self._constrained_alpha_observable = "alpha " + self._constrained_observable
-        self._constrained_beta_observable = "beta " + self._constrained_observable
 
-        # Select the type of solver for the SCF algorithm and where to start the iterations.
+        # Select the type of solver for the SCF algorithm.
         self._solver = solver
         self._initial_guess = initial_guess
 
-        # Wheter to perform a stability check for each calculation.
+        # Whether to perform a stability check for each calculation.
         self._stability_analysis = stability_analysis
 
 
-    # A solver for the UHF problem.
-    def _solveUHFProblem(self, hamiltonian):
+    # A solver for the GHF problem.
+    # The GHF solver always takes a random guess, in order to activate the `off-diagonal` blocks. 
+    def _solveGHFProblem(self, hamiltonian):
         """
-        A method used to solve the iterative UHF problem. A stability check is performed automatically. If an internal instability is encountered, it will be followed by rotating the coefficeints in the direction of the lowest Hessian eigenvector. This will be shown in the output.
+        A method used to solve the iterative GHF problem. A stability check is performed automatically. If an internal instability is encountered, it will be followed by rotating the coefficients in the direction of the lowest Hessian eigenvector. This will be shown in the output.
 
-        :param hamiltonian:      The USQHamiltonian used for the calculation.
+        :param hamiltonian:      The GSQHamiltonian used for the calculation.
 
         :returns:                The ground state energy.
         :returns:                The ground state parameters
         """
 
         # To solve the GHF problem we need an environment and a solver.
-        if type(hamiltonian) is gqcpy.gqcpy.USQHamiltonian_d:
-            environment = gqcpy.UHFSCFEnvironment_d(self._Na, self._Nb, hamiltonian, self._overlap, self._initial_guess)
-            qc_structure = gqcpy.UHF_d.optimize(self._solver, environment)
+        if type(hamiltonian) is gqcpy.gqcpy.GSQHamiltonian_d:
+            environment = gqcpy.GHFSCFEnvironment_d(self._N, hamiltonian, self._overlap, self._initial_guess)
+            qc_structure = gqcpy.GHF_d.optimize(self._solver, environment)
         else:
-            environment = gqcpy.UHFSCFEnvironment_cd(self._Na, self._Nb, hamiltonian, self._overlap, self._initial_guess)
-            qc_structure = gqcpy.UHF_cd.optimize(self._solver, environment)
+            environment = gqcpy.GHFSCFEnvironment_cd(self._N, hamiltonian, self._overlap, self._initial_guess)
+            qc_structure = gqcpy.GHF_cd.optimize(self._solver, environment)
 
         if self._stability_analysis:
-            # For unrestricted Hartree-Fock, a stability check can be performed.
+            # For generalized Hartree-Fock, a stability check is always performed.
             # Transform the hamiltonian to MO basis and calculate the stability matrices. Print the resulting stabilities of the wavefunction model.
             coefficients = qc_structure.groundStateParameters().expansion()
             MO_hamiltonian = hamiltonian.transformed(coefficients)
             stability_matrices = qc_structure.groundStateParameters().calculateStabilityMatrices(MO_hamiltonian)
 
             internal_stability = stability_matrices.isInternallyStable(-1e-5)
 
             while internal_stability is False:
                 print("**************************************************************")
                 print("There is an internal instability. Follow it using the Hessian.")
                 print("**************************************************************")
 
                 # Rotate the coefficients in the direction of the lowest Hessian eigenvector.
-                rotation = stability_matrices.instabilityRotationMatrix(self._Na, self._Nb, self._Ka-self._Na, self._Kb-self._Nb)
+                rotation = stability_matrices.instabilityRotationMatrix(self._N, self._K-self._N)
                 coefficients_rotated = coefficients.rotated(rotation)
 
                 # Perform a new SCF calculation with the rotated coefficients as initial guess.
-                if type(hamiltonian) is gqcpy.gqcpy.USQHamiltonian_d:
-                    environment_rotated = gqcpy.UHFSCFEnvironment_d(self._Na, self._Nb, hamiltonian, self._overlap, coefficients_rotated)
-                    qc_structure = gqcpy.UHF_d.optimize(self._solver, environment_rotated)
+                if type(hamiltonian) is gqcpy.gqcpy.GSQHamiltonian_d:
+                    environment_rotated = gqcpy.GHFSCFEnvironment_d(self._N, hamiltonian, self._overlap, coefficients_rotated)
+                    qc_structure = gqcpy.GHF_d.optimize(self._solver, environment_rotated)
                 else:
-                    environment_rotated = gqcpy.UHFSCFEnvironment_d(self._Na, self._Nb, hamiltonian, self._overlap, coefficients_rotated)
-                    qc_structure = gqcpy.UHF_d.optimize(self._solver, environment_rotated)
+                    environment_rotated = gqcpy.GHFSCFEnvironment_cd(self._N, hamiltonian, self._overlap, coefficients_rotated)
+                    qc_structure = gqcpy.GHF_cd.optimize(self._solver, environment_rotated)
 
                 coefficients_2 = qc_structure.groundStateParameters().expansion()
 
                 # Perform a new stability check. Print the resulting stabilities.
                 hamiltonian_MO_2 = hamiltonian.transformed(coefficients_2)
                 stability_matrices_2 = qc_structure.groundStateParameters().calculateStabilityMatrices(hamiltonian_MO_2)
 
-                # Print the new stability consitions.
+                # Print the new stability conditions.
                 stability_matrices_2.printStabilityDescription()
 
                 # Update the internal stability parameter.
                 internal_stability = stability_matrices_2.isInternallyStable(-1e-5)
 
                 if internal_stability:
                     print("**************************************************************")
 
         return qc_structure.groundStateEnergy(), qc_structure.groundStateParameters()
 
 
-    # A function to calculate the energy and expectation value value of UHF at a certain multiplier. 
-    def calculateEnergyAndExpectationValue(self, multiplier_array, return_parameters=False, verbose=0):
+    # A function to calculate the energy and expectation value value of GHF at a certain multiplier. 
+    def calculateEnergyAndExpectationValue(self, multiplier, return_parameters=False, verbose=0):
         """
         A method used to calculate the energy and the expectation value at a given multiplier `mu`.
 
-        :param multiplier_array:      The multiplier used to modify the Hamiltonian.
-        :param verbose:               An integer representing the amount of output that will be printed.
-        :return_parameters:           A boolean flag that specifies whether the wavefunction parameters are also returned.
-
-        :returns:                     The energy at the given `mu` values.
-        :returns:                     The alpha/beta expectation values at the given `mu` values.
-        :returns:                     The total spin unresolved expectation value at the given `mu`.
-        :returns:                     The wavefunction parameters (only if `return_parameters` is set to `True`).
-        """
-        # Raise an exception if the multiplier is not conform with the requirements.
-        if type(multiplier_array) is float or len(multiplier_array) != 2:
-             raise ValueError("Multiplier_array must be of dimension 2 as it must contain both an alpha and beta value.")
+        :param multiplier:      The multiplier used to modify the Hamiltonian.
+        :param verbose:         An integer representing the amount of output that will be printed.
+        :return_parameters:     A boolean flag that specifies whether the wavefunction parameters are also returned.
 
-        # Modify the Hamiltonian with the given multiplier.
-        # Do this respectively for the alpha and beta parts.
-        if type(self._operator) in [gqcpy.gqcpy.ScalarUSQOneElectronOperator_d, gqcpy.gqcpy.ScalarUSQOneElectronOperator_cd]:
-            unrestricted_operator = type(self._operator)((self._operator.alpha * multiplier_array[0]), (self._operator.beta * multiplier_array[1]))
-            modified_hamiltonian = self._sq_hamiltonian - unrestricted_operator
-        # Or a two electron operator.
-        elif type(self._operator) in [gqcpy.gqcpy.ScalarUSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_cd]:
-            raise NotImplementedError("This is to be implemented after the general refactor is done.")
-        else:
-            raise ValueError("Something went wrong with the operator type.")
+        :returns:               The energy at the given `mu` values.
+        :returns:               The expectation value of the operator at the given `mu` value.
+        :returns:               The wavefunction parameters (only if `return_parameters` is set to `True`).
 
+        In order to calculate the energy and expectation value of your operator, associated with a certain Lagrange multiplier (let's say -1).
 
-        gs_energy, gs_parameters = self._solveUHFProblem(modified_hamiltonian)
+        .. code-block:: python
 
-        # Calculate the expectation value of the operator.
+            energy, expval = Constrained_object.calculateEnergyAndExpectationValue(-1)
+        
+        """
+        # Modify the Hamiltonian with the given multiplier.
+        # For a one- or two- electron operator this happens in the same way.
+        # Note that the one-electron operator modifies the one-electron intergrals, and the two-electron operator modifies the two-electron integrals.
+        if type(self._operator) in [gqcpy.gqcpy.ScalarGSQOneElectronOperator_d, gqcpy.gqcpy.ScalarGSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_cd]:
+            modified_hamiltonian = self._sq_hamiltonian - multiplier * self._operator
+        # For an operator product.
+        elif type(self._operator) in [gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_d, gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_cd]:
+            modified_hamiltonian = self._sq_hamiltonian - (multiplier * self._operator.oneElectron()) - (multiplier * self._operator.twoElectron())
+        else:
+            raise ValueError("Something went wrong with the operator type.") 
+        
+        gs_energy, gs_parameters = self._solveGHFProblem(modified_hamiltonian)
+
+        # Calculate the density matrices.
         D = gs_parameters.calculateScalarBasis1DM()
+        d = gs_parameters.calculateScalarBasis2DM()
 
-        total_expectation_value = self._operator.calculateExpectationValue(D)[0]
-        alpha_expectation_value = self._operator.alpha.calculateExpectationValue(D.alpha)[0]
-        beta_expectation_value = self._operator.beta.calculateExpectationValue(D.beta)[0]
+        # Calculate the expectation value of the constrained operator.
+        # This differs depending on which kind of operator is being used.
+        # For a one electron operator.
+        if type(self._operator) in [gqcpy.gqcpy.ScalarGSQOneElectronOperator_d, gqcpy.gqcpy.ScalarGSQOneElectronOperator_cd]:
+            expectation_value = self._operator.calculateExpectationValue(D)[0]
+        # For a two electron operator.
+        elif type(self._operator) in [gqcpy.gqcpy.ScalarGSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_cd]:
+            expectation_value = self._operator.calculateExpectationValue(d)[0]
+        # For an operator product.
+        elif type(self._operator) in [gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_d, gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_cd]:
+            expectation_value = self._operator.calculateExpectationValue(D, d)
 
-        # Calculate the energy by correcting the ground state energy of the modified Hamiltonian.
-        energy = gs_energy + (multiplier_array[0] * alpha_expectation_value) + (multiplier_array[1] * beta_expectation_value) + self._nuclear_repulsion
+        # Perform the energy correction
+        energy = gs_energy + ((multiplier * expectation_value) + self._nuclear_repulsion)
 
         # Print the progress of which mu values have been completed if verbose >= 2.
         if verbose >= 2:
             print("--------------------------------------------------------")
-            print("Mu combo: alpha = " + str(np.around(multiplier_array[0], 2)) + " , beta = " + str(np.around(multiplier_array[1], 2)) + " done.")
+            print("Mu = " + str(np.around(multiplier, 2)) + " done.")
+
         if return_parameters:
-            return energy, [alpha_expectation_value, beta_expectation_value], total_expectation_value, gs_parameters
+            return energy, expectation_value, gs_parameters
         else:
-            return energy, [alpha_expectation_value, beta_expectation_value], total_expectation_value
+            return energy, expectation_value
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/UNOCI.py` & `GQCConstraints-1.1.0/GQCC/SpinResolvedConstraints/UNOCI.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-Spin resolved constraints applied to Non-Orthogonal CI in an Unrestricted basis
--------------------------------------------------------------------------------
+Spin Resolved Constraints - UNOCI
+---------------------------------
 
-This class sets up everything needed for a Constrained NOCI calculation, based on unrestricted states. The required variables (Hamiltonian, Basis,...), as well as the required methods. 
+This module is used for constraining spin-resolved operators in non-orthogonal configuration interaction calculations, carried out in a basis of unrestricted states. By setting up the constrained UNOCI object, the module prepares the basic functionalities to run constrained calculations for single values or to be used in one of the pre-set methods offered by GQCC.
 
 """
 
 # Import statements
 import gqcpy
 import numpy as np
 
@@ -21,25 +21,54 @@
     :param electrons:                   The amount of alpha and beta electrons in the molecule as an array.
     :param SQ_basis:                    The second quantized GQCP basis set used for the calculations, defined for a molecule in a certain basis set. Make sure it is the same basis as in which the operator is defined.
     :param basis_state_vector:          A vector of non-orthogonal states that will serve as a basis for NOCI.
     :param operator:                    The GQCP operator that will be constrained.    
     :param constrained_observable:      The name of the observable being constrained.
 
     :returns:                           An object which contains all required data (basis, Hamiltonian,... ) and possesses the necessary methods to perform calculations.
+
+    First we need to set up some basic variables with GQCP.
+
+    .. code-block:: python
+
+        H3 =  gqcpy.Molecule.HRingFromDistance(3, 1.88972, 0)   # The molecule.
+        electrons = [2,1]                                       # The number of alpha and beta electrons.
+        spinor_basis = gqcpy.USpinOrbitalBasis_d(H3, "STO-3G")  # The spin orbital basis.
+
+    We also set up an operator (Mulliken in this case).
+
+    .. code-block:: python
+
+        S = spinor_basis.quantize(gqcpy.OverlapOperator())
+        mulliken_domain = spinor_basis.mullikenDomain(lambda shell: shell.nucleus().position()[1] == 0 and shell.nucleus().position()[2] == 0)
+        P = mulliken_domain.projectionMatrix(spinor_basis.expansion())
+        mulliken_operator = S.partitioned(P)
+
+    For UNOCI we need a vector of basis states consisting of unrestricted states, `basis_vector`. One way to generate such states is by running several constrained UHF calculations. 
+
+    .. note:: 
+    
+        For info on generating states with constrained UHF see the `Constrained Hartree-Fock <https://gqcg-res.github.io/GQCConstraints/ConstrainedHartreeFock.html>`_ section or look at our `examples on github <https://github.com/GQCG-res/GQCConstraints/tree/develop/examples>`_.
+
+    Once we have a everything, the constrained NOCI object can be created with GQCC.
+
+    .. code-block:: python
+
+        Constrained_object = GQCC.SpinResolvedConstraints.UNOCI(H3, electrons, spinor_basis, basis_vector, mulliken_operator, "population")
     """
     def __init__(self, molecule, electrons, SQ_basis, basis_state_vector, operator, constrained_observable):
         # Raise an exception if the electrons array is not conform with the requirements.
         if type(electrons[0]) is float or type(electrons[1]) is float or len(electrons) != 2:
             raise ValueError("Electrons must be of dimension 2 and must contain two ìnt`s as it must contain the number of alpha and beta electrons.")
         
         # Check compatibility of the operator type based on the used basis type.
         if type(SQ_basis) is gqcpy.gqcpy.USpinOrbitalBasis_d:
-            compatible_operators = [gqcpy.gqcpy.ScalarUSQOneElectronOperator_d, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_d]
+            compatible_operators = [gqcpy.gqcpy.ScalarUSQOneElectronOperator_d, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarUSQOneElectronOperatorProduct_d]
         elif type(SQ_basis) is gqcpy.gqcpy.USpinOrbitalBasis_cd:
-            compatible_operators = [gqcpy.gqcpy.ScalarUSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_cd]
+            compatible_operators = [gqcpy.gqcpy.ScalarUSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_cd, gqcpy.gqcpy.ScalarUSQOneElectronOperatorProduct_cd]
         else:
             raise ValueError("the chosen `SQ_basis` or `solver` is not compatible with this type of calculation. Use `gqcpy.USpinOrbitalBasis_(c)d`instead.")
         assert (type(operator) in compatible_operators), "Only `ScalarUSQOneElectronOperator_(c)d` or `ScalarUSQTwoElectronOperator_(c)d` can be constrained with this method."     
 
         # Here, a molecule does need to be saved as it is needed to construct the NOCI Hamiltonian.
         self._molecule = molecule
 
@@ -95,30 +124,40 @@
         :param verbose:               An integer representing the amount of output that will be printed.
         :return_parameters:           A boolean flag that specifies whether the wavefunction parameters are also returned.
 
         :returns:                     The energy at the given `mu` values.
         :returns:                     The alpha/beta expectation values at the given `mu` values.
         :returns:                     The total spin unresolved expectation value at the given `mu`.
         :returns:                     The wavefunction parameters (only if `return_parameters` is set to `True`).
+
+        In order to calculate the energy and expectation value of your operator, associated with a certain Lagrange multiplier for the alpha and beta part (let's say -1 and -1).
+
+        .. code-block:: python
+
+            energy, alpha_beta_expval, total_expval = Constrained_object.calculateEnergyAndExpectationValue([-1, -1])
+        
         """
         # Raise an exception if the multiplier is not conform with the requirements.
         if type(multiplier_array) is float or len(multiplier_array) != 2:
              raise ValueError("Multiplier_array must be of dimension 2 as it must contain both an alpha and beta value.")
 
         # Modify the Hamiltonian with the given multiplier. Do this respectively for the alpha and beta parts.
         # This is done differently when the operator is a one electron operator.
         if type(self._operator) in [gqcpy.gqcpy.ScalarUSQOneElectronOperator_d, gqcpy.gqcpy.ScalarUSQOneElectronOperator_cd]:
             unrestricted_operator = type(self._operator)((self._operator.alpha * multiplier_array[0]), (self._operator.beta * multiplier_array[1]))
             modified_hamiltonian = self._sq_hamiltonian - unrestricted_operator
         # Or a two electron operator.
         elif type(self._operator) in [gqcpy.gqcpy.ScalarUSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_cd]:
-            raise NotImplementedError("This is to be implemented after the general refactor is done.")
+            raise NotImplementedError("This is not yet implemented. Some general issues need to be cleared out before this can be added.")
+        # Or an operator product.
+        elif type(self._operator) in [gqcpy.gqcpy.ScalarUSQOneElectronOperatorProduct_d, gqcpy.gqcpy.ScalarUSQOneElectronOperatorProduct_cd]:
+            raise NotImplementedError("This is not yet implemented. Some general issues need to be cleared out before this can be added.")
         else:
             raise ValueError("Something went wrong with the operator type.")
-
+        
         # Use the private method to solve the full CI eigenproblem.
         gs_energy, gs_parameters = self._solveNOCIEigenproblem(modified_hamiltonian)
 
         # Use the ground state parameters to calculate the 1DM and use it to calculate the expectation value of the Mulliken operator.
         # The separate alpha and beta expectation values are calculated as well.
         D = gs_parameters.calculate1DM()
```

### Comparing `GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/FCI.py` & `GQCConstraints-1.1.0/GQCC/SpinUnresolvedConstraints/FCI.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-Spin unresolved constraints applied on full configuration interaction calculations
------------------------------------------------------------------------------
+Spin Unresolved Constraints - FCI
+---------------------------------
 
-This class sets up everything needed for an unresolved constrained CI calculation. The required variables (Hamiltonian, ONV-Basis,...), as well as the required methods. 
+This module is used for constraining spin-unresolved operators in full configuration interaction calculations. By setting up the constrained FCI object, the module prepares the basic functionalities to run constrained calculations for single values or to be used in one of the pre-set methods offered by GQCC.
 
 """
 
 # Import statements
 import gqcpy
 import numpy as np
 
@@ -19,25 +19,59 @@
 
     :param molecule:         The molecule used for the calculations.
     :param basis_set:        The basis set used for the calculations.
     :param operator:         The operator that will be constrained.
     :param basis:            The type of basis in which the FCI calculation will be performed. Default is restricted.
 
     :returns:                An object which contains all required data (basis, Hamiltonian,... ) and possesses the necessary methods to perform calculations.
+    
+    To initialize a constrained FCI object, we need several objects from GQCP.
+
+    First, we need a molecule.
+
+    .. code-block:: python
+
+        H2 =  gqcpy.Molecule.HChain(2, 4.5, 0)
+
+    Secondly, we need to create our spin-orbital basis. Since this is FCI, it should be orthonormal.
+
+    .. code-block:: python
+
+        basis = gqcpy.RSpinOrbitalBasis_d(H2, "6-31G")
+        basis.lowdinOrthonormalize()
+
+    Finally we can create a spin-unresolved operator to constrain. Let's use a Mulliken operator in this example.
+
+    .. code-block:: python
+
+        S = basis.quantize(gqcpy.OverlapOperator())
+        mulliken_domain = basis.mullikenDomain(lambda shell: shell.nucleus().position()[1] == 0 and shell.nucleus().position()[2] == 0)
+        P = mulliken_domain.projectionMatrix(basis.expansion())
+        mulliken_operator = S.partitioned(P)
+
+    Now we can use GQCC to construct our constrained ansatz.
+
+    .. code-block:: python
+
+        Constrained_object = GQCC.SpinUnresolvedConstraints.FCI(H2, basis, mulliken_operator, "population")
+
+    .. note:
+
+        The spin-unresolved FCI module also works with generalized `gqcpy.GSpinorBasis_(c)d` bases.
     """
     def __init__(self, molecule, SQ_basis, operator, constrained_observable):
        # Check compatibility of the operator type based on the used basis_type.
         if type(SQ_basis) is gqcpy.gqcpy.RSpinOrbitalBasis_d:
             compatible_operators = [gqcpy.gqcpy.ScalarRSQOneElectronOperator_d, gqcpy.gqcpy.ScalarRSQTwoElectronOperator_d]
         elif type(SQ_basis) is gqcpy.gqcpy.RSpinOrbitalBasis_cd:
             compatible_operators = [gqcpy.gqcpy.ScalarRSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarRSQTwoElectronOperator_cd]
         elif type(SQ_basis) is gqcpy.gqcpy.GSpinorBasis_d:
-            compatible_operators = [gqcpy.gqcpy.ScalarGSQOneElectronOperator_d, gqcpy.gqcpy.ScalarRSQTwoElectronOperator_d]
+            compatible_operators = [gqcpy.gqcpy.ScalarGSQOneElectronOperator_d, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_d]
         elif type(SQ_basis) is gqcpy.gqcpy.GSpinorBasis_cd:
-            compatible_operators = [gqcpy.gqcpy.ScalarGSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_cd]
+            compatible_operators = [gqcpy.gqcpy.ScalarGSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_cd, gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_cd]
         else:
             raise ValueError("the chosen `SQ_basis` is not compatible with this type of calculation. Use `gqcpy.R/GSpinOrbitalBasis_(c)d`instead.")
         
         assert (type(operator) in compatible_operators), "Only `ScalarR/GSQOneElectronOperator_(c)d` or `ScalarR/GSQTwoElectronOperator_(c)d` can be constrained with this method."
 
         # We can now create a first quantized hamiltonian and use the spin orbital basis to "quantize" it to second quantization.
         # The SQHamiltonian is stored in the class object.
@@ -104,36 +138,57 @@
         :param multiplier:              The multiplier used to modify the Hamiltonian.
         :param return_parameters:       A boolean flag to indicate whether only the wavefunction parameters should also be returned.
         :param verbose:                 An integer representing the amount of output that will be printed.
 
         :returns:                       The energy at the given `mu` value.
         :returns:                       The expectation value of the operator at the given `mu` value.
         :returns:                       The wavefunction parameters (only if `return_parameters` is set to `True`).
+
+        In order to calculate the energy and expectation value of your operator, associated with a certain Lagrange multiplier (let's say -1).
+
+        .. code-block:: python
+
+            energy, expval = Constrained_object.calculateEnergyAndExpectationValue(-1)
+        
         """
         # Modify the Hamiltonian with the given multiplier.
-        if type(self._operator) in [gqcpy.gqcpy.ScalarRSQOneElectronOperator_d, gqcpy.gqcpy.ScalarRSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarGSQOneElectronOperator_d, gqcpy.gqcpy.ScalarGSQOneElectronOperator_cd]:
+        # For a one- or two- electron operator this happens in the same way.
+        # Note that the one-electron operator modifies the one-electron intergrals, and the two-electron operator modifies the two-electron integrals.
+        if type(self._operator) in [gqcpy.gqcpy.ScalarRSQOneElectronOperator_d, gqcpy.gqcpy.ScalarRSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarGSQOneElectronOperator_d, gqcpy.gqcpy.ScalarGSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarRSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarRSQTwoElectronOperator_cd, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_cd]:
             modified_hamiltonian = self._sq_hamiltonian - multiplier * self._operator
-        # Or a two electron operator.
-        elif type(self._operator) in [gqcpy.gqcpy.ScalarRSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarRSQTwoElectronOperator_cd, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_cd]:
-            raise NotImplementedError("This is to be implemented after the general refactor is done.")
+        # For an operator product.
+        elif type(self._operator) in [gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_d, gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_cd]:
+            modified_hamiltonian = self._sq_hamiltonian - (multiplier * self._operator.oneElectron()) - (multiplier * self._operator.twoElectron())
         else:
             raise ValueError("Something went wrong with the operator type.")
         
         # Use the private method to solve the full CI eigenproblem.
         gs_energy, gs_parameters = self._solveCIEigenproblem(modified_hamiltonian)
 
-        # Use the ground state parameters to calculate the 1DM and use it to calculate the expectation value of the Mulliken operator.
+        # Calculate the density matrices.
         D = gs_parameters.calculate1DM()
-        W = self._operator.calculateExpectationValue(D)[0]
+        d = gs_parameters.calculate2DM()
 
+        # Calculate the expectation value of the constrained operator.
+        # This differs depending on which kind of operator is being used.
+        # For a one electron operator.
+        if type(self._operator) in [gqcpy.gqcpy.ScalarRSQOneElectronOperator_d, gqcpy.gqcpy.ScalarRSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarGSQOneElectronOperator_d, gqcpy.gqcpy.ScalarGSQOneElectronOperator_cd]:
+            expectation_value = self._operator.calculateExpectationValue(D)[0]
+        # For a two electron operator.
+        elif type(self._operator) in [gqcpy.gqcpy.ScalarRSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarRSQTwoElectronOperator_cd, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_cd]:
+            expectation_value = self._operator.calculateExpectationValue(d)[0]
+        # For an operator product.
+        elif type(self._operator) in [gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_d, gqcpy.gqcpy.ScalarGSQOneElectronOperatorProduct_cd]:
+            expectation_value = self._operator.calculateExpectationValue(D, d)
+        
         # Calculate the energy by correcting the ground state energy of the modified Hamiltonian.
-        energy = gs_energy + (multiplier * W) + self._nuclear_repulsion
+        energy = gs_energy + (multiplier * expectation_value) + self._nuclear_repulsion
 
         # Print the progress of which mu values have been completed if verbose >= 2.
         if verbose >= 2:
             print("--------------------------------------------------------")
             print("Mu = " + str(np.around(multiplier, 2)) + " done.")
 
         if return_parameters:
-            return energy, W, gs_parameters
+            return energy, expectation_value, gs_parameters
         else:
-            return energy, W
+            return energy, expectation_value
```

### Comparing `GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/GHF.py` & `GQCConstraints-1.1.0/GQCC/SpinUnresolvedConstraints/UHF.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,171 @@
 """
-Spin unresolved constraints applied to generalized Hartree-Fock calculations.
-------------------------------------------------------------------------
+Spin Unresolved Constraints - UHF
+----------------------------------
 
-This class sets up everything needed for a Constrained GHF calculation. The required variables (Hamiltonian, Basis,...), as well as the required methods. 
+This module is used for constraining spin-unresolved operators in unrestricted Hartree-Fock calculations. By setting up the constrained UHF object, the module prepares the basic functionalities to run constrained calculations for single values or to be used in one of the pre-set methods offered by GQCC.
 
 """
 
 # Import statements
 import gqcpy
 import numpy as np
 import numpy.random as rand
 
 from GQCC.Optimization.SpinUnresolvedOptimizer import SpinUnresolvedOptimizer
 
 
-class GHF(SpinUnresolvedOptimizer):
+class UHF(SpinUnresolvedOptimizer):
     """
-    A constructor that sets up everything needed for constrained GHF calculations.
+    A constructor that sets up everything needed for constrained UHF calculations.
 
     :param molecule:                    The GQCP molecule used for the calculations.
+    :param electrons:                   The amount of alpha and beta electrons in the molecule as an array.
     :param SQ_basis:                    The second quantized GQCP basis set used for the calculations, defined for a molecule in a certain basis set. Make sure it is the same basis as in which the operator is defined.
     :param solver:                      The solver used for the UHF calculations.
     :param initial_guess:               The initial guess for the UHF calculation.
     :param operator:                    The GQCP operator that will be constrained.     
     :param constrained_observable:      The name of the observable being constrained.
     :param stability_analysis:          Boolean flag denoting whether stability analysis is performed. Default is `True`.
 
+    :returns:                           An object which contains all required data (basis, Hamiltonian,... ) and possesses the necessary methods to perform calculations.
 
-    :returns:                An object which contains all required data (basis, Hamiltonian,... ) and possesses the necessary methods to perform calculations.
+    In order to set up a UHF calculation with spin resolved constraints we need several GQCP elements. First, set up some basic variables.
+
+    .. code-block:: python
+
+        H2 =  gqcpy.Molecule.HChain(2, 2.5, 0)                                                      # The molecule.
+        electrons = [1,1]                                                                           # The number of alpha and beta electrons.
+        basis = gqcpy.USpinOrbitalBasis_d(H2, "6-31G")                                              # The spin orbital basis.
+        solver = gqcpy.UHFSCFSolver_d.Plain(threshold=1e-6, maximum_number_of_iterations=250000)    # The solver for the Hartree-Fock algorithm.
+
+    We also need to give the object an initial guess for the SCF procedure. In this case, let's generate a random symmetric guess that's different for alpha and beta.
+
+    .. code-block:: python
+
+        import numpy.random as rand
+
+        rand.seed(2)
+        random_matrix_alpha = np.random.rand(basis.numberOfSpinors() // 2, basis.numberOfSpinors() // 2)
+        random_matrix_alpha_transpose = random_matrix_alpha.T
+        symmetric_random_matrix_alpha = random_matrix_alpha + random_matrix_alpha_transpose
+        _, alpha_guess = np.linalg.eigh(symmetric_random_matrix_alpha)
+
+        rand.seed(3)
+        random_matrix_beta = np.random.rand(basis.numberOfSpinors() // 2, basis.numberOfSpinors() // 2)
+        random_matrix_beta_transpose = random_matrix_beta.T
+        symmetric_random_matrix_beta = random_matrix_beta + random_matrix_beta_transpose
+        _, beta_guess = np.linalg.eigh(symmetric_random_matrix_beta)
+
+        guess = gqcpy.UTransformation_d(gqcpy.UTransformationComponent_d(alpha_guess), gqcpy.UTransformationComponent_d(beta_guess))
+
+    Now we choose an operator to constrain. Let's set up an :math:`S^2` operator product.
+
+    .. code-block:: python
+
+        S = basis.quantize(gqcpy.ElectronicSpinSquaredOperator())
+
+    The construction of the constrained object can now be done with GQCC.
+
+    .. code-block:: python
+
+        Constrained_object = GQCC.SpinUnresolvedConstraints.UHF(H2, electrons, basis, solver, guess, S, "population")
     """
-    def __init__ (self, molecule, SQ_basis, solver, initial_guess, operator, constrained_observable, stability_analysis=True):
+    def __init__(self, molecule, electrons, SQ_basis, solver, initial_guess, operator, constrained_observable, stability_analysis=True):
+        # Raise an exception if the electrons array is not conform with the requirements.
+        if type(electrons[0]) is float or type(electrons[1]) is float or len(electrons) != 2:
+            raise ValueError("Electrons must be of dimension 2 and must contain two ìnt`s as it must contain the number of alpha and beta electrons.")
+        
         # Check compatibility of the operator type based on the used basis type.
-        if type(SQ_basis) is gqcpy.gqcpy.GSpinorBasis_d:
-            compatible_operators = [gqcpy.gqcpy.ScalarGSQOneElectronOperator_d, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_d]
-            assert (type(solver) is gqcpy.gqcpy.IterativeAlgorithm_GHFSCFEnvironment_d)
-
-        elif type(SQ_basis) is gqcpy.gqcpy.GSpinorBasis_cd:
-            compatible_operators = [gqcpy.gqcpy.ScalarGSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_cd]
-            assert (type(solver) is gqcpy.gqcpy.IterativeAlgorithm_GHFSCFEnvironment_cd)
+        if type(SQ_basis) is gqcpy.gqcpy.USpinOrbitalBasis_d:
+            compatible_operators = [gqcpy.gqcpy.ScalarUSQOneElectronOperator_d, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarUSQOneElectronOperatorProduct_d]
+            assert (type(solver) is gqcpy.gqcpy.IterativeAlgorithm_UHFSCFEnvironment)
+
+        elif type(SQ_basis) is gqcpy.gqcpy.USpinOrbitalBasis_cd:
+            compatible_operators = [gqcpy.gqcpy.ScalarUSQOneElectronOperator_cd, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_cd, gqcpy.gqcpy.ScalarUSQOneElectronOperatorProduct_cd]
+            assert (type(solver) is gqcpy.gqcpy.IterativeAlgorithm_UHFSCFEnvironment_cd)
 
         else:
-            raise ValueError("the chosen `SQ_basis` or `solver` is not compatible with this type of calculation. Use `gqcpy.GSpinorBasis_(c)d`instead.")
-        assert (type(operator) in compatible_operators), "Only `ScalarGSQOneElectronOperator_(c)d` or `ScalarGSQTwoElectronOperator_(c)d` can be constrained with this method."     
+            raise ValueError("the chosen `SQ_basis` or `solver` is not compatible with this type of calculation. Use `gqcpy.USpinOrbitalBasis_(c)d`instead.")
+        assert (type(operator) in compatible_operators), "Only `ScalarUSQOneElectronOperator_(c)d` or `ScalarUSQTwoElectronOperator_(c)d` can be constrained with this method."     
 
         # This basis can now quantize the Hamiltonian.
         self._sq_hamiltonian = SQ_basis.quantize(gqcpy.FQMolecularHamiltonian(molecule))
 
         # We will need the number of electrons, as well as the total number of Spinors later on.        
-        self._K = SQ_basis.numberOfSpinors()
-        self._N = molecule.numberOfElectrons()
+        self._K = SQ_basis.numberOfSpinors() // 2
+        self._Ka = self._K
+        self._Kb = self._K
+
+        self._Na = electrons[0]
+        self._Nb = electrons[1]
 
         # Save the overlap and nuclear repulsion operators. 
         self._nuclear_repulsion = gqcpy.NuclearRepulsionOperator(molecule.nuclearFramework()).value()
         self._overlap = SQ_basis.quantize(gqcpy.OverlapOperator())
 
         # Save the operator you want to constrain.
         self._operator = operator
+
         self._constrained_observable = constrained_observable
+        self._constrained_alpha_observable = "alpha " + self._constrained_observable
+        self._constrained_beta_observable = "beta " + self._constrained_observable
 
-        # Select the type of solver for the SCF algorithm.
+        # Select the type of solver for the SCF algorithm and where to start the iterations.
         self._solver = solver
         self._initial_guess = initial_guess
 
         # Wheter to perform a stability check for each calculation.
         self._stability_analysis = stability_analysis
 
 
-    # A solver for the GHF problem.
-    # The GHF solver always takes a random guess, in order to activate the `off-diagonal` blocks. 
-    def _solveGHFProblem(self, hamiltonian):
+    # A solver for the UHF problem.
+    def _solveUHFProblem(self, hamiltonian):
         """
-        A method used to solve the iterative GHF problem. A stability check is performed automatically. If an internal instability is encountered, it will be followed by rotating the coefficeints in the direction of the lowest Hessian eigenvector. This will be shown in the output.
+        A method used to solve the iterative UHF problem. A stability check is performed automatically. If an internal instability is encountered, it will be followed by rotating the coefficeints in the direction of the lowest Hessian eigenvector. This will be shown in the output.
 
-        :param hamiltonian:      The GSQHamiltonian used for the calculation.
+        :param hamiltonian:      The USQHamiltonian used for the calculation.
 
         :returns:                The ground state energy.
         :returns:                The ground state parameters
         """
 
         # To solve the GHF problem we need an environment and a solver.
-        if type(hamiltonian) is gqcpy.gqcpy.GSQHamiltonian_d:
-            environment = gqcpy.GHFSCFEnvironment_d(self._N, hamiltonian, self._overlap, self._initial_guess)
-            qc_structure = gqcpy.GHF_d.optimize(self._solver, environment)
+        if type(hamiltonian) is gqcpy.gqcpy.USQHamiltonian_d:
+            environment = gqcpy.UHFSCFEnvironment_d(self._Na, self._Nb, hamiltonian, self._overlap, self._initial_guess)
+            qc_structure = gqcpy.UHF_d.optimize(self._solver, environment)
         else:
-            environment = gqcpy.GHFSCFEnvironment_cd(self._N, hamiltonian, self._overlap, self._initial_guess)
-            qc_structure = gqcpy.GHF_cd.optimize(self._solver, environment)
+            environment = gqcpy.UHFSCFEnvironment_cd(self._Na, self._Nb, hamiltonian, self._overlap, self._initial_guess)
+            qc_structure = gqcpy.UHF_cd.optimize(self._solver, environment)
 
         if self._stability_analysis:
-            # For generalized Hartree-Fock, a stability check is always performed.
+            # For unrestricted Hartree-Fock, a stability check can be performed.
             # Transform the hamiltonian to MO basis and calculate the stability matrices. Print the resulting stabilities of the wavefunction model.
             coefficients = qc_structure.groundStateParameters().expansion()
             MO_hamiltonian = hamiltonian.transformed(coefficients)
             stability_matrices = qc_structure.groundStateParameters().calculateStabilityMatrices(MO_hamiltonian)
 
             internal_stability = stability_matrices.isInternallyStable(-1e-5)
 
             while internal_stability is False:
                 print("**************************************************************")
                 print("There is an internal instability. Follow it using the Hessian.")
                 print("**************************************************************")
 
                 # Rotate the coefficients in the direction of the lowest Hessian eigenvector.
-                rotation = stability_matrices.instabilityRotationMatrix(self._N, self._K-self._N)
+                rotation = stability_matrices.instabilityRotationMatrix(self._Na, self._Nb, self._Ka-self._Na, self._Kb-self._Nb)
                 coefficients_rotated = coefficients.rotated(rotation)
 
                 # Perform a new SCF calculation with the rotated coefficients as initial guess.
-                if type(hamiltonian) is gqcpy.gqcpy.GSQHamiltonian_d:
-                    environment_rotated = gqcpy.GHFSCFEnvironment_d(self._N, hamiltonian, self._overlap, coefficients_rotated)
-                    qc_structure = gqcpy.GHF_d.optimize(self._solver, environment_rotated)
+                if type(hamiltonian) is gqcpy.gqcpy.USQHamiltonian_d:
+                    environment_rotated = gqcpy.UHFSCFEnvironment_d(self._Na, self._Nb, hamiltonian, self._overlap, coefficients_rotated)
+                    qc_structure = gqcpy.UHF_d.optimize(self._solver, environment_rotated)
                 else:
-                    environment_rotated = gqcpy.GHFSCFEnvironment_cd(self._N, hamiltonian, self._overlap, coefficients_rotated)
-                    qc_structure = gqcpy.GHF_cd.optimize(self._solver, environment_rotated)
+                    environment_rotated = gqcpy.UHFSCFEnvironment_d(self._Na, self._Nb, hamiltonian, self._overlap, coefficients_rotated)
+                    qc_structure = gqcpy.UHF_d.optimize(self._solver, environment_rotated)
 
                 coefficients_2 = qc_structure.groundStateParameters().expansion()
 
                 # Perform a new stability check. Print the resulting stabilities.
                 hamiltonian_MO_2 = hamiltonian.transformed(coefficients_2)
                 stability_matrices_2 = qc_structure.groundStateParameters().calculateStabilityMatrices(hamiltonian_MO_2)
 
@@ -126,46 +177,84 @@
 
                 if internal_stability:
                     print("**************************************************************")
 
         return qc_structure.groundStateEnergy(), qc_structure.groundStateParameters()
 
 
-    # A function to calculate the energy and expectation value value of GHF at a certain multiplier. 
+    # A function to calculate the energy and expectation value value of UHF at a certain multiplier. 
     def calculateEnergyAndExpectationValue(self, multiplier, return_parameters=False, verbose=0):
         """
         A method used to calculate the energy and the expectation value at a given multiplier `mu`.
 
         :param multiplier:      The multiplier used to modify the Hamiltonian.
         :param verbose:         An integer representing the amount of output that will be printed.
         :return_parameters:     A boolean flag that specifies whether the wavefunction parameters are also returned.
 
         :returns:               The energy at the given `mu` values.
         :returns:               The expectation value of the operator at the given `mu` value.
         :returns:               The wavefunction parameters (only if `return_parameters` is set to `True`).
+
+        In order to calculate the energy and expectation value of your operator, associated with a certain Lagrange multiplier (let's say -1).
+
+        .. code-block:: python
+
+            energy, expval = Constrained_object.calculateEnergyAndExpectationValue(-1)
+        
         """
         # Modify the Hamiltonian with the given multiplier.
         # Do this respectively for the alpha and beta parts.
-        if type(self._operator) in [gqcpy.gqcpy.ScalarGSQOneElectronOperator_d, gqcpy.gqcpy.ScalarGSQOneElectronOperator_cd]:
-            modified_hamiltonian = self._sq_hamiltonian - (multiplier * self._operator)
+        if type(self._operator) in [gqcpy.gqcpy.ScalarUSQOneElectronOperator_d, gqcpy.gqcpy.ScalarUSQOneElectronOperator_cd]:
+            unrestricted_operator = type(self._operator)((self._operator.alpha * multiplier), (self._operator.beta * multiplier))
+
+            modified_hamiltonian = self._sq_hamiltonian - unrestricted_operator
         # Or a two electron operator.
-        elif type(self._operator) in [gqcpy.gqcpy.ScalarGSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarGSQTwoElectronOperator_cd]:
-            raise NotImplementedError("This is to be implemented after the general refactor is done.")
+        elif type(self._operator) in [gqcpy.gqcpy.ScalarUSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_cd]:
+            zero_component = type(self._operator.alphaBeta())(np.zeros((self._K, self._K, self._K, self._K)))
+            dense_component_aa = type(self._operator.alphaAlpha())((self._operator.alphaAlpha() + self._operator.alphaBeta()) * multiplier)
+            dense_component_bb = type(self._operator.betaBeta())((self._operator.betaAlpha() + self._operator.betaBeta()) * multiplier)
+            unrestricted_operator = type(self._operator)(dense_component_aa, zero_component, zero_component, dense_component_bb)
+
+            modified_hamiltonian = self._sq_hamiltonian - unrestricted_operator
+        elif type(self._operator) in [gqcpy.gqcpy.ScalarUSQOneElectronOperatorProduct_d, gqcpy.gqcpy.ScalarUSQOneElectronOperatorProduct_cd]:
+            unrestricted_matrix_operator = type(self._operator.oneElectron())((self._operator.oneElectron().alpha * multiplier), (self._operator.oneElectron().beta * multiplier))
+
+            zero_component = type(self._operator.twoElectron().alphaBeta())(np.zeros((self._K, self._K, self._K, self._K)))
+            
+            parameters_aa = self._operator.twoElectron().alphaAlpha().parameters()
+            parameters_ab = self._operator.twoElectron().alphaBeta().parameters()
+            parameters_ba = self._operator.twoElectron().betaAlpha().parameters()
+            parameters_bb = self._operator.twoElectron().betaBeta().parameters()
+
+            dense_component_aa = type(self._operator.twoElectron().alphaAlpha())(parameters_aa + parameters_ab) * multiplier
+            dense_component_bb = type(self._operator.twoElectron().betaBeta())(parameters_ba + parameters_bb) * multiplier
+
+            unrestricted_tensor_operator = type(self._operator.twoElectron())(dense_component_aa, zero_component, zero_component, dense_component_bb)
+
+            modified_hamiltonian = self._sq_hamiltonian - unrestricted_matrix_operator - unrestricted_tensor_operator
         else:
             raise ValueError("Something went wrong with the operator type.")
 
-        
-        gs_energy, gs_parameters = self._solveGHFProblem(modified_hamiltonian)
-
-        # Calculate the expectation value of the operator.
-        DM = gs_parameters.calculateScalarBasis1DM()
-        expectation_value = self._operator.calculateExpectationValue(DM)[0]
+        gs_energy, gs_parameters = self._solveUHFProblem(modified_hamiltonian)
 
-        # Perform the energy correction
-        energy = gs_energy + ((multiplier * expectation_value) + self._nuclear_repulsion)
+        # Calculate the density matrices.
+        D = gs_parameters.calculateScalarBasis1DM()
+        d = gs_parameters.calculateScalarBasis2DM()
+
+        if type(self._operator) in [gqcpy.gqcpy.ScalarUSQOneElectronOperator_d, gqcpy.gqcpy.ScalarUSQOneElectronOperator_cd]:
+            expectation_value = self._operator.calculateExpectationValue(D)[0]
+        # For a two electron operator.
+        elif type(self._operator) in [gqcpy.gqcpy.ScalarUSQTwoElectronOperator_d, gqcpy.gqcpy.ScalarUSQTwoElectronOperator_cd]:
+            expectation_value = self._operator.calculateExpectationValue(d)[0]
+        # For an operator product.
+        elif type(self._operator) in [gqcpy.gqcpy.ScalarUSQOneElectronOperatorProduct_d, gqcpy.gqcpy.ScalarUSQOneElectronOperatorProduct_cd]:
+            expectation_value = self._operator.calculateExpectationValue(D, d)
+        
+        # Calculate the energy by correcting the ground state energy of the modified Hamiltonian.
+        energy = gs_energy + (multiplier * expectation_value) + self._nuclear_repulsion
 
         # Print the progress of which mu values have been completed if verbose >= 2.
         if verbose >= 2:
             print("--------------------------------------------------------")
             print("Mu = " + str(np.around(multiplier, 2)) + " done.")
 
         if return_parameters:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/HubbardFCI.py` & `GQCConstraints-1.1.0/GQCC/SpinUnresolvedConstraints/HubbardFCI.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-Spin unresolved constraints applied to FCI calculations on the Hubbard model.
------------------------------------------------------------------------------
+Spin Unresolved Constraints - Hubbard FCI
+-----------------------------------------
 
-This class sets up everything needed for an unresolved constrained Hubbard calculation. The required variables (Hamiltonian, ONV-Basis,...), as well as the required methods. 
+This module is used for constraining spin-unresolved operators in full configuration interaction calculations on the Hubbard model. By setting up the constrained Hubbard FCI object, the module prepares the basic functionalities to run constrained calculations for single values or to be used in one of the pre-set methods offered by GQCC.
 
 """
 
 # Import statements
 import gqcpy
 import numpy as np
 
@@ -17,14 +17,48 @@
     A constructor that sets up everything needed for constrained Hubbard model calculations.
 
     :param hubbard_hamiltonian:              The GQCP Hubbard Hamiltonian defining the Hubbard model.
     :param operator:                         The GQCP operator that will be constrained.        
     :param constrained_observable:           The name of the observable being constrained.
 
     :returns:                       An object which contains all required data (basis, Hamiltonian,... ) and possesses the necessary methods to perform calculations.
+
+    To initialize a Hubbard FCI object we need a Hubbard Hamiltonian and an operator from GQCP. The Hubbard Hamiltonian can be constructed.
+
+    .. code-block:: python
+
+        L = 3       # number of sites
+        t = 1e-4    # hopping parameter
+        U = 1.0     # on-site repulsion
+        
+        adjacency_matrix = gqcpy.AdjacencyMatrix.Linear(L)
+        hopping_matrix = gqcpy.HoppingMatrix.Homogeneous(adjacency_matrix, t)
+        unmodified_hubbard_chain = gqcpy.HubbardHamiltonian(hopping_matrix, U)
+
+    .. note::
+
+        The Hubbard Hamiltonian does not need to be Homogeneous. Any GQCP Hubbard Hamiltonian will work.
+    
+    and an operator (e.g. number operator) can be made with the following code.
+
+    .. code-block:: python
+
+        P = np.zeros((L, L))
+        P[0, 0] = 1
+        number_operator = gqcpy.ScalarRSQOneElectronOperator_d(P)
+
+    .. note::
+
+        Contrary to the regular spin-unresolved FCI module, the Hubbard FCI module only works with **restricted** operators.
+
+    A constrained Hubbard FCI object can then be constructed.
+
+    .. code-block:: python
+
+        Constrained_object = GQCC.SpinUnresolvedConstraints.HubbardFCI(unmodified_hubbard_chain, number_operator, "population")
     """
     def __init__(self, hubbard_hamiltonian, operator, constrained_observable):
         # Check compatibility of the operator type based on the used basis_type.
         compatible_operators = [gqcpy.gqcpy.ScalarRSQOneElectronOperator_d, gqcpy.gqcpy.ScalarRSQTwoElectronOperator_d]        
         assert (type(operator) in compatible_operators), "Only `ScalarRSQOneElectronOperator_d` or `ScalarRSQTwoElectronOperator_d` can be constrained with this method."
         
         # Hopping matrix of the defined Hubbard model.
@@ -53,14 +87,32 @@
         """
         A method to calculate the von Neumann entropy of a certain partition within the Hubbard model.
 
         :param domain_partition:              The partition of the universe into "system" and "environment" for which the entropic relations will be calculated.
         :param wavefunction_parameters:       The parameters of the final wavefunction for which the entropic measures will be calculated.
 
         :returns:                             The Von Neumann entropy calculated according to eq. 6 in the following paper by Rissler et. al.: https://doi.org/10.1016/j.chemphys.2005.10.018.
+
+        The Hubbard module can also look at the entanglement between different **domain partitions**. To do so we need to define certain domain partitions.
+
+        .. code-block:: python
+
+            domain_partition_p = gqcpy.DiscreteDomainPartition([0, 1, 1])
+            domain_partition_q = gqcpy.DiscreteDomainPartition([1, 0, 1])
+
+        .. note::
+
+            To calculate entanglement you need the wavefunction parameters. To get them, set **return_parameters** to **True** in the `calculateEnergyAndExpectationValue()` or the `verifyCombination()` method.
+
+        Using these partitions along with the wavefunction parameters, we can calculate the von Neumann entropy.
+
+        .. code-block:: python
+
+            Sp = Constrained_object.vonNeumannEntropy(domain_partition_p, parameters)
+            Sq = Constrained_object.vonNeumannEntropy(domain_partition_q, parameters)
         """
         # Sometimes, the result will not fullfil the constraint. If this is the case, no parameters are saved.
         # This clause circumvents the error that would arise if the type of the saved wavefunction parameters is wrong.
         if type(wavefunction_parameters) is not gqcpy.gqcpy.LinearExpansion_SpinResolved:
             return None
 
         # Calculate the orbital RDM.
@@ -83,14 +135,33 @@
 
         :param domain_partition_p:               The partition of the universe into "system" and "environment" for which the first domain.
         :param domain_partition_q:               The partition of the universe into "system" and "environment" for which the second domain.
         :param domain_partition_pq:              The partition of the universe into "system" and "environment" for which the domain containing domain one and two.
         :param wavefunction_parameters:          The parameters of the final wavefunction for which the entropic measures will be calculated.
 
         :returns:                                The mutual information of site one and two calculated according to eq. 8 in the following paper by Rissler et. al.: https://doi.org/10.1016/j.chemphys.2005.10.018.
+
+        The mutual information is an entanglement measure that elucidates how much two domains know about one another. To use this we need domain partitions for the two single site von Neumann entropies and one of the two site entropy.
+
+        .. code-block:: python
+
+            domain_partition_pq = gqcpy.DiscreteDomainPartition([0, 0, 1])
+            domain_partition_p = gqcpy.DiscreteDomainPartition([0, 1, 1])
+            domain_partition_q = gqcpy.DiscreteDomainPartition([1, 0, 1])
+
+        Now we can call the mutual information.
+
+        .. note::
+
+            To calculate mutual information you need the wavefunction parameters. To get them, set **return_parameters** to **True** in the `calculateEnergyAndExpectationValue()` or the `verifyCombination()` method.
+
+        .. code-block:: python
+
+            I_pq = Constrained_object.mutualInformation(domain_partition_p, domain_partition_q, domain_partition_pq, parameters)
+
         """
         # Sometimes, the result will not fullfil the constraint. If this is the case, no parameters are saved.
         # This clause circumvents the error that would arise if the type of the saved wavefunction parameters is wrong.
         if type(wavefunction_parameters) is not gqcpy.gqcpy.LinearExpansion_SpinResolved:
             return None
         
         S_p = self.vonNeumannEntropy(domain_partition_p, wavefunction_parameters)
```

### Comparing `GQCConstraints-1.0.0/GQCConstraints.egg-info/PKG-INFO` & `GQCConstraints-1.1.0/GQCConstraints.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 Metadata-Version: 2.1
 Name: GQCConstraints
-Version: 1.0.0
+Version: 1.1.0
 Summary: This library build on GQCP provides easy to work with utilities in order to perform constrained quantum chemical calculations.
 Author: The Ghent Quantum Chemistry Group
 Keywords: quantum chemistry,constraints,GQCP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GQCConstraints
 GQCConstraints or GQCC for short is a python library, based on [GQCP](https://github.com/GQCG/GQCP), that can be used to run several constrained quantum chemical calculations.
 
 Constraint and symmetries are closely related and as such, applying different kind of constraints on quantum chemical calculations can lead to some very interesting insights. 
 
 # Getting started
 In order to get started you first of all need a working `GQCP docker container`.
 
-First [install Docker](https://docs.docker.com/get-docker/). Then pull our `GQCP` image to the infrastructure in question
+First [install Docker](https://docs.docker.com/get-docker/). Then pull our `GQCP` image to the infrastructure in question.
 
 ```bash
 docker pull gqcg/gqcp
 ```
 
-Next, on top of this installation you can install GQCConstraints
+Next, on top of this installation you can install GQCConstraints.
 
 ```bash
 pip install GQCConstraints
 ```
-## Documentation
 
-The latest documentation on the API's of GQCC can be downloaded from the Github Actions page. The `.pdf` file is automatically generated and saved as an artifact.
+To use the code import both GQCPy and GQCConstraints.
+
+```python
+import gqcpy
+import GQCC
+```
 
 ## Reasearch
 
-GQCC is a research tool first and foremost. And research for which this library is used can be found here:
+GQCC is a research tool first and foremost. And research for which this library is used can be found here.
 
 - [Constraining chemical wavefunctions](https://github.com/GQCG-res/constraining_chemical_wave_functions)
 - [Constrained entanglement](https://github.com/GQCG-res/constrained-entanglement)
 - [Constrained NOCI](https://github.com/GQCG-res/constrained-NOCI)
 - [Fukui Hubbard](https://github.com/GQCG-res/fukui-hubbard)
 - [Spin contamination constraints](https://github.com/GQCG-res/spin-contamination-constraints)
```

### Comparing `GQCConstraints-1.0.0/GQCConstraints.egg-info/SOURCES.txt` & `GQCConstraints-1.1.0/GQCConstraints.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,13 +17,14 @@
 GQCC/SpinResolvedConstraints/UHF.py
 GQCC/SpinResolvedConstraints/UNOCI.py
 GQCC/SpinResolvedConstraints/__init__.py
 GQCC/SpinUnresolvedConstraints/FCI.py
 GQCC/SpinUnresolvedConstraints/GHF.py
 GQCC/SpinUnresolvedConstraints/GNOCI.py
 GQCC/SpinUnresolvedConstraints/HubbardFCI.py
+GQCC/SpinUnresolvedConstraints/UHF.py
 GQCC/SpinUnresolvedConstraints/__init__.py
 GQCConstraints.egg-info/PKG-INFO
 GQCConstraints.egg-info/SOURCES.txt
 GQCConstraints.egg-info/dependency_links.txt
 GQCConstraints.egg-info/requires.txt
 GQCConstraints.egg-info/top_level.txt
```

### Comparing `GQCConstraints-1.0.0/LICENSE` & `GQCConstraints-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GQCConstraints-1.0.0/PKG-INFO` & `GQCConstraints-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 Metadata-Version: 2.1
 Name: GQCConstraints
-Version: 1.0.0
+Version: 1.1.0
 Summary: This library build on GQCP provides easy to work with utilities in order to perform constrained quantum chemical calculations.
 Author: The Ghent Quantum Chemistry Group
 Keywords: quantum chemistry,constraints,GQCP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GQCConstraints
 GQCConstraints or GQCC for short is a python library, based on [GQCP](https://github.com/GQCG/GQCP), that can be used to run several constrained quantum chemical calculations.
 
 Constraint and symmetries are closely related and as such, applying different kind of constraints on quantum chemical calculations can lead to some very interesting insights. 
 
 # Getting started
 In order to get started you first of all need a working `GQCP docker container`.
 
-First [install Docker](https://docs.docker.com/get-docker/). Then pull our `GQCP` image to the infrastructure in question
+First [install Docker](https://docs.docker.com/get-docker/). Then pull our `GQCP` image to the infrastructure in question.
 
 ```bash
 docker pull gqcg/gqcp
 ```
 
-Next, on top of this installation you can install GQCConstraints
+Next, on top of this installation you can install GQCConstraints.
 
 ```bash
 pip install GQCConstraints
 ```
-## Documentation
 
-The latest documentation on the API's of GQCC can be downloaded from the Github Actions page. The `.pdf` file is automatically generated and saved as an artifact.
+To use the code import both GQCPy and GQCConstraints.
+
+```python
+import gqcpy
+import GQCC
+```
 
 ## Reasearch
 
-GQCC is a research tool first and foremost. And research for which this library is used can be found here:
+GQCC is a research tool first and foremost. And research for which this library is used can be found here.
 
 - [Constraining chemical wavefunctions](https://github.com/GQCG-res/constraining_chemical_wave_functions)
 - [Constrained entanglement](https://github.com/GQCG-res/constrained-entanglement)
 - [Constrained NOCI](https://github.com/GQCG-res/constrained-NOCI)
 - [Fukui Hubbard](https://github.com/GQCG-res/fukui-hubbard)
 - [Spin contamination constraints](https://github.com/GQCG-res/spin-contamination-constraints)
```

### Comparing `GQCConstraints-1.0.0/setup.py` & `GQCConstraints-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 long_description = long_description.split('\n', 8)[8]
 
 setuptools.setup(
       name='GQCConstraints',
-      version='1.0.0',
+      version='1.1.0',
       description='This library build on GQCP provides easy to work with utilities in order to perform constrained quantum chemical calculations.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='The Ghent Quantum Chemistry Group',
       packages=setuptools.find_packages(),
       install_requires=['pandas==1.2.5', 'numpy==1.22.4', 'scipy==1.7.0'],
       keywords=['quantum chemistry', 'constraints', 'GQCP']
```

