# Comparing `tmp/baytune-0.4.0.tar.gz` & `tmp/baytune-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/baytune-0.4.0.tar", last modified: Wed Dec 30 18:51:17 2020, max compression
+gzip compressed data, was "baytune-0.5.0.tar", last modified: Fri Jul 28 16:54:14 2023, max compression
```

## Comparing `baytune-0.4.0.tar` & `baytune-0.5.0.tar`

### file list

```diff
@@ -1,107 +1,76 @@
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      337 2020-08-03 19:49:49.000000 baytune-0.4.0/AUTHORS.rst
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     8534 2020-12-30 18:51:09.000000 baytune-0.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 pacho     (1000) pacho     (1000)    10483 2020-12-30 18:51:09.000000 baytune-0.4.0/HISTORY.md
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     1076 2020-08-03 19:49:49.000000 baytune-0.4.0/LICENSE
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      265 2020-08-03 19:49:49.000000 baytune-0.4.0/MANIFEST.in
--rw-rw-r--   0 pacho     (1000) pacho     (1000)    24968 2020-12-30 18:51:17.000000 baytune-0.4.0/PKG-INFO
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     9291 2020-12-30 18:51:09.000000 baytune-0.4.0/README.md
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/baytune.egg-info/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)    24968 2020-12-30 18:51:16.000000 baytune-0.4.0/baytune.egg-info/PKG-INFO
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     2477 2020-12-30 18:51:17.000000 baytune-0.4.0/baytune.egg-info/SOURCES.txt
--rw-rw-r--   0 pacho     (1000) pacho     (1000)        1 2020-12-30 18:51:16.000000 baytune-0.4.0/baytune.egg-info/dependency_links.txt
--rw-rw-r--   0 pacho     (1000) pacho     (1000)        1 2020-12-30 18:51:16.000000 baytune-0.4.0/baytune.egg-info/not-zip-safe
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      669 2020-12-30 18:51:16.000000 baytune-0.4.0/baytune.egg-info/requires.txt
--rw-rw-r--   0 pacho     (1000) pacho     (1000)        4 2020-12-30 18:51:16.000000 baytune-0.4.0/baytune.egg-info/top_level.txt
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/btb/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      216 2020-12-30 18:51:09.000000 baytune-0.4.0/btb/__init__.py
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/btb/selection/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      474 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/selection/__init__.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     2653 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/selection/best.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      281 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/selection/custom_selector.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     1394 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/selection/hierarchical.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     2609 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/selection/pure.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     2487 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/selection/recent.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     2331 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/selection/selector.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     1463 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/selection/ucb1.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      242 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/selection/uniform.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)    13134 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/session.py
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/btb/tuning/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      726 2020-09-08 09:39:27.000000 baytune-0.4.0/btb/tuning/__init__.py
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/btb/tuning/acquisition/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      331 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/tuning/acquisition/__init__.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     1043 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/tuning/acquisition/base.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      569 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/tuning/acquisition/expected_improvement.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      334 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/tuning/acquisition/predicted_score.py
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/btb/tuning/hyperparams/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      386 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/tuning/hyperparams/__init__.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     9604 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/tuning/hyperparams/base.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     4315 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/tuning/hyperparams/boolean.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     6326 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/tuning/hyperparams/categorical.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)    13787 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/tuning/hyperparams/numerical.py
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/btb/tuning/metamodels/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      199 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/tuning/metamodels/__init__.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     2999 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/tuning/metamodels/base.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     3811 2020-12-28 12:20:14.000000 baytune-0.4.0/btb/tuning/metamodels/gaussian_process.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)    10518 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/tuning/tunable.py
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/btb/tuning/tuners/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      325 2020-09-08 09:39:27.000000 baytune-0.4.0/btb/tuning/tuners/__init__.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)    16492 2020-12-14 09:57:49.000000 baytune-0.4.0/btb/tuning/tuners/base.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     5570 2020-09-08 09:39:27.000000 baytune-0.4.0/btb/tuning/tuners/gaussian_process.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      812 2020-08-03 19:49:49.000000 baytune-0.4.0/btb/tuning/tuners/uniform.py
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/docs/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      604 2020-08-03 19:49:49.000000 baytune-0.4.0/docs/Makefile
--rw-rw-r--   0 pacho     (1000) pacho     (1000)       28 2020-08-03 19:49:49.000000 baytune-0.4.0/docs/authors.rst
--rw-rw-r--   0 pacho     (1000) pacho     (1000)       38 2020-08-03 19:49:49.000000 baytune-0.4.0/docs/benchmark.rst
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     5857 2020-12-30 18:51:09.000000 baytune-0.4.0/docs/conf.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)       33 2020-08-03 19:49:49.000000 baytune-0.4.0/docs/contributing.rst
--rw-rw-r--   0 pacho     (1000) pacho     (1000)       29 2020-08-03 19:49:49.000000 baytune-0.4.0/docs/history.rst
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/docs/images/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)    13701 2020-08-03 19:49:49.000000 baytune-0.4.0/docs/images/BTB-Icon-small.png
--rw-rw-r--   0 pacho     (1000) pacho     (1000)    33432 2020-08-03 19:49:49.000000 baytune-0.4.0/docs/images/dai-logo-white-200.png
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     3783 2020-12-30 18:51:09.000000 baytune-0.4.0/docs/index.rst
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     1330 2020-12-30 18:51:09.000000 baytune-0.4.0/docs/install.rst
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      263 2020-08-03 19:49:49.000000 baytune-0.4.0/docs/kubernetes.rst
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      765 2020-08-03 19:49:49.000000 baytune-0.4.0/docs/make.bat
--rw-rw-r--   0 pacho     (1000) pacho     (1000)       28 2020-08-03 19:49:49.000000 baytune-0.4.0/docs/readme.rst
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     1335 2020-12-30 18:51:17.000000 baytune-0.4.0/setup.cfg
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     2622 2020-12-30 18:51:09.000000 baytune-0.4.0/setup.py
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/tests/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)        0 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/__init__.py
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/tests/integration/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)        0 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/integration/__init__.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     6197 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/integration/test_session.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     1555 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/integration/test_tuning.py
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/tests/selection/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)        0 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/selection/__init__.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     4679 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/selection/test_best.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      841 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/selection/test_custom_selector.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     2261 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/selection/test_hierarchical.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     3209 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/selection/test_pure.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     3539 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/selection/test_recent.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     1611 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/selection/test_selector.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     1103 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/selection/test_ucb1.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)      723 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/selection/test_uniform.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)    14829 2020-12-30 18:51:09.000000 baytune-0.4.0/tests/test_session.py
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/tests/tuning/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)        0 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/tuning/__init__.py
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/tests/tuning/acquisition/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)        0 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/tuning/acquisition/__init__.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     1004 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/tuning/acquisition/test_expected_improvement.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     2199 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/tuning/acquisition/test_predicted_score.py
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/tests/tuning/hyperparams/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)        0 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/tuning/hyperparams/__init__.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     9696 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/tuning/hyperparams/test_base.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     3564 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/tuning/hyperparams/test_boolean.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     5478 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/tuning/hyperparams/test_categorical.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)    18776 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/tuning/hyperparams/test_numerical.py
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/tests/tuning/metamodels/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)        0 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/tuning/metamodels/__init__.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     2161 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/tuning/metamodels/test_base.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     5405 2020-09-08 09:39:27.000000 baytune-0.4.0/tests/tuning/metamodels/test_gaussian_process.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)    12647 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/tuning/test_tunable.py
-drwxrwxr-x   0 pacho     (1000) pacho     (1000)        0 2020-12-30 18:51:17.000000 baytune-0.4.0/tests/tuning/tuners/
--rw-rw-r--   0 pacho     (1000) pacho     (1000)        0 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/tuning/tuners/__init__.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)    16921 2020-09-08 09:39:27.000000 baytune-0.4.0/tests/tuning/tuners/test_base.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     3526 2020-09-08 09:39:27.000000 baytune-0.4.0/tests/tuning/tuners/test_gaussian_process.py
--rw-rw-r--   0 pacho     (1000) pacho     (1000)     1337 2020-08-03 19:49:49.000000 baytune-0.4.0/tests/tuning/tuners/test_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:54:14.157042 baytune-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-28 16:53:57.000000 baytune-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-07-28 16:54:14.157042 baytune-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-07-28 16:53:57.000000 baytune-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:54:14.149042 baytune-0.5.0/baytune/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:54:14.153042 baytune-0.5.0/baytune/selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/selection/best.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/selection/custom_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/selection/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/selection/pure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/selection/recent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/selection/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/selection/ucb1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/selection/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:54:14.153042 baytune-0.5.0/baytune/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:54:14.153042 baytune-0.5.0/baytune/tuning/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/acquisition/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/acquisition/expected_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/acquisition/predicted_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:54:14.153042 baytune-0.5.0/baytune/tuning/hyperparams/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/hyperparams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/hyperparams/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/hyperparams/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/hyperparams/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/hyperparams/numerical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:54:14.153042 baytune-0.5.0/baytune/tuning/metamodels/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/metamodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/metamodels/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/metamodels/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/tunable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:54:14.153042 baytune-0.5.0/baytune/tuning/tuners/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/tuners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/tuners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/tuners/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/tuning/tuners/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 16:53:57.000000 baytune-0.5.0/baytune/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:54:14.149042 baytune-0.5.0/baytune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-07-28 16:54:14.000000 baytune-0.5.0/baytune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-28 16:54:14.000000 baytune-0.5.0/baytune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:54:14.000000 baytune-0.5.0/baytune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-28 16:54:14.000000 baytune-0.5.0/baytune.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 16:54:14.000000 baytune-0.5.0/baytune.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:54:14.153042 baytune-0.5.0/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:54:14.153042 baytune-0.5.0/benchmark/btb_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:54:14.157042 baytune-0.5.0/benchmark/btb_benchmark/challenges/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/challenges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/challenges/bohachevsky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/challenges/branin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/challenges/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15610 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/challenges/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/challenges/mlchallenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/challenges/randomforest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/challenges/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/challenges/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/challenges/xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12511 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:54:14.157042 baytune-0.5.0/benchmark/btb_benchmark/tuning_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/tuning_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/tuning_functions/ax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/tuning_functions/btb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/tuning_functions/hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/tuning_functions/skopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/btb_benchmark/tuning_functions/smac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-28 16:53:57.000000 baytune-0.5.0/benchmark/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-28 16:53:57.000000 baytune-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 16:54:14.157042 baytune-0.5.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `baytune-0.4.0/LICENSE` & `baytune-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `baytune-0.4.0/README.md` & `baytune-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `baytune-0.4.0/btb/selection/best.py` & `baytune-0.5.0/baytune/selection/best.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 
 import numpy as np
 
-from btb.selection.ucb1 import UCB1
+from baytune.selection.ucb1 import UCB1
 
 # the minimum number of scores that each choice must have in order to use best-K
 # optimizations. If not all choices meet this threshold, default UCB1 selection
 # will be used.
 K_MIN = 2
 
-logger = logging.getLogger('btb')
+logger = logging.getLogger("btb")
 
 
 class BestKReward(UCB1):
     """Best K reward selector
 
     Computes the average reward from the past scores by using only the highest k scores. In
     implementation, the other scores are replaced with ``nan``s such that they still factor into
@@ -27,36 +27,40 @@
         super(BestKReward, self).__init__(choices)
         self.k = k
 
     def compute_rewards(self, scores):
         """Retain the K best scores, and replace the rest with nans"""
         if len(scores) > self.k:
             scores = np.copy(scores)
-            inds = np.argsort(scores)[:-self.k]
+            inds = np.argsort(scores)[: -self.k]
             scores[inds] = np.nan
 
         return list(scores)
 
     def select(self, choice_scores):
         """Select a choice using the K best scores
 
         Keeps the choice counts intact, but only let the bandit see the top k learners' scores.
         If there is not enough score history to do K-selection, use the default UCB1 reward
         function.
         """
         min_num_scores = min(len(s) for s in choice_scores.values())
         if min_num_scores >= K_MIN:
             logger.info(
-                '{klass}: using Best K bandit selection'
-                .format(klass=type(self).__name__))
+                "{klass}: using Best K bandit selection".format(
+                    klass=type(self).__name__
+                )
+            )
             compute_rewards = self.compute_rewards
         else:
             logger.warning(
-                '{klass}: Not enough choices to do K-selection; using plain UCB1'
-                .format(klass=type(self).__name__))
+                "{klass}: Not enough choices to do K-selection; using plain UCB1".format(
+                    klass=type(self).__name__
+                )
+            )
             compute_rewards = super(BestKReward, self).compute_rewards
 
         # convert the raw scores list for each choice to a "rewards" list
         choice_rewards = {
             choice: compute_rewards(choice_scores[choice])
             for choice in choice_scores
             if choice in self.choices
@@ -71,11 +75,11 @@
     def compute_rewards(self, scores):
         """Compute the velocity of the best scores
 
         The velocities are the k distances between the k+1 best scores.
         """
         k = self.k
         m = max(len(scores) - k, 0)
-        best_scores = sorted(scores)[-k - 1:]
+        best_scores = sorted(scores)[-k - 1 :]
         velocities = np.diff(best_scores)
         nans = np.full(m, np.nan)
         return list(velocities) + list(nans)
```

