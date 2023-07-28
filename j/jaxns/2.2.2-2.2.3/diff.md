# Comparing `tmp/jaxns-2.2.2.tar.gz` & `tmp/jaxns-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxns-2.2.2.tar", last modified: Fri Jul 28 16:51:29 2023, max compression
+gzip compressed data, was "jaxns-2.2.3.tar", last modified: Fri Jul 28 17:34:10 2023, max compression
```

## Comparing `jaxns-2.2.2.tar` & `jaxns-2.2.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.612375 jaxns-2.2.2/
--rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-07-28 03:56:53.000000 jaxns-2.2.2/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     5150 2023-07-28 16:51:29.612375 jaxns-2.2.2/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     4711 2023-07-28 16:50:15.000000 jaxns-2.2.2/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.608375 jaxns-2.2.2/jaxns/
--rw-rw-r--   0 albert    (1000) albert    (1000)      581 2023-07-28 03:56:53.000000 jaxns-2.2.2/jaxns/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    13249 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/adaptive_refinement.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     6940 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/initial_state.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.612375 jaxns-2.2.2/jaxns/internals/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      849 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/linalg.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12651 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/log_semiring.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4919 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/maps.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/shapes.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1853 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/stats.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.612375 jaxns-2.2.2/jaxns/internals/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      277 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/tests/test_linalg.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5490 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/tests/test_log_semiring.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2898 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/tests/test_maps.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1110 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/tests/test_shapes.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1186 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/tests/test_stats.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.612375 jaxns-2.2.2/jaxns/likelihood_samplers/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/likelihood_samplers/__init__.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.612375 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:53.000000 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3192 2023-07-28 03:56:53.000000 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/em_gmm.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    29797 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/multi_ellipsoid_utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.612375 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:53.000000 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1320 2023-07-28 03:56:53.000000 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_em_gmm.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5263 2023-07-28 03:56:53.000000 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3103 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/model.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4425 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/multi_ellipsoidal_samplers.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    18526 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/nested_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    16165 2023-07-28 03:56:53.000000 jaxns-2.2.2/jaxns/plotting.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12554 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/prior.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2787 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/random.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    26263 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/slice_samplers.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    10153 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/special_priors.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    16335 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/static_nested_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    18919 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/statistics.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     6607 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/termination.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.612375 jaxns-2.2.2/jaxns/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3884 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/tests/test_initial_state.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    18625 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/tests/test_nested_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9019 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/tests/test_prior.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1306 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/tests/test_random.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    24211 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/tests/test_statistics.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      477 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/tests/test_utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5118 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/types.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5122 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/uniform_samplers.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    17668 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      716 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/warnings.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.608375 jaxns-2.2.2/jaxns.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     5150 2023-07-28 16:51:29.000000 jaxns-2.2.2/jaxns.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     1633 2023-07-28 16:51:29.000000 jaxns-2.2.2/jaxns.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-28 16:51:29.000000 jaxns-2.2.2/jaxns.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        6 2023-07-28 16:51:29.000000 jaxns-2.2.2/jaxns.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-07-28 03:56:05.000000 jaxns-2.2.2/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-07-28 16:51:29.612375 jaxns-2.2.2/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)      949 2023-07-28 16:50:40.000000 jaxns-2.2.2/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 17:34:10.952447 jaxns-2.2.3/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-07-28 03:56:53.000000 jaxns-2.2.3/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5025 2023-07-28 17:34:10.952447 jaxns-2.2.3/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4586 2023-07-28 17:25:38.000000 jaxns-2.2.3/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 17:34:10.952447 jaxns-2.2.3/jaxns/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      581 2023-07-28 03:56:53.000000 jaxns-2.2.3/jaxns/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    13249 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/adaptive_refinement.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6940 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/initial_state.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 17:34:10.952447 jaxns-2.2.3/jaxns/internals/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/internals/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      849 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/internals/linalg.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    12651 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/internals/log_semiring.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4919 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/internals/maps.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/internals/shapes.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1853 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/internals/stats.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 17:34:10.952447 jaxns-2.2.3/jaxns/internals/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/internals/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      277 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/internals/tests/test_linalg.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5490 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/internals/tests/test_log_semiring.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2898 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/internals/tests/test_maps.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1110 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/internals/tests/test_shapes.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1186 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/internals/tests/test_stats.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 17:34:10.952447 jaxns-2.2.3/jaxns/likelihood_samplers/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/likelihood_samplers/__init__.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 17:34:10.952447 jaxns-2.2.3/jaxns/likelihood_samplers/multi_ellipsoid/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:53.000000 jaxns-2.2.3/jaxns/likelihood_samplers/multi_ellipsoid/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3192 2023-07-28 03:56:53.000000 jaxns-2.2.3/jaxns/likelihood_samplers/multi_ellipsoid/em_gmm.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    29797 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/likelihood_samplers/multi_ellipsoid/multi_ellipsoid_utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 17:34:10.952447 jaxns-2.2.3/jaxns/likelihood_samplers/multi_ellipsoid/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:53.000000 jaxns-2.2.3/jaxns/likelihood_samplers/multi_ellipsoid/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1320 2023-07-28 03:56:53.000000 jaxns-2.2.3/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_em_gmm.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5263 2023-07-28 03:56:53.000000 jaxns-2.2.3/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3103 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/model.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4425 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/multi_ellipsoidal_samplers.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    18526 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    16165 2023-07-28 03:56:53.000000 jaxns-2.2.3/jaxns/plotting.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    12502 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/prior.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2787 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/random.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    26263 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/slice_samplers.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    10153 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/special_priors.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    16335 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/static_nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    18919 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/statistics.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6607 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/termination.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 17:34:10.952447 jaxns-2.2.3/jaxns/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3884 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/tests/test_initial_state.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    18625 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/tests/test_nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     9324 2023-07-28 16:52:54.000000 jaxns-2.2.3/jaxns/tests/test_prior.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1306 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/tests/test_random.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    24211 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/tests/test_statistics.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      477 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/tests/test_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5118 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/types.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5122 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/uniform_samplers.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    17668 2023-07-28 17:03:24.000000 jaxns-2.2.3/jaxns/utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      716 2023-07-28 03:56:05.000000 jaxns-2.2.3/jaxns/warnings.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 17:34:10.952447 jaxns-2.2.3/jaxns.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5025 2023-07-28 17:34:10.000000 jaxns-2.2.3/jaxns.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1633 2023-07-28 17:34:10.000000 jaxns-2.2.3/jaxns.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-28 17:34:10.000000 jaxns-2.2.3/jaxns.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        6 2023-07-28 17:34:10.000000 jaxns-2.2.3/jaxns.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-07-28 03:56:05.000000 jaxns-2.2.3/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-07-28 17:34:10.952447 jaxns-2.2.3/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)      971 2023-07-28 17:22:26.000000 jaxns-2.2.3/setup.py
```

### Comparing `jaxns-2.2.2/LICENSE` & `jaxns-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/PKG-INFO` & `jaxns-2.2.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,15 @@
-Metadata-Version: 2.1
-Name: jaxns
-Version: 2.2.2
-Summary: Nested Sampling in JAX
-Home-page: https://github.com/joshuaalbert/jaxns
-Author: Joshua G. Albert
-Author-email: albert@strw.leidenuniv.nl
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Python](https://img.shields.io/pypi/pyversions/jaxns.svg)](https://badge.fury.io/py/jaxns)
 [![PyPI](https://badge.fury.io/py/jaxns.svg)](https://badge.fury.io/py/jaxns)
-[![Documentation Status](https://readthedocs.org/projects/jaxns/badge/?version=latest)](https://jaxns.readthedocs.io/en/latest/?badge=latest)
-
 
 Main
-Status: ![Workflow name](https://github.com/JoshuaAlbert/jaxns/actions/workflows/unittests.yml/badge.svg?branch=main)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=main)
 
 Develop
-Status: ![Workflow name](https://github.com/JoshuaAlbert/jaxns/actions/workflows/unittests.yml/badge.svg?branch=develop)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 ![JAXNS](https://github.com/Joshuaalbert/jaxns/raw/main/jaxns_logo.png)
 
 ## Mission: _To make nested sampling **faster, easier, and more powerful**_
 
 # What is it?
 
@@ -100,15 +84,15 @@
 improvement in speed on cheap likelihood evaluations.
 This is shown in (https://arxiv.org/abs/2012.15286). With regards to how efficiently JAXNS used likelihood evaluations,
 JAXNS prizes exactness over efficiency, however since it employs an adaptive strategy, users can control efficiency by
 controlling some precision parameters.
 
 # Change Log
 
-28 July, 2023 -- JAXNS 2.2.2 released. Bug fix for singular priors.
+28 July, 2023 -- JAXNS 2.2.3 released. Bug fix for singular priors.
 
 26 June, 2023 -- JAXNS 2.2.1 released. Multi-ellipsoidal sampler added back in. Adaptive refinement disabled, as a bias
 has been detected in it.
 
 15 June, 2023 -- JAXNS 2.2.0 released. Added support to allow TFP bijectors to defined transformed distributions. Other
 minor improvements.
```

### Comparing `jaxns-2.2.2/README.md` & `jaxns-2.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,29 @@
+Metadata-Version: 2.1
+Name: jaxns
+Version: 2.2.3
+Summary: Nested Sampling in JAX
+Home-page: https://github.com/joshuaalbert/jaxns
+Author: Joshua G. Albert
+Author-email: albert@strw.leidenuniv.nl
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Python](https://img.shields.io/pypi/pyversions/jaxns.svg)](https://badge.fury.io/py/jaxns)
 [![PyPI](https://badge.fury.io/py/jaxns.svg)](https://badge.fury.io/py/jaxns)
-[![Documentation Status](https://readthedocs.org/projects/jaxns/badge/?version=latest)](https://jaxns.readthedocs.io/en/latest/?badge=latest)
-
 
 Main
-Status: ![Workflow name](https://github.com/JoshuaAlbert/jaxns/actions/workflows/unittests.yml/badge.svg?branch=main)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=main)
 
 Develop
-Status: ![Workflow name](https://github.com/JoshuaAlbert/jaxns/actions/workflows/unittests.yml/badge.svg?branch=develop)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 ![JAXNS](https://github.com/Joshuaalbert/jaxns/raw/main/jaxns_logo.png)
 
 ## Mission: _To make nested sampling **faster, easier, and more powerful**_
 
 # What is it?
 
@@ -86,15 +98,15 @@
 improvement in speed on cheap likelihood evaluations.
 This is shown in (https://arxiv.org/abs/2012.15286). With regards to how efficiently JAXNS used likelihood evaluations,
 JAXNS prizes exactness over efficiency, however since it employs an adaptive strategy, users can control efficiency by
 controlling some precision parameters.
 
 # Change Log
 
-28 July, 2023 -- JAXNS 2.2.2 released. Bug fix for singular priors.
+28 July, 2023 -- JAXNS 2.2.3 released. Bug fix for singular priors.
 
 26 June, 2023 -- JAXNS 2.2.1 released. Multi-ellipsoidal sampler added back in. Adaptive refinement disabled, as a bias
 has been detected in it.
 
 15 June, 2023 -- JAXNS 2.2.0 released. Added support to allow TFP bijectors to defined transformed distributions. Other
 minor improvements.
```

### Comparing `jaxns-2.2.2/jaxns/__init__.py` & `jaxns-2.2.3/jaxns/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/adaptive_refinement.py` & `jaxns-2.2.3/jaxns/adaptive_refinement.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/initial_state.py` & `jaxns-2.2.3/jaxns/initial_state.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/internals/linalg.py` & `jaxns-2.2.3/jaxns/internals/linalg.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/internals/log_semiring.py` & `jaxns-2.2.3/jaxns/internals/log_semiring.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/internals/maps.py` & `jaxns-2.2.3/jaxns/internals/maps.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/internals/shapes.py` & `jaxns-2.2.3/jaxns/internals/shapes.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/internals/stats.py` & `jaxns-2.2.3/jaxns/internals/stats.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/internals/tests/test_log_semiring.py` & `jaxns-2.2.3/jaxns/internals/tests/test_log_semiring.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/internals/tests/test_maps.py` & `jaxns-2.2.3/jaxns/internals/tests/test_maps.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/internals/tests/test_shapes.py` & `jaxns-2.2.3/jaxns/internals/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/internals/tests/test_stats.py` & `jaxns-2.2.3/jaxns/internals/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/em_gmm.py` & `jaxns-2.2.3/jaxns/likelihood_samplers/multi_ellipsoid/em_gmm.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/multi_ellipsoid_utils.py` & `jaxns-2.2.3/jaxns/likelihood_samplers/multi_ellipsoid/multi_ellipsoid_utils.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_em_gmm.py` & `jaxns-2.2.3/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_em_gmm.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py` & `jaxns-2.2.3/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/model.py` & `jaxns-2.2.3/jaxns/model.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/multi_ellipsoidal_samplers.py` & `jaxns-2.2.3/jaxns/multi_ellipsoidal_samplers.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/nested_sampler.py` & `jaxns-2.2.3/jaxns/nested_sampler.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/plotting.py` & `jaxns-2.2.3/jaxns/plotting.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/prior.py` & `jaxns-2.2.3/jaxns/prior.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,16 +201,15 @@
 
 class Prior(AbstractPrior):
     def __init__(self, dist_or_value: Union[tfpd.Distribution, jnp.ndarray], name: Optional[str] = None):
         super(Prior, self).__init__(name=name)
         if isinstance(dist_or_value, tfpd.Distribution):
             self._type = 'dist'
             self._dist = Distribution(dist_or_value)
-
-        elif isinstance(dist_or_value, (jnp.ndarray, np.ndarray)):
+        else:
             self._type = 'value'
             self._value = jnp.asarray(dist_or_value)
         self.name = name
 
     @property
     def dist(self) -> Distribution:
         if self._type != 'dist':
@@ -221,15 +220,15 @@
     def value(self) -> jnp.ndarray:
         if self._type != 'value':
             raise ValueError(f"Wrong type, got {self._type}")
         return self._value
 
     def _base_shape(self) -> Tuple[int, ...]:
         if self._type == 'value':
-            return ()
+            return (0,)
         elif self._type == 'dist':
             return self.dist.base_shape
         else:
             raise NotImplementedError()
 
     def _shape(self) -> Tuple[int, ...]:
         if self._type == 'value':
```

### Comparing `jaxns-2.2.2/jaxns/random.py` & `jaxns-2.2.3/jaxns/random.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/slice_samplers.py` & `jaxns-2.2.3/jaxns/slice_samplers.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/special_priors.py` & `jaxns-2.2.3/jaxns/special_priors.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/static_nested_sampler.py` & `jaxns-2.2.3/jaxns/static_nested_sampler.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/statistics.py` & `jaxns-2.2.3/jaxns/statistics.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/termination.py` & `jaxns-2.2.3/jaxns/termination.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/tests/test_initial_state.py` & `jaxns-2.2.3/jaxns/tests/test_initial_state.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/tests/test_nested_sampler.py` & `jaxns-2.2.3/jaxns/tests/test_nested_sampler.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/tests/test_prior.py` & `jaxns-2.2.3/jaxns/tests/test_prior.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 
 import tensorflow_probability.substrates.jax as tfp
 from jax import random, numpy as jnp, vmap
 
+from jaxns.model import Model
 from jaxns.prior import PriorModelGen, Prior, parse_prior, compute_log_likelihood, InvalidDistribution, \
     InvalidPriorName, prepare_input, distribution_chain
 from jaxns.special_priors import Bernoulli, Categorical, Poisson, Beta, ForcedIdentifiability
 from jaxns.types import float_type
 
 logger = logging.getLogger('jaxns')
 tfpd = tfp.distributions
@@ -97,15 +98,15 @@
 
 
 def test_priors():
     d = Prior(jnp.zeros(5))
     print(d)
     assert d.forward(jnp.ones(d.base_shape, float_type)).shape == d.shape
     assert d.forward(jnp.zeros(d.base_shape, float_type)).shape == d.shape
-    assert d.base_shape == ()
+    assert d.base_shape == (0,)
     assert d.shape == (5,)
 
     d = Prior(tfpd.Uniform(low=jnp.zeros(5), high=jnp.ones(5)))
     print(d)
     assert d.forward(jnp.ones(d.base_shape, float_type)).shape == d.shape
     assert d.forward(jnp.zeros(d.base_shape, float_type)).shape == d.shape
     assert d.base_shape == (5,)
@@ -243,7 +244,19 @@
     assert d.base_shape == (10, 5)
     assert d.shape == (10, 5)
 
     u_input = vmap(lambda key: random.uniform(key, shape=d.base_shape))(random.split(random.PRNGKey(42), 1))
     x = vmap(lambda u: d.forward(u))(u_input)
     u = vmap(lambda x: d.inverse(x))(x)
     assert jnp.allclose(u, u_input)
+
+
+def test_gh95():
+    def prior_model():
+        x = yield Prior(dist_or_value=jnp.asarray(0.))
+        return x
+
+    def log_likelihood(x):
+        return jnp.sum(x)
+
+    model = Model(prior_model=prior_model, log_likelihood=log_likelihood)
+    assert model.U_ndims == 0
```

### Comparing `jaxns-2.2.2/jaxns/tests/test_random.py` & `jaxns-2.2.3/jaxns/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/tests/test_statistics.py` & `jaxns-2.2.3/jaxns/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/types.py` & `jaxns-2.2.3/jaxns/types.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/uniform_samplers.py` & `jaxns-2.2.3/jaxns/uniform_samplers.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/utils.py` & `jaxns-2.2.3/jaxns/utils.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns/warnings.py` & `jaxns-2.2.3/jaxns/warnings.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/jaxns.egg-info/PKG-INFO` & `jaxns-2.2.3/jaxns.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: jaxns
-Version: 2.2.2
+Version: 2.2.3
 Summary: Nested Sampling in JAX
 Home-page: https://github.com/joshuaalbert/jaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Python](https://img.shields.io/pypi/pyversions/jaxns.svg)](https://badge.fury.io/py/jaxns)
 [![PyPI](https://badge.fury.io/py/jaxns.svg)](https://badge.fury.io/py/jaxns)
-[![Documentation Status](https://readthedocs.org/projects/jaxns/badge/?version=latest)](https://jaxns.readthedocs.io/en/latest/?badge=latest)
-
 
 Main
-Status: ![Workflow name](https://github.com/JoshuaAlbert/jaxns/actions/workflows/unittests.yml/badge.svg?branch=main)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=main)
 
 Develop
-Status: ![Workflow name](https://github.com/JoshuaAlbert/jaxns/actions/workflows/unittests.yml/badge.svg?branch=develop)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 ![JAXNS](https://github.com/Joshuaalbert/jaxns/raw/main/jaxns_logo.png)
 
 ## Mission: _To make nested sampling **faster, easier, and more powerful**_
 
 # What is it?
 
@@ -100,15 +98,15 @@
 improvement in speed on cheap likelihood evaluations.
 This is shown in (https://arxiv.org/abs/2012.15286). With regards to how efficiently JAXNS used likelihood evaluations,
 JAXNS prizes exactness over efficiency, however since it employs an adaptive strategy, users can control efficiency by
 controlling some precision parameters.
 
 # Change Log
 
-28 July, 2023 -- JAXNS 2.2.2 released. Bug fix for singular priors.
+28 July, 2023 -- JAXNS 2.2.3 released. Bug fix for singular priors.
 
 26 June, 2023 -- JAXNS 2.2.1 released. Multi-ellipsoidal sampler added back in. Adaptive refinement disabled, as a bias
 has been detected in it.
 
 15 June, 2023 -- JAXNS 2.2.0 released. Added support to allow TFP bijectors to defined transformed distributions. Other
 minor improvements.
```

### Comparing `jaxns-2.2.2/jaxns.egg-info/SOURCES.txt` & `jaxns-2.2.3/jaxns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.2/setup.py` & `jaxns-2.2.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages
 from setuptools import setup
 
 __minimum_jax_version__ = '0.2.9'
 
-setup_requires = ['jax>=' + __minimum_jax_version__]
+setup_requires = [
+    'jax',
+    'jaxlib',
+    'tensorflow_probability'
+]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='jaxns',
-      version='2.2.2',
+      version='2.2.3',
       description='Nested Sampling in JAX',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/jaxns",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=setup_requires,
```

