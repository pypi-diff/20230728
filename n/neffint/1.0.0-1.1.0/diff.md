# Comparing `tmp/neffint-1.0.0.tar.gz` & `tmp/neffint-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/esvik/Documents/code/neffint/dist/.tmp-ddfy4n5z/neffint-1.0.0.tar", last modified: Fri Jun  9 08:42:25 2023, max compression
+gzip compressed data, was "/home/runner/work/neffint/neffint/dist/.tmp-swgvxt0_/neffint-1.1.0.tar", last modified: Fri Jul 28 16:21:35 2023, max compression
```

## Comparing `neffint-1.0.0.tar` & `neffint-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxr-x   0 esvik     (1001) esvik     (1001)        0 2023-06-09 08:42:25.000000 neffint-1.0.0/
--rw-rw-r--   0 esvik     (1001) esvik     (1001)    11358 2023-06-02 09:27:59.000000 neffint-1.0.0/LICENSE
--rw-rw-r--   0 esvik     (1001) esvik     (1001)     3530 2023-06-09 08:42:25.000000 neffint-1.0.0/PKG-INFO
--rw-rw-r--   0 esvik     (1001) esvik     (1001)     3151 2023-06-09 08:42:09.000000 neffint-1.0.0/README.md
-drwxrwxr-x   0 esvik     (1001) esvik     (1001)        0 2023-06-09 08:42:25.000000 neffint-1.0.0/neffint/
--rw-rw-r--   0 esvik     (1001) esvik     (1001)      160 2023-06-09 07:59:59.000000 neffint-1.0.0/neffint/__init__.py
--rw-rw-r--   0 esvik     (1001) esvik     (1001)    17946 2023-06-08 08:44:37.000000 neffint-1.0.0/neffint/fixed_grid_fourier_integral.py
-drwxrwxr-x   0 esvik     (1001) esvik     (1001)        0 2023-06-09 08:42:25.000000 neffint-1.0.0/neffint.egg-info/
--rw-rw-r--   0 esvik     (1001) esvik     (1001)     3530 2023-06-09 08:42:25.000000 neffint-1.0.0/neffint.egg-info/PKG-INFO
--rw-rw-r--   0 esvik     (1001) esvik     (1001)      296 2023-06-09 08:42:25.000000 neffint-1.0.0/neffint.egg-info/SOURCES.txt
--rw-rw-r--   0 esvik     (1001) esvik     (1001)        1 2023-06-09 08:42:25.000000 neffint-1.0.0/neffint.egg-info/dependency_links.txt
--rw-rw-r--   0 esvik     (1001) esvik     (1001)       47 2023-06-09 08:42:25.000000 neffint-1.0.0/neffint.egg-info/requires.txt
--rw-rw-r--   0 esvik     (1001) esvik     (1001)        8 2023-06-09 08:42:25.000000 neffint-1.0.0/neffint.egg-info/top_level.txt
--rw-rw-r--   0 esvik     (1001) esvik     (1001)       81 2023-06-02 09:27:59.000000 neffint-1.0.0/pyproject.toml
--rw-rw-r--   0 esvik     (1001) esvik     (1001)       38 2023-06-09 08:42:25.000000 neffint-1.0.0/setup.cfg
--rw-rw-r--   0 esvik     (1001) esvik     (1001)     1035 2023-06-09 08:42:15.000000 neffint-1.0.0/setup.py
-drwxrwxr-x   0 esvik     (1001) esvik     (1001)        0 2023-06-09 08:42:25.000000 neffint-1.0.0/tests/
--rw-rw-r--   0 esvik     (1001) esvik     (1001)     6874 2023-06-02 12:22:27.000000 neffint-1.0.0/tests/test_fixed_grid_fourier_integral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:21:35.000000 neffint-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-28 16:21:22.000000 neffint-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-28 16:21:35.000000 neffint-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-28 16:21:22.000000 neffint-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:21:35.000000 neffint-1.1.0/neffint/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 16:21:22.000000 neffint-1.1.0/neffint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-28 16:21:22.000000 neffint-1.1.0/neffint/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31907 2023-07-28 16:21:22.000000 neffint-1.1.0/neffint/adaptive_fourier_integral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15791 2023-07-28 16:21:22.000000 neffint-1.1.0/neffint/fixed_grid_fourier_integral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-28 16:21:22.000000 neffint-1.1.0/neffint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:21:35.000000 neffint-1.1.0/neffint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-28 16:21:35.000000 neffint-1.1.0/neffint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-28 16:21:35.000000 neffint-1.1.0/neffint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:21:35.000000 neffint-1.1.0/neffint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-28 16:21:35.000000 neffint-1.1.0/neffint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 16:21:35.000000 neffint-1.1.0/neffint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-28 16:21:22.000000 neffint-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 16:21:35.000000 neffint-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-28 16:21:22.000000 neffint-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:21:35.000000 neffint-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-07-28 16:21:22.000000 neffint-1.1.0/tests/test_adaptive_fourier_integral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-07-28 16:21:22.000000 neffint-1.1.0/tests/test_fixed_grid_fourier_integral.py
```

### Comparing `neffint-1.0.0/LICENSE` & `neffint-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neffint-1.0.0/neffint/fixed_grid_fourier_integral.py` & `neffint-1.1.0/neffint/fixed_grid_fourier_integral.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,43 +8,43 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
+import logging
 from enum import Enum
