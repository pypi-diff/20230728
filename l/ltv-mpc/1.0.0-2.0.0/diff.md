# Comparing `tmp/ltv-mpc-1.0.0.tar.gz` & `tmp/ltv-mpc-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltv-mpc-1.0.0.tar", last modified: Fri Aug 12 14:42:17 2022, max compression
+gzip compressed data, was "ltv-mpc-2.0.0.tar", last modified: Fri Jul 28 09:01:35 2023, max compression
```

## Comparing `ltv-mpc-1.0.0.tar` & `ltv-mpc-2.0.0.tar`

### file list

```diff
@@ -1,26 +1,35 @@
--rw-r--r--   0        0        0     1094 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0       91 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/.gitignore
--rw-r--r--   0        0        0      711 2022-04-02 22:52:50.155130 ltv-mpc-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      646 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/LICENSE
--rw-r--r--   0        0        0     5590 2022-08-12 14:38:04.426567 ltv-mpc-1.0.0/README.md
--rw-r--r--   0        0        0     1177 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/doc/Makefile
--rw-r--r--   0        0        0     9386 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/doc/src/conf.py
--rw-r--r--   0        0        0      533 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/doc/src/developer-notes.rst
--rw-r--r--   0        0        0     2477 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/doc/src/examples.rst
--rw-r--r--   0        0        0    55007 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/doc/src/images/ltv-mpc.svg
--rw-r--r--   0        0        0      908 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/doc/src/index.rst
--rw-r--r--   0        0        0      171 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/doc/src/installation.rst
--rw-r--r--   0        0        0      367 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/doc/src/usage.rst
--rw-r--r--   0        0        0     3804 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/examples/humanoid_stepping.py
--rw-r--r--   0        0        0     2240 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/examples/triple_integrator.py
--rw-r--r--   0        0        0      873 2022-08-12 14:41:34.820967 ltv-mpc-1.0.0/ltv_mpc/__init__.py
--rw-r--r--   0        0        0     6705 2022-04-02 22:46:41.272012 ltv-mpc-1.0.0/ltv_mpc/problem.py
--rw-r--r--   0        0        0     2061 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/ltv_mpc/solution.py
--rw-r--r--   0        0        0     5735 2022-08-12 14:38:04.598566 ltv-mpc-1.0.0/ltv_mpc/solve_mpc.py
--rw-r--r--   0        0        0     1327 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      699 2022-04-02 22:39:21.369567 ltv-mpc-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     3912 2022-08-12 14:38:04.754566 ltv-mpc-1.0.0/tests/test_humanoid_stepping.py
--rw-r--r--   0        0        0      759 2022-08-12 14:38:04.754566 ltv-mpc-1.0.0/tox.ini
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 ltv-mpc-1.0.0/setup.py
--rw-r--r--   0        0        0      207 1970-01-01 00:00:00.000000 ltv-mpc-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-07-24 09:29:39.214456 ltv-mpc-2.0.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0       91 2022-04-02 22:39:21.369567 ltv-mpc-2.0.0/.gitignore
+-rw-r--r--   0        0        0     2026 2023-07-28 08:50:13.210176 ltv-mpc-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      646 2022-04-02 22:39:21.369567 ltv-mpc-2.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2022-04-02 22:39:21.369567 ltv-mpc-2.0.0/LICENSE
+-rw-r--r--   0        0        0     5488 2023-07-24 09:49:18.610157 ltv-mpc-2.0.0/README.md
+-rw-r--r--   0        0        0     1077 2023-07-24 09:29:39.214456 ltv-mpc-2.0.0/doc/Makefile
+-rw-r--r--   0        0        0     9392 2023-07-24 09:29:39.214456 ltv-mpc-2.0.0/doc/src/conf.py
+-rw-r--r--   0        0        0      435 2023-07-26 14:35:00.918089 ltv-mpc-2.0.0/doc/src/developer-notes.rst
+-rw-r--r--   0        0        0     2471 2023-07-24 08:52:40.755158 ltv-mpc-2.0.0/doc/src/examples.rst
+-rw-r--r--   0        0        0    55007 2022-04-02 22:39:21.369567 ltv-mpc-2.0.0/doc/src/images/ltv-mpc.svg
+-rw-r--r--   0        0        0      822 2023-07-24 09:29:39.214456 ltv-mpc-2.0.0/doc/src/index.rst
+-rw-r--r--   0        0        0      169 2023-07-24 08:52:40.755158 ltv-mpc-2.0.0/doc/src/installation.rst
+-rw-r--r--   0        0        0      383 2023-07-24 09:29:39.214456 ltv-mpc-2.0.0/doc/src/usage.rst
+-rw-r--r--   0        0        0     3998 2023-07-25 12:19:13.581452 ltv-mpc-2.0.0/examples/cart_pole.py
+-rw-r--r--   0        0        0     4427 2023-07-24 08:52:40.755158 ltv-mpc-2.0.0/examples/humanoid_one_step.py
+-rw-r--r--   0        0        0    11607 2023-07-24 08:52:40.755158 ltv-mpc-2.0.0/examples/lipm_walking_controller.py
+-rw-r--r--   0        0        0     2212 2023-07-18 18:24:49.969835 ltv-mpc-2.0.0/examples/triple_integrator.py
+-rw-r--r--   0        0        0      908 2023-07-28 08:50:27.870980 ltv-mpc-2.0.0/ltv_mpc/__init__.py
+-rw-r--r--   0        0        0      980 2023-07-25 12:19:13.581452 ltv-mpc-2.0.0/ltv_mpc/exceptions.py
+-rw-r--r--   0        0        0      773 2023-07-25 12:19:13.581452 ltv-mpc-2.0.0/ltv_mpc/live_plots/__init__.py
+-rw-r--r--   0        0        0     5026 2023-07-25 12:19:13.581452 ltv-mpc-2.0.0/ltv_mpc/live_plots/cart_pole_plot.py
+-rw-r--r--   0        0        0     4000 2023-07-25 12:19:13.581452 ltv-mpc-2.0.0/ltv_mpc/live_plots/live_plot.py
+-rw-r--r--   0        0        0    11913 2023-07-26 14:35:00.918089 ltv-mpc-2.0.0/ltv_mpc/mpc_problem.py
+-rw-r--r--   0        0        0     5996 2023-07-28 08:48:05.570632 ltv-mpc-2.0.0/ltv_mpc/mpc_qp.py
+-rw-r--r--   0        0        0     3756 2023-07-23 19:45:49.801016 ltv-mpc-2.0.0/ltv_mpc/plan.py
+-rw-r--r--   0        0        0     1948 2023-07-26 14:35:00.918089 ltv-mpc-2.0.0/ltv_mpc/solve_mpc.py
+-rw-r--r--   0        0        0      750 2023-07-24 08:52:40.755158 ltv-mpc-2.0.0/ltv_mpc/systems/__init__.py
+-rw-r--r--   0        0        0     5263 2023-07-28 08:48:05.570632 ltv-mpc-2.0.0/ltv_mpc/systems/cart_pole.py
+-rw-r--r--   0        0        0     1677 2023-07-24 08:52:40.755158 ltv-mpc-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      699 2022-04-02 22:39:21.369567 ltv-mpc-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     3825 2023-07-26 14:35:00.918089 ltv-mpc-2.0.0/tests/test_humanoid_one_step.py
+-rw-r--r--   0        0        0      832 2023-07-24 09:00:00.690010 ltv-mpc-2.0.0/tox.ini
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 ltv-mpc-2.0.0/setup.py
+-rw-r--r--   0        0        0     6694 1970-01-01 00:00:00.000000 ltv-mpc-2.0.0/PKG-INFO
```

### Comparing `ltv-mpc-1.0.0/.github/workflows/build.yml` & `ltv-mpc-2.0.0/.github/workflows/build.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 name: CI
 
 on:
   push:
-    branches: [ master ]
+    branches: [ main ]
   pull_request:
-    branches: [ master ]
+    branches: [ main ]
   workflow_dispatch:
 
 jobs:
     build:
         runs-on: ubuntu-latest
         env:
             USING_COVERAGE: "3.8"
 
         strategy:
             matrix:
-                python-version: [3.8, 3.9]
+                python-version: ["3.8", "3.9", "3.10"]
 
         steps:
             - name: "Checkout sources"
-              uses: actions/checkout@v2
+              uses: actions/checkout@v3
 
             - name: "Set up Python"
-              uses: actions/setup-python@v2
+              uses: actions/setup-python@v4
               with:
                   python-version: "${{ matrix.python-version }}"
 
             - name: "Install dependencies"
               run: |
                   python -m pip install --upgrade pip
                   python -m pip install black coverage coveralls flake8 flit mccabe mypy numpy pylint pytest tox tox-gh-actions
```

### Comparing `ltv-mpc-1.0.0/CONTRIBUTING.md` & `ltv-mpc-2.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ltv-mpc-1.0.0/LICENSE` & `ltv-mpc-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ltv-mpc-1.0.0/README.md` & `ltv-mpc-2.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,35 @@
 # ltv-mpc
 
-[**Installation**](https://github.com/tasts-robots/ltv-mpc#installation)
-| [**Usage**](https://github.com/tasts-robots/ltv-mpc#usage)
-| [**Example**](https://github.com/tasts-robots/ltv-mpc#example)
-| [**Areas of improvement**](https://github.com/tasts-robots/ltv-mpc#areas-of-improvement)
-| [**Alternatives**](https://github.com/tasts-robots/ltv-mpc#alternatives)
-
-[![Build](https://img.shields.io/github/workflow/status/tasts-robots/ltv-mpc/CI)](https://github.com/tasts-robots/ltv-mpc/actions)
-[![Coverage](https://coveralls.io/repos/github/tasts-robots/ltv-mpc/badge.svg?branch=master)](https://coveralls.io/github/tasts-robots/ltv-mpc?branch=master)
+[![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/ltv-mpc/build.yml?branch=main)](https://github.com/stephane-caron/ltv-mpc/actions)
+[![Coverage](https://coveralls.io/repos/github/stephane-caron/ltv-mpc/badge.svg?branch=main)](https://coveralls.io/github/stephane-caron/ltv-mpc?branch=main)
 [![Documentation](https://img.shields.io/badge/docs-online-brightgreen?logo=read-the-docs&style=flat)](https://tasts-robots.org/doc/ltv-mpc/)
 [![PyPI version](https://img.shields.io/pypi/v/ltv-mpc)](https://pypi.org/project/ltv-mpc/0.6.0/)
-![Status](https://img.shields.io/pypi/status/ltv-mpc)
 
-Linear time-variant (LTV) model predictive control in Python. Solve a quadratic program of the form:
+Model predictive control (MPC) in Python for systems whose problems can be cast as a quadratic program (QP). This includes linear time-invariant (LTI) and time-variant (LTV) systems with linear constraints. The resulting QP has the form:
 
-> ![ltv-mpc](https://raw.githubusercontent.com/tasts-robots/ltv-mpc/master/doc/src/images/ltv-mpc.svg)
+> ![ltv-mpc](https://raw.githubusercontent.com/stephane-caron/ltv-mpc/main/doc/src/images/ltv-mpc.svg)
 
 This module is designed for prototyping. If you need performance, check out the [alternatives](#alternatives) below.
 
-📢 **2022-08:** the brand new [mpc_interface](https://github.com/Gepetto/mpc-interface) handles more general cost functions.
-
 ## Installation
 
 ```sh
 pip install ltv-mpc
 ```
 
 ## Usage
 
 This module defines a one-stop shop function:
 
 ```python
-solve_mpc(problem: Problem, solver: str) -> Solution
+solve_mpc(problem: MPCProblem, solver: str) -> Plan
 ```
 
-The [``Problem``](https://tasts-robots.org/doc/ltv-mpc/usage.html#ltv_mpc.problem.Problem) type defines the model predictive control problem (LTV system, LTV constraints, initial state and cost function to optimize) while the [``Solution``](https://tasts-robots.org/doc/ltv-mpc/usage.html#ltv_mpc.solution.Solution) holds the resulting state and input trajectories.
+The [``MPCProblem``](https://tasts-robots.org/doc/ltv-mpc/usage.html#ltv_mpc.mpc_problem.MPCProblem) defines the model predictive control problem (LTV system, LTV constraints, initial state and cost function to optimize) while the returned [``Plan``](https://tasts-robots.org/doc/ltv-mpc/usage.html#ltv_mpc.plan.Plan) holds the state and input trajectories that result from optimizing the problem (if a solution exists). The ``solver`` string is used to select the backend [quadratic programming solver](https://github.com/stephane-caron/qpsolvers#solvers).
 
 ## Example
 
 Let us define a triple integrator:
 
 ```python
     import numpy as np
@@ -58,19 +49,19 @@
     C = np.vstack([+accel_from_state, -accel_from_state])
     e = np.array([+max_accel, +max_accel])
 ```
 
 This leads us to the following linear MPC problem:
 
 ```python
-    from ltv_mpc import Problem
+    from ltv_mpc import MPCProblem
 
     x_init = np.array([0.0, 0.0, 0.0])
     x_goal = np.array([1.0, 0.0, 0.0])
-    problem = Problem(
+    problem = MPCProblem(
         transition_state_matrix=A,
         transition_input_matrix=B,
         ineq_state_matrix=C,
         ineq_input_matrix=None,
         ineq_vector=e,
         initial_state=x_init,
         goal_state=x_goal,
@@ -91,15 +82,15 @@
 
 The solution holds complete state and input trajectories as stacked vectors. For instance, we can plot positions, velocities and accelerations as follows:
 
 ```python
     import pylab
 
     t = np.linspace(0.0, horizon_duration, N + 1)
-    X = solution.stacked_states
+    X = solution.states
     positions, velocities, accelerations = X[:, 0], X[:, 1], X[:, 2]
     pylab.ion()
     pylab.plot(t, positions)
     pylab.plot(t, velocities)
     pylab.plot(t, accelerations)
     pylab.grid(True)
     pylab.legend(("position", "velocity", "acceleration"))
@@ -115,19 +106,20 @@
 
 This module is incomplete with regards to the following points:
 
 - Cost functions: can be extended to general linear stage cost functions
 - Documentation: there are some undocumented functions
 - Test coverage: only one end-to-end test
 
-New [contributions](CONTRIBUTING.md) are welcome :)
+Check out the [contribution guidelines](CONTRIBUTING.md) if you are interested in lending a hand.
 
 ## Alternatives
 
-This module is designed for prototyping. If you need performance, check out one of the following libraries, and [open a PR](https://github.com/tasts-robots/ltv-mpc/pulls) if you know other relevant ones:
+This module is designed for faster prototyping rather than performance. You can also check out the following open-source libraries:
 
-| Library                                                    | System                | Language   | License      |
+| Name                                                       | Systems               | Languages  | License      |
 |------------------------------------------------------------|-----------------------|------------|--------------|
-| [Copra (original)](https://github.com/jrl-umi3218/copra)   | Linear time-invariant | C++        | BSD-2-Clause |
-| [Copra (fork)](https://github.com/ANYbotics/copra)         | Linear time-variant   | C++        | BSD-2-Clause |
-| [mpc\_interface](https://github.com/Gepetto/mpc-interface) | Linear time-variant   | C++/Python | BSD-2-Clause |
-| [Crocoddyl](https://github.com/loco-3d/crocoddyl)          | Nonlinear             | C++        | BSD-3-Clause |
+| [Copra (LTV fork)](https://github.com/ANYbotics/copra)     | Linear time-variant   | Python/C++ | BSD-2-Clause |
+| [Copra (original)](https://github.com/jrl-umi3218/copra)   | Linear time-invariant | Python/C++ | BSD-2-Clause |
+| [Crocoddyl](https://github.com/loco-3d/crocoddyl)          | Nonlinear             | Python/C++ | BSD-3-Clause |
+| [mpc-interface](https://github.com/Gepetto/mpc-interface)  | Linear time-variant   | Python/C++ | BSD-2-Clause |
+| [pyMPC](https://github.com/forgi86/pyMPC)                  | Linear time-variant   | Python     | MIT          |
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ltv-mpc-1.0.0/doc/src/conf.py` & `ltv-mpc-2.0.0/doc/src/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
 import sys
-
-from os.path import dirname, join, abspath
+from os.path import abspath, dirname, join
 
 sys.path.insert(0, abspath("../.."))
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
@@ -32,15 +31,15 @@
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.coverage",
     "sphinx-mathjax-offline",
     "sphinx.ext.napoleon",  # before sphinx_autodoc_typehints
-    "sphinx_autodoc_typehints"
+    "sphinx_autodoc_typehints",
 ]
 
 # List of modules to be mocked up
 autodoc_mock_imports = ["ecos", "gurobipy", "mosek", "osqp", "qpoases"]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = []
@@ -70,31 +69,29 @@
 # The short X.Y version.
 version = None  # read from __init__.py
 
 # The full version, including alpha/beta/rc tags.
 release = None  # read from __init__.py
 
 # Read version info directly from the module's __init__.py
-init_path = join(
-    dirname(dirname(dirname(str(abspath(__file__))))), "ltv_mpc"
-)
+init_path = join(dirname(dirname(dirname(str(abspath(__file__))))), "ltv_mpc")
 with open(f"{init_path}/__init__.py", "r") as fh:
     for line in fh:
-        match = re.match('__version__ = "((\\d.\\d).\\d)".*', line)
+        match = re.match('__version__ = "((\\d.\\d).\\d)[a-z0-9\\-]*".*', line)
         if match is not None:
             release = match.group(1)
             version = match.group(2)
             break
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #
 # today = ''
 #
 # Else, today_fmt is used as the format for a strftime call.
```

### Comparing `ltv-mpc-1.0.0/doc/src/examples.rst` & `ltv-mpc-2.0.0/doc/src/examples.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-:github_url: https://github.com/tasts-robots/ltv-mpc/tree/master/doc/src/examples.rst
+:github_url: https://github.com/tasts-robots/ltv-mpc/tree/main/doc/src/examples.rst
 
 ********
 Examples
 ********
 
 Triple integrator
 =================
@@ -28,19 +28,19 @@
     ineq_matrix = np.vstack([+accel_from_state, -accel_from_state])
     ineq_vector = np.array([+max_accel, +max_accel])
 
 This leads us to the following linear MPC problem:
 
 .. code:: python
 
-    from ltv_mpc import Problem
+    from ltv_mpc import MPCProblem
 
     initial_pos = 0.0
     goal_pos = 1.0
-    problem = ltv_mpc.Problem(
+    problem = ltv_mpc.MPCProblem(
         transition_state_matrix=A,
         transition_input_matrix=B,
         ineq_state_matrix=ineq_matrix,
         ineq_input_matrix=None,
         ineq_vector=ineq_vector,
         initial_state=np.array([initial_pos, 0.0, 0.0]),
         goal_state=np.array([goal_pos, 0.0, 0.0]),
@@ -52,24 +52,24 @@
 
 We can solve it with:
 
 .. code:: python
 
     from ltv_mpc import solve_mpc
 
-    solution = solve_mpc(problem, mpc)
+    plan = solve_mpc(problem, mpc)
 
-The solution holds complete state and input trajectories as stacked vectors. For instance, we can plot positions, velocities and accelerations as follows:
+The resulting plan holds complete state and input trajectories as stacked vectors. For instance, we can plot positions, velocities and accelerations as follows:
 
 .. code:: python
 
     import pylab
 
     t = np.linspace(0.0, horizon_duration, nb_timesteps + 1)
-    X = solution.stacked_states
+    X = plan.states
     positions, velocities, accelerations = X[:, 0], X[:, 1], X[:, 2]
     pylab.ion()
     pylab.plot(t, positions)
     pylab.plot(t, velocities)
     pylab.plot(t, accelerations)
     pylab.grid(True)
     pylab.legend(("position", "velocity", "acceleration"))
```

### Comparing `ltv-mpc-1.0.0/doc/src/images/ltv-mpc.svg` & `ltv-mpc-2.0.0/doc/src/images/ltv-mpc.svg`

 * *Files identical despite different names*

### Comparing `ltv-mpc-1.0.0/examples/triple_integrator.py` & `ltv-mpc-2.0.0/examples/triple_integrator.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""Triple integrator LTV system."""
+
 import numpy as np
 import pylab
 
-from ltv_mpc import Problem
-from ltv_mpc import solve_mpc
-
+from ltv_mpc import MPCProblem, solve_mpc
 
 if __name__ == "__main__":
-    # Double integrator LTV system
     horizon_duration = 1.0
     nb_timesteps = 16
     T = horizon_duration / nb_timesteps
     A = np.array([[1.0, T, T ** 2 / 2.0], [0.0, 1.0, T], [0.0, 0.0, 1.0]])
     B = np.array([T ** 3 / 6.0, T ** 2 / 2.0, T]).reshape((3, 1))
 
     # Acceleration limits
@@ -35,34 +34,34 @@
     max_accel = 3.0  # [m] / [s] / [s]
     ineq_matrix = np.vstack([+accel_from_state, -accel_from_state])
     ineq_vector = np.array([+max_accel, +max_accel])
 
     # Complete LTV problem
     initial_pos = 0.0
     goal_pos = 1.0
-    problem = Problem(
+    problem = MPCProblem(
         transition_state_matrix=A,
         transition_input_matrix=B,
         ineq_state_matrix=ineq_matrix,
         ineq_input_matrix=None,
         ineq_vector=ineq_vector,
         initial_state=np.array([initial_pos, 0.0, 0.0]),
         goal_state=np.array([goal_pos, 0.0, 0.0]),
         nb_timesteps=nb_timesteps,
         terminal_cost_weight=1.0,
         stage_state_cost_weight=None,
         stage_input_cost_weight=1e-6,
     )
 
     # Solve our LTV problem
-    solution = solve_mpc(problem, solver="osqp")
+    plan = solve_mpc(problem, solver="osqp")
 
     # Plot solution
     t = np.linspace(0.0, horizon_duration, nb_timesteps + 1)
-    X = solution.stacked_states
+    X = plan.states
     positions, velocities, accelerations = X[:, 0], X[:, 1], X[:, 2]
     pylab.ion()
     pylab.clf()
     pylab.plot(t, positions)
     pylab.plot(t, velocities)
     pylab.plot(t, accelerations)
     pylab.grid(True)
```

### Comparing `ltv-mpc-1.0.0/ltv_mpc/__init__.py` & `ltv-mpc-2.0.0/ltv_mpc/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Linear time-variant model predictive control in Python.
-"""
+"""Linear time-variant model predictive control in Python."""
 
-from .problem import Problem
-from .solution import Solution
+from .mpc_problem import MPCProblem
+from .mpc_qp import MPCQP
+from .plan import Plan
 from .solve_mpc import solve_mpc
 
 __all__ = [
-    "Problem",
-    "Solution",
+    "MPCProblem",
+    "MPCQP",
+    "Plan",
     "solve_mpc",
 ]
 
-__version__ = "1.0.0"
+__version__ = "2.0.0"
```

### Comparing `ltv-mpc-1.0.0/ltv_mpc/solve_mpc.py` & `ltv-mpc-2.0.0/ltv_mpc/mpc_qp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,166 +1,161 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright 2022 Stéphane Caron
+# Copyright 2023 Inria
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from dataclasses import dataclass
-from typing import Optional, Union
+"""MPC problem represented as a quadratic program."""
 
-import numpy as np
+from logging import warn
 
+import numpy as np
+import qpsolvers
 from scipy.sparse import csc_matrix
-from qpsolvers import solve_qp
-
-from .problem import Problem
-from .solution import Solution
-
 
-@dataclass
-class QuadraticProgram:
-
-    """
-    Quadratic program (QP) with inequality constraints.
-    """
+from .exceptions import ProblemDefinitionError
+from .mpc_problem import MPCProblem
 
-    cost_matrix: Union[np.ndarray, csc_matrix]
-    cost_vector: np.ndarray
-    ineq_matrix: Union[np.ndarray, csc_matrix]
-    ineq_vector: np.ndarray
 
+class MPCQP:
+    r"""MPC problem represented as a quadratic program.
 
-def build_qp(problem: Problem, sparse: bool = False) -> QuadraticProgram:
-    """
-    Build the quadratic program corresponding to an LTV-MPC problem.
-
-    Args:
-        problem: Model predictive control problem.
-        sparse: Whether to use sparse or dense matrices in the output quadratic
-            program. Enable it if you are calling a sparse solver afterwards.
-
-    Returns:
-        Quadratic program representing the input problem.
-
-    Notes:
-        In numerical analysis, there are three classes of methods to solve
-        boundary value problems: single shooting, multiple shooting and
-        collocation. The QP built by this function implements a `single
-        shooting method <https://en.wikipedia.org/wiki/Shooting_method>`_.
-    """
-    input_dim = problem.input_dim
-    state_dim = problem.state_dim
-    stacked_input_dim = problem.input_dim * problem.nb_timesteps
-
-    phi = np.eye(state_dim)
-    psi = np.zeros((state_dim, stacked_input_dim))
-    G_list, h_list = [], []
-    phi_list, psi_list = [], []
-    for k in range(problem.nb_timesteps):
-        # Loop invariant: x == psi * U + phi * x_init
-        if problem.stage_state_cost_weight is not None:
+    This class further stores intermediate matrices used to recompute cost and
+    linear inequality vectors.
+    """
+
+    G: np.ndarray
+    P: np.ndarray
+    Phi: np.ndarray
+    Psi: np.ndarray
+    h: np.ndarray
+    phi_last: np.ndarray
+    psi_last: np.ndarray
+    q: np.ndarray
+
+    def __init__(self, mpc_problem: MPCProblem, sparse: bool = False) -> None:
+        """Create a new QP representation.
+
+        Args:
+            mpc_problem: Model predictive control problem to cast as a QP.
+            sparse: If set, use sparse matrix representation.
+        """
+        input_dim = mpc_problem.input_dim
+        state_dim = mpc_problem.state_dim
+        stacked_input_dim = mpc_problem.input_dim * mpc_problem.nb_timesteps
+        if mpc_problem.initial_state is None:
+            raise ProblemDefinitionError("initial state is undefined")
+        initial_state: np.ndarray = mpc_problem.initial_state
+
+        phi = np.eye(state_dim)
+        psi = np.zeros((state_dim, stacked_input_dim))
+        G_list, h_list = [], []
+        phi_list, psi_list = [], []
+        for k in range(mpc_problem.nb_timesteps):
+            # Loop invariant: x == psi * U + phi * x_init
             phi_list.append(phi)
             psi_list.append(psi)
-        A = problem.get_transition_state_matrix(k)
-        B = problem.get_transition_input_matrix(k)
-        C = problem.get_ineq_state_matrix(k)
-        D = problem.get_ineq_input_matrix(k)
-        e = problem.get_ineq_vector(k)
-        G = np.zeros((e.shape[0], stacked_input_dim))
-        h = e if C is None else e - np.dot(C.dot(phi), problem.initial_state)
-        input_slice = slice(k * input_dim, (k + 1) * input_dim)
-        if D is not None:
-            # we rely on G == 0 to avoid a slower +=
-            G[:, input_slice] = D
-        if C is not None:
-            G += C.dot(psi)
-        if k == 0 and D is None:  # corner case, input has no effect
-            assert np.all(h >= 0.0)
-        else:  # regular case, G is non-zero
-            G_list.append(G)
-            h_list.append(h)
-        phi = A.dot(phi)
-        psi = A.dot(psi)
-        psi[:, input_slice] = B
-
-    P = problem.stage_input_cost_weight * np.eye(stacked_input_dim)
-    q = np.zeros(stacked_input_dim)
-    if (
-        problem.terminal_cost_weight is not None
-        and problem.terminal_cost_weight > 1e-10
-    ):
-        c = np.dot(phi, problem.initial_state) - problem.goal_state
-        P += problem.terminal_cost_weight * np.dot(psi.T, psi)
-        q += problem.terminal_cost_weight * np.dot(c.T, psi)
-    if (
-        problem.stage_state_cost_weight is not None
-        and problem.stage_state_cost_weight > 1e-10
-    ):
+            A_k = mpc_problem.get_transition_state_matrix(k)
+            B_k = mpc_problem.get_transition_input_matrix(k)
+            C_k = mpc_problem.get_ineq_state_matrix(k)
+            D_k = mpc_problem.get_ineq_input_matrix(k)
+            e_k = mpc_problem.get_ineq_vector(k)
+            G_k = np.zeros((e_k.shape[0], stacked_input_dim))
+            h_k = (
+                e_k
+                if C_k is None
+                else e_k - np.dot(C_k.dot(phi), initial_state)
+            )
+            input_slice = slice(k * input_dim, (k + 1) * input_dim)
+            if D_k is not None:
+                # we rely on G == 0 to avoid a slower +=
+                G_k[:, input_slice] = D_k
+            if C_k is not None:
+                G_k += C_k.dot(psi)
+            if k == 0 and D_k is None and np.any(h_k < 0.0):
+                # in this case, the initial state constraint is violated and
+                # cannot be compensated by any input (D_k is None)
+                warn(
+                    "initial state is unfeasible: "
+                    f"G_0 * x <= h_0 with G_0 == 0 and min(h_0) == {min(h_k)}"
+                )
+            G_list.append(G_k)
+            h_list.append(h_k)
+            phi = A_k.dot(phi)
+            psi = A_k.dot(psi)
+            psi[:, input_slice] = B_k
+        G: np.ndarray = np.vstack(G_list)
+        h: np.ndarray = np.hstack(h_list)
         Phi = np.vstack(phi_list)
         Psi = np.vstack(psi_list)
-        X_goal = np.hstack([problem.goal_state] * problem.nb_timesteps)
-        c = np.dot(Phi, problem.initial_state) - X_goal
-        P += problem.stage_state_cost_weight * np.dot(Psi.T, Psi)
-        q += problem.stage_state_cost_weight * np.dot(c.T, Psi)
-
-    G = np.vstack(G_list)
-    h = np.hstack(h_list)
-    if sparse:
-        P = csc_matrix(P)
-        G = csc_matrix(G)
-    return QuadraticProgram(
-        cost_matrix=P, cost_vector=q, ineq_matrix=G, ineq_vector=h
-    )
-
-
-def solve_mpc(
-    problem: Problem,
-    sparse: bool = False,
-    solver: Optional[str] = None,
-    **kwargs
-) -> Solution:
-    """
-    Solve a linear time-invariant model predictive control problem.
-
-    Args:
-        problem: Model predictive control problem to solve.
-        solver: Quadratic programming solver to use, to choose in
-            :data:`qpsolvers.available_solvers`. Both "quadprog" and "osqp"
-            tend to perform well on model predictive control problems. See for
-            instance `this benchmark
-            <https://github.com/stephane-caron/qpsolvers#benchmark>`__.
-        sparse: Whether to use sparse or dense matrices in the output quadratic
-            program. Enable it if the QP solver is sparse (e.g. OSQP).
-
-    Returns:
-        Solution to the problem, if found.
-
-    Note:
-        Keyword arguments are passed to the QP solver via the `solve_qp`_
-        function. In particular, the ``solver`` string can be set to select a
-        different QP solver.
 
-    .. _solve_qp:
-        https://scaron.info/doc/qpsolvers/quadratic-programming.html#qpsolvers.solve_qp
-    """
-    qp = build_qp(problem, sparse=sparse)
-    U = solve_qp(
-        qp.cost_matrix,
-        qp.cost_vector,
-        qp.ineq_matrix,
-        qp.ineq_vector,
-        solver=solver,
-        **kwargs
-    )
-    U = U.reshape((problem.nb_timesteps, problem.input_dim))
-    return Solution(problem, U)
+        P: np.ndarray = mpc_problem.stage_input_cost_weight * np.eye(
+            stacked_input_dim,
+        )
+        if mpc_problem.terminal_cost_weight is not None:
+            P += mpc_problem.terminal_cost_weight * np.dot(psi.T, psi)
+        if mpc_problem.stage_state_cost_weight is not None:
+            P += mpc_problem.stage_state_cost_weight * np.dot(Psi.T, Psi)
+        q: np.ndarray = np.zeros(stacked_input_dim)
+
+        self.G = csc_matrix(G) if sparse else G
+        self.P = csc_matrix(P) if sparse else P
+        self.Phi = Phi
+        self.Psi = Psi
+        self.h = h
+        self.phi_last = phi
+        self.psi_last = psi
+        self.q = q  # initialized below
+        #
+        try:
+            self.update_cost_vector(mpc_problem)
+        except ProblemDefinitionError:
+            pass
+
+    @property
+    def problem(self) -> qpsolvers.Problem:
+        """Get quadratic program to call a QP solver."""
+        return qpsolvers.Problem(self.P, self.q, self.G, self.h)
+
+    def update_cost_vector(self, mpc_problem: MPCProblem) -> None:
+        """Update the gradient vector in the cost function.
+
+        Args:
+            mpc_problem: New model predictive control problem. It should have
+                the same structure as the one used to initialize the MPCQP.
+        """
+        if mpc_problem.initial_state is None:
+            raise ProblemDefinitionError("initial state is undefined")
+        initial_state = mpc_problem.initial_state
+        self.q[:] = 0.0
+        if mpc_problem.has_terminal_cost:
+            c = np.dot(self.phi_last, initial_state) - mpc_problem.goal_state
+            self.q += mpc_problem.terminal_cost_weight * np.dot(
+                c.T, self.psi_last
+            )
+        if mpc_problem.has_stage_state_cost:
+            c = np.dot(self.Phi, initial_state) - mpc_problem.target_states
+            self.q += mpc_problem.stage_state_cost_weight * np.dot(
+                c.T, self.Psi
+            )
+
+    def update_constraint_vector(self, mpc_problem: MPCProblem) -> None:
+        """Update the inequality constraint vector.
+
+        Args:
+            mpc_problem: New model predictive control problem. It should have
+                the same structure as the one used to initialize the MPCQP.
+        """
+        raise NotImplementedError(
+            "Time-varying constraints are handled cold-start for now"
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ltv-mpc-1.0.0/pyproject.toml` & `ltv-mpc-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -24,25 +24,46 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 dependencies = [
     "qpsolvers >=1.8.0",
 ]
-keywords = ["rate", "loop", "frequency", "regulator"]
+keywords = ["model", "predictive", "control", "linear", "time-varying"]
 
 [project.optional-dependencies]
 doc = [
     "sphinx",
 ]
 
 [project.urls]
 Documentation = "https://tasts-robots.org/doc/ltv-mpc/"
 Source = "https://github.com/tasts-robots/ltv-mpc"
 Tracker = "https://github.com/tasts-robots/ltv-mpc/issues"
-Changelog = "https://github.com/tasts-robots/ltv-mpc/blob/master/CHANGELOG.md"
+Changelog = "https://github.com/tasts-robots/ltv-mpc/blob/main/CHANGELOG.md"
 
 [tool.black]
 line-length = 79
 
 [tool.flit.module]
 name = "ltv_mpc"
+
+[tool.ruff]
+line-length = 79
+select = [
+    # pyflakes
+    "F",
+    # pycodestyle
+    "E",
+    "W",
+    # isort
+    "I001",
+    # pydocstyle
+    "D"
+]
+ignore = [
+    "D401",  # good for methods but not for class docstrings
+    "D405",  # British-style section names are also "proper"!
+]
+
+[tool.ruff.pydocstyle]
+convention = "google"
```

### Comparing `ltv-mpc-1.0.0/tests/__init__.py` & `ltv-mpc-2.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ltv-mpc-1.0.0/tests/test_humanoid_stepping.py` & `ltv-mpc-2.0.0/tests/test_humanoid_one_step.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,24 +12,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
-
 from dataclasses import dataclass
 
 import numpy as np
 
-import ltv_mpc
-
-from ltv_mpc.solve_mpc import build_qp
-from ltv_mpc import solve_mpc
-
+from ltv_mpc import MPCProblem, solve_mpc
+from ltv_mpc.solve_mpc import MPCQP
 
 gravity = 9.81  # [m] / [s]^2
 
 
 @dataclass
 class HumanoidSteppingProblem:
 
@@ -70,15 +66,15 @@
             else np.array([+cur_max, -cur_min])
             if i - nb_init_dsp_steps <= nb_init_ssp_steps
             else np.array([+1000.0, +1000.0])
             if i - nb_init_dsp_steps - nb_init_ssp_steps < nb_dsp_steps
             else np.array([+next_max, -next_min])
             for i in range(problem.nb_timesteps)
         ]
-        mpc_problem = ltv_mpc.Problem(
+        mpc_problem = MPCProblem(
             transition_state_matrix=state_matrix,
             transition_input_matrix=input_matrix,
             ineq_state_matrix=ineq_matrix,
             ineq_input_matrix=None,
             ineq_vector=ineq_vector,
             initial_state=np.array([problem.start_pos, 0.0, 0.0]),
             goal_state=np.array([problem.end_pos, 0.0, 0.0]),
@@ -87,28 +83,25 @@
             stage_state_cost_weight=None,
             stage_input_cost_weight=1e-3,
         )
         #
         self.stepping_problem = problem
         self.problem = mpc_problem
 
-    def test_build_qp(self):
-        qp = build_qp(self.problem)
-        G = qp.ineq_matrix
-        self.assertNotAlmostEqual(np.linalg.norm(G[0]), 0.0)
-        self.assertNotAlmostEqual(np.linalg.norm(G[1]), 0.0)
+    def test_mpc_qp_first_constraints(self):
+        mpc_qp = MPCQP(self.problem)
+        qp = mpc_qp.problem
+        self.assertAlmostEqual(np.linalg.norm(qp.G[0:2]), 0.0)
 
     def test_solve_mpc(self):
         solution = solve_mpc(self.problem, solver="quadprog")
         N = self.problem.nb_timesteps
         input_dim = self.problem.input_dim
         state_dim = self.problem.state_dim
-        self.assertEqual(
-            solution.stacked_inputs.flatten().shape, (N * input_dim,)
-        )
-        self.assertEqual(
-            solution.stacked_states.flatten().shape, ((N + 1) * state_dim,)
-        )
+        U = solution.inputs
+        X = solution.states
+        self.assertEqual(U.flatten().shape, (N * input_dim,))
+        self.assertEqual(X.flatten().shape, ((N + 1) * state_dim,))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `ltv-mpc-1.0.0/setup.py` & `ltv-mpc-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # setup.py generated by flit for tools that don't yet use PEP 517
 
 from distutils.core import setup
 
 packages = \
-['ltv_mpc']
+['ltv_mpc', 'ltv_mpc.live_plots', 'ltv_mpc.systems']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['qpsolvers >=1.8.0']
 
 extras_require = \
 {'doc': ['sphinx']}
 
 setup(name='ltv-mpc',
-      version='1.0.0',
+      version='2.0.0',
       description='Linear time-variant model predictive control in Python.',
       author=None,
       author_email='Stéphane Caron <stephane.caron@normalesup.org>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