### Comparing `baytune-0.4.0/btb/selection/hierarchical.py` & `baytune-0.5.0/baytune/selection/hierarchical.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from btb.selection.ucb1 import UCB1
+from baytune.selection.ucb1 import UCB1
 
 
 class HierarchicalByAlgorithm(UCB1):
     """Hierarchical selector
 
     Args:
         by_algorithm (Dict[str, List]): mapping of ML algorithms to frozen set choices
```

### Comparing `baytune-0.4.0/btb/selection/pure.py` & `baytune-0.5.0/baytune/selection/pure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 
-from btb.selection.selector import Selector
+from baytune.selection.selector import Selector
 
 # the minimum number of scores that each choice must have in order to use best-K
 # optimizations. If not all choices meet this threshold, default UCB1 selection
 # will be used.
 K_MIN = 3
 
-logger = logging.getLogger('btb')
+logger = logging.getLogger("btb")
 
 
 class PureBestKVelocity(Selector):
     """Pure Best K Velocity Selector
 
     Simply returns the choice with the best best-K velocity.
     """
@@ -23,37 +23,38 @@
     def compute_rewards(self, scores):
         """
         Compute the "velocity" of (average distance between) the k+1 best
         scores. Return a list with those k velocities padded out with zeros so
         that the count remains the same.
         """
         # get the k + 1 best scores in descending order
-        best_scores = sorted(scores, reverse=True)[:self.k + 1]
-        velocities = [best_scores[i] - best_scores[i + 1]
-                      for i in range(len(best_scores) - 1)]
+        best_scores = sorted(scores, reverse=True)[: self.k + 1]
+        velocities = [
+            best_scores[i] - best_scores[i + 1] for i in range(len(best_scores) - 1)
+        ]
 
         # pad the list out with zeros to maintain the length of the list
         zeros = (len(scores) - self.k) * [0]
         return velocities + zeros
 
     def select(self, choice_scores):
         """
         Select the choice with the highest best-K velocity. If any choices
         don't have MIN_K scores yet, return the one with the fewest.
         """
         # if we don't have enough scores to do K-selection, fall back to UCB1
         min_num_scores = min([len(s) for s in choice_scores.values()])
         if min_num_scores >= K_MIN:
-            logger.info('PureBestKVelocity: using Pure Best K velocity selection')
+            logger.info("PureBestKVelocity: using Pure Best K velocity selection")
             reward_func = self.compute_rewards
         else:
             logger.warning(
-                '{klass}: Not enough choices to do K-selection; '
-                'returning choice with fewest scores'
-                .format(klass=type(self).__name__))
+                "{klass}: Not enough choices to do K-selection; "
+                "returning choice with fewest scores".format(klass=type(self).__name__)
+            )
             # reward choices with the fewest scores
             # NOTE: "reward_func = lambda " changed to "def reward_func"
             # as per flake8 suggestions
             # reward_func = lambda s: [1] if len(s) == min_num_scores else [0]
 
             def reward_func(scores):
                 return [1] if len(scores) == min_num_scores else [0]
```

### Comparing `baytune-0.4.0/btb/selection/recent.py` & `baytune-0.5.0/baytune/selection/recent.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 
-from btb.selection.ucb1 import UCB1
+from baytune.selection.ucb1 import UCB1
 
 # the minimum number of scores that each choice must have in order to use
 # best-K optimizations. If not all choices meet this threshold, default UCB1
 # selection will be used.
 K_MIN = 2
 
-logger = logging.getLogger('btb')
+logger = logging.getLogger("btb")
 
 
 class RecentKReward(UCB1):
     """Recent K reward selector
 
     Args:
         k (int): number of best scores to consider
@@ -21,28 +21,34 @@
         super(RecentKReward, self).__init__(choices)
         self.k = k
 
     def compute_rewards(self, scores):
         """Retain the K most recent scores, and replace the rest with zeros"""
         for i in range(len(scores)):
             if i >= self.k:
-                scores[i] = 0.
+                scores[i] = 0.0
         return scores
 
     def select(self, choice_scores):
         """Use the top k learner's scores for usage in rewards for the bandit calculation"""
         # if we don't have enough scores to do K-selection, fall back to UCB1
         min_num_scores = min([len(s) for s in choice_scores.values()])
         if min_num_scores >= K_MIN:
-            logger.info('{klass}: using Best K bandit selection'.format(klass=type(self).__name__))
+            logger.info(
+                "{klass}: using Best K bandit selection".format(
+                    klass=type(self).__name__
+                )
+            )
             reward_func = self.compute_rewards
         else:
             logger.warning(
-                '{klass}: Not enough choices to do K-selection; using plain UCB1'
-                .format(klass=type(self).__name__))
+                "{klass}: Not enough choices to do K-selection; using plain UCB1".format(
+                    klass=type(self).__name__
+                )
+            )
             reward_func = super(RecentKReward, self).compute_rewards
 
         choice_rewards = {}
         for choice, scores in choice_scores.items():
             if choice not in self.choices:
                 continue
             choice_rewards[choice] = reward_func(scores)
@@ -56,14 +62,16 @@
     def compute_rewards(self, scores):
         """Compute the velocity of thte k+1 most recent scores.
 
         The velocity is the average distance between scores. Return a list with those k velocities
         padded out with zeros so that the count remains the same.
         """
         # take the k + 1 most recent scores so we can get k velocities
-        recent_scores = scores[:-self.k - 2:-1]
-        velocities = [recent_scores[i] - recent_scores[i + 1] for i in
-                      range(len(recent_scores) - 1)]
+        recent_scores = scores[: -self.k - 2 : -1]
+        velocities = [
+            recent_scores[i] - recent_scores[i + 1]
+            for i in range(len(recent_scores) - 1)
+        ]
         # pad the list out with zeros, so the length of the list is
         # maintained
         zeros = (len(scores) - self.k) * [0]
         return velocities + zeros
```

### Comparing `baytune-0.4.0/btb/selection/selector.py` & `baytune-0.5.0/baytune/selection/selector.py`

 * *Files identical despite different names*

### Comparing `baytune-0.4.0/btb/selection/ucb1.py` & `baytune-0.5.0/baytune/selection/ucb1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import random
 
 import numpy as np
 
-from btb.selection.selector import Selector
+from baytune.selection.selector import Selector
 
 
 class UCB1(Selector):
     """UCB1 selector
 
     Uses Upper Confidence Bound 1 algorithm (UCB1) for bandit selection.
```

### Comparing `baytune-0.4.0/btb/session.py` & `baytune-0.5.0/baytune/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import logging
 from collections import Counter, defaultdict
 from hashlib import md5
 
 import numpy as np
 from tqdm.auto import trange
 
-from btb.selection.ucb1 import UCB1
-from btb.tuning.tunable import Tunable
-from btb.tuning.tuners.base import StopTuning
-from btb.tuning.tuners.gaussian_process import GPTuner
+from baytune.selection.ucb1 import UCB1
+from baytune.tuning.tunable import Tunable
+from baytune.tuning.tuners.base import StopTuning
+from baytune.tuning.tuners.gaussian_process import GPTuner
 
 LOGGER = logging.getLogger(__name__)
 
 
 class BTBSession:
     """BTBSession class.
 
