# Comparing `tmp/pymc-experimental-0.0.8.tar.gz` & `tmp/pymc-experimental-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymc-experimental-0.0.8.tar", last modified: Wed Jul 12 08:10:32 2023, max compression
+gzip compressed data, was "pymc-experimental-0.0.9.tar", last modified: Fri Jul 28 05:55:01 2023, max compression
```

## Comparing `pymc-experimental-0.0.8.tar` & `pymc-experimental-0.0.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/distributions/histogram_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental/distributions/multivariate/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/distributions/multivariate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15199 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/distributions/multivariate/r2d2m2cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/distributions/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental/gp/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/gp/latent_approx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/inference/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/inference/pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/linearmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/marginal_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    25674 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental/model_transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/model_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/model_transform/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/model_transform/conditioning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/preprocessing/standard_scaler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/pymc_experimental/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/pymc_experimental/tests/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/distributions/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/distributions/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/distributions/test_discrete_markov_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/distributions/test_multivariate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/pymc_experimental/tests/model_transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/model_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/model_transform/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/model_transform/test_conditioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_histogram_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_linearmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_marginal_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_prior_from_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_splines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/pymc_experimental/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/utils/test_model_fgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/pymc_experimental/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/utils/linear_cg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/utils/model_fgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/utils/pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/utils/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/utils/pytensorf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/utils/spline.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-12 08:10:32.000000 pymc-experimental-0.0.8/pymc_experimental.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-12 08:10:32.000000 pymc-experimental-0.0.8/pymc_experimental.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:10:32.000000 pymc-experimental-0.0.8/pymc_experimental.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-12 08:10:32.000000 pymc-experimental-0.0.8/pymc_experimental.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 08:10:32.000000 pymc-experimental-0.0.8/pymc_experimental.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.369126 pymc-experimental-0.0.9/pymc_experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.373127 pymc-experimental-0.0.9/pymc_experimental/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/distributions/histogram_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.373127 pymc-experimental-0.0.9/pymc_experimental/distributions/multivariate/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/distributions/multivariate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15199 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/distributions/multivariate/r2d2m2cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/distributions/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.373127 pymc-experimental-0.0.9/pymc_experimental/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/gp/latent_approx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.373127 pymc-experimental-0.0.9/pymc_experimental/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/inference/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/inference/pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/linearmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/marginal_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26219 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.373127 pymc-experimental-0.0.9/pymc_experimental/model_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/model_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/model_transform/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/model_transform/conditioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.373127 pymc-experimental-0.0.9/pymc_experimental/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/preprocessing/standard_scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/pymc_experimental/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/pymc_experimental/tests/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/distributions/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/distributions/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/distributions/test_discrete_markov_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/distributions/test_multivariate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/pymc_experimental/tests/model_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/model_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/model_transform/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/model_transform/test_conditioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_histogram_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_linearmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_marginal_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_prior_from_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/test_splines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/pymc_experimental/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13097 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/tests/utils/test_model_fgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/pymc_experimental/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/utils/linear_cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/utils/model_fgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/utils/pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/utils/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/utils/pytensorf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/utils/spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pymc_experimental/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:55:01.373127 pymc-experimental-0.0.9/pymc_experimental.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-28 05:55:01.000000 pymc-experimental-0.0.9/pymc_experimental.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-28 05:55:01.000000 pymc-experimental-0.0.9/pymc_experimental.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 05:55:01.000000 pymc-experimental-0.0.9/pymc_experimental.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-28 05:55:01.000000 pymc-experimental-0.0.9/pymc_experimental.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 05:55:01.000000 pymc-experimental-0.0.9/pymc_experimental.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-28 05:55:01.377128 pymc-experimental-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-28 05:54:50.000000 pymc-experimental-0.0.9/setup.py
```

### Comparing `pymc-experimental-0.0.8/CODE_OF_CONDUCT.md` & `pymc-experimental-0.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/LICENSE` & `pymc-experimental-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/PKG-INFO` & `pymc-experimental-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-experimental
-Version: 0.0.8
+Version: 0.0.9
 Summary: A home for new additions to PyMC, which may include unusual probability distribitions, advanced model fitting algorithms, or any code that may be inappropriate to include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.8 Summary: A home
+Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.9 Summary: A home
 for new additions to PyMC, which may include unusual probability distribitions,
 advanced model fitting algorithms, or any code that may be inappropriate to
 include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental Maintainer: PyMC
 Developers Maintainer-email: pymc.devs@gmail.com License: Apache License,
 Version 2.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `pymc-experimental-0.0.8/README.md` & `pymc-experimental-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/__init__.py` & `pymc-experimental-0.0.9/pymc_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/distributions/__init__.py` & `pymc-experimental-0.0.9/pymc_experimental/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/distributions/continuous.py` & `pymc-experimental-0.0.9/pymc_experimental/distributions/continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/distributions/discrete.py` & `pymc-experimental-0.0.9/pymc_experimental/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/distributions/histogram_utils.py` & `pymc-experimental-0.0.9/pymc_experimental/distributions/histogram_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/distributions/multivariate/r2d2m2cp.py` & `pymc-experimental-0.0.9/pymc_experimental/distributions/multivariate/r2d2m2cp.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/distributions/timeseries.py` & `pymc-experimental-0.0.9/pymc_experimental/distributions/timeseries.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/gp/__init__.py` & `pymc-experimental-0.0.9/pymc_experimental/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/gp/latent_approx.py` & `pymc-experimental-0.0.9/pymc_experimental/gp/latent_approx.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/inference/__init__.py` & `pymc-experimental-0.0.9/pymc_experimental/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/inference/fit.py` & `pymc-experimental-0.0.9/pymc_experimental/inference/fit.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/inference/pathfinder.py` & `pymc-experimental-0.0.9/pymc_experimental/inference/pathfinder.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/linearmodel.py` & `pymc-experimental-0.0.9/pymc_experimental/linearmodel.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/marginal_model.py` & `pymc-experimental-0.0.9/pymc_experimental/marginal_model.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/model_builder.py` & `pymc-experimental-0.0.9/pymc_experimental/model_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -377,22 +377,29 @@
         if self.idata is not None and "posterior" in self.idata:
             file = Path(str(fname))
             self.idata.to_netcdf(str(file))
         else:
             raise RuntimeError("The model hasn't been fit yet, call .fit() first")
 
     @classmethod
-    def _convert_dims_to_tuple(cls, model_config: Dict) -> Dict:
+    def _model_config_formatting(cls, model_config: Dict) -> Dict:
+        """
+        Because of json serialization, model_config values that were originally tuples or numpy are being encoded as lists.
+        This function converts them back to tuples and numpy arrays to ensure correct id encoding.
+        """
         for key in model_config:
-            if (
-                isinstance(model_config[key], dict)
-                and "dims" in model_config[key]
-                and isinstance(model_config[key]["dims"], list)
-            ):
-                model_config[key]["dims"] = tuple(model_config[key]["dims"])
+            if isinstance(model_config[key], dict):
+                for sub_key in model_config[key]:
+                    if isinstance(model_config[key][sub_key], list):
+                        # Check if "dims" key to convert it to tuple
+                        if sub_key == "dims":
+                            model_config[key][sub_key] = tuple(model_config[key][sub_key])
+                        # Convert all other lists to numpy arrays
+                        else:
+                            model_config[key][sub_key] = np.array(model_config[key][sub_key])
         return model_config
 
     @classmethod
     def load(cls, fname: str):
         """
         Creates a ModelBuilder instance from a file,
         Loads inference data for the model.
@@ -416,15 +423,15 @@
         >>>     ...
         >>> name = './mymodel.nc'
         >>> imported_model = MyModel.load(name)
         """
         filepath = Path(str(fname))
         idata = az.from_netcdf(filepath)
         # needs to be converted, because json.loads was changing tuple to list
-        model_config = cls._convert_dims_to_tuple(json.loads(idata.attrs["model_config"]))
+        model_config = cls._model_config_formatting(json.loads(idata.attrs["model_config"]))
         model = cls(
             model_config=model_config,
             sampler_config=json.loads(idata.attrs["sampler_config"]),
         )
         model.idata = idata
         dataset = idata.fit_data.to_dataframe()
         X = dataset.drop(columns=[model.output_var])
```

