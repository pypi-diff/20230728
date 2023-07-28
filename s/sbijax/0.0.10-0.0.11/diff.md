# Comparing `tmp/sbijax-0.0.10.tar.gz` & `tmp/sbijax-0.0.11.tar.gz`

## Comparing `sbijax-0.0.10.tar` & `sbijax-0.0.11.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sbijax-0.0.10/Makefile
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 sbijax-0.0.10/examples/abc_bivariate_gaussian.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 sbijax-0.0.10/examples/bivariate_gaussian_smcabc.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 sbijax-0.0.10/examples/bivariate_gaussian_snl.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 sbijax-0.0.10/examples/bivariate_gaussian_snp.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 sbijax-0.0.10/examples/slcp_smcabc.py
--rw-r--r--   0        0        0     6114 2020-02-02 00:00:00.000000 sbijax-0.0.10/examples/slcp_snl.py
--rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 sbijax-0.0.10/examples/slcp_snl_masked_autoregressive.py
--rw-r--r--   0        0        0     6114 2020-02-02 00:00:00.000000 sbijax-0.0.10/examples/slcp_snp.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sbijax-0.0.10/sbijax/__init__.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 sbijax-0.0.10/sbijax/_sbi_base.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 sbijax-0.0.10/sbijax/_sne_base.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 sbijax-0.0.10/sbijax/generator.py
--rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 sbijax-0.0.10/sbijax/snl.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sbijax-0.0.10/sbijax/snl_test.py
--rw-r--r--   0        0        0     8958 2020-02-02 00:00:00.000000 sbijax-0.0.10/sbijax/snp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sbijax-0.0.10/sbijax/abc/__init__.py
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 sbijax-0.0.10/sbijax/abc/rejection_abc.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 sbijax-0.0.10/sbijax/abc/smc_abc.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 sbijax-0.0.10/sbijax/mcmc/__init__.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 sbijax-0.0.10/sbijax/mcmc/nuts.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 sbijax-0.0.10/sbijax/mcmc/sample.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 sbijax-0.0.10/sbijax/mcmc/slice.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 sbijax-0.0.10/.gitignore
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 sbijax-0.0.10/LICENSE
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 sbijax-0.0.10/README.md
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 sbijax-0.0.10/pyproject.toml
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 sbijax-0.0.10/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sbijax-0.0.11/Makefile
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 sbijax-0.0.11/examples/abc_bivariate_gaussian.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 sbijax-0.0.11/examples/bivariate_gaussian_smcabc.py
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 sbijax-0.0.11/examples/bivariate_gaussian_snl.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 sbijax-0.0.11/examples/bivariate_gaussian_snp.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 sbijax-0.0.11/examples/slcp_smcabc.py
+-rw-r--r--   0        0        0     6114 2020-02-02 00:00:00.000000 sbijax-0.0.11/examples/slcp_snl.py
+-rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 sbijax-0.0.11/examples/slcp_snl_masked_autoregressive.py
+-rw-r--r--   0        0        0     6114 2020-02-02 00:00:00.000000 sbijax-0.0.11/examples/slcp_snp.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sbijax-0.0.11/sbijax/__init__.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 sbijax-0.0.11/sbijax/_sbi_base.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 sbijax-0.0.11/sbijax/_sne_base.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 sbijax-0.0.11/sbijax/generator.py
+-rw-r--r--   0        0        0     8366 2020-02-02 00:00:00.000000 sbijax-0.0.11/sbijax/snl.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 sbijax-0.0.11/sbijax/snl_test.py
+-rw-r--r--   0        0        0     8958 2020-02-02 00:00:00.000000 sbijax-0.0.11/sbijax/snp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sbijax-0.0.11/sbijax/abc/__init__.py
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 sbijax-0.0.11/sbijax/abc/rejection_abc.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 sbijax-0.0.11/sbijax/abc/smc_abc.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 sbijax-0.0.11/sbijax/mcmc/__init__.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 sbijax-0.0.11/sbijax/mcmc/nuts.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 sbijax-0.0.11/sbijax/mcmc/sample.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 sbijax-0.0.11/sbijax/mcmc/slice.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 sbijax-0.0.11/.gitignore
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 sbijax-0.0.11/LICENSE
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 sbijax-0.0.11/README.md
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 sbijax-0.0.11/pyproject.toml
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 sbijax-0.0.11/PKG-INFO
```

### Comparing `sbijax-0.0.10/examples/abc_bivariate_gaussian.py` & `sbijax-0.0.11/examples/abc_bivariate_gaussian.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/examples/bivariate_gaussian_smcabc.py` & `sbijax-0.0.11/examples/bivariate_gaussian_smcabc.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/examples/bivariate_gaussian_snl.py` & `sbijax-0.0.11/examples/bivariate_gaussian_snl.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/examples/bivariate_gaussian_snp.py` & `sbijax-0.0.11/examples/bivariate_gaussian_snp.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/examples/slcp_smcabc.py` & `sbijax-0.0.11/examples/slcp_smcabc.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/examples/slcp_snl.py` & `sbijax-0.0.11/examples/slcp_snl.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/examples/slcp_snl_masked_autoregressive.py` & `sbijax-0.0.11/examples/slcp_snl_masked_autoregressive.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/examples/slcp_snp.py` & `sbijax-0.0.11/examples/slcp_snp.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/sbijax/_sbi_base.py` & `sbijax-0.0.11/sbijax/_sbi_base.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/sbijax/_sne_base.py` & `sbijax-0.0.11/sbijax/_sne_base.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/sbijax/generator.py` & `sbijax-0.0.11/sbijax/generator.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/sbijax/snl.py` & `sbijax-0.0.11/sbijax/snl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from collections import namedtuple
 from functools import partial
 
 import jax
 import numpy as np
 import optax
 from absl import logging