@@ -42,35 +42,36 @@
         errors (Counter):
             A Counter of the errors that each Tunable had during the session.
 
     Args:
         tunables (dict):
             Python dictionary that has as keys the name of the tunable and
             as value a dictionary with the tunable hyperparameters or an
-            ``btb.tuning.tunable.Tunable`` instance.
+            ``baytune.tuning.tunable.Tunable`` instance.
         scorer (callable object / function):
             A callable object or function with signature ``scorer(tunable_name, config)``
             wich should return only a single value.
-        tuner_class (btb.tuning.tuner.BaseTuner):
+        tuner_class (baytune.tuning.tuner.BaseTuner):
             A tuner based on BTB ``BaseTuner`` class. This tuner will manage the new proposals.
-            Defaults to ``btb.tuning.tuners.gaussian_process.GPTuner``
-        selector_class (btb.selection.selector.Selector):
+            Defaults to ``baytune.tuning.tuners.gaussian_process.GPTuner``
+        selector_class (baytune.selection.selector.Selector):
             A selector based on BTB ``Selector`` class. This will determinate which one of
             the tunables is performing better, and which one to test next. Defaults to
-            ``btb.selection.selectors.ucb1.UCB1``
+            ``baytune.selection.selectors.ucb1.UCB1``
         maximize (bool):
             If ``True`` the scores are interpreted as bigger is better, if ``False`` then smaller
             is better, this should depend on the problem type (maximization or minimization).
             Defaults to ``True``.
         max_erors (int):
             Amount of errors allowed for a tunable to not generate a score. Once this amount of
             errors is reached, the tunable will be removed from the list. Defaults to 1.
         verbose (bool):
             If ``True`` a progress bar will be displayed for the ``run`` process.
     """
+
     _tunables = None
     _scorer = None
     _tuner_class = None
     _selector = None
     _maximize = None
     _max_errors = None
     _best_normalized = None
@@ -85,17 +86,24 @@
     iterations = None
     errors = None
 
     def _normalize(self, score):
         if score is not None:
             return score if self._maximize else -score
 
-    def __init__(self, tunables, scorer, tuner_class=GPTuner, selector_class=UCB1,
-                 maximize=True, max_errors=1, verbose=False):
-
+    def __init__(
+        self,
+        tunables,
+        scorer,
+        tuner_class=GPTuner,
+        selector_class=UCB1,
+        maximize=True,
+        max_errors=1,
+        verbose=False,
+    ):
         self._tunables = tunables
         self._scorer = scorer
         self._tuner_class = tuner_class
         self._tunable_names = list(self._tunables.keys())
         self._selector = selector_class(self._tunable_names)
         self._maximize = maximize
         self._max_errors = max_errors
@@ -121,26 +129,26 @@
                 value = int(value)
             elif isinstance(value, np.floating):
                 value = float(value)
             elif isinstance(value, np.ndarray):
                 value = value.tolist()
             elif isinstance(value, np.bool_):
                 value = bool(value)
-            elif value == 'None':
+            elif value == "None":
                 value = None
 
             dumpable[key] = value
 
         return dumpable
 
     def _make_id(self, name, config):
         dumpable_config = self._make_dumpable(config)
         proposal = {
-            'name': name,
-            'config': dumpable_config,
+            "name": name,
+            "config": dumpable_config,
         }
         hashable = json.dumps(proposal, sort_keys=True).encode()
 
         return md5(hashable).hexdigest()
 
     def _remove_tunable(self, tunable_name):
         """Remove a tunable from the candidates list.
@@ -194,60 +202,68 @@
                 * Hyperparameters proposal.
 
         Raises:
             StopTuning:
                 If the ``BTBSession`` has run out of proposals to generate.
         """
         if not self._tunables:
-            raise StopTuning('There are no tunables left to try.')
+            raise StopTuning("There are no tunables left to try.")
 
         if len(self._tuners) < len(self._tunable_names):
             tunable_name = self._tunable_names[len(self._tuners)]
             tunable = self._tunables[tunable_name]
 
             if isinstance(tunable, dict):
-                LOGGER.info('Creating Tunable instance from dict.')
+                LOGGER.info("Creating Tunable instance from dict.")
                 tunable = Tunable.from_dict(tunable)
 
             if not isinstance(tunable, Tunable):
-                raise TypeError('Tunable can only be an instance of btb.tuning.Tunable or dict')
+                raise TypeError(
+                    "Tunable can only be an instance of baytune.tuning.Tunable or dict"
+                )
 
-            LOGGER.info('Obtaining default configuration for %s', tunable_name)
+            LOGGER.info("Obtaining default configuration for %s", tunable_name)
             config = tunable.get_defaults()
 
             if tunable.cardinality == 1:
-                LOGGER.warn('Skipping tuner creation for Tunable %s with cardinality 1',
-                            tunable_name)
+                LOGGER.warn(
+                    "Skipping tuner creation for Tunable %s with cardinality 1",
+                    tunable_name,
+                )
                 tuner = None
             else:
                 tuner = self._tuner_class(tunable)
 
             self._tuners[tunable_name] = tuner
 
         else:
             tunable_name = self._get_next_tunable_name()
             tuner = self._tuners[tunable_name]
 
             try:
                 if tuner is None:
-                    raise StopTuning('Tunable %s has no tunable hyperparameters', tunable_name)
+                    raise StopTuning(
+                        "Tunable %s has no tunable hyperparameters", tunable_name
+                    )
 
-                LOGGER.info('Generating new proposal configuration for %s', tunable_name)
+                LOGGER.info(
+                    "Generating new proposal configuration for %s", tunable_name
+                )
                 config = tuner.propose(1)
 
             except StopTuning:
-                LOGGER.info('%s has no more configs to propose.', tunable_name)
+                LOGGER.info("%s has no more configs to propose.", tunable_name)
                 self._remove_tunable(tunable_name)
                 tunable_name, config = self.propose()
 
         proposal_id = self._make_id(tunable_name, config)
         self.proposals[proposal_id] = {
-            'id': proposal_id,
-            'name': tunable_name,
-            'config': config
+            "id": proposal_id,
+            "name": tunable_name,
+            "config": config,
         }
 
         return tunable_name, config
 
     def handle_error(self, tunable_name):
         """Handle errors when ``score`` is ``None``.
 
@@ -258,15 +274,17 @@
             tunable_name (str):
                 The name of the tunable to which this configuration belongs.
         """
         self.errors[tunable_name] += 1
         errors = self.errors[tunable_name]
 
         if errors >= self._max_errors:
-            LOGGER.warning('Too many errors: %s. Removing tunable %s', errors, tunable_name)
+            LOGGER.warning(
+                "Too many errors: %s. Removing tunable %s", errors, tunable_name
+            )
             self._remove_tunable(tunable_name)
 
     def record(self, tunable_name, config, score):
         """Record the configuration and the obtained score to the tuner.
 
         If the score is the best one so far, the ``best_proposal`` and ``best_score`` are
         updated.
@@ -277,37 +295,42 @@
             config (dict):
                 Hyperparameter proposal, as given by the tunable.
             score (float):
                 Obtained score with the given configuration.
         """
         proposal_id = self._make_id(tunable_name, config)
         proposal = self.proposals[proposal_id]
-        proposal['score'] = score
+        proposal["score"] = score
 
         if score is None:
             self.handle_error(tunable_name)
         else:
             normalized = self._normalize(score)
             self._normalized_scores[tunable_name].append(normalized)
 
             if normalized > self._best_normalized:
-                LOGGER.info('New optimal found: %s - %s', tunable_name, score)
+                LOGGER.info("New optimal found: %s - %s", tunable_name, score)
                 self.best_proposal = proposal
                 self.best_score = score
                 self._best_normalized = normalized
             try:
                 tuner = self._tuners[tunable_name]
                 if tuner is None:
-                    LOGGER.warn('Skipping record for Tunable %s with cardinality 1', tunable_name)
+                    LOGGER.warn(
+                        "Skipping record for Tunable %s with cardinality 1",
+                        tunable_name,
+                    )
                 else:
                     tuner.record(config, normalized)
 
             except Exception:
-                LOGGER.exception('Could not record configuration and score for tuner %s.',
-                                 tunable_name)
+                LOGGER.exception(
+                    "Could not record configuration and score for tuner %s.",
+                    tunable_name,
+                )
 
     def run(self, iterations=None):
         """Run the selection and tuning loop for the given number of iterations.
 
         At each iteration, the `BTBSession` will generate a new proposal calling
         ``self.propose``, score it using the `self.scorer`, and finally record the
         obtained score back to the tuner calling `self.record`.
@@ -328,24 +351,29 @@
             iterator = self._range(iterations)
 
         for _ in iterator:
             self.iterations += 1
             tunable_name, config = self.propose()
 
             try:
-                LOGGER.debug('Scoring proposal %s - %s: %s', self.iterations, tunable_name, config)
+                LOGGER.debug(
+                    "Scoring proposal %s - %s: %s",
+                    self.iterations,
+                    tunable_name,
+                    config,
+                )
                 score = self._scorer(tunable_name, config)
 
             except Exception:
-                params = '\n'.join('{}: {}'.format(k, v) for k, v in config.items())
+                params = "\n".join("{}: {}".format(k, v) for k, v in config.items())
                 LOGGER.exception(
-                    'Proposal %s - %s crashed with the following configuration: %s',
+                    "Proposal %s - %s crashed with the following configuration: %s",
                     self.iterations,
                     tunable_name,
-                    params
+                    params,
                 )
 
                 score = None
 
             self.record(tunable_name, config, score)
 
         return self.best_proposal
```

### Comparing `baytune-0.4.0/btb/tuning/acquisition/base.py` & `baytune-0.5.0/baytune/tuning/acquisition/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from abc import ABCMeta, abstractmethod
 
 import numpy as np
 
 
 class BaseAcquisition(metaclass=ABCMeta):
-
     def __init_acquisition__(self, **kwargs):
         pass
 
     @staticmethod
     def _get_max_candidates(candidates, n):
         k = min(n, len(candidates) - 1)  # kth element
         sorted_candidates = np.argpartition(-candidates, k)