### Comparing `pymc-experimental-0.0.8/pymc_experimental/model_transform/basic.py` & `pymc-experimental-0.0.9/pymc_experimental/model_transform/basic.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/model_transform/conditioning.py` & `pymc-experimental-0.0.9/pymc_experimental/model_transform/conditioning.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/preprocessing/standard_scaler.py` & `pymc-experimental-0.0.9/pymc_experimental/preprocessing/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/__init__.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,11 +7,7 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
-
-from numpy.testing import Tester
-
-test = Tester().test
```

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/distributions/__init__.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/distributions/test_continuous.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/distributions/test_continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/distributions/test_discrete.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/distributions/test_discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/distributions/test_discrete_markov_chain.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/distributions/test_discrete_markov_chain.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/distributions/test_multivariate.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/distributions/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/model_transform/test_basic.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/model_transform/test_basic.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/model_transform/test_conditioning.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/model_transform/test_conditioning.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/test_histogram_approximation.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/test_histogram_approximation.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/test_linearmodel.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/test_linearmodel.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/test_marginal_model.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/test_marginal_model.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/test_model_builder.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/test_model_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,28 +146,14 @@
     prediction_data = pd.DataFrame({"input": x_pred})
     pred1 = fitted_model_instance.predict(prediction_data["input"])
     pred2 = test_builder2.predict(prediction_data["input"])
     assert pred1.shape == pred2.shape
     temp.close()
 
 
-def test_convert_dims_to_tuple(fitted_model_instance):
-    model_config = {
-        "a": {
-            "loc": 0,
-            "scale": 10,
-            "dims": [
-                "x",
-            ],
-        },
-    }
-    converted_model_config = fitted_model_instance._convert_dims_to_tuple(model_config)
-    assert converted_model_config["a"]["dims"] == ("x",)
-
-
 def test_initial_build_and_fit(fitted_model_instance, check_idata=True) -> ModelBuilder:
     if check_idata:
         assert fitted_model_instance.idata is not None
         assert "posterior" in fitted_model_instance.idata.groups()
 
 
 def test_save_without_fit_raises_runtime_error():
@@ -224,14 +210,30 @@
     chains = fitted_model_instance.idata.sample_stats.dims["chain"]
     draws = fitted_model_instance.idata.sample_stats.dims["draw"]
     expected_shape = (n_pred, chains * draws) if combined else (chains, draws, n_pred)
     assert pred[fitted_model_instance.output_var].shape == expected_shape
     assert np.issubdtype(pred[fitted_model_instance.output_var].dtype, np.floating)
 
 
+def test_model_config_formatting():
+    model_config = {
+        "a": {
+            "loc": [0, 0],
+            "scale": 10,
+            "dims": [
+                "x",
+            ],
+        },
+    }
+    model_builder = test_ModelBuilder()
+    converted_model_config = model_builder._model_config_formatting(model_config)
+    np.testing.assert_equal(converted_model_config["a"]["dims"], ("x",))
+    np.testing.assert_equal(converted_model_config["a"]["loc"], np.array([0, 0]))
+
+
 def test_id():
     model_builder = test_ModelBuilder()
     expected_id = hashlib.sha256(
         str(model_builder.model_config.values()).encode()
         + model_builder.version.encode()
         + model_builder._model_type.encode()
     ).hexdigest()[:16]
```

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/test_pathfinder.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/test_pathfinder.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/test_pivoted_cholesky.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/test_pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/test_prior_from_trace.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/test_prior_from_trace.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/test_splines.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/test_splines.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/tests/utils/test_model_fgraph.py` & `pymc-experimental-0.0.9/pymc_experimental/tests/utils/test_model_fgraph.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import numpy as np
 import pymc as pm
 import pytensor.tensor as pt
 import pytest
+from pytensor import config, shared
 from pytensor.graph import Constant, FunctionGraph, node_rewriter
 from pytensor.graph.rewriting.basic import in2out
 from pytensor.tensor.exceptions import NotScalarConstantError
 
 from pymc_experimental.utils.model_fgraph import (
     ModelDeterministic,
     ModelFreeRV,
     ModelNamed,
     ModelObservedRV,
     ModelPotential,
     ModelVar,
+    clone_model,
     fgraph_from_model,
     model_deterministic,
     model_free_rv,
     model_from_fgraph,
 )
 
 
@@ -72,25 +74,30 @@
     ip = m_new.initial_point()
     np.testing.assert_equal(
         m_new.compile_logp()(ip),
         m_old.compile_logp()(ip),
     )
 
 
+def same_storage(shared_1, shared_2) -> bool:
+    """Check if two shared variables have the same storage containers (i.e., they point to the same memory)."""
+    return shared_1.container.storage is shared_2.container.storage
+
+
 @pytest.mark.parametrize("inline_views", (False, True))
 def test_data(inline_views):
-    """Test shared RNGs, MutableData, ConstantData and Dim lengths are handled correctly.
+    """Test shared RNGs, MutableData, ConstantData and dim lengths are handled correctly.
 
