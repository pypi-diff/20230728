# Comparing `tmp/surjectors-0.2.3.tar.gz` & `tmp/surjectors-0.2.4.tar.gz`

## Comparing `surjectors-0.2.3.tar` & `surjectors-0.2.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 surjectors-0.2.3/Makefile
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 surjectors-0.2.3/examples/autoregressive_inference_surjection.py
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 surjectors-0.2.3/examples/conditional_density_estimation.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 surjectors-0.2.3/examples/coupling_inference_surjection.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/__init__.py
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/bijectors/__init__.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/bijectors/_bijector.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/bijectors/lu_linear.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/bijectors/masked_autoregressive.py
--rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/bijectors/masked_autoregressive_test.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/bijectors/masked_coupling.py
--rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/bijectors/masked_coupling_test.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/bijectors/permutation.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/conditioners/__init__.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/conditioners/mlp.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/conditioners/transformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/conditioners/nn/__init__.py
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/conditioners/nn/made.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/conditioners/nn/made_test.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/conditioners/nn/masked_linear.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/distributions/__init__.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/distributions/transformed_distribution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/__init__.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/_transform.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/affine_masked_autoregressive_inference_funnel.py
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/affine_masked_autoregressive_inference_funnel_test.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/affine_masked_coupling_generative_funnel.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/affine_masked_coupling_inference_funnel.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/affine_masked_coupling_inference_funnel_test.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/augment.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/chain.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/funnel.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/masked_coupling_inference_funnel.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/mlp.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/rq_masked_autoregressive_inference_funnel.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/rq_masked_coupling_inference_funnel.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/rq_masked_coupling_inference_funnel_test.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/slice.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/surjector.py
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 surjectors-0.2.3/surjectors/surjectors/surjectors_test.py
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 surjectors-0.2.3/.gitignore
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 surjectors-0.2.3/LICENSE
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 surjectors-0.2.3/README.md
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 surjectors-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 surjectors-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 surjectors-0.2.4/Makefile
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 surjectors-0.2.4/examples/autoregressive_inference_surjection.py
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 surjectors-0.2.4/examples/conditional_density_estimation.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 surjectors-0.2.4/examples/coupling_inference_surjection.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/__init__.py
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/bijectors/__init__.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/bijectors/_bijector.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/bijectors/lu_linear.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/bijectors/masked_autoregressive.py
+-rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/bijectors/masked_autoregressive_test.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/bijectors/masked_coupling.py
+-rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/bijectors/masked_coupling_test.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/bijectors/permutation.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/conditioners/__init__.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/conditioners/mlp.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/conditioners/transformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/conditioners/nn/__init__.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/conditioners/nn/made.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/conditioners/nn/made_test.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/conditioners/nn/masked_linear.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/distributions/__init__.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/distributions/transformed_distribution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/__init__.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/_transform.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/affine_masked_autoregressive_inference_funnel.py
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/affine_masked_autoregressive_inference_funnel_test.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/affine_masked_coupling_generative_funnel.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/affine_masked_coupling_inference_funnel.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/affine_masked_coupling_inference_funnel_test.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/augment.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/chain.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/funnel.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/masked_coupling_inference_funnel.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/mlp.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/rq_masked_autoregressive_inference_funnel.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/rq_masked_coupling_inference_funnel.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/rq_masked_coupling_inference_funnel_test.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/slice.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/surjector.py
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 surjectors-0.2.4/surjectors/surjectors/surjectors_test.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 surjectors-0.2.4/.gitignore
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 surjectors-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 surjectors-0.2.4/README.md
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 surjectors-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 surjectors-0.2.4/PKG-INFO
```

### Comparing `surjectors-0.2.3/examples/autoregressive_inference_surjection.py` & `surjectors-0.2.4/examples/autoregressive_inference_surjection.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/examples/conditional_density_estimation.py` & `surjectors-0.2.4/examples/conditional_density_estimation.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/examples/coupling_inference_surjection.py` & `surjectors-0.2.4/examples/coupling_inference_surjection.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/__init__.py` & `surjectors-0.2.4/surjectors/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 surjectors: Surjection layers for density estimation with normalizing flows
 """
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 from surjectors.bijectors.lu_linear import LULinear
 from surjectors.bijectors.masked_autoregressive import MaskedAutoregressive
 from surjectors.bijectors.masked_coupling import MaskedCoupling
 from surjectors.bijectors.permutation import Permutation
 from surjectors.distributions.transformed_distribution import (
     TransformedDistribution,
```

### Comparing `surjectors-0.2.3/surjectors/util.py` & `surjectors-0.2.4/surjectors/util.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/bijectors/_bijector.py` & `surjectors-0.2.4/surjectors/bijectors/_bijector.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/bijectors/lu_linear.py` & `surjectors-0.2.4/surjectors/bijectors/lu_linear.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/bijectors/masked_autoregressive.py` & `surjectors-0.2.4/surjectors/bijectors/masked_autoregressive.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/bijectors/masked_autoregressive_test.py` & `surjectors-0.2.4/surjectors/bijectors/masked_autoregressive_test.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/bijectors/masked_coupling.py` & `surjectors-0.2.4/surjectors/bijectors/masked_coupling.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/bijectors/masked_coupling_test.py` & `surjectors-0.2.4/surjectors/bijectors/masked_coupling_test.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/bijectors/permutation.py` & `surjectors-0.2.4/surjectors/bijectors/permutation.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/conditioners/transformer.py` & `surjectors-0.2.4/surjectors/conditioners/transformer.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/conditioners/nn/made.py` & `surjectors-0.2.4/surjectors/conditioners/nn/made.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/conditioners/nn/made_test.py` & `surjectors-0.2.4/surjectors/conditioners/nn/made_test.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/conditioners/nn/masked_linear.py` & `surjectors-0.2.4/surjectors/conditioners/nn/masked_linear.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/distributions/transformed_distribution.py` & `surjectors-0.2.4/surjectors/distributions/transformed_distribution.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/_transform.py` & `surjectors-0.2.4/surjectors/surjectors/_transform.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/affine_masked_autoregressive_inference_funnel.py` & `surjectors-0.2.4/surjectors/surjectors/affine_masked_autoregressive_inference_funnel.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/affine_masked_autoregressive_inference_funnel_test.py` & `surjectors-0.2.4/surjectors/surjectors/affine_masked_autoregressive_inference_funnel_test.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/affine_masked_coupling_generative_funnel.py` & `surjectors-0.2.4/surjectors/surjectors/affine_masked_coupling_generative_funnel.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/affine_masked_coupling_inference_funnel.py` & `surjectors-0.2.4/surjectors/surjectors/affine_masked_coupling_inference_funnel.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/affine_masked_coupling_inference_funnel_test.py` & `surjectors-0.2.4/surjectors/surjectors/affine_masked_coupling_inference_funnel_test.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/augment.py` & `surjectors-0.2.4/surjectors/surjectors/augment.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/chain.py` & `surjectors-0.2.4/surjectors/surjectors/chain.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/masked_coupling_inference_funnel.py` & `surjectors-0.2.4/surjectors/surjectors/masked_coupling_inference_funnel.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/mlp.py` & `surjectors-0.2.4/surjectors/surjectors/mlp.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/rq_masked_autoregressive_inference_funnel.py` & `surjectors-0.2.4/surjectors/surjectors/rq_masked_autoregressive_inference_funnel.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/rq_masked_coupling_inference_funnel.py` & `surjectors-0.2.4/surjectors/surjectors/rq_masked_coupling_inference_funnel.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/rq_masked_coupling_inference_funnel_test.py` & `surjectors-0.2.4/surjectors/surjectors/rq_masked_coupling_inference_funnel_test.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/slice.py` & `surjectors-0.2.4/surjectors/surjectors/slice.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/surjector.py` & `surjectors-0.2.4/surjectors/surjectors/surjector.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/surjectors/surjectors/surjectors_test.py` & `surjectors-0.2.4/surjectors/surjectors/surjectors_test.py`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/.gitignore` & `surjectors-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/LICENSE` & `surjectors-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/README.md` & `surjectors-0.2.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # surjectors
 
 [![status](http://www.repostatus.org/badges/latest/concept.svg)](http://www.repostatus.org/#concept)
 [![ci](https://github.com/dirmeier/surjectors/actions/workflows/ci.yaml/badge.svg)](https://github.com/dirmeier/surjectors/actions/workflows/ci.yaml)
+[![version](https://img.shields.io/pypi/v/surjectors.svg?colorB=black&style=flat)](https://pypi.org/project/surjectors/)
 
 > Surjection layers for density estimation with normalizing flows
 
 ## About
 
 Surjectors is a light-weight library of inference and generative surjection layers, i.e., layers that reduce or increase dimensionality, for density estimation using normalizing flows.
 Surjectors builds on Distrax and Haiku and is fully compatible with both of them.
@@ -15,15 +16,19 @@
 You can find several self-contained examples on how to use the algorithms in `examples`.
 
 ## Installation
 
 Make sure to have a working `JAX` installation. Depending whether you want to use CPU/GPU/TPU,
 please follow [these instructions](https://github.com/google/jax#installation).
 
-You can install
+To install the package from PyPI, call:
+
+```bash
+pip install surjectors
+```
 
 To install the latest GitHub <RELEASE>, just call the following on the command line:
 
 ```bash
 pip install git+https://github.com/dirmeier/surjectors@<RELEASE>
 ```
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
 # surjectors [![status](http://www.repostatus.org/badges/latest/concept.svg)]
 (http://www.repostatus.org/#concept) [![ci](https://github.com/dirmeier/
 surjectors/actions/workflows/ci.yaml/badge.svg)](https://github.com/dirmeier/
-surjectors/actions/workflows/ci.yaml) > Surjection layers for density
-estimation with normalizing flows ## About Surjectors is a light-weight library
-of inference and generative surjection layers, i.e., layers that reduce or
-increase dimensionality, for density estimation using normalizing flows.
-Surjectors builds on Distrax and Haiku and is fully compatible with both of
-them. ## Examples You can find several self-contained examples on how to use
-the algorithms in `examples`. ## Installation Make sure to have a working `JAX`
-installation. Depending whether you want to use CPU/GPU/TPU, please follow
-[these instructions](https://github.com/google/jax#installation). You can
-install To install the latest GitHub , just call the following on the command
-line: ```bash pip install git+https://github.com/dirmeier/surjectors@ ``` ##
-Author Simon Dirmeier sfyrbnd_@_pm_me
+surjectors/actions/workflows/ci.yaml) [![version](https://img.shields.io/pypi/
+v/surjectors.svg?colorB=black&style=flat)](https://pypi.org/project/surjectors/
+) > Surjection layers for density estimation with normalizing flows ## About
+Surjectors is a light-weight library of inference and generative surjection
+layers, i.e., layers that reduce or increase dimensionality, for density
+estimation using normalizing flows. Surjectors builds on Distrax and Haiku and
+is fully compatible with both of them. ## Examples You can find several self-
+contained examples on how to use the algorithms in `examples`. ## Installation
+Make sure to have a working `JAX` installation. Depending whether you want to
+use CPU/GPU/TPU, please follow [these instructions](https://github.com/google/
+jax#installation). To install the package from PyPI, call: ```bash pip install
+surjectors ``` To install the latest GitHub , just call the following on the
+command line: ```bash pip install git+https://github.com/dirmeier/surjectors@
+``` ## Author Simon Dirmeier sfyrbnd_@_pm_me
```

### Comparing `surjectors-0.2.3/pyproject.toml` & `surjectors-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `surjectors-0.2.3/PKG-INFO` & `surjectors-0.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surjectors
-Version: 0.2.3
+Version: 0.2.4
 Summary: Surjection layers for density estimation with normalizing flows
 Project-URL: homepage, https://github.com/dirmeier/surjectors
 Author-email: Simon Dirmeier <sfyrbnd@pm.me>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: density estimation,normalizing flows,surjections
 Classifier: Development Status :: 1 - Planning
@@ -19,14 +19,15 @@
 Requires-Dist: optax>=0.1.3
 Description-Content-Type: text/markdown
 
 # surjectors
 
 [![status](http://www.repostatus.org/badges/latest/concept.svg)](http://www.repostatus.org/#concept)
 [![ci](https://github.com/dirmeier/surjectors/actions/workflows/ci.yaml/badge.svg)](https://github.com/dirmeier/surjectors/actions/workflows/ci.yaml)
+[![version](https://img.shields.io/pypi/v/surjectors.svg?colorB=black&style=flat)](https://pypi.org/project/surjectors/)
 
 > Surjection layers for density estimation with normalizing flows
 
 ## About
 
 Surjectors is a light-weight library of inference and generative surjection layers, i.e., layers that reduce or increase dimensionality, for density estimation using normalizing flows.
 Surjectors builds on Distrax and Haiku and is fully compatible with both of them.
@@ -36,15 +37,19 @@
 You can find several self-contained examples on how to use the algorithms in `examples`.
 
 ## Installation
 
 Make sure to have a working `JAX` installation. Depending whether you want to use CPU/GPU/TPU,
 please follow [these instructions](https://github.com/google/jax#installation).
 
-You can install
+To install the package from PyPI, call:
+
+```bash
+pip install surjectors
+```
 
 To install the latest GitHub <RELEASE>, just call the following on the command line:
 
 ```bash
 pip install git+https://github.com/dirmeier/surjectors@<RELEASE>
 ```
```

#### html2text {}

```diff
@@ -1,26 +1,28 @@
-Metadata-Version: 2.1 Name: surjectors Version: 0.2.3 Summary: Surjection
+Metadata-Version: 2.1 Name: surjectors Version: 0.2.4 Summary: Surjection
 layers for density estimation with normalizing flows Project-URL: homepage,
 https://github.com/dirmeier/surjectors Author-email: Simon Dirmeier
 pm.me> License-Expression: Apache-2.0 License-File: LICENSE Keywords: density
 estimation,normalizing flows,surjections Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Requires-Python: >=3.8 Requires-Dist:
 distrax>=0.1.2 Requires-Dist: dm-haiku>=0.0.9 Requires-Dist: optax>=0.1.3
 Description-Content-Type: text/markdown # surjectors [![status](http://
 www.repostatus.org/badges/latest/concept.svg)](http://www.repostatus.org/
 #concept) [![ci](https://github.com/dirmeier/surjectors/actions/workflows/
 ci.yaml/badge.svg)](https://github.com/dirmeier/surjectors/actions/workflows/
-ci.yaml) > Surjection layers for density estimation with normalizing flows ##
-About Surjectors is a light-weight library of inference and generative
-surjection layers, i.e., layers that reduce or increase dimensionality, for
-density estimation using normalizing flows. Surjectors builds on Distrax and
-Haiku and is fully compatible with both of them. ## Examples You can find
-several self-contained examples on how to use the algorithms in `examples`. ##
-Installation Make sure to have a working `JAX` installation. Depending whether
-you want to use CPU/GPU/TPU, please follow [these instructions](https://
-github.com/google/jax#installation). You can install To install the latest
-GitHub , just call the following on the command line: ```bash pip install
-git+https://github.com/dirmeier/surjectors@ ``` ## Author Simon Dirmeier
-sfyrbnd_@_pm_me
+ci.yaml) [![version](https://img.shields.io/pypi/v/
+surjectors.svg?colorB=black&style=flat)](https://pypi.org/project/surjectors/
+) > Surjection layers for density estimation with normalizing flows ## About
+Surjectors is a light-weight library of inference and generative surjection
+layers, i.e., layers that reduce or increase dimensionality, for density
+estimation using normalizing flows. Surjectors builds on Distrax and Haiku and
+is fully compatible with both of them. ## Examples You can find several self-
+contained examples on how to use the algorithms in `examples`. ## Installation
+Make sure to have a working `JAX` installation. Depending whether you want to
+use CPU/GPU/TPU, please follow [these instructions](https://github.com/google/
+jax#installation). To install the package from PyPI, call: ```bash pip install
+surjectors ``` To install the latest GitHub , just call the following on the
+command line: ```bash pip install git+https://github.com/dirmeier/surjectors@
+``` ## Author Simon Dirmeier sfyrbnd_@_pm_me
```