```

### Comparing `baytune-0.4.0/btb/tuning/acquisition/expected_improvement.py` & `baytune-0.5.0/baytune/tuning/acquisition/expected_improvement.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # -*- coding: utf-8 -*-
 
 """Package where the ExpectedImprovementAcquisition class is defined."""
 
 import numpy as np
 from scipy.stats import norm
 
-from btb.tuning.acquisition.base import BaseAcquisition
+from baytune.tuning.acquisition.base import BaseAcquisition
 
 
 class ExpectedImprovementAcquisition(BaseAcquisition):
-
     def _acquire(self, candidates, num_candidates=1):
         Phi = norm.cdf
         N = norm.pdf
 
         mu, sigma = candidates.T
         y_best = np.max(self.scores)
```

### Comparing `baytune-0.4.0/btb/tuning/hyperparams/base.py` & `baytune-0.5.0/baytune/tuning/hyperparams/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Attributes:
         dimensions (int):
             Number of dimensions that the hyperparameter uses to be represented in the search
             space.
         cardinality (int or np.inf):
             Number of possible values for this hyperparameter.
     """
+
     dimensions = 0
     cardinality = 0
     default = None
 
     def _to_array(self, values):
         """Validate and convert ``values`` to a ``numpy.ndarray`` with the expected shape.
 
@@ -59,39 +60,43 @@
                 If the given values cannot fit into the expected output shape.
         """
 
         if np.isscalar(values):
             if self.dimensions == 1:
                 return np.array([[values]])
             else:
-                raise ValueError('Only lists or numpy.ndarrays are supported for dimensions > 1')
+                raise ValueError(
+                    "Only lists or numpy.ndarrays are supported for dimensions > 1"
+                )
 
         if isinstance(values, list):
             if not all(np.isscalar(value) for value in values):
                 if not all(isinstance(value, list) for value in values):
-                    raise ValueError('Only list of lists are supported')
+                    raise ValueError("Only list of lists are supported")
                 elif not all(len(value) == self.dimensions for value in values):
-                    raise ValueError('All sublists must have len == dimensions')
+                    raise ValueError("All sublists must have len == dimensions")
 
             values = np.array(values)
 
         if len(values.shape) > 2:
-            raise ValueError('Invalid shape: Too many dimensions')
+            raise ValueError("Invalid shape: Too many dimensions")
 
         if self.dimensions == 1:
             if len(values.shape) == 1:
                 values = values.reshape(-1, 1)
             elif values.shape[1] != 1:
-                raise ValueError('Invalid shape: Only 1 column is supported if dimensions == 1')
+                raise ValueError(
+                    "Invalid shape: Only 1 column is supported if dimensions == 1"
+                )
 
         elif len(values.shape) == 1:
             if len(values) != self.dimensions:
-                raise ValueError('Number of elements != number of dimensions')
+                raise ValueError("Number of elements != number of dimensions")
             elif not all(np.isscalar(value) for value in values):
-                raise ValueError('Numpy arrays must only contain scalars')
+                raise ValueError("Numpy arrays must only contain scalars")
 
             values = values.reshape(1, -1)
 
         return values
 
     def _within_range(self, values, min=0, max=1):
         """Ensure that the values are within a certain range.
@@ -104,15 +109,17 @@
             ValueError:
                 A ``ValueError`` is raised if any value from ``values`` is not within the range.
         """
         inside_mask = np.ma.masked_inside(values, min, max)
         if inside_mask.any():
             outside = inside_mask[~inside_mask.mask].data.reshape(-1).tolist()
             raise ValueError(
-                'Values found outside of the valid range [{}, {}]: {}'.format(min, max, outside)
+                "Values found outside of the valid range [{}, {}]: {}".format(
+                    min, max, outside
+                )
             )
 
     def _within_hyperparam_space(self, values):
         """Ensure that the values are within the range of the hyperparameter space.
 
         Args:
             values (numpy.ndarray):
@@ -123,15 +130,15 @@
     def _within_search_space(self, values):
         """Ensure that the values are within the range of the search space.
 
         Args:
             values (numpy.ndarray):
                 2D array of values that will be validated.
         """
-        self._within_range(values.astype(np.float), min=0, max=1)
+        self._within_range(values.astype(np.float64), min=0, max=1)
 
     @abstractmethod
     def _inverse_transform(self, values):
         """Method to be implemented by child classes."""
         pass
 
     @abstractmethod
@@ -155,15 +162,15 @@
 
         Example:
             The example below shows simple usage case where an ``IntHyperParam`` is being imported,
             instantiated with a range from 1 to 4, and its method ``inverse_transform`` is being
             called two times with a scalar from the search space and an array of two valid values
             from the search space.
 
-            >>> from btb.tuning.hyperparams.numerical import IntHyperParam
+            >>> from baytune.tuning.hyperparams.numerical import IntHyperParam
             >>> ihp = IntHyperParam(min=1, max=4)
             >>> ihp.inverse_transform(0.125)
             array([[1]])
             >>> ihp.inverse_transform([0.125, 0.375])
             array([[1],
                    [2]])
         """
@@ -186,15 +193,15 @@
 
         Example:
             The example below shows simple usage case where an ``IntHyperParam`` is being imported,
             instantiated with a range from 1 to 4, and its method ``sample`` is being called
             with a number of samples to be obtained. A ``numpy.ndarray`` with values from the
             search space is being returned.
 
-            >>> from btb.tuning.hyperparams.numerical import IntHyperParam
+            >>> from baytune.tuning.hyperparams.numerical import IntHyperParam
             >>> instance = IntHyperParam(min=1, max=4)
             >>> instance.sample(2)
             array([[0.625],
                    [0.375]])
         """
 
     def transform(self, values):
@@ -225,15 +232,15 @@
 
         Example:
             The example below shows simple usage case where an ``IntHyperParam`` is being imported,
             instantiated with a range from 1 to 4, and its method ``transform`` is being called
             three times with a single scalar value, an array of two valid values and a 2D array
             with 1 dimension.
 
-            >>> from btb.tuning.hyperparams.numerical import IntHyperParam
+            >>> from baytune.tuning.hyperparams.numerical import IntHyperParam
             >>> ihp = IntHyperParam(min=1, max=4)
             >>> ihp.transform(1)
             array([[0.125]])
             >>> ihp.transform([1, 2])
             array([[0.125],
                    [0.375]])
             >>> ihp.transform([[1], [2]])
@@ -242,18 +249,18 @@
         """
 
         if not isinstance(values, np.ndarray):
             values = np.asarray(values)
 
         dimensions = len(values.shape)
         if dimensions > 2:
-            raise ValueError('Too many dimensions.')
+            raise ValueError("Too many dimensions.")
 
         elif dimensions < 2:
             values = values.reshape(-1, 1)
 
         if values.shape[1] > 1:
-            raise ValueError('Only one column is supported.')
+            raise ValueError("Only one column is supported.")
 
         self._within_hyperparam_space(values)
 
         return self._transform(values)
```

### Comparing `baytune-0.4.0/btb/tuning/hyperparams/boolean.py` & `baytune-0.5.0/baytune/tuning/hyperparams/boolean.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Package where the BooleanHyperParam class is defined."""
 
 import numpy as np
 
-from btb.tuning.hyperparams.base import BaseHyperParam
+from baytune.tuning.hyperparams.base import BaseHyperParam
 
 
 class BooleanHyperParam(BaseHyperParam):
     """BooleanHyperParam class.
 
     The BooleanHyperParam class is responsible for the transformation of boolean values in
     to normalized search space of :math:`[0, 1]`, providing the ability to sample values of those
@@ -25,18 +25,20 @@
     dimensions = 1
     cardinality = 2
 
     def __init__(self, default=False):
         self.default = default
 
     def _within_hyperparam_space(self, values):
-        if values.dtype is not np.dtype('bool'):
+        if values.dtype is not np.dtype("bool"):
             # values is expected to be np.ndarray(n, 1) [[False], [True]]
             if not all(isinstance(value[0], bool) for value in values):
-                raise ValueError('Values: {} not within hyperparameter space.'.format(values))
+                raise ValueError(
+                    "Values: {} not within hyperparameter space.".format(values)
+                )
 
     def _inverse_transform(self, values):
         """Invert one or more search space values.
 
         Converts a ``numpy.ndarray`` with normalized values from the search space :math:`{0, 1}`
         to the original space of ``True`` and ``False`` by casting those values to ``boolean``.
 
@@ -114,8 +116,8 @@
                    [1]])
         """
         sampled = np.random.random((n_samples, self.dimensions))
 
         return np.round(sampled).astype(int)
 
     def __repr__(self):
-        return 'BooleanHyperParam(default={})'.format(self.default)
+        return "BooleanHyperParam(default={})".format(self.default)
```

### Comparing `baytune-0.4.0/btb/tuning/hyperparams/categorical.py` & `baytune-0.5.0/baytune/tuning/hyperparams/categorical.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Package where the CategoricalHyperParamClass is defined."""
 
 from copy import deepcopy
 
 import numpy as np
 from sklearn.preprocessing import OneHotEncoder
 
-from btb.tuning.hyperparams.base import BaseHyperParam
+from baytune.tuning.hyperparams.base import BaseHyperParam
 
 
 class CategoricalHyperParam(BaseHyperParam):
     r"""CategoricalHyperParam Class.
 
     The CategoricalHyperParam class is responsible for the transform of categorical values
     in to normalized search space and provides the inverse transform from search space to
@@ -37,35 +37,37 @@
 
         Creates an instance with a list of ``choices`` and fit an instance of
         ``sklearn.preprocessing.OneHotEncoder`` with those values.
         """
         if default is self.NO_DEFAULT:
             self.default = choices[0]
         elif default not in choices:
-            raise ValueError('`default` not within `choices`')
+            raise ValueError("`default` not within `choices`")
         else:
             self.default = default
 
         self.choices = deepcopy(choices)
         self.dimensions = len(choices)
         self.cardinality = self.dimensions