-    Everything should be preserved across new and old models, except for shared RNGs
+    All model-related shared variables should be copied to become independent across models.
     """
     with pm.Model(coords_mutable={"test_dim": range(3)}) as m_old:
         x = pm.MutableData("x", [0.0, 1.0, 2.0], dims=("test_dim",))
         y = pm.MutableData("y", [10.0, 11.0, 12.0], dims=("test_dim",))
-        b0 = pm.ConstantData("b0", np.zeros(3))
-        b1 = pm.Normal("b1")
+        b0 = pm.ConstantData("b0", np.zeros((1,)))
+        b1 = pm.DiracDelta("b1", 1.0)
         mu = pm.Deterministic("mu", b0 + b1 * x, dims=("test_dim",))
         obs = pm.Normal("obs", mu, sigma=1e-5, observed=y, dims=("test_dim",))
 
     m_fgraph, memo = fgraph_from_model(m_old, inlined_views=inline_views)
     assert isinstance(memo[x].owner.op, ModelNamed)
     assert isinstance(memo[y].owner.op, ModelNamed)
     assert isinstance(memo[b0].owner.op, ModelNamed)
@@ -105,30 +112,54 @@
     else:
         assert mu_inp.owner.inputs[0] is memo[b0]
         assert mu_inp.owner.inputs[1].owner.inputs[1] is memo[x]
         assert obs.owner.inputs[1] is memo[y]
 
     m_new = model_from_fgraph(m_fgraph)
 
-    # ConstantData is preserved
-    assert np.all(m_new["b0"].data == m_old["b0"].data)
-
-    # Shared non-rng shared variables are preserved
-    assert m_new["x"].container is x.container
-    assert m_new["y"].container is y.container
+    # The rv-data mapping is preserved
     assert m_new.rvs_to_values[m_new["obs"]] is m_new["y"]
 
-    # Shared rng shared variables are not preserved
-    m_new["b1"].owner.inputs[0].container is not m_old["b1"].owner.inputs[0].container
+    # ConstantData is still accessible as a model variable
+    np.testing.assert_array_equal(m_new["b0"], m_old["b0"])
 
-    with m_old:
-        pm.set_data({"x": [100.0, 200.0]}, coords={"test_dim": range(2)})
+    # Shared model variables, dim lengths, and rngs are copied and no longer point to the same memory
+    assert not same_storage(m_new["x"], x)
+    assert not same_storage(m_new["y"], y)
+    assert not same_storage(m_new["b1"].owner.inputs[0], b1.owner.inputs[0])
+    assert not same_storage(m_new.dim_lengths["test_dim"], m_old.dim_lengths["test_dim"])
 
+    # Updating model shared variables in new model, doesn't affect old one
+    with m_new:
+        pm.set_data({"x": [100.0, 200.0]}, coords={"test_dim": range(2)})
     assert m_new.dim_lengths["test_dim"].eval() == 2
-    np.testing.assert_array_almost_equal(pm.draw(m_new["x"], random_seed=63), [100.0, 200.0])
+    assert m_old.dim_lengths["test_dim"].eval() == 3
+    np.testing.assert_allclose(pm.draw(m_new["mu"]), [100.0, 200.0])
+    np.testing.assert_allclose(pm.draw(m_old["mu"]), [0.0, 1.0, 2.0], atol=1e-6)
+
+
+@config.change_flags(floatX="float64")  # Avoid downcasting Ops in the graph
+def test_shared_variable():
+    """Test that user defined shared variables (other than RNGs) aren't copied."""
+    x = shared(np.array([1, 2, 3.0]), name="x")
+    y = shared(np.array([1, 2, 3.0]), name="y")
+
+    with pm.Model() as m_old:
+        test = pm.Normal("test", mu=x, observed=y)
+
+    assert test.owner.inputs[3] is x
+    assert m_old.rvs_to_values[test] is y
+
+    m_new = clone_model(m_old)
+    test_new = m_new["test"]
+    # Shared Variables are cloned but still point to the same memory
+    assert test_new.owner.inputs[3] is not x
+    assert m_new.rvs_to_values[test_new] is not y
+    assert same_storage(test_new.owner.inputs[3], x)
+    assert same_storage(m_new.rvs_to_values[test_new], y)
 
 
 @pytest.mark.parametrize("inline_views", (False, True))
 def test_deterministics(inline_views):
     """Test handling of deterministics.
 
     We don't want Deterministics in the middle of the FunctionGraph, as they would make rewrites cumbersome
```

### Comparing `pymc-experimental-0.0.8/pymc_experimental/utils/__init__.py` & `pymc-experimental-0.0.9/pymc_experimental/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/utils/linear_cg.py` & `pymc-experimental-0.0.9/pymc_experimental/utils/linear_cg.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/utils/model_fgraph.py` & `pymc-experimental-0.0.9/pymc_experimental/utils/model_fgraph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+from copy import copy
 from typing import Dict, Optional, Sequence, Tuple
 
 import pytensor
 from pymc.logprob.transforms import RVTransform
 from pymc.model import Model
 from pymc.pytensorf import find_rng_nodes
-from pytensor import Variable
+from pytensor import Variable, shared
+from pytensor.compile import SharedVariable
 from pytensor.graph import Apply, FunctionGraph, Op, node_rewriter
 from pytensor.graph.rewriting.basic import out2in
 from pytensor.scalar import Identity
 from pytensor.tensor.elemwise import Elemwise
+from pytensor.tensor.sharedvar import ScalarSharedVariable
 
 from pymc_experimental.utils.pytensorf import StringType
 
 
 class ModelVar(Op):
     """A dummy Op that describes the purpose of a Model variable and contains
     meta-information as additional inputs (value and dims).