+
+# TODO(simon): this is a bit an annoying dependency to have
 from flax.training.early_stopping import EarlyStopping
 from jax import numpy as jnp
 
 from sbijax._sne_base import SNE
 from sbijax.mcmc import mcmc_diagnostics, sample_with_nuts, sample_with_slice
```

### Comparing `sbijax-0.0.10/sbijax/snp.py` & `sbijax-0.0.11/sbijax/snp.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/sbijax/abc/rejection_abc.py` & `sbijax-0.0.11/sbijax/abc/rejection_abc.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/sbijax/abc/smc_abc.py` & `sbijax-0.0.11/sbijax/abc/smc_abc.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/sbijax/mcmc/nuts.py` & `sbijax-0.0.11/sbijax/mcmc/nuts.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/sbijax/mcmc/sample.py` & `sbijax-0.0.11/sbijax/mcmc/sample.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/sbijax/mcmc/slice.py` & `sbijax-0.0.11/sbijax/mcmc/slice.py`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/.gitignore` & `sbijax-0.0.11/.gitignore`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/LICENSE` & `sbijax-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/README.md` & `sbijax-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `sbijax-0.0.10/pyproject.toml` & `sbijax-0.0.11/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -21,21 +21,24 @@
 requires-python = ">=3.8"
 dependencies = [
     "blackjax-nightly>=0.9.6.post127",
     "distrax>=0.1.2",
     "dm-haiku>=0.0.9",
     "flax>=0.6.3",
     "optax>=0.1.3",
-    "surkectors==0.2.2",
+    "surjectors>=0.2.2",
 ]
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://github.com/dirmeier/sbijax"
 
+[tool.hatch.metadata]
+allow-direct-references = true
+
 [tool.hatch.version]
 path = "sbijax/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
     "/.github",
     "./gitignore",
@@ -47,15 +50,15 @@
     "pylint>=2.15.10",
     "pytest>=7.2.0",
     "pytest-cov>=4.0.0"
 ]
 
 [tool.hatch.envs.test.scripts]
 lint = 'pylint sbijax'
-test = 'pytest -v --doctest-modules --cov=./sbi --cov-report=xml sbijax'
+test = 'pytest -v --doctest-modules --cov=./sbijax --cov-report=xml sbijax'
 
 
 [tool.black]
 line-length = 80
 extend-ignore = "E203"
 target-version = ['py39']
 exclude = '''
```

### Comparing `sbijax-0.0.10/PKG-INFO` & `sbijax-0.0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbijax
-Version: 0.0.10
+Version: 0.0.11
 Summary:  Simulation-based inference in JAX
 Project-URL: homepage, https://github.com/dirmeier/sbijax
 Author-email: Simon Dirmeier <sfyrbnd@pm.me>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: abc,approximate Bayesian computation,normalizing flows,simulation-based inference,smc-abc
 Classifier: Development Status :: 1 - Planning
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Requires-Dist: blackjax-nightly>=0.9.6.post127
 Requires-Dist: distrax>=0.1.2
 Requires-Dist: dm-haiku>=0.0.9
 Requires-Dist: flax>=0.6.3
 Requires-Dist: optax>=0.1.3
-Requires-Dist: surkectors==0.2.2
+Requires-Dist: surjectors>=0.2.2
 Description-Content-Type: text/markdown
 
 # sbijax
 
 [![status](http://www.repostatus.org/badges/latest/concept.svg)](http://www.repostatus.org/#concept)
 [![ci](https://github.com/dirmeier/sbijax/actions/workflows/ci.yaml/badge.svg)](https://github.com/dirmeier/sbijax/actions/workflows/ci.yaml)
 [![version](https://img.shields.io/pypi/v/sbijax.svg?colorB=black&style=flat)](https://pypi.org/project/sbijax/)
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: sbijax Version: 0.0.10 Summary: Simulation-based
+Metadata-Version: 2.1 Name: sbijax Version: 0.0.11 Summary: Simulation-based
 inference in JAX Project-URL: homepage, https://github.com/dirmeier/sbijax
 Author-email: Simon Dirmeier
 pm.me> License-Expression: Apache-2.0 License-File: LICENSE Keywords:
 abc,approximate Bayesian computation,normalizing flows,simulation-based
 inference,smc-abc Classifier: Development Status :: 1 - Planning Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Requires-Python: >=3.8 Requires-Dist: blackjax-
 nightly>=0.9.6.post127 Requires-Dist: distrax>=0.1.2 Requires-Dist: dm-
 haiku>=0.0.9 Requires-Dist: flax>=0.6.3 Requires-Dist: optax>=0.1.3 Requires-
-Dist: surkectors==0.2.2 Description-Content-Type: text/markdown # sbijax [!
+Dist: surjectors>=0.2.2 Description-Content-Type: text/markdown # sbijax [!
 [status](http://www.repostatus.org/badges/latest/concept.svg)](http://
 www.repostatus.org/#concept) [![ci](https://github.com/dirmeier/sbijax/actions/
 workflows/ci.yaml/badge.svg)](https://github.com/dirmeier/sbijax/actions/
 workflows/ci.yaml) [![version](https://img.shields.io/pypi/v/
 sbijax.svg?colorB=black&style=flat)](https://pypi.org/project/sbijax/) >
 Simulation-based inference in JAX ## About SbiJAX implements several algorithms
 for simulation-based inference using [JAX](https://github.com/google/jax),
```

