# Comparing `tmp/piqp-0.1.3.tar.gz` & `tmp/piqp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piqp-0.1.3.tar", last modified: Thu Jul 20 13:26:13 2023, max compression
+gzip compressed data, was "piqp-0.2.0.tar", last modified: Fri Jul 28 14:17:51 2023, max compression
```

## Comparing `piqp-0.1.3.tar` & `piqp-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:26:13.672752 piqp-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-20 13:25:57.000000 piqp-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-20 13:26:13.672752 piqp-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-20 13:25:57.000000 piqp-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:26:13.668752 piqp-0.1.3/interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:26:13.668752 piqp-0.1.3/interfaces/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:26:13.668752 piqp-0.1.3/interfaces/python/piqp/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-20 13:25:57.000000 piqp-0.1.3/interfaces/python/piqp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:26:13.672752 piqp-0.1.3/piqp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-20 13:26:13.000000 piqp-0.1.3/piqp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-20 13:26:13.000000 piqp-0.1.3/piqp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:26:13.000000 piqp-0.1.3/piqp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:26:13.000000 piqp-0.1.3/piqp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 13:26:13.000000 piqp-0.1.3/piqp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 13:26:13.000000 piqp-0.1.3/piqp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 13:25:57.000000 piqp-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:26:13.672752 piqp-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-20 13:25:57.000000 piqp-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:17:51.657259 piqp-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-28 14:17:35.000000 piqp-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-28 14:17:51.657259 piqp-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-28 14:17:35.000000 piqp-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:17:51.653258 piqp-0.2.0/interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:17:51.653258 piqp-0.2.0/interfaces/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:17:51.657259 piqp-0.2.0/interfaces/python/piqp/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-28 14:17:35.000000 piqp-0.2.0/interfaces/python/piqp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:17:51.657259 piqp-0.2.0/piqp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-28 14:17:51.000000 piqp-0.2.0/piqp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-28 14:17:51.000000 piqp-0.2.0/piqp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:17:51.000000 piqp-0.2.0/piqp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:17:51.000000 piqp-0.2.0/piqp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 14:17:51.000000 piqp-0.2.0/piqp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 14:17:51.000000 piqp-0.2.0/piqp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-28 14:17:35.000000 piqp-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 14:17:51.657259 piqp-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-28 14:17:35.000000 piqp-0.2.0/setup.py
```

### Comparing `piqp-0.1.3/LICENSE` & `piqp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `piqp-0.1.3/PKG-INFO` & `piqp-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: piqp
-Version: 0.1.3
-Summary: An embedded Proximal Interior Point Quadratic Programming solver
+Version: 0.2.0
+Summary: A Proximal Interior Point Quadratic Programming solver
 Home-page: https://github.com/PREDICT-EPFL/piqp
 Author: Roland Schwan
 Author-email: roland.schwan@epfl.ch
 License: BSD-2-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # PIQP
 
 [![DOI](https://img.shields.io/badge/DOI-10.48550/arXiv.2304.00290-green.svg)](https://doi.org/10.48550/arXiv.2304.00290)
 [![Preprint](https://img.shields.io/badge/Preprint-arXiv-blue.svg)](https://arxiv.org/abs/2304.00290)
-[![Funding](https://img.shields.io/badge/Grant-NCCR%20Automation%20(51NF40180545)-90e3dc.svg)](https://nccr-automation.ch/)
+[![Funding](https://img.shields.io/badge/Grant-NCCR%20Automation%20(51NF40__180545)-90e3dc.svg)](https://nccr-automation.ch/)
+
 [![Docs](https://img.shields.io/badge/Docs-available-brightgreen.svg)](https://predict-epfl.github.io/piqp/)
+![License](https://img.shields.io/badge/License-BSD--2--Clause-brightgreen.svg)
+![PyPI - downloads](https://img.shields.io/pypi/dm/piqp.svg?label=PyPI%20downloads)
 
-PIQP is an embedded Proximal Interior Point Quadratic Programming solver, which can solve dense and sparse quadratic programs of the form
+PIQP is a Proximal Interior Point Quadratic Programming solver, which can solve dense and sparse quadratic programs of the form
 
 $$
 \begin{aligned}
 \min_{x} \quad & \frac{1}{2} x^\top P x + c^\top x \\
 \text {s.t.}\quad & Ax=b, \\
 & Gx \leq h, \\
 & x_{lb} \leq x \leq x_{ub},
@@ -32,22 +35,24 @@
 Combining an infeasible interior point method with the proximal method of multipliers, the algorithm can handle ill-conditioned convex QP problems without the need for linear independence of the constraints.
 
 ## Features
 
 * PIQP is written in header only C++ 14 leveraging the [Eigen](https://eigen.tuxfamily.org/index.php?title=Main_Page) library for vectorized linear algebra.
 * Dense and sparse problem formulations are supported. For small dense problems, vectorized instructions and cache locality can be exploited more efficiently.
 * Interface to Python with many more to follow.
+* Allocation free problem updates and re-solves.
 * Open source under the BSD 2-Clause License.
 
 ## Interfaces
 
 PIQP support a wide range of interfaces including
 * C/C++ (with Eigen support)
 * Python
-* Matlab (soon)
+* Matlab
+* R (soon)
 * Julia (soon)
 * Rust (soon)
 
 ## Credits
 
 PIQP is developed by the following people:
 * Roland Schwan (main developer)
@@ -61,15 +66,15 @@
 
 PIQP is build on the following open-source libraries:
 * [Eigen](https://eigen.tuxfamily.org/index.php?title=Main_Page): It's the work horse under the hood, responsible for producing optimized numerical linear algebra code.
 * [ProxSuite](https://github.com/Simple-Robotics/proxsuite): The code structure (folder/namespace structure, etc.), some utility functions/helper macros, and the instruction set optimized python bindings are based on ProxSuite.
 * [SuiteSparse - LDL](https://github.com/DrTimothyAldenDavis/SuiteSparse) (modified version): Used for solving linear systems in the sparse solver.
 * [pybind11](https://github.com/pybind/pybind11): Used for generating the python bindings.
 * [cpu_features](https://github.com/google/cpu_features): Used for run-time instruction set detection in the interface bindings.
-* [OSQP](https://github.com/osqp/osqp): The C interface is inspired by OSQP.
+* [OSQP](https://github.com/osqp/osqp): The C and Matlab interface is inspired by OSQP.
 * [Clarabel](https://github.com/oxfordcontrol/Clarabel.rs): Parts of the iterative refinement scheme are inspired by Clarabel's implementation.
 
 ## Citing our Work
 
 If you found PIQP useful in your scientific work, we encourage you to cite our accompanying paper:
 
 ```