-        choices = np.array(choices, dtype='object')
-        self._encoder = OneHotEncoder(categories=[choices], sparse=False)
+        choices = np.array(choices, dtype="object")
+        self._encoder = OneHotEncoder(categories=[choices], sparse_output=False)
         self._encoder.fit(choices.reshape(-1, 1))
 
     def _within_hyperparam_space(self, values):
         mask = np.isin(values, self.choices)
 
         if not mask.all():
             if not isinstance(values, np.ndarray):
                 values = np.asarray(values)
 
             not_in_space = values[~mask].tolist()
             raise ValueError(
-                'Values found outside of the valid space {}: {}'.format(self.choices, not_in_space)
+                "Values found outside of the valid space {}: {}".format(
+                    self.choices, not_in_space
+                )
             )
 
     def _inverse_transform(self, values):
         """Invert one or more values.
 
         Converts a ``numpy.ndarray`` with normalized values from the search space to the original
         hyperparameter space of ``self.choices``.
@@ -91,15 +93,15 @@
             >>> instance._inverse_transform(np.array([[1, 0, 0], [0, 0, 1]]))
             array([['Cat'],
                    ['Tiger']])
         """
         if len(values.shape) == 1:
             values = values.reshape(1, -1)
 
-        return self._encoder.inverse_transform(values.astype('object'))
+        return self._encoder.inverse_transform(values.astype("object"))
 
     def _transform(self, values):
         """Transform one or more categorical values.
 
         Encodes one or more categorical values in to the normalized search space of
         :math:`[0, 1]^K` by using ``sklearn.preprocessing.OneHotEncoder`` that has been
         fitted during the instantiation.
@@ -123,15 +125,15 @@
             >>> instance = CategoricalHyperParam(choices=['Cat', 'Dog', 'Tiger'])
             >>> instance._transform(np.array([['Cat']]))
             array([[1, 0, 0]])
             >>> instance._transform(np.array([['Cat'], ['Tiger']]))
             array([[1, 0, 0],
                    [0, 0, 1]])
         """
-        return self._encoder.transform(values.astype('object')).astype(int)
+        return self._encoder.transform(values.astype("object")).astype(int)
 
     def sample(self, n_samples):
         """Generate sample values in the hyperparameter search space of ``[0, 1]^K``.
 
         Args:
             n_samples (int):
                 Number of values to sample.
@@ -156,8 +158,10 @@
         indexes = np.argmax(randomized_values, axis=1)
 
         sampled = [self.choices[index] for index in indexes]
 
         return self.transform(sampled)
 
     def __repr__(self):
-        return 'CategoricalHyperParam(choices={}, default={})'.format(self.choices, self.default)
+        return "CategoricalHyperParam(choices={}, default={})".format(
+            self.choices, self.default
+        )
```

### Comparing `baytune-0.4.0/btb/tuning/hyperparams/numerical.py` & `baytune-0.5.0/baytune/tuning/hyperparams/numerical.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 
 """Package where the NumericalHyperParam class and it's childs are defined."""
 
 import sys
 
 import numpy as np
 
-from btb.tuning.hyperparams.base import BaseHyperParam
+from baytune.tuning.hyperparams.base import BaseHyperParam
 
 
 class NumericalHyperParam(BaseHyperParam):
     """NumericalHyperParam class.
 
     The NumericalHyperParam class defines an abstraction to hyperparameters which ranges are
     defined by a numerical value and can take any number within that range.
     """
 
     dimensions = 1
 
     def _within_range(self, values, min=0, max=1):
         if (values < min).any() or (values > max).any():
-            raise ValueError('Value not within range [{}, {}]: {}'.format(min, max, values))
+            raise ValueError(
+                "Value not within range [{}, {}]: {}".format(min, max, values)
+            )
 
 
 class FloatHyperParam(NumericalHyperParam):
     """FloatHyperParam class.
 
     The FloatHyperParam class represents a single hyperparameter within a range of ``float``
     numbers, where ``min`` and ``max`` can take as value any float number within that range,
@@ -54,27 +56,30 @@
 
         include_max (bool):
             Either or not to include the maximum value in the search space.
     """
 
     cardinality = np.inf
 
-    def __init__(self, min=None, max=None, default=None, include_min=True, include_max=True):
-
+    def __init__(
+        self, min=None, max=None, default=None, include_min=True, include_max=True
+    ):
         self.include_min = include_min
         self.include_max = include_max
 
         if min is None or min == -np.inf:
             min = sys.float_info.min
 
         if max is None or max == np.inf:
             max = sys.float_info.max
 
         if min >= max:
-            raise ValueError('The ``min`` value can not be greater or equal to ``max`` value.')
+            raise ValueError(
+                "The ``min`` value can not be greater or equal to ``max`` value."
+            )
 
         if default is None:
             self.default = float(min)
         else:
             self.default = float(default)
 
         self.min = float(min)
@@ -168,16 +173,18 @@
             array([[0.52058728],
                    [0.00582452]])
         """
         return np.random.random((n_samples, self.dimensions))
 
     def __repr__(self):
         args = (self.min, self.max, self.default, self.include_min, self.include_max)
-        args = 'min={}, max={}, default={}, include_min={}, include_max={}'.format(*args)
-        return 'FloatHyperParam({})'.format(args)
+        args = "min={}, max={}, default={}, include_min={}, include_max={}".format(
+            *args
+        )
+        return "FloatHyperParam({})".format(args)
 
 
 class IntHyperParam(NumericalHyperParam):
     """IntHyperParam class.
 
     The IntHyperParam class represents a single hyperparameter within an range of ``int``
     numbers, where ``min`` and ``max`` can take as value any ``int`` number that compose this range
@@ -210,42 +217,52 @@
 
         include_max (bool):
             Either or not to include the maximum value in the search space.
     """
 
     dimensions = 1
 
-    def __init__(self, min=None, max=None, default=None,
-                 include_min=True, include_max=True, step=1):
-
+    def __init__(
+        self,
+        min=None,
+        max=None,
+        default=None,
+        include_min=True,
+        include_max=True,
+        step=1,
+    ):
         self.include_min = include_min
         self.include_max = include_max
 
         if min is None or min == -np.inf:
             min = -(sys.maxsize / 2)
 
         if max is None or max == np.inf:
             max = sys.maxsize / 2
 
         if min >= max:
-            raise ValueError('The `min` value can not be greater or equal to `max` value.')
+            raise ValueError(
+                "The `min` value can not be greater or equal to `max` value."
+            )
 
         if default is None:
             self.default = min
         else:
             self.default = int(default)
 
         self.min = int(min) if include_min else int(min) + 1
         self.max = int(max) if include_max else int(max) - 1
         self.step = step
         self.cardinality = ((self.max - self.min) // step) + 1
 
         if (self.max - self.min) % self.step:
             raise ValueError(
-                "Invalid step of {} for values inside [{}, {}]".format(step, self.min, self.max)
+                "Invalid step of {} for values inside [{}, {}]".format(
+                    step, self.min, self.max
+                )
             )
 
         self.interval = self.step / (self.max - self.min + self.step)
 
     def _inverse_transform(self, values):
         """Invert one or more search space values.
 
@@ -342,10 +359,19 @@
         """
         sampled = np.random.random((n_samples, self.dimensions))
         inverted = self._inverse_transform(sampled)
 
         return self._transform(inverted)
 
     def __repr__(self):
-        args = (self.min, self.max, self.default, self.include_min, self.include_max, self.step)
-        args = 'min={}, max={}, default={}, include_min={}, include_max={}, step={}'.format(*args)
-        return 'IntHyperParam({})'.format(args)
+        args = (
+            self.min,
+            self.max,
+            self.default,
+            self.include_min,
+            self.include_max,
+            self.step,
+        )
+        args = "min={}, max={}, default={}, include_min={}, include_max={}, step={}".format(
+            *args
+        )
+        return "IntHyperParam({})".format(args)
```

### Comparing `baytune-0.4.0/btb/tuning/metamodels/base.py` & `baytune-0.5.0/baytune/tuning/metamodels/base.py`

 * *Files identical despite different names*

### Comparing `baytune-0.4.0/btb/tuning/metamodels/gaussian_process.py` & `baytune-0.5.0/baytune/tuning/metamodels/gaussian_process.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 
-import numpy
+import numpy as np
 import scipy
 from copulas import EPSILON
 from copulas.univariate import Univariate
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.gaussian_process.kernels import RBF
 
-from btb.tuning.metamodels.base import BaseMetaModel
+from baytune.tuning.metamodels.base import BaseMetaModel
 
 
 class GaussianProcessMetaModel(BaseMetaModel):
     """GaussianProcessMetaModel class.
 
     This class represents a meta-model using an underlying ``GaussianProcessRegressor`` from
     ``sklearn.gaussian_process``.
@@ -20,29 +20,28 @@
         _MODEL_KWARGS (dict):
             Dictionary with the default ``kwargs`` for the ``GaussianProcessRegressor``
             instantiation.
         _MODEL_CLASS (type):
             Class to be instantiated and used for the ``self._model`` instantiation. In
             this case ``sklearn.gaussian_process.GaussainProcessRegressor``
     """
+
     _MODEL_CLASS = GaussianProcessRegressor
 
-    _MODEL_KWARGS_DEFAULT = {
-        'normalize_y': True
-    }
+    _MODEL_KWARGS_DEFAULT = {"normalize_y": True}
 
     def __init_metamodel__(self, length_scale=1):
         if self._model_kwargs is None:
             self._model_kwargs = {}
 
-        self._model_kwargs['kernel'] = RBF(length_scale=length_scale)
+        self._model_kwargs["kernel"] = RBF(length_scale=length_scale)
 
     def _predict(self, candidates):
         predictions = self._model_instance.predict(candidates, return_std=True)
-        return numpy.column_stack(predictions)
+        return np.column_stack(predictions)
 
 
 class GaussianCopulaProcessMetaModel(GaussianProcessMetaModel):
     """GaussianCopulaProcessMetaModel class.
 
     This class represents a meta-model using an underlying ``GaussianProcessRegressor`` from
     ``sklearn.gaussian_process`` applying ``copulas.univariate.Univariate`` transformations