-from typing import Sequence, Tuple, Union
+from typing import Tuple
 
 import numpy as np
 from numpy.typing import ArrayLike
-from scipy.interpolate import pchip_interpolate
+
+from .utils import complex_pchip
 
 MAX_TAYLOR_ITERATIONS = 1000
 
 class InterpolationMode(Enum):
     PCHIP = "pchip"
     LINEAR = "linear"
 
 def _lambda(x: ArrayLike) -> np.ndarray:
-    """Calculates the Lambda function defined in equations E.136 in [1], which is given by:
+    """Calculates the Lambda function defined in equations E.136 in [N.Mounet-PhD]_, which is given by:
 
     Lambda(x) = -j*exp(j*x)/x + (exp(j*x)-1)/x^2,
 
     where j = sqrt(-1) is the imaginary unit.
 
-    For |x| < 1, a Taylor series approximation is summed until convergence is reached.
+    For \|x\| < 1, a Taylor series approximation is summed until convergence is reached.
 
     :param x: The input variable x, given as a single float or an array of floats.
     :type x: ArrayLike
     :raises RuntimeError: If the Taylor series summation did not converge after 1000 iterations.
     :return: Lambda, an array with the same shape as x
     :rtype: np.ndarray
-
-    [1] N. Mounet. The LHC Transverse Coupled-Bunch Instability, PhD thesis 5305 (EPFL, 2012)
     """
     # Make input into array if it is not already, and prepare output arrays
     x = np.asarray(x)
     result = np.zeros_like(1j*x)
 
     # Set relative tolerance to machine precision
     rel_tolerance = np.finfo(x.dtype).eps
@@ -83,63 +83,30 @@
         
     # If loop finished without converging, raise error
     if n == MAX_TAYLOR_ITERATIONS:
         raise RuntimeError(f"Lambda calculation failed to converge after {MAX_TAYLOR_ITERATIONS} iterations")
     
     return result
 
-def complex_pchip(xi: ArrayLike, zi: ArrayLike, x: ArrayLike, derivative_order: Union[int, Sequence[int]] = 0, axis: int = 0) -> np.ndarray:
-    """Compute the piecewise cubic hermite interpolating polynomial (PCHIP) characterized by the points (xi, zi), where xi are real and zi are complex,
-    and evaluate this polynomial or its derivatives at the points x.
-    The real and imaginary components are treated separately, using the implementation in scipy.interpolate for
-    each component, as that implementation is only designed to take in real-valued functions.
-    The PCHIP interpolation is a cubic interpolation that guarantees to preserve monotonicity on each subinterval of the input data. In this case,
-    monotonicity is therefore preserved for both real and imaginary components.
-    
-    For more information about the PCHIP algorithm, see [1].
-    
-    [1] F. N. Fritsch and J. Butland, A method for constructing local monotone piecewise cubic interpolants, SIAM J. Sci. Comput., 5(2), 300-304 (1984). DOI:10.1137/0905021.
-
-    :param xi: A 1D array of N real input points
-    :type xi: ArrayLike
-    :param func_values: An array of shape (N, X1, X2, ...) containing the output of the function to compute the interpolation for at each xi.
-    :type func_values: ArrayLike
-    :param x: A 1D array of M real inputs to evaluate the interpolation at
-    :type x: ArrayLike
-    :param derivative_order: The order(s) of derivatives to compute (`0` gives the function values). If a sequence, a list of arrays is returned, one for each order. Defaults to 0
-    :type derivative_order: Union[int, Sequence[int]], optional
-    :param axis: The axis in func_values that corresponds to xi, defaults to 0. By setting this argument, N does not need to be the first axis of func_values
-    :type axis: int, optional
-    :return: The computed PCHIP values or derivatives evaluated at the points x. If more than one derivative order is given, a list of arrays is returned
-    :rtype: np.ndarray
-    """
-    return (
-        (pchip_interpolate(xi, np.real(zi), x, der=derivative_order, axis=axis)
-        + 1j*pchip_interpolate(xi, np.imag(zi), x, der=derivative_order, axis=axis))
-    )
-
-
 def _phi_and_psi(x: ArrayLike) -> Tuple[np.ndarray, np.ndarray]:
-    """Calculates the Phi and Psi functions defined in equations E.142 and E.143 in [1], which are given by:
+    """Calculates the Phi and Psi functions defined in equations E.142 and E.143 in [N.Mounet-PhD]_, which are given by:
 
     Phi(x) = -j*exp(j*x)/x - 6j*(exp(j*x)+1)/x^3 + 12(exp(j*x)-1)/x^4,
 
     Psi(x) = exp(j*x)/x^2 + 2j*(2*exp(j*x)+1)/x^3 - 6(exp(j*x)-1)/x^4,
 
     Where j = sqrt(-1) is the imaginary unit.
 
-    For |x| < 1, a Taylor series approximation is summed until convergence is reached.
+    For \|x\| < 1, a Taylor series approximation is summed until convergence is reached.
 
     :param x: The input variable x, given as a single float or an array of floats.
     :type x: ArrayLike
     :raises RuntimeError: If the Taylor series summation did not converge after 1000 iterations.
     :return: Tuple of two arrays: Phi and Psi, with the same shape as x
     :rtype: Tuple[np.ndarray, np.ndarray]
-
-    [1] N. Mounet. The LHC Transverse Coupled-Bunch Instability, PhD thesis 5305 (EPFL, 2012)
     """
 
     # Make input into array if it is not already, and prepare output arrays
     x = np.asarray(x)
     phi = np.zeros_like(1j*x)
     psi = np.zeros_like(phi)
 