```

### Comparing `piqp-0.1.3/README.md` & `piqp-0.2.0/piqp.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,31 @@
+Metadata-Version: 2.1
+Name: piqp
+Version: 0.2.0
+Summary: A Proximal Interior Point Quadratic Programming solver
+Home-page: https://github.com/PREDICT-EPFL/piqp
+Author: Roland Schwan
+Author-email: roland.schwan@epfl.ch
+License: BSD-2-Clause
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # PIQP
 
 [![DOI](https://img.shields.io/badge/DOI-10.48550/arXiv.2304.00290-green.svg)](https://doi.org/10.48550/arXiv.2304.00290)
 [![Preprint](https://img.shields.io/badge/Preprint-arXiv-blue.svg)](https://arxiv.org/abs/2304.00290)
-[![Funding](https://img.shields.io/badge/Grant-NCCR%20Automation%20(51NF40180545)-90e3dc.svg)](https://nccr-automation.ch/)
+[![Funding](https://img.shields.io/badge/Grant-NCCR%20Automation%20(51NF40__180545)-90e3dc.svg)](https://nccr-automation.ch/)
+
 [![Docs](https://img.shields.io/badge/Docs-available-brightgreen.svg)](https://predict-epfl.github.io/piqp/)
+![License](https://img.shields.io/badge/License-BSD--2--Clause-brightgreen.svg)
+![PyPI - downloads](https://img.shields.io/pypi/dm/piqp.svg?label=PyPI%20downloads)
 
-PIQP is an embedded Proximal Interior Point Quadratic Programming solver, which can solve dense and sparse quadratic programs of the form
+PIQP is a Proximal Interior Point Quadratic Programming solver, which can solve dense and sparse quadratic programs of the form
 
 $$
 \begin{aligned}
 \min_{x} \quad & \frac{1}{2} x^\top P x + c^\top x \\
 \text {s.t.}\quad & Ax=b, \\
 & Gx \leq h, \\
 & x_{lb} \leq x \leq x_{ub},
@@ -19,22 +35,24 @@
 Combining an infeasible interior point method with the proximal method of multipliers, the algorithm can handle ill-conditioned convex QP problems without the need for linear independence of the constraints.
 
 ## Features
 
 * PIQP is written in header only C++ 14 leveraging the [Eigen](https://eigen.tuxfamily.org/index.php?title=Main_Page) library for vectorized linear algebra.
 * Dense and sparse problem formulations are supported. For small dense problems, vectorized instructions and cache locality can be exploited more efficiently.
 * Interface to Python with many more to follow.
+* Allocation free problem updates and re-solves.
 * Open source under the BSD 2-Clause License.
 
 ## Interfaces
 
 PIQP support a wide range of interfaces including
 * C/C++ (with Eigen support)
 * Python
-* Matlab (soon)
+* Matlab
+* R (soon)
 * Julia (soon)
 * Rust (soon)
 
 ## Credits
 
 PIQP is developed by the following people:
 * Roland Schwan (main developer)
@@ -48,15 +66,15 @@
 
 PIQP is build on the following open-source libraries:
 * [Eigen](https://eigen.tuxfamily.org/index.php?title=Main_Page): It's the work horse under the hood, responsible for producing optimized numerical linear algebra code.
 * [ProxSuite](https://github.com/Simple-Robotics/proxsuite): The code structure (folder/namespace structure, etc.), some utility functions/helper macros, and the instruction set optimized python bindings are based on ProxSuite.
 * [SuiteSparse - LDL](https://github.com/DrTimothyAldenDavis/SuiteSparse) (modified version): Used for solving linear systems in the sparse solver.
 * [pybind11](https://github.com/pybind/pybind11): Used for generating the python bindings.
 * [cpu_features](https://github.com/google/cpu_features): Used for run-time instruction set detection in the interface bindings.
-* [OSQP](https://github.com/osqp/osqp): The C interface is inspired by OSQP.
+* [OSQP](https://github.com/osqp/osqp): The C and Matlab interface is inspired by OSQP.
 * [Clarabel](https://github.com/oxfordcontrol/Clarabel.rs): Parts of the iterative refinement scheme are inspired by Clarabel's implementation.
 
 ## Citing our Work
 
 If you found PIQP useful in your scientific work, we encourage you to cite our accompanying paper:
 
 ```
@@ -66,8 +84,8 @@
     year = {2023},
     eprint = {arXiv:2304.00290},
 }
 ```
 
 ## License
 
-PIQP is licensed under the BSD 2-Clause License.
+PIQP is licensed under the BSD 2-Clause License.
```

### Comparing `piqp-0.1.3/interfaces/python/piqp/__init__.py` & `piqp-0.2.0/interfaces/python/piqp/__init__.py`

 * *Files identical despite different names*

### Comparing `piqp-0.1.3/piqp.egg-info/PKG-INFO` & `piqp-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,18 @@
-Metadata-Version: 2.1
-Name: piqp
-Version: 0.1.3
-Summary: An embedded Proximal Interior Point Quadratic Programming solver
-Home-page: https://github.com/PREDICT-EPFL/piqp
-Author: Roland Schwan
-Author-email: roland.schwan@epfl.ch
-License: BSD-2-Clause
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # PIQP
 
 [![DOI](https://img.shields.io/badge/DOI-10.48550/arXiv.2304.00290-green.svg)](https://doi.org/10.48550/arXiv.2304.00290)
 [![Preprint](https://img.shields.io/badge/Preprint-arXiv-blue.svg)](https://arxiv.org/abs/2304.00290)
-[![Funding](https://img.shields.io/badge/Grant-NCCR%20Automation%20(51NF40180545)-90e3dc.svg)](https://nccr-automation.ch/)
+[![Funding](https://img.shields.io/badge/Grant-NCCR%20Automation%20(51NF40__180545)-90e3dc.svg)](https://nccr-automation.ch/)
+
 [![Docs](https://img.shields.io/badge/Docs-available-brightgreen.svg)](https://predict-epfl.github.io/piqp/)
+![License](https://img.shields.io/badge/License-BSD--2--Clause-brightgreen.svg)
+![PyPI - downloads](https://img.shields.io/pypi/dm/piqp.svg?label=PyPI%20downloads)
 
-PIQP is an embedded Proximal Interior Point Quadratic Programming solver, which can solve dense and sparse quadratic programs of the form
+PIQP is a Proximal Interior Point Quadratic Programming solver, which can solve dense and sparse quadratic programs of the form
 
 $$
 \begin{aligned}
 \min_{x} \quad & \frac{1}{2} x^\top P x + c^\top x \\
 \text {s.t.}\quad & Ax=b, \\
 & Gx \leq h, \\
 & x_{lb} \leq x \leq x_{ub},
@@ -32,22 +22,24 @@
 Combining an infeasible interior point method with the proximal method of multipliers, the algorithm can handle ill-conditioned convex QP problems without the need for linear independence of the constraints.
 
 ## Features
 
 * PIQP is written in header only C++ 14 leveraging the [Eigen](https://eigen.tuxfamily.org/index.php?title=Main_Page) library for vectorized linear algebra.
 * Dense and sparse problem formulations are supported. For small dense problems, vectorized instructions and cache locality can be exploited more efficiently.
 * Interface to Python with many more to follow.
+* Allocation free problem updates and re-solves.
 * Open source under the BSD 2-Clause License.
 
 ## Interfaces
 
 PIQP support a wide range of interfaces including
 * C/C++ (with Eigen support)
 * Python
-* Matlab (soon)
+* Matlab
+* R (soon)
 * Julia (soon)
 * Rust (soon)
 
 ## Credits
 
 PIQP is developed by the following people:
 * Roland Schwan (main developer)
@@ -61,15 +53,15 @@
 
 PIQP is build on the following open-source libraries:
 * [Eigen](https://eigen.tuxfamily.org/index.php?title=Main_Page): It's the work horse under the hood, responsible for producing optimized numerical linear algebra code.
 * [ProxSuite](https://github.com/Simple-Robotics/proxsuite): The code structure (folder/namespace structure, etc.), some utility functions/helper macros, and the instruction set optimized python bindings are based on ProxSuite.
 * [SuiteSparse - LDL](https://github.com/DrTimothyAldenDavis/SuiteSparse) (modified version): Used for solving linear systems in the sparse solver.
 * [pybind11](https://github.com/pybind/pybind11): Used for generating the python bindings.
 * [cpu_features](https://github.com/google/cpu_features): Used for run-time instruction set detection in the interface bindings.
-* [OSQP](https://github.com/osqp/osqp): The C interface is inspired by OSQP.
+* [OSQP](https://github.com/osqp/osqp): The C and Matlab interface is inspired by OSQP.
 * [Clarabel](https://github.com/oxfordcontrol/Clarabel.rs): Parts of the iterative refinement scheme are inspired by Clarabel's implementation.
 
 ## Citing our Work
 
 If you found PIQP useful in your scientific work, we encourage you to cite our accompanying paper:
 
 ```
@@ -79,8 +71,8 @@
     year = {2023},
     eprint = {arXiv:2304.00290},
 }
 ```
 
 ## License
 
-PIQP is licensed under the BSD 2-Clause License.
+PIQP is licensed under the BSD 2-Clause License.
```

### Comparing `piqp-0.1.3/pyproject.toml` & `piqp-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `piqp-0.1.3/setup.py` & `piqp-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,20 +138,20 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="piqp",
-    version="0.1.3",
+    version="0.2.0",
     url='https://github.com/PREDICT-EPFL/piqp',
     author="Roland Schwan",
     author_email="roland.schwan@epfl.ch",
     license='BSD-2-Clause',
-    description="An embedded Proximal Interior Point Quadratic Programming solver",
+    description="A Proximal Interior Point Quadratic Programming solver",
     long_description=long_description,
     long_description_content_type='text/markdown',
     ext_modules=[CMakeExtension("piqp.piqp")],
     package_dir={"piqp": "interfaces/python/piqp"},
     packages=["piqp"],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
```