@@ -178,30 +181,47 @@
 
     model_vars = (
         rvs + potentials + deterministics + other_named_vars + named_value_vars + unnamed_value_vars
     )
 
     memo = {}
 
-    # Replace RNG nodes so that seeding does not interfere with old model
-    for rng in find_rng_nodes(model_vars):
-        new_rng = rng.clone()
-        new_rng.set_value(rng.get_value(borrow=False))
-        memo[rng] = new_rng
+    # Replace the following shared variables in the model:
+    # 1. RNGs
+    # 2. MutableData (could increase memory usage significantly)
+    # 3. Mutable coords dim lengths
+    shared_vars_to_copy = find_rng_nodes(model_vars)
+    shared_vars_to_copy += [v for v in model.dim_lengths.values() if isinstance(v, SharedVariable)]
+    shared_vars_to_copy += [v for v in model.named_vars.values() if isinstance(v, SharedVariable)]
+    for var in shared_vars_to_copy:
+        # FIXME: ScalarSharedVariables are converted to 0d numpy arrays internally,
+        #  so calling shared(shared(5).get_value()) returns a different type: TensorSharedVariables!
+        #  Furthermore, PyMC silently ignores mutable dim changes that are SharedTensorVariables...
+        #  https://github.com/pymc-devs/pytensor/issues/396
+        if isinstance(var, ScalarSharedVariable):
+            new_var = shared(var.get_value(borrow=False).item())
+        else:
+            new_var = shared(var.get_value(borrow=False))
+
+        assert new_var.type == var.type
+        new_var.name = var.name
+        new_var.tag = copy(var.tag)
+        # We can replace input variables by placing them in the memo
+        memo[var] = new_var
 
     fgraph = FunctionGraph(
         outputs=model_vars,
         clone=True,
         memo=memo,
         copy_orphans=True,
         copy_inputs=True,
     )
     # Copy model meta-info to fgraph
     fgraph._coords = model._coords.copy()
-    fgraph._dim_lengths = model._dim_lengths.copy()
+    fgraph._dim_lengths = {k: memo.get(v, v) for k, v in model._dim_lengths.items()}
 
     rvs_to_transforms = model.rvs_to_transforms
     named_vars_to_dims = model.named_vars_to_dims
 
     # Introduce dummy `ModelVar` Ops
     free_rvs_to_transforms = {memo[k]: tr for k, tr in rvs_to_transforms.items()}
     free_rvs_to_values = {memo[k]: memo[v] for k, v in zip(rvs, value_vars) if k in free_rvs}
```

### Comparing `pymc-experimental-0.0.8/pymc_experimental/utils/pivoted_cholesky.py` & `pymc-experimental-0.0.9/pymc_experimental/utils/pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/utils/prior.py` & `pymc-experimental-0.0.9/pymc_experimental/utils/prior.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/utils/pytensorf.py` & `pymc-experimental-0.0.9/pymc_experimental/utils/pytensorf.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental/utils/spline.py` & `pymc-experimental-0.0.9/pymc_experimental/utils/spline.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/pymc_experimental.egg-info/PKG-INFO` & `pymc-experimental-0.0.9/pymc_experimental.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-experimental
-Version: 0.0.8
+Version: 0.0.9
 Summary: A home for new additions to PyMC, which may include unusual probability distribitions, advanced model fitting algorithms, or any code that may be inappropriate to include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.8 Summary: A home
+Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.9 Summary: A home
 for new additions to PyMC, which may include unusual probability distribitions,
 advanced model fitting algorithms, or any code that may be inappropriate to
 include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental Maintainer: PyMC
 Developers Maintainer-email: pymc.devs@gmail.com License: Apache License,
 Version 2.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `pymc-experimental-0.0.8/pymc_experimental.egg-info/SOURCES.txt` & `pymc-experimental-0.0.9/pymc_experimental.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.8/setup.py` & `pymc-experimental-0.0.9/setup.py`

 * *Files identical despite different names*