@@ -208,27 +175,26 @@
     positive_inf: bool=True
 ) -> np.ndarray:
     """Calculate the asymptotic correction term as omega -> +-inf of a Fourier integral for the given times.
     Uses a first or second (if func_derivative_end is given) order Taylor expansion around the angular frequency omega_end.
 
     :param times: Float or 1D array of floats of length M, the time(s) [s]* to compute the fourier integral for
     :type times: ArrayLike
-    :param omega_end: An angular frequency [rad/s]* to expand the Taylor series from. If `positive_inf == True`, this should be the highest angular frequency used.
-    Otherwise, it should be the lowest (closest to -inf).
+    :param omega_end: An angular frequency [rad/s]* to expand the Taylor series from. If ``positive_inf == True``, this should be the highest angular frequency used. Otherwise, it should be the lowest (closest to -inf).
     :type omega_end: float
     :param func_value_end: An array of shape (X1, X2, ...) containing the values of the function to be transformed evaluated at omega_end
     :type func_value_end: ArrayLike
     :param func_derivative_end: An array of shape (X1, X2, ...) containing the derivative of the function to be transformed, evaluated at omega_end, defaults to 0
     :type func_derivative_end: ArrayLike, optional
     :param positive_inf: Flag set to True if the asymptotic correction towards +inf should be calculated, and False if the correction towards -inf should be calculated
     :type positive_inf: bool, optional
     :return: The asymptotic terms of the Fourier Integral for all times, given as an array of shape (M, X1, X2, ...)
     :rtype: np.ndarray
     
-    * Though the units s and rad/s are used here, any coherent set of time and angular frequency units will work
+    \*Though the units s and rad/s are used here, any coherent set of time and angular frequency units will work
     """
     
     sign = (1 if positive_inf else -1)
     
     times = np.asarray(times)
     func_value_end = np.asarray(func_value_end)
     func_derivative_end = np.asarray(func_derivative_end)