@@ -62,22 +61,25 @@
         _MODEL_KWARGS (dict):
             Dictionary with the default ``kwargs`` for the ``GaussianProcessRegressor``
             instantiation.
         _MODEL_CLASS (type):
             Class to be instantiated and used for the ``self._model`` instantiation. In
             this case ``sklearn.gaussian_process.GaussainProcessRegressor``
     """
+
     def _transform(self, trials):
         transformed = []
         for column, distribution in zip(trials.T, self._distributions):
             transformed.append(
-                scipy.stats.norm.ppf(distribution.cdf(column).clip(0 + EPSILON, 1 - EPSILON))
+                scipy.stats.norm.ppf(
+                    distribution.cdf(column).clip(0 + EPSILON, 1 - EPSILON)
+                )
             )
 
-        return numpy.column_stack(transformed)
+        return np.column_stack(transformed)
 
     def _fit(self, trials, scores):
         self._distributions = []
         for column in trials.T:
             distribution = Univariate()
             distribution.fit(column)
             self._distributions.append(distribution)
@@ -92,9 +94,11 @@
         )
 
         super()._fit(trans_trials, trans_scores)
 
     def _predict(self, candidates):
         trans_candidates = self._transform(candidates)
         predicted = super()._predict(trans_candidates)
-
-        return self._score_distribution.ppf(scipy.stats.norm.cdf(predicted))
+        cdf = scipy.stats.norm.cdf(predicted)
+        if len(cdf.shape) == 2:
+            cdf = cdf[:, 0]
+        return self._score_distribution.ppf(cdf)
```

### Comparing `baytune-0.4.0/btb/tuning/tunable.py` & `baytune-0.5.0/baytune/tuning/tunable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import pandas as pd
 
-from btb.tuning.hyperparams.boolean import BooleanHyperParam
-from btb.tuning.hyperparams.categorical import CategoricalHyperParam
-from btb.tuning.hyperparams.numerical import FloatHyperParam, IntHyperParam
+from baytune.tuning.hyperparams.boolean import BooleanHyperParam
+from baytune.tuning.hyperparams.categorical import CategoricalHyperParam
+from baytune.tuning.hyperparams.numerical import FloatHyperParam, IntHyperParam
 
 """Package where the Tunable class is defined."""
 
 
 class Tunable:
     """Tunable class.
 
@@ -23,14 +23,15 @@
             Int or ``np.inf`` amount that indicates the number of combinations possible for this
             tunable.
 
     Args:
         hyperparams (dict):
             Dictionary object that contains the name and the hyperparameter asociated to it.
     """
+
     hyperparams = None
     names = None
     dimensions = 0
     cardinality = 1
 
     def __init__(self, hyperparams):
         self.hyperparams = hyperparams
@@ -55,17 +56,17 @@
                 2D array of shape ``(len(values), dimensions)`` where ``dimensions`` is the sum of
                 dimensions from all the ``HyperParams`` that compose this ``tunable``.
 
         Example:
             The example below shows a simple usage of a Tunable class which will transform a valid
             data from a 2D list and a ``numpy.ndarray`` is being returned.
 
-            >>> from btb.tuning.hyperparams.boolean import BooleanHyperParam
-            >>> from btb.tuning.hyperparams.categorical import CategoricalHyperParam
-            >>> from btb.tuning.hyperparams.numerical import IntHyperParam
+            >>> from baytune.tuning.hyperparams.boolean import BooleanHyperParam
+            >>> from baytune.tuning.hyperparams.categorical import CategoricalHyperParam
+            >>> from baytune.tuning.hyperparams.numerical import IntHyperParam
             >>> chp = CategoricalHyperParam(['cat', 'dog'])
             >>> bhp = BooleanHyperParam()
             >>> ihp = IntHyperParam(1, 10)
             >>> hyperparams = {
             ...     'chp': chp,
             ...     'bhp': bhp,
             ...     'ihp': ihp
@@ -118,17 +119,17 @@
         Returns:
             pandas.DataFrame
 
         Example:
             The example below shows a simple usage of a Tunable class which will inverse transform
             a valid data from a 2D list and a ``pandas.DataFrame`` will be returned.
 
-            >>> from btb.tuning.hyperparams.boolean import BooleanHyperParam
-            >>> from btb.tuning.hyperparams.categorical import CategoricalHyperParam
-            >>> from btb.tuning.hyperparams.numerical import IntHyperParam
+            >>> from baytune.tuning.hyperparams.boolean import BooleanHyperParam
+            >>> from baytune.tuning.hyperparams.categorical import CategoricalHyperParam
+            >>> from baytune.tuning.hyperparams.numerical import IntHyperParam
             >>> chp = CategoricalHyperParam(['cat', 'dog'])
             >>> bhp = BooleanHyperParam()
             >>> ihp = IntHyperParam(1, 10)
             >>> hyperparams = {
             ...     'chp': chp,
             ...     'bhp': bhp,
             ...     'ihp': ihp
@@ -147,17 +148,17 @@
         inverse_transform = list()
 
         for value in values:
             transformed = list()
 
             for name in self.names:
                 hyperparam = self.hyperparams[name]
-                item = value[:hyperparam.dimensions]
+                item = value[: hyperparam.dimensions]
                 transformed.append(hyperparam.inverse_transform(item))
-                value = value[hyperparam.dimensions:]
+                value = value[hyperparam.dimensions :]
 
             transformed = np.array(transformed, dtype=object)
             inverse_transform.append(np.concatenate(transformed, axis=1))
 
         return pd.DataFrame(np.concatenate(inverse_transform), columns=self.names)
 
     def sample(self, n_samples):
@@ -172,17 +173,17 @@
                 2D array with shape of ``(n_samples, dimensions)`` where ``dimensions``  is the
                 sum of dimensions from all the ``HyperParams`` that compose this ``tunable``.
 
         Example:
             The example below shows a simple usage of a Tunable class which will generate 2
             samples by calling it's sample method. This will return a ``numpy.ndarray``.
 
-            >>> from btb.tuning.hyperparams.boolean import BooleanHyperParam
-            >>> from btb.tuning.hyperparams.categorical import CategoricalHyperParam
-            >>> from btb.tuning.hyperparams.numerical import IntHyperParam
+            >>> from baytune.tuning.hyperparams.boolean import BooleanHyperParam
+            >>> from baytune.tuning.hyperparams.categorical import CategoricalHyperParam
+            >>> from baytune.tuning.hyperparams.numerical import IntHyperParam
             >>> chp = CategoricalHyperParam(['cat', 'dog'])
             >>> bhp = BooleanHyperParam()
             >>> ihp = IntHyperParam(1, 10)
             >>> hyperparams = {
             ...     'chp': chp,
             ...     'bhp': bhp,
             ...     'ihp': ihp
@@ -199,16 +200,15 @@
             samples.append(items)
 
         return np.concatenate(samples, axis=1)
 
     def get_defaults(self):
         """Return the default combination for the hyperparameters."""
         return {
-            name: hyperparam.default
-            for name, hyperparam in self.hyperparams.items()
+            name: hyperparam.default for name, hyperparam in self.hyperparams.items()
         }
 
     @classmethod
     def from_dict(cls, dict_hyperparams):
         """Create an instance from a dictionary containing information over hyperparameters.
 
         Class method that creates an instance from a dictionary that describes the type of a
@@ -235,40 +235,44 @@
 
         Returns:
             Tunable:
                 A ``Tunable`` instance with the given hyperparameters.
         """
 
         if not isinstance(dict_hyperparams, dict):
-            raise TypeError('Hyperparams must be a dictionary.')
+            raise TypeError("Hyperparams must be a dictionary.")
 
         hyperparams = {}
 
         for name, hyperparam in dict_hyperparams.items():
-            hp_type = hyperparam['type']
-            hp_default = hyperparam.get('default')
+            hp_type = hyperparam["type"]
+            hp_default = hyperparam.get("default")
 
-            if hp_type == 'int':
-                hp_range = hyperparam.get('range') or hyperparam.get('values')
+            if hp_type == "int":
+                hp_range = hyperparam.get("range") or hyperparam.get("values")
                 hp_min = min(hp_range) if hp_range else None
                 hp_max = max(hp_range) if hp_range else None
                 hp_instance = IntHyperParam(min=hp_min, max=hp_max, default=hp_default)
 
-            elif hp_type == 'float':
-                hp_range = hyperparam.get('range') or hyperparam.get('values')
+            elif hp_type == "float":
+                hp_range = hyperparam.get("range") or hyperparam.get("values")
                 hp_min = min(hp_range)
                 hp_max = max(hp_range)
-                hp_instance = FloatHyperParam(min=hp_min, max=hp_max, default=hp_default)
+                hp_instance = FloatHyperParam(
+                    min=hp_min, max=hp_max, default=hp_default
+                )
 
-            elif hp_type == 'bool':
+            elif hp_type == "bool":
                 hp_instance = BooleanHyperParam(default=hp_default)
 
-            elif hp_type == 'str':
-                hp_choices = hyperparam.get('range') or hyperparam.get('values')
-                hp_instance = CategoricalHyperParam(choices=hp_choices, default=hp_default)
+            elif hp_type == "str":
+                hp_choices = hyperparam.get("range") or hyperparam.get("values")
+                hp_instance = CategoricalHyperParam(
+                    choices=hp_choices, default=hp_default
+                )
 
             hyperparams[name] = hp_instance
 
         return cls(hyperparams)
 
     def __repr__(self):
-        return 'Tunable({})'.format(self.hyperparams)
+        return "Tunable({})".format(self.hyperparams)
```

### Comparing `baytune-0.4.0/btb/tuning/tuners/base.py` & `baytune-0.5.0/baytune/tuning/tuners/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,59 +3,61 @@
 """Package where the BaseTuner class and BaseMetaModelTuner are defined."""
 
 import logging
 from abc import abstractmethod
 
 import numpy as np
 
-from btb.tuning.acquisition.base import BaseAcquisition
-from btb.tuning.metamodels.base import BaseMetaModel
+from baytune.tuning.acquisition.base import BaseAcquisition
+from baytune.tuning.metamodels.base import BaseMetaModel
 
 LOGGER = logging.getLogger(__name__)
 
 
 class StopTuning(Exception):
     pass
 
 
 class BaseTuner:
     """BaseTuner class.
 
     BaseTuner class is the abstract representation of a tuner that is not based on a model.
 
     Attributes:
-        tunable (btb.tuning.tunable.Tunable):
+        tunable (baytune.tuning.tunable.Tunable):
             Instance of a tunable class containing hyperparameters to be tuned.
         trials (numpy.ndarray):
             A ``numpy.ndarray`` with shape ``(n, self.tunable.dimensions)`` where ``n`` is the
             number of trials recorded.
         raw_scores (numpy.ndarray):
             A ``numpy.ndarray`` with shape ``(n, 1)`` where ``n`` is the number of scores recorded.
         scores (numpy.ndarray):
             A ``numpy.ndarray`` with shape ``(n, 1)`` where ``n`` is the number of normalized
             scores recorded.
 
     Args:
