# Comparing `tmp/jaxns-2.2.1.tar.gz` & `tmp/jaxns-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxns-2.2.1.tar", last modified: Mon Jun 26 12:50:15 2023, max compression
+gzip compressed data, was "jaxns-2.2.2.tar", last modified: Fri Jul 28 16:51:29 2023, max compression
```

## Comparing `jaxns-2.2.1.tar` & `jaxns-2.2.2.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.359704 jaxns-2.2.1/
--rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-06-19 23:43:03.000000 jaxns-2.2.1/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     4810 2023-06-26 12:50:15.359704 jaxns-2.2.1/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     4371 2023-06-15 14:34:45.000000 jaxns-2.2.1/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.355704 jaxns-2.2.1/jaxns/
--rw-rw-r--   0 albert    (1000) albert    (1000)      581 2023-06-23 10:30:30.000000 jaxns-2.2.1/jaxns/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    13249 2023-06-23 10:30:30.000000 jaxns-2.2.1/jaxns/adaptive_refinement.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     6940 2023-04-21 01:26:04.000000 jaxns-2.2.1/jaxns/initial_state.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.359704 jaxns-2.2.1/jaxns/internals/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.1/jaxns/internals/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      849 2023-01-03 05:33:37.000000 jaxns-2.2.1/jaxns/internals/linalg.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12651 2023-06-15 13:49:53.000000 jaxns-2.2.1/jaxns/internals/log_semiring.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4919 2023-04-21 14:08:43.000000 jaxns-2.2.1/jaxns/internals/maps.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2022-10-13 02:52:05.000000 jaxns-2.2.1/jaxns/internals/shapes.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1853 2023-01-03 05:33:37.000000 jaxns-2.2.1/jaxns/internals/stats.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.359704 jaxns-2.2.1/jaxns/internals/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.1/jaxns/internals/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      277 2023-01-03 05:33:37.000000 jaxns-2.2.1/jaxns/internals/tests/test_linalg.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5490 2023-01-03 05:33:37.000000 jaxns-2.2.1/jaxns/internals/tests/test_log_semiring.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2898 2023-06-14 16:43:12.000000 jaxns-2.2.1/jaxns/internals/tests/test_maps.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1110 2022-12-29 07:48:31.000000 jaxns-2.2.1/jaxns/internals/tests/test_shapes.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1186 2023-01-03 05:33:37.000000 jaxns-2.2.1/jaxns/internals/tests/test_stats.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.359704 jaxns-2.2.1/jaxns/likelihood_samplers/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.1/jaxns/likelihood_samplers/__init__.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.359704 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3192 2023-06-23 00:05:06.000000 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/em_gmm.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    29797 2023-06-23 10:35:37.000000 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/multi_ellipsoid_utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.359704 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1320 2023-06-20 09:16:37.000000 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_em_gmm.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5263 2023-06-20 09:51:44.000000 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3103 2023-05-18 20:19:33.000000 jaxns-2.2.1/jaxns/model.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4425 2023-06-23 10:35:53.000000 jaxns-2.2.1/jaxns/multi_ellipsoidal_samplers.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    18526 2023-06-26 12:35:12.000000 jaxns-2.2.1/jaxns/nested_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    16165 2023-06-23 11:05:56.000000 jaxns-2.2.1/jaxns/plotting.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12554 2023-06-14 10:16:12.000000 jaxns-2.2.1/jaxns/prior.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2787 2023-04-20 15:27:03.000000 jaxns-2.2.1/jaxns/random.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    26263 2023-06-23 08:35:53.000000 jaxns-2.2.1/jaxns/slice_samplers.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    10153 2023-05-18 20:55:58.000000 jaxns-2.2.1/jaxns/special_priors.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    16335 2023-06-26 12:39:04.000000 jaxns-2.2.1/jaxns/static_nested_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    18919 2023-06-23 10:15:39.000000 jaxns-2.2.1/jaxns/statistics.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     6607 2023-05-12 13:17:17.000000 jaxns-2.2.1/jaxns/termination.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.359704 jaxns-2.2.1/jaxns/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-01-03 05:33:37.000000 jaxns-2.2.1/jaxns/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2198 2023-06-23 10:30:30.000000 jaxns-2.2.1/jaxns/tests/debug_adaptive_refinement.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3884 2023-06-23 10:30:30.000000 jaxns-2.2.1/jaxns/tests/test_initial_state.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    18625 2023-06-23 10:37:16.000000 jaxns-2.2.1/jaxns/tests/test_nested_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9019 2023-06-20 23:01:19.000000 jaxns-2.2.1/jaxns/tests/test_prior.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1306 2023-04-15 16:37:14.000000 jaxns-2.2.1/jaxns/tests/test_random.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    24211 2023-06-23 10:30:30.000000 jaxns-2.2.1/jaxns/tests/test_statistics.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      477 2023-01-03 05:33:37.000000 jaxns-2.2.1/jaxns/tests/test_utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5118 2023-05-12 12:43:32.000000 jaxns-2.2.1/jaxns/types.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5122 2023-06-23 08:35:53.000000 jaxns-2.2.1/jaxns/uniform_samplers.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    17668 2023-05-15 05:41:18.000000 jaxns-2.2.1/jaxns/utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      716 2023-05-07 18:38:45.000000 jaxns-2.2.1/jaxns/warnings.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.355704 jaxns-2.2.1/jaxns.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     4810 2023-06-26 12:50:15.000000 jaxns-2.2.1/jaxns.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     1676 2023-06-26 12:50:15.000000 jaxns-2.2.1/jaxns.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-26 12:50:15.000000 jaxns-2.2.1/jaxns.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        6 2023-06-26 12:50:15.000000 jaxns-2.2.1/jaxns.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 jaxns-2.2.1/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-26 12:50:15.359704 jaxns-2.2.1/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)      949 2023-06-26 12:40:43.000000 jaxns-2.2.1/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.612375 jaxns-2.2.2/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-07-28 03:56:53.000000 jaxns-2.2.2/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5150 2023-07-28 16:51:29.612375 jaxns-2.2.2/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4711 2023-07-28 16:50:15.000000 jaxns-2.2.2/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.608375 jaxns-2.2.2/jaxns/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      581 2023-07-28 03:56:53.000000 jaxns-2.2.2/jaxns/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    13249 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/adaptive_refinement.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6940 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/initial_state.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.612375 jaxns-2.2.2/jaxns/internals/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      849 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/linalg.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    12651 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/log_semiring.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4919 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/maps.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/shapes.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1853 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/stats.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.612375 jaxns-2.2.2/jaxns/internals/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      277 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/tests/test_linalg.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5490 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/tests/test_log_semiring.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2898 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/tests/test_maps.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1110 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/tests/test_shapes.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1186 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/internals/tests/test_stats.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.612375 jaxns-2.2.2/jaxns/likelihood_samplers/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/likelihood_samplers/__init__.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.612375 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:53.000000 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3192 2023-07-28 03:56:53.000000 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/em_gmm.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    29797 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/multi_ellipsoid_utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.612375 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:53.000000 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1320 2023-07-28 03:56:53.000000 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_em_gmm.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5263 2023-07-28 03:56:53.000000 jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3103 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/model.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4425 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/multi_ellipsoidal_samplers.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    18526 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    16165 2023-07-28 03:56:53.000000 jaxns-2.2.2/jaxns/plotting.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    12554 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/prior.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2787 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/random.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    26263 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/slice_samplers.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    10153 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/special_priors.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    16335 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/static_nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    18919 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/statistics.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6607 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/termination.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.612375 jaxns-2.2.2/jaxns/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3884 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/tests/test_initial_state.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    18625 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/tests/test_nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     9019 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/tests/test_prior.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1306 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/tests/test_random.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    24211 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/tests/test_statistics.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      477 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/tests/test_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5118 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/types.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5122 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/uniform_samplers.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    17668 2023-07-28 16:49:59.000000 jaxns-2.2.2/jaxns/utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      716 2023-07-28 03:56:05.000000 jaxns-2.2.2/jaxns/warnings.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-28 16:51:29.608375 jaxns-2.2.2/jaxns.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5150 2023-07-28 16:51:29.000000 jaxns-2.2.2/jaxns.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1633 2023-07-28 16:51:29.000000 jaxns-2.2.2/jaxns.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-28 16:51:29.000000 jaxns-2.2.2/jaxns.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        6 2023-07-28 16:51:29.000000 jaxns-2.2.2/jaxns.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-07-28 03:56:05.000000 jaxns-2.2.2/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-07-28 16:51:29.612375 jaxns-2.2.2/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)      949 2023-07-28 16:50:40.000000 jaxns-2.2.2/setup.py
```

### Comparing `jaxns-2.2.1/LICENSE` & `jaxns-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/PKG-INFO` & `jaxns-2.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,17 @@
-Metadata-Version: 2.1
-Name: jaxns
-Version: 2.2.1
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
+[![Documentation Status](https://readthedocs.org/projects/jaxns/badge/?version=latest)](https://jaxns.readthedocs.io/en/latest/?badge=latest)
+
 
 Main
-Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=main)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/jaxns/actions/workflows/unittests.yml/badge.svg?branch=main)
 
 Develop
-Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=develop)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/jaxns/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 ![JAXNS](https://github.com/Joshuaalbert/jaxns/raw/main/jaxns_logo.png)
 
 ## Mission: _To make nested sampling **faster, easier, and more powerful**_
 
 # What is it?
 
@@ -98,14 +86,19 @@
 improvement in speed on cheap likelihood evaluations.
 This is shown in (https://arxiv.org/abs/2012.15286). With regards to how efficiently JAXNS used likelihood evaluations,
 JAXNS prizes exactness over efficiency, however since it employs an adaptive strategy, users can control efficiency by
 controlling some precision parameters.
 
 # Change Log
 
+28 July, 2023 -- JAXNS 2.2.2 released. Bug fix for singular priors.
+
+26 June, 2023 -- JAXNS 2.2.1 released. Multi-ellipsoidal sampler added back in. Adaptive refinement disabled, as a bias
+has been detected in it.
+
 15 June, 2023 -- JAXNS 2.2.0 released. Added support to allow TFP bijectors to defined transformed distributions. Other
 minor improvements.
 
 15 April, 2023 -- JAXNS 2.1.0 released. pmap used on outer-most loops allowing efficient device-device communication
 during parallel runs.
 
 8 March, 2023 -- JAXNS 2.0.1 released. Changed how we're doing annotations to support python 3.8 again.
```

### Comparing `jaxns-2.2.1/README.md` & `jaxns-2.2.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,31 @@
+Metadata-Version: 2.1
+Name: jaxns
+Version: 2.2.2
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
+[![Documentation Status](https://readthedocs.org/projects/jaxns/badge/?version=latest)](https://jaxns.readthedocs.io/en/latest/?badge=latest)
+
 
 Main
-Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=main)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/jaxns/actions/workflows/unittests.yml/badge.svg?branch=main)
 
 Develop
-Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=develop)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/jaxns/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 ![JAXNS](https://github.com/Joshuaalbert/jaxns/raw/main/jaxns_logo.png)
 
 ## Mission: _To make nested sampling **faster, easier, and more powerful**_
 
 # What is it?
 
@@ -84,14 +100,19 @@
 improvement in speed on cheap likelihood evaluations.
 This is shown in (https://arxiv.org/abs/2012.15286). With regards to how efficiently JAXNS used likelihood evaluations,
 JAXNS prizes exactness over efficiency, however since it employs an adaptive strategy, users can control efficiency by
 controlling some precision parameters.
 
 # Change Log
 
+28 July, 2023 -- JAXNS 2.2.2 released. Bug fix for singular priors.
+
+26 June, 2023 -- JAXNS 2.2.1 released. Multi-ellipsoidal sampler added back in. Adaptive refinement disabled, as a bias
+has been detected in it.
+
 15 June, 2023 -- JAXNS 2.2.0 released. Added support to allow TFP bijectors to defined transformed distributions. Other
 minor improvements.
 
 15 April, 2023 -- JAXNS 2.1.0 released. pmap used on outer-most loops allowing efficient device-device communication
 during parallel runs.
 
 8 March, 2023 -- JAXNS 2.0.1 released. Changed how we're doing annotations to support python 3.8 again.
```

### Comparing `jaxns-2.2.1/jaxns/__init__.py` & `jaxns-2.2.2/jaxns/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/adaptive_refinement.py` & `jaxns-2.2.2/jaxns/adaptive_refinement.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/initial_state.py` & `jaxns-2.2.2/jaxns/initial_state.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/internals/linalg.py` & `jaxns-2.2.2/jaxns/internals/linalg.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/internals/log_semiring.py` & `jaxns-2.2.2/jaxns/internals/log_semiring.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/internals/maps.py` & `jaxns-2.2.2/jaxns/internals/maps.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/internals/shapes.py` & `jaxns-2.2.2/jaxns/internals/shapes.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/internals/stats.py` & `jaxns-2.2.2/jaxns/internals/stats.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/internals/tests/test_log_semiring.py` & `jaxns-2.2.2/jaxns/internals/tests/test_log_semiring.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/internals/tests/test_maps.py` & `jaxns-2.2.2/jaxns/internals/tests/test_maps.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/internals/tests/test_shapes.py` & `jaxns-2.2.2/jaxns/internals/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/internals/tests/test_stats.py` & `jaxns-2.2.2/jaxns/internals/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/em_gmm.py` & `jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/em_gmm.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/multi_ellipsoid_utils.py` & `jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/multi_ellipsoid_utils.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_em_gmm.py` & `jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_em_gmm.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py` & `jaxns-2.2.2/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/model.py` & `jaxns-2.2.2/jaxns/model.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/multi_ellipsoidal_samplers.py` & `jaxns-2.2.2/jaxns/multi_ellipsoidal_samplers.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/nested_sampler.py` & `jaxns-2.2.2/jaxns/nested_sampler.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/plotting.py` & `jaxns-2.2.2/jaxns/plotting.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/prior.py` & `jaxns-2.2.2/jaxns/prior.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/random.py` & `jaxns-2.2.2/jaxns/random.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/slice_samplers.py` & `jaxns-2.2.2/jaxns/slice_samplers.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/special_priors.py` & `jaxns-2.2.2/jaxns/special_priors.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/static_nested_sampler.py` & `jaxns-2.2.2/jaxns/static_nested_sampler.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/statistics.py` & `jaxns-2.2.2/jaxns/statistics.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/termination.py` & `jaxns-2.2.2/jaxns/termination.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/tests/test_initial_state.py` & `jaxns-2.2.2/jaxns/tests/test_initial_state.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/tests/test_nested_sampler.py` & `jaxns-2.2.2/jaxns/tests/test_nested_sampler.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/tests/test_prior.py` & `jaxns-2.2.2/jaxns/tests/test_prior.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/tests/test_random.py` & `jaxns-2.2.2/jaxns/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/tests/test_statistics.py` & `jaxns-2.2.2/jaxns/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/types.py` & `jaxns-2.2.2/jaxns/types.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/uniform_samplers.py` & `jaxns-2.2.2/jaxns/uniform_samplers.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/utils.py` & `jaxns-2.2.2/jaxns/utils.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns/warnings.py` & `jaxns-2.2.2/jaxns/warnings.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.1/jaxns.egg-info/PKG-INFO` & `jaxns-2.2.2/jaxns.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: jaxns
-Version: 2.2.1
+Version: 2.2.2
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
+[![Documentation Status](https://readthedocs.org/projects/jaxns/badge/?version=latest)](https://jaxns.readthedocs.io/en/latest/?badge=latest)
+
 
 Main
-Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=main)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/jaxns/actions/workflows/unittests.yml/badge.svg?branch=main)
 
 Develop
-Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=develop)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/jaxns/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 ![JAXNS](https://github.com/Joshuaalbert/jaxns/raw/main/jaxns_logo.png)
 
 ## Mission: _To make nested sampling **faster, easier, and more powerful**_
 
 # What is it?
 
@@ -98,14 +100,19 @@
 improvement in speed on cheap likelihood evaluations.
 This is shown in (https://arxiv.org/abs/2012.15286). With regards to how efficiently JAXNS used likelihood evaluations,
 JAXNS prizes exactness over efficiency, however since it employs an adaptive strategy, users can control efficiency by
 controlling some precision parameters.
 
 # Change Log
 
+28 July, 2023 -- JAXNS 2.2.2 released. Bug fix for singular priors.
+
+26 June, 2023 -- JAXNS 2.2.1 released. Multi-ellipsoidal sampler added back in. Adaptive refinement disabled, as a bias
+has been detected in it.
+
 15 June, 2023 -- JAXNS 2.2.0 released. Added support to allow TFP bijectors to defined transformed distributions. Other
 minor improvements.
 
 15 April, 2023 -- JAXNS 2.1.0 released. pmap used on outer-most loops allowing efficient device-device communication
 during parallel runs.
 
 8 March, 2023 -- JAXNS 2.0.1 released. Changed how we're doing annotations to support python 3.8 again.
```

### Comparing `jaxns-2.2.1/jaxns.egg-info/SOURCES.txt` & `jaxns-2.2.2/jaxns.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,13 @@
 ./jaxns/likelihood_samplers/multi_ellipsoid/__init__.py
 ./jaxns/likelihood_samplers/multi_ellipsoid/em_gmm.py
 ./jaxns/likelihood_samplers/multi_ellipsoid/multi_ellipsoid_utils.py
 ./jaxns/likelihood_samplers/multi_ellipsoid/tests/__init__.py
 ./jaxns/likelihood_samplers/multi_ellipsoid/tests/test_em_gmm.py
 ./jaxns/likelihood_samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py
 ./jaxns/tests/__init__.py
-./jaxns/tests/debug_adaptive_refinement.py
 ./jaxns/tests/test_initial_state.py
 ./jaxns/tests/test_nested_sampler.py
 ./jaxns/tests/test_prior.py
 ./jaxns/tests/test_random.py
 ./jaxns/tests/test_statistics.py
 ./jaxns/tests/test_utils.py
```

### Comparing `jaxns-2.2.1/setup.py` & `jaxns-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup_requires = ['jax>=' + __minimum_jax_version__]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='jaxns',
-      version='2.2.1',
+      version='2.2.2',
       description='Nested Sampling in JAX',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/jaxns",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=setup_requires,
```