@@ -251,20 +217,20 @@
     neg_inf_correction_term: bool,
     interpolation: str
 ) -> np.ndarray:
     """Calculates the fourier integral of a function for the time values given as input:
     
     integral from fmin to fmax of : exp(2*pi*j*f*t)*func(f)*df,
     
-    where t is the time, fmin is the first frequency in the input `frequencies`, fmax is either the highest frequency or (positive) infinity, depending on `inf_correction_term`,
+    where t is the time, fmin is the first frequency in the input ``frequencies``, fmax is either the highest frequency or (positive) infinity, depending on ``inf_correction_term``,
     and func(f) is the input function of frequency. The function is given as an array of outputs corresponding to the array of frequencies given. 
     
-    A Filon type algorithm using a either a piecewise cubic Hermite interpolating polynomial (pchip) or a piecewise linear polynomial, depending on the interpolation argument.
+    A Filon type algorithm using a either a piecewise cubic Hermite interpolating polynomial ([PCHIP]_) or a piecewise linear polynomial, depending on the interpolation argument.
     Optionally, an asymptotic correction term can also be computed at each end.
-    For details on implementation, see [1].
+    For details on implementation, see [N.Mounet-PhD]_.
 
     :param times: Float or 1D array of floats of length M, the time(s) [s]* to compute the fourier integral for
     :type times: ArrayLike
     :param frequencies: Float or 1D array of floats of length N, the frequencies [Hz]* the function to be transformed have been evaluated at
     :type frequencies: ArrayLike
     :param func_values: Complex or ND array of complex of shape (N, X1, X2, ...), the outputs of the function to be transformed at the frequencies given as input
     :type func_values: ArrayLike
@@ -273,25 +239,28 @@
     :param neg_inf_correction_term: True if an asymptotic correction term towards -infinity should be added, otherwise the integral is effectively truncated at the lowest (closest to -inf) frequency
     :type neg_inf_correction_term: bool
     :param interpolation: String either equal to "pchip" or "linear", to select the integration methods using PCHIP or piecewise linear interpolation, respectively.
     :type interpolation: str
     :return: The fourier integral of the input function at the input times, given as an array of shape (M, X1, X2, ...)
     :rtype: np.ndarray
     
-    * Though the units s and Hz are used here, any coherent set of time and frequency units will work
-    
-    [1] N. Mounet. The LHC Transverse Coupled-Bunch Instability, PhD thesis 5305 (EPFL, 2012)
+    \*Though the units s and Hz are used here, any coherent set of time and frequency units will work
     """
     
     assert interpolation in [mode.value for mode in InterpolationMode]
     interpolation_mode = InterpolationMode(interpolation)
     
     # Turn inputs into arrays if they are not already, switch to angular frequencies
-    omegas = 2 * np.pi * np.asarray(frequencies)
-    func_values = np.asarray(func_values)
+    # Filter out infinities and nan's
+    isfinite = np.isfinite(frequencies) & np.all(np.isfinite(func_values), axis=tuple(range(1, len(func_values.shape))))
+    if not np.all(isfinite):
+        logging.info("Removing infinite frequencies and values from arrays.")
+        
+    omegas = 2 * np.pi * np.asarray(frequencies[isfinite])
+    func_values = np.asarray(func_values[isfinite])
     times = np.asarray(times)
     
     # Set up result array, shape (M, X1, X2, ...)
     result = np.zeros((len(times), *[axis_size for axis_size in func_values.shape[1:]]), dtype=complex)
 
     # Do mode specific setup
     if interpolation_mode == InterpolationMode.PCHIP:
```

### Comparing `neffint-1.0.0/setup.py` & `neffint-1.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-# Use semantic versioning
-VERSION = "1.0.0"
+def get_version(path):
+    with path.open("rt") as f:
+        for line in f.readlines():
+            if line.startswith('__version__'):
+                delim = '"' if '"' in line else "'"
+                return line.split(delim)[1]
+        else:
+            raise RuntimeError("Unable to find version string.")
 
+# Minimum python version. Remember to also change in github workflows if increased
 PY_VERSION_REQUIRED = ">=3.7"
+
 PACKAGES_REQUIRED = {
     "core": [
         "numpy",
-        "scipy"
+        "scipy",
+    ],
+    "test": [
+        "pytest",
+    ],
+    "docs": [
+        "sphinx",
+        "sphinx-rtd-theme",
+        "nbsphinx",
+        "nbsphinx-link",
+        "ipykernel",
     ],
-    "test":[
-        "pytest"
-    ]
 }
 
-# Read README.md to use as long description in package metadata
 root_dir = Path(__file__).parent.absolute()
+
+# Read README.md to use as long description in package metadata
 with (root_dir / "README.md").open("rt") as readme_file:
     long_description = readme_file.read().strip()
 
 setup(
     name="neffint",
-    version=VERSION,
-    description="A python package for computing Fourier integrals using a Filon type method with non-equidistant grid spacing.",
+    version=get_version(root_dir / "neffint" / "_version.py"),
+    description="Python package for computing Fourier integrals using a Filon type method with non-equidistant grid spacing.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/neffint/neffint/",
     author="Eskil Vik, Nicolas Mounet",
     packages=find_packages(), # finds all the packages in the repository
     python_requires=PY_VERSION_REQUIRED,
     install_requires=PACKAGES_REQUIRED["core"],
     extras_require=PACKAGES_REQUIRED
-    )
+)
```

### Comparing `neffint-1.0.0/tests/test_fixed_grid_fourier_integral.py` & `neffint-1.1.0/tests/test_fixed_grid_fourier_integral.py`

 * *Files identical despite different names*