-        tunable (btb.tuning.tunable.Tunable):
+        tunable (baytune.tuning.tunable.Tunable):
             Instance of a tunable class containing hyperparameters to be tuned.
         maximize (bool):
             If ``True`` the scores are interpreted as bigger is better, if ``False`` then smaller
             is better. Defaults to ``True``.
     """
 
     def __init__(self, tunable, maximize=True):
         self.tunable = tunable
-        self.trials = np.empty((0, self.tunable.dimensions), dtype=np.float)
+        self.trials = np.empty((0, self.tunable.dimensions), dtype=np.float64)
         self._trials_set = set()
-        self.raw_scores = np.empty((0, 1), dtype=np.float)
-        self.scores = np.empty((0, 1), dtype=np.float)
+        self.raw_scores = np.empty((0, 1), dtype=np.float64)
+        self.scores = np.empty((0, 1), dtype=np.float64)
         self.maximize = maximize
         LOGGER.debug(
-            ('Creating %s instance with %s hyperparameters and cardinality %s.'),
-            self.__class__.__name__, len(self.tunable.hyperparams), self.tunable.cardinality
+            ("Creating %s instance with %s hyperparameters and cardinality %s."),
+            self.__class__.__name__,
+            len(self.tunable.hyperparams),
+            self.tunable.cardinality,
         )
 
     def _check_proposals(self, num_proposals):
         """Validate ``num_proposals`` with ``self.tunable.cardinality`` and ``self.trials``.
 
         Raises:
             StopTuning:
@@ -66,32 +68,32 @@
                 trials is the same as the amount of combinations available for ``self.tunable``.
             StopTuning:
                 A ``StopTuning`` exception is being produced if the unique amount of recorded
                 trials is the same as the amount of combinations available for ``self.tunable``.
         """
         if num_proposals > self.tunable.cardinality:
             raise StopTuning(
-                'The number of proposals requested is bigger than the combinations: {} of the'
-                '``tunable``. Use ``allow_duplicates=True``, if you would like to generate that'
-                'amount of combinations.'.format(self.tunable.cardinality)
+                "The number of proposals requested is bigger than the combinations: {} of the"
+                "``tunable``. Use ``allow_duplicates=True``, if you would like to generate that"
+                "amount of combinations.".format(self.tunable.cardinality)
             )
 
         num_tried = len(self._trials_set)
         if num_tried == self.tunable.cardinality:
             raise StopTuning(
-                'All of the possible combinations where recorded. Use ``allow_duplicates=True``'
-                'to keep generating combinations.'
+                "All of the possible combinations where recorded. Use ``allow_duplicates=True``"
+                "to keep generating combinations."
             )
 
         if num_tried + num_proposals > self.tunable.cardinality:
             raise StopTuning(
-                'The maximum amount of new proposed combinations will exceed the amount of'
-                'possible combinations, either use ``num_proposals={}`` to generate the remaining'
-                'combinations or ``allow_duplicates=True`` to keep generating more'
-                'combinations.'.format(self.tunable.cardinality - num_tried)
+                "The maximum amount of new proposed combinations will exceed the amount of"
+                "possible combinations, either use ``num_proposals={}`` to generate the remaining"
+                "combinations or ``allow_duplicates=True`` to keep generating more"
+                "combinations.".format(self.tunable.cardinality - num_tried)
             )
 
     def _sample(self, num_proposals, allow_duplicates):
         """Generate a ``numpy.ndarray`` of valid proposals.
 
         Generates ``num_proposals`` of valid combinations by generating ``proposals`` until
         ``len(valid_proposals) == num_proposals`` different from the ones that have been recorded.
@@ -174,18 +176,18 @@
 
         Example:
             The example below shows simple usage case where an ``UniformTuner`` is being imported,
             instantiated with a ``tunable`` object and it's method propose is being called
             three times, first with a single proposal, a second with two proposals forcing them to
             be different and once where the values can be repeated.
 
-            >>> from btb.tuning.tunable import Tunable
-            >>> from btb.tuning.hyperparams import BooleanHyperParam
-            >>> from btb.tuning.hyperparams import CategoricalHyperParam
-            >>> from btb.tuning.tuners import UniformTuner
+            >>> from baytune.tuning.tunable import Tunable
+            >>> from baytune.tuning.hyperparams import BooleanHyperParam
+            >>> from baytune.tuning.hyperparams import CategoricalHyperParam
+            >>> from baytune.tuning.tuners import UniformTuner
             >>> bhp = BooleanHyperParam()
             >>> chp = CategoricalHyperParam(['cat', 'dog'])
             >>> tunable = Tunable({'bhp': bhp, 'chp': chp})
             >>> tuner = UniformTuner(tunable)
             >>> tuner.propose(1)
             {'bhp': True, 'chp': 'dog'}
             >>> tuner.propose(2)
@@ -196,15 +198,15 @@
 
         if not allow_duplicates:
             self._check_proposals(n)
 
         proposed = self._propose(n, allow_duplicates)
 
         hyperparameters = self.tunable.inverse_transform(proposed)
-        hyperparameters = hyperparameters.to_dict(orient='records')
+        hyperparameters = hyperparameters.to_dict(orient="records")
 
         if n == 1:
             hyperparameters = hyperparameters[0]
 
         return hyperparameters
 
     def record(self, trials, scores):
@@ -228,72 +230,71 @@
                 ``len(scores)``.
 
         Example:
             The example below shows simple usage case where an ``UniformTuner`` is being imported,
             instantiated with a ``tunable`` object and it's method record is being called two times
             with valid trials and scores.
 
-            >>> from btb.tuning.tunable import Tunable
-            >>> from btb.tuning.hyperparams import BooleanHyperParam
-            >>> from btb.tuning.hyperparams import CategoricalHyperParam
-            >>> from btb.tuning.tuners import UniformTuner
+            >>> from baytune.tuning.tunable import Tunable
+            >>> from baytune.tuning.hyperparams import BooleanHyperParam
+            >>> from baytune.tuning.hyperparams import CategoricalHyperParam
+            >>> from baytune.tuning.tuners import UniformTuner
             >>> bhp = BooleanHyperParam()
             >>> chp = CategoricalHyperParam(['cat', 'dog'])
             >>> tunable = Tunable({'bhp': bhp, 'chp': chp})
             >>> tuner = UniformTuner(tunable)
             >>> tuner.record({'bhp': True, 'chp': 'cat'}, 0.8)
             >>> trials = [{'bhp': False, 'chp': 'cat'}, {'bhp': True, 'chp': 'dog'}]
             >>> scores = [0.8, 0.1]
             >>> tuner.record(trials, scores)
         """
 
         trials = self.tunable.transform(trials)
         scores = scores if isinstance(scores, (list, np.ndarray)) else [scores]
 
         if len(trials) != len(scores):
-            raise ValueError('The amount of trials must be equal to the amount of scores.')
+            raise ValueError(
+                "The amount of trials must be equal to the amount of scores."
+            )
 
         self.trials = np.append(self.trials, trials, axis=0)
         self._trials_set.update(map(tuple, trials))
         self.raw_scores = np.append(self.raw_scores, scores)
         self.scores = self.raw_scores if self.maximize else -self.raw_scores
 
     def __str__(self):
         return (
-            "{}\n"
-            "  hyperparameters: {}\n"
-            "  dimensions: {}\n"
-            "  cardinality: {}"
+            "{}\n" "  hyperparameters: {}\n" "  dimensions: {}\n" "  cardinality: {}"
         ).format(
             self.__class__.__name__,
             len(self.tunable.hyperparams),
             self.tunable.dimensions,
-            self.tunable.cardinality
+            self.tunable.cardinality,
         )
 
 
 class BaseMetaModelTuner(BaseTuner, BaseMetaModel, BaseAcquisition):
     """BaseMetaModelTuner class.
 
     BaseMetaModelTuner class is the abstract representation of a tuner that is based
     on a model and an ``Acquisition``. This model will try to `predict` the
     score that will be obtained with the proposed parameters by being trained
     over the ``self.trials`` and ``self.raw_scores`` recorded by the user.
 
     Attributes:
-        tunable (btb.tuning.tunable.Tunable):
+        tunable (baytune.tuning.tunable.Tunable):
             Instance of a tunable class containing hyperparameters to be tuned.
         trials (numpy.ndarray):
             A ``numpy.ndarray`` with shape ``(n, self.tunable.dimensions)`` where ``n`` is the
             number of trials recorded.
         scores (numpy.ndarray):
             A ``numpy.ndarray`` with shape ``(n, 1)`` where ``n`` is the number of scores recorded.
 
     Args:
-        tunable (btb.tuning.tunable.Tunable):
+        tunable (baytune.tuning.tunable.Tunable):
             Instance of a tunable class containing hyperparameters to be tuned.
         num_candidates (int):
             Number of samples to generate and select the best of it for each proposal. Defaults to
             1000.
         maximize (bool):
             If ``True`` the model will understand that the score bigger is better, if ``False``
             the smaller is better. Defaults to ``True``.
@@ -310,16 +311,18 @@
         self.min_trials = min_trials
         super().__init__(tunable, maximize)
         self.__init_metamodel__(**(self._metamodel_kwargs or dict()))
         self.__init_acquisition__(**(self._acquisition_kwargs or dict()))
 
     def _propose(self, num_proposals, allow_duplicates):
         if self.min_trials > len(self._trials_set):
-            LOGGER.debug('Not enough samples recorded to generate predictions, '
-                         'generating random proposal.')
+            LOGGER.debug(
+                "Not enough samples recorded to generate predictions, "
+                "generating random proposal."
+            )
             return self._sample(num_proposals, allow_duplicates)
 
         num_samples = num_proposals * self.num_candidates
         if not allow_duplicates:
             remaining = self.tunable.cardinality - len(self._trials_set)
             num_samples = min(remaining, num_samples)
 
@@ -353,24 +356,24 @@
                 ``len(scores)``.
 
         Example:
             The example below shows simple usage case where an ``UniformTuner`` is being imported,
             instantiated with a ``tunable`` object and it's method record is being called two times
             with valid trials and scores.
 
-            >>> from btb.tuning.tunable import Tunable
-            >>> from btb.tuning.hyperparams import BooleanHyperParam
-            >>> from btb.tuning.hyperparams import CategoricalHyperParam
-            >>> from btb.tuning.tuners import UniformTuner
+            >>> from baytune.tuning.tunable import Tunable
+            >>> from baytune.tuning.hyperparams import BooleanHyperParam
+            >>> from baytune.tuning.hyperparams import CategoricalHyperParam
+            >>> from baytune.tuning.tuners import UniformTuner
             >>> bhp = BooleanHyperParam()
             >>> chp = CategoricalHyperParam(['cat', 'dog'])
             >>> tunable = Tunable({'bhp': bhp, 'chp': chp})
             >>> tuner = UniformTuner(tunable)
             >>> tuner.record({'bhp': True, 'chp': 'cat'}, 0.8)
             >>> trials = [{'bhp': False, 'chp': 'cat'}, {'bhp': True, 'chp': 'dog'}]
             >>> scores = [0.8, 0.1]
             >>> tuner.record(trials, scores)
         """
         super().record(trials, scores)
         if len(self.trials) >= self.min_trials:
-            LOGGER.debug('Fitting the model with %s samples.' % len(self.trials))
+            LOGGER.debug("Fitting the model with %s samples." % len(self.trials))
             self._fit(self.trials, self.scores)
```

### Comparing `baytune-0.4.0/btb/tuning/tuners/gaussian_process.py` & `baytune-0.5.0/baytune/tuning/tuners/gaussian_process.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,114 +1,168 @@
 # -*- coding: utf-8 -*-
 
 """Package where the tuners based on GaussianProcessMetaModel are defined."""
 
-from btb.tuning.acquisition.expected_improvement import ExpectedImprovementAcquisition
-from btb.tuning.acquisition.predicted_score import PredictedScoreAcquisition
-from btb.tuning.metamodels.gaussian_process import (
-    GaussianCopulaProcessMetaModel, GaussianProcessMetaModel)
-from btb.tuning.tuners.base import BaseMetaModelTuner
+from baytune.tuning.acquisition.expected_improvement import (
+    ExpectedImprovementAcquisition,
+)
+from baytune.tuning.acquisition.predicted_score import PredictedScoreAcquisition
+from baytune.tuning.metamodels.gaussian_process import (
+    GaussianCopulaProcessMetaModel,
+    GaussianProcessMetaModel,
+)
+from baytune.tuning.tuners.base import BaseMetaModelTuner
 
 
 class GPTuner(GaussianProcessMetaModel, PredictedScoreAcquisition, BaseMetaModelTuner):
     """Gaussian Process Tuner.
 
     This class uses a ``GaussianProcessRegressor`` model from the ``sklearn.gaussian_process``
     package, using a ``numpy.argmax`` function to return the better configurations predicted
     from the model.
     """
-    def __init__(self, tunable, maximize=True, num_candidates=1000,
-                 min_trials=5, length_scale=0.1):
+
+    def __init__(
+        self,
+        tunable,
+        maximize=True,
+        num_candidates=1000,
+        min_trials=5,
+        length_scale=0.1,
+    ):
         """Create an instance of ``GPTuner``.
 
         Args:
-            tunable (btb.tuning.tunable.Tunable):
+            tunable (baytune.tuning.tunable.Tunable):
                 Instance of a tunable class containing hyperparameters to be tuned.
             num_candidates (int):
                 Number of samples to generate and select the best of it for each proposal.
                 Defaults to 1000.
             maximize (bool):
                 If ``True`` the model will understand that the score bigger is better, if ``False``
                 the smaller is better. Defaults to ``True``.
             min_trials (int):
                 Number of recorded ``trials`` needed to perform a fitting over the model.
                 Defaults to 2.
             length_scale (float or array):
                 A float or array with shape ``(n_features,)``, used for the default ``RBF`` kernel.
         """
-        self._metamodel_kwargs = {'length_scale': length_scale}
+        self._metamodel_kwargs = {"length_scale": length_scale}
         super().__init__(tunable, maximize, num_candidates, min_trials)
 
     def __repr__(self):
-        length_scale = self._metamodel_kwargs.get('length_scale')
-        args = (self.tunable, self.maximize, self.num_candidates, self.min_trials, length_scale)
-        return ('GPTuner(tunable={}, maximize={}, '
-                'num_candidates={}, min_trials={}, '
-                'length_scale={})').format(*args)
-
-
-class GPEiTuner(GaussianProcessMetaModel, ExpectedImprovementAcquisition, BaseMetaModelTuner):
+        length_scale = self._metamodel_kwargs.get("length_scale")
+        args = (
+            self.tunable,
+            self.maximize,
+            self.num_candidates,
+            self.min_trials,
+            length_scale,
+        )
+        return (
+            "GPTuner(tunable={}, maximize={}, "
+            "num_candidates={}, min_trials={}, "
+            "length_scale={})"
+        ).format(*args)
+
+
+class GPEiTuner(
+    GaussianProcessMetaModel, ExpectedImprovementAcquisition, BaseMetaModelTuner
+):
     """Gaussian Process Expected Improvement Tuner.
 
     This class uses a ``GaussianProcessRegressor`` model from the ``sklearn.gaussian_process``
     package, using an ``ExpectedImprovement`` function to return the better configurations
     predicted from the model.
     """
-    def __init__(self, tunable, maximize=True, num_candidates=1000,
-                 min_trials=5, length_scale=0.1):
+
+    def __init__(
+        self,
+        tunable,
+        maximize=True,
+        num_candidates=1000,
+        min_trials=5,
+        length_scale=0.1,
+    ):
         """Create an instance of ``GPEiTuner``.
 
         Args:
-            tunable (btb.tuning.tunable.Tunable):
+            tunable (baytune.tuning.tunable.Tunable):
                 Instance of a tunable class containing hyperparameters to be tuned.
             num_candidates (int):
                 Number of samples to generate and select the best of it for each proposal.
                 Defaults to 1000.
             maximize (bool):
                 If ``True`` the model will understand that the score bigger is better, if ``False``
                 the smaller is better. Defaults to ``True``.
             min_trials (int):
                 Number of recorded ``trials`` needed to perform a fitting over the model.
                 Defaults to 2.
             length_scale (float or array):
                 A float or array with shape ``(n_features,)``, used for the default ``RBF`` kernel.
         """
         self.length_scale = length_scale
-        self._metamodel_kwargs = {'length_scale': self.length_scale}
+        self._metamodel_kwargs = {"length_scale": self.length_scale}
         super().__init__(tunable, maximize, num_candidates, min_trials)
 
     def __repr__(self):
-        length_scale = self._metamodel_kwargs.get('length_scale')
-        args = (self.tunable, self.maximize, self.num_candidates, self.min_trials, length_scale)
-        return ('GPEiTuner(tunable={}, maximize={}, '
-                'num_candidates={}, min_trials={}, '
-                'length_scale={})').format(*args)
+        length_scale = self._metamodel_kwargs.get("length_scale")
+        args = (
+            self.tunable,
+            self.maximize,
+            self.num_candidates,
+            self.min_trials,
+            length_scale,
+        )
+        return (
+            "GPEiTuner(tunable={}, maximize={}, "
+            "num_candidates={}, min_trials={}, "
+            "length_scale={})"
+        ).format(*args)
 
 
 class GCPTuner(GaussianCopulaProcessMetaModel, GPTuner):
     """Gaussian Copula Process Tuner.
 
     This class uses a ``GaussianProcessRegressor`` model from the ``sklearn.gaussian_process``
     package, using a ``numpy.argmax`` function to return the better configurations predicted
     from the meta model that converts the input data using a ``Univariate`` copula.
     """
+
     def __repr__(self):
-        length_scale = self._metamodel_kwargs.get('length_scale')
-        args = (self.tunable, self.maximize, self.num_candidates, self.min_trials, length_scale)
-        return ('GCPTuner(tunable={}, maximize={}, '
-                'num_candidates={}, min_trials={}, '
-                'length_scale={})').format(*args)
+        length_scale = self._metamodel_kwargs.get("length_scale")
+        args = (
+            self.tunable,
+            self.maximize,
+            self.num_candidates,
+            self.min_trials,
+            length_scale,
+        )
+        return (
+            "GCPTuner(tunable={}, maximize={}, "
+            "num_candidates={}, min_trials={}, "
+            "length_scale={})"
+        ).format(*args)
 
 
 class GCPEiTuner(GaussianCopulaProcessMetaModel, GPEiTuner):
     """Gaussian Copula Process Expected Improvement Tuner.
 
     This class uses a ``GaussianProcessRegressor`` model from the ``sklearn.gaussian_process``
     package, using an ``ExpectedImprovement`` function to return the better configurations
     predicted from the meta model that converts the input data using a ``Univariate`` copula.
     """
+
     def __repr__(self):
-        length_scale = self._metamodel_kwargs.get('length_scale')
-        args = (self.tunable, self.maximize, self.num_candidates, self.min_trials, length_scale)
-        return ('GCPEiTuner(tunable={}, maximize={}, '
-                'num_candidates={}, min_trials={}, '
-                'length_scale={})').format(*args)
+        length_scale = self._metamodel_kwargs.get("length_scale")
+        args = (
+            self.tunable,
+            self.maximize,
+            self.num_candidates,
+            self.min_trials,
+            length_scale,
+        )
+        return (
+            "GCPEiTuner(tunable={}, maximize={}, "
+            "num_candidates={}, min_trials={}, "
+            "length_scale={})"
+        ).format(*args)
```

### Comparing `baytune-0.4.0/btb/tuning/tuners/uniform.py` & `baytune-0.5.0/baytune/tuning/tuners/uniform.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """Package where the UniformTuner class is defined."""
 
-from btb.tuning.tuners.base import BaseTuner
+from baytune.tuning.tuners.base import BaseTuner
 
 
 class UniformTuner(BaseTuner):
-
     def _propose(self, num_proposals, allow_duplicates):
         """Generate ``num_proposals`` number of candidates.
 
         Args:
             num_proposals (int):
                 Number of candidates to create.
             allow_duplicates (bool):
```

