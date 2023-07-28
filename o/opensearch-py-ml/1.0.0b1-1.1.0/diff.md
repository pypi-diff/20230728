# Comparing `tmp/opensearch_py_ml-1.0.0b1.tar.gz` & `tmp/opensearch_py_ml-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensearch_py_ml-1.0.0b1.tar", last modified: Wed Nov 23 19:50:20 2022, max compression
+gzip compressed data, was "opensearch_py_ml-1.1.0.tar", last modified: Thu Jul 27 23:58:36 2023, max compression
```

## Comparing `opensearch_py_ml-1.0.0b1.tar` & `opensearch_py_ml-1.1.0.tar`

### file list

```diff
@@ -1,58 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-23 19:50:20.443930 opensearch_py_ml-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      256 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2022-11-23 19:50:20.443930 opensearch_py_ml-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-23 19:50:20.443930 opensearch_py_ml-1.0.0b1/opensearch_py_ml/
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (123)    15895 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    82171 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    21966 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/etl.py
--rw-r--r--   0 runner    (1001) docker     (123)    32709 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/field_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29452 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-23 19:50:20.443930 opensearch_py_ml-1.0.0b1/opensearch_py_ml/ml_commons_integration/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/ml_commons_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-23 19:50:20.443930 opensearch_py_ml-1.0.0b1/opensearch_py_ml/ml_commons_integration/load/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/ml_commons_integration/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/ml_commons_integration/load/ml_common_load_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/ml_commons_integration/ml_common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/ml_commons_integration/ml_common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-23 19:50:20.443930 opensearch_py_ml-1.0.0b1/opensearch_py_ml/ml_commons_integration/predict/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/ml_commons_integration/predict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/ml_commons_integration/predict/ml_common_predict_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-23 19:50:20.443930 opensearch_py_ml-1.0.0b1/opensearch_py_ml/ml_commons_integration/upload/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/ml_commons_integration/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/ml_commons_integration/upload/ml_common_model_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)    23796 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/ndframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    58628 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-23 19:50:20.443930 opensearch_py_ml-1.0.0b1/opensearch_py_ml/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/plotting/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-23 19:50:20.443930 opensearch_py_ml-1.0.0b1/opensearch_py_ml/plotting/_matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/plotting/_matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/plotting/_matplotlib/hist.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    27438 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/query_compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-23 19:50:20.443930 opensearch_py_ml-1.0.0b1/opensearch_py_ml/sentence_transformer_model/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/sentence_transformer_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29366 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/sentence_transformer_model/sentencetransformermodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    52106 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/series.py
--rw-r--r--   0 runner    (1001) docker     (123)    13112 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-23 19:50:20.443930 opensearch_py_ml-1.0.0b1/opensearch_py_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2022-11-23 19:50:20.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2022-11-23 19:50:20.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-23 19:50:20.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-23 19:50:20.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-11-23 19:50:20.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-11-23 19:50:20.000000 opensearch_py_ml-1.0.0b1/opensearch_py_ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2022-11-23 19:50:20.443930 opensearch_py_ml-1.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2022-11-23 19:50:11.000000 opensearch_py_ml-1.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:58:36.602665 opensearch_py_ml-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-07-27 23:58:36.602665 opensearch_py_ml-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:58:36.602665 opensearch_py_ml-1.1.0/opensearch_py_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14908 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83394 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22041 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32709 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/field_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30027 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:58:36.602665 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_commons/ml_common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22200 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_commons/ml_commons_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_commons/model_execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_commons/model_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:58:36.602665 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:58:36.602665 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_models/metrics_correlation/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_models/metrics_correlation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_models/metrics_correlation/dip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_models/metrics_correlation/event_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_models/metrics_correlation/mcorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_models/metrics_correlation/nmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_models/metrics_correlation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_models/metrics_correlation/wavelet_piecewise_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_models/metrics_correlation/wavelet_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48117 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ml_models/sentencetransformermodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24425 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/ndframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58621 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:58:36.602665 opensearch_py_ml-1.1.0/opensearch_py_ml/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/plotting/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:58:36.602665 opensearch_py_ml-1.1.0/opensearch_py_ml/plotting/_matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/plotting/_matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/plotting/_matplotlib/hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27437 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/query_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53756 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/opensearch_py_ml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:58:36.602665 opensearch_py_ml-1.1.0/opensearch_py_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-07-27 23:58:36.000000 opensearch_py_ml-1.1.0/opensearch_py_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-27 23:58:36.000000 opensearch_py_ml-1.1.0/opensearch_py_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:58:36.000000 opensearch_py_ml-1.1.0/opensearch_py_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:58:36.000000 opensearch_py_ml-1.1.0/opensearch_py_ml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 23:58:36.000000 opensearch_py_ml-1.1.0/opensearch_py_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 23:58:36.000000 opensearch_py_ml-1.1.0/opensearch_py_ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-27 23:58:36.602665 opensearch_py_ml-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:58:36.602665 opensearch_py_ml-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/tests/test_common_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-27 23:28:04.000000 opensearch_py_ml-1.1.0/tests/test_utils_pytest.py
```

### Comparing `opensearch_py_ml-1.0.0b1/LICENSE` & `opensearch_py_ml-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensearch_py_ml-1.0.0b1/PKG-INFO` & `opensearch_py_ml-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: opensearch_py_ml
-Version: 1.0.0b1
+Version: 1.1.0
 Summary: Python Client and Toolkit for DataFrames, Big Data, Machine Learning and ETL in OpenSearch
 Home-page: https://github.com/opensearch-project/opensearch-py-ml
 Author: Dhrubo Saha
 Author-email: dhrubo@amazon.com, 
-Maintainer: Dhrubo Saha, Yaliang Wu
-Maintainer-email: dhrubo@amazon.com, ylwu@amazon.com
+Maintainer: Dhrubo Saha, Yaliang Wu, Alexander Greaves-Tunnell, Sicheng Song, Jing Zhang, Bhavana Goud Ramaram
+Maintainer-email: dhrubo@amazon.com, ylwu@amazon.com, greaa@amazon.com, seasonsg@amazon.com, jngz@amazon.com, rbhavna@amazon.com
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/opensearch-project/opensearch-py-ml
 Project-URL: Issue Tracker, https://github.com/opensearch-project/opensearch-py-ml/issues
 Keywords: Opensearch opensearch_py_ml pandas python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Environment :: Console
@@ -46,23 +46,35 @@
 - [Code of Conduct](https://github.com/opensearch-project/opensearch-py-ml#code-of-conduct)
 - [License](https://github.com/opensearch-project/opensearch-py-ml#license)
 - [Copyright](https://github.com/opensearch-project/opensearch-py-ml#copyright)
 
 ## Welcome!
 
 **opensearch-py-ml** is a Python client that provides a suite of data analytics and machine learning tools for OpenSearch.
-**Opensearch-py-ml is an experimental project**
+
 It is [a community-driven, open source fork](https://aws.amazon.com/blogs/opensource/introducing-opensearch/) a fork of [eland](https://github.com/elastic/eland), which provides data analysis and machine learning
 licensed under the [Apache v2.0 License](https://github.com/opensearch-project/opensearch-py/blob/main/LICENSE.txt). 
 
 **opensearch-py-ml** lets users call OpenSearch indices and manipulate them as if they were pandas DataFrames, supporting
 complex filtering and aggregation operations. It also provides rudimentary support for uploading models to OpenSearch
 clusters using the [ml-commons](https://github.com/opensearch-project/ml-commons) plugin.
 
 
+For more information, see [opensearch.org](https://opensearch.org/docs/latest/clients/opensearch-py-ml/) and the [API Doc](https://opensearch-project.github.io/opensearch-py-ml/index.html).
+
+
+##Installing Opensearch-py-ml
+
+
+Opensearch-py-ml can be installed from [PyPI](https://pypi.org/project/opensearch-py-ml) via pip:
+
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+    $ python -m pip install opensearch-py-ml
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
 ## Code of Conduct
 
 This project has adopted the 
 [Amazon Open Source Code of Conduct](https://github.com/opensearch-project/opensearch-py-ml/blob/main/CODE_OF_CONDUCT.md).
 For more information see the [Code of Conduct FAQ](https://aws.github.io/code-of-conduct-faq), or contact 
 [opensource-codeofconduct@amazon.com](mailto:opensource-codeofconduct@amazon.com) with any additional questions or comments.
```

### Comparing `opensearch_py_ml-1.0.0b1/README.md` & `opensearch_py_ml-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -14,23 +14,35 @@
 - [Code of Conduct](https://github.com/opensearch-project/opensearch-py-ml#code-of-conduct)
 - [License](https://github.com/opensearch-project/opensearch-py-ml#license)
 - [Copyright](https://github.com/opensearch-project/opensearch-py-ml#copyright)
 
 ## Welcome!
 
 **opensearch-py-ml** is a Python client that provides a suite of data analytics and machine learning tools for OpenSearch.
-**Opensearch-py-ml is an experimental project**
+
 It is [a community-driven, open source fork](https://aws.amazon.com/blogs/opensource/introducing-opensearch/) a fork of [eland](https://github.com/elastic/eland), which provides data analysis and machine learning
 licensed under the [Apache v2.0 License](https://github.com/opensearch-project/opensearch-py/blob/main/LICENSE.txt). 
 
 **opensearch-py-ml** lets users call OpenSearch indices and manipulate them as if they were pandas DataFrames, supporting
 complex filtering and aggregation operations. It also provides rudimentary support for uploading models to OpenSearch
 clusters using the [ml-commons](https://github.com/opensearch-project/ml-commons) plugin.
 
 
+For more information, see [opensearch.org](https://opensearch.org/docs/latest/clients/opensearch-py-ml/) and the [API Doc](https://opensearch-project.github.io/opensearch-py-ml/index.html).
+
+
+##Installing Opensearch-py-ml
+
+
+Opensearch-py-ml can be installed from [PyPI](https://pypi.org/project/opensearch-py-ml) via pip:
+
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+    $ python -m pip install opensearch-py-ml
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
 ## Code of Conduct
 
 This project has adopted the 
 [Amazon Open Source Code of Conduct](https://github.com/opensearch-project/opensearch-py-ml/blob/main/CODE_OF_CONDUCT.md).
 For more information see the [Code of Conduct FAQ](https://aws.github.io/code-of-conduct-faq), or contact 
 [opensource-codeofconduct@amazon.com](mailto:opensource-codeofconduct@amazon.com) with any additional questions or comments.
```

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/__init__.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/_version.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/_version.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,12 +23,12 @@
 #  specific language governing permissions and limitations
 #  under the License.
 
 # TODO fill out this information
 __title__ = "opensearch_py_ml"
 __description__ = "Python Client and Toolkit for DataFrames, Big Data, Machine Learning and ETL in OpenSearch"
 __url__ = "https://github.com/opensearch-project/opensearch-py-ml"
-__version__ = "1.0.0b1"
+__version__ = "1.1.0"
 __author__ = "Dhrubo Saha"
 __author_email__ = "dhrubo@amazon.com, "
-__maintainer__ = "Dhrubo Saha, Yaliang Wu"
-__maintainer_email__ = "dhrubo@amazon.com, ylwu@amazon.com"
+__maintainer__ = "Dhrubo Saha, Yaliang Wu, Alexander Greaves-Tunnell, Sicheng Song, Jing Zhang, Bhavana Goud Ramaram"
+__maintainer_email__ = "dhrubo@amazon.com, ylwu@amazon.com, greaa@amazon.com, seasonsg@amazon.com, jngz@amazon.com, rbhavna@amazon.com"
```

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/actions.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/actions.py`

 * *Files identical despite different names*

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/arithmetics.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/arithmetics.py`

 * *Files identical despite different names*

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/common.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 #  under the License.
 
 import re
 import warnings
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple, Union, cast
 
-import opensearchpy
 import pandas as pd  # type: ignore
 from opensearchpy import OpenSearch
 
 from ._version import __version__ as _opensearch_py_ml_version
 
 if TYPE_CHECKING:
     from numpy.typing import DTypeLike
@@ -328,32 +327,7 @@
                 "as your cluster major version.",
                 stacklevel=2,
             )
 
     else:
         opensearch_py_ml_os_version = os_client._os_ml_py_version  # type: ignore
     return opensearch_py_ml_os_version
-
-
-OPENSEARCH_HOST = "https://instance:9200"
-OPENSEARCH_ADMIN_USER, OPENSEARCH_ADMIN_PASSWORD = "admin", "admin"
-
-# Define client to use in tests
-OPENSEARCH_TEST_CLIENT = OpenSearch(
-    hosts=[OPENSEARCH_HOST],
-    http_auth=(OPENSEARCH_ADMIN_USER, OPENSEARCH_ADMIN_PASSWORD),
-    verify_certs=False,
-)
-# in github integration test, host url is: https://instance:9200
-# in development, usually host url is: https://localhost:9200
-# it's hard to remember changing the host url. So applied a try catch so that we don't have to keep change this config
-try:
-    OS_VERSION = os_version(OPENSEARCH_TEST_CLIENT)
-except opensearchpy.exceptions.ConnectionError:
-    OPENSEARCH_HOST = "https://localhost:9200"
-    # Define client to use in tests
-    OPENSEARCH_TEST_CLIENT = OpenSearch(
-        hosts=[OPENSEARCH_HOST],
-        http_auth=(OPENSEARCH_ADMIN_USER, OPENSEARCH_ADMIN_PASSWORD),
-        verify_certs=False,
-    )
-    OS_VERSION = os_version(OPENSEARCH_TEST_CLIENT)
```

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/conftest.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/conftest.py`

 * *Files identical despite different names*

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/dataframe.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 from pandas.io.common import _expand_user, stringify_path  # type: ignore
 from pandas.io.formats import console  # type: ignore
 from pandas.io.formats import format as fmt
 from pandas.io.formats.printing import pprint_thing  # type: ignore
 from pandas.util._validators import validate_bool_kwarg  # type: ignore
 
 import opensearch_py_ml.plotting as gfx
-from opensearch_py_ml.common import OPENSEARCH_TEST_CLIENT  # noqa: F401
 from opensearch_py_ml.common import DEFAULT_NUM_ROWS_DISPLAYED, docstring_parameter
 from opensearch_py_ml.filter import BooleanFilter
 from opensearch_py_ml.groupby import DataFrameGroupBy
 from opensearch_py_ml.ndframe import NDFrame
 from opensearch_py_ml.series import Series
 from opensearch_py_ml.utils import is_valid_attr_name
 
@@ -74,14 +73,17 @@
     --------
     :pandas_api_docs:`pandas.DataFrame`
 
     Examples
     --------
     Constructing DataFrame from an OpenSearch configuration arguments and an OpenSearch index
 
+    >>> from tests import OPENSEARCH_TEST_CLIENT
+
+
     >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
     >>> df.head()
        AvgTicketPrice  Cancelled  ... dayOfWeek           timestamp
     0      841.265642      False  ...         0 2018-01-01 00:00:00
     1      882.982662      False  ...         0 2018-01-01 18:27:00
     2      190.636904      False  ...         0 2018-01-01 17:11:14
     3      181.694216       True  ...         0 2018-01-01 10:33:28
@@ -167,14 +169,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.columns`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
         >>> assert isinstance(df.columns, pd.Index)
         >>> df.columns
         Index(['AvgTicketPrice', 'Cancelled', 'Carrier', 'Dest', 'DestAirportID', 'DestCityName',
         ...   'DestCountry', 'DestLocation', 'DestRegion', 'DestWeather', 'DistanceKilometers',
         ...   'DistanceMiles', 'FlightDelay', 'FlightDelayMin', 'FlightDelayType', 'FlightNum',
         ...   'FlightTimeHour', 'FlightTimeMin', 'Origin', 'OriginAirportID', 'OriginCityName',
@@ -195,14 +199,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.empty`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
         >>> df.empty
         False
         """
         return len(self.columns) == 0 or len(self.index) == 0
 
     def head(self, n: int = 5) -> "DataFrame":
@@ -225,14 +231,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.head`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=['Origin', 'Dest'])
         >>> df.head(3)
                                     Origin                                          Dest
         0        Frankfurt am Main Airport  Sydney Kingsford Smith International Airport
         1  Cape Town International Airport                     Venice Marco Polo Airport
         2        Venice Marco Polo Airport                     Venice Marco Polo Airport
         <BLANKLINE>
@@ -260,14 +268,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.tail`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=['Origin', 'Dest'])
         >>> df.tail()
                                                                     Origin  \\
         13054                                   Pisa International Airport...
         13055  Winnipeg / James Armstrong Richardson International Airport...
         13056               Licenciado Benito Juarez International Airport...
         13057                                                Itami Airport...
@@ -362,14 +372,16 @@
         --------
         :pandas_api_docs:`pandas.DataFrame.drop`
 
         Examples
         --------
         Drop a column
 
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce', columns=['customer_first_name', 'email', 'user'])
         >>> df.drop(columns=['user'])
              customer_first_name                       email
         0                  Eddie  eddie@underwood-family.zzz
         1                   Mary      mary@bailey-family.zzz
         2                   Gwen      gwen@butler-family.zzz
         3                  Diane   diane@chandler-family.zzz
@@ -572,14 +584,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.count`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce', columns=['customer_first_name', 'geoip.city_name'])
         >>> df.count()
         customer_first_name    4675
         geoip.city_name        4094
         dtype: int64
         """
         return self._query_compiler.count()
@@ -594,14 +608,16 @@
         Returns
         -------
         str
             A debug summary of an opensearch_py_ml DataFrame internals.
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
         >>> df = df[(df.OriginAirportID == 'AMS') & (df.FlightDelayMin > 60)]
         >>> df = df[['timestamp', 'OriginAirportID', 'DestAirportID', 'FlightDelayMin']]
         >>> df = df.tail()
         >>> df
                         timestamp OriginAirportID DestAirportID  FlightDelayMin
         12608 2018-02-10 01:20:52             AMS          CYEG             120
@@ -689,14 +705,16 @@
         Returns
         -------
         DataFrame
             A filtered :py:class:`opensearch_py_ml.DataFrame` with the given match query
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, "ecommerce")
         >>> df.os_match("Men's", columns=["category"])
                                                       category currency  ...   type     user
         0                                     [Men's Clothing]      EUR  ...  order    eddie
         4                  [Men's Clothing, Men's Accessories]      EUR  ...  order    eddie
         6                                     [Men's Clothing]      EUR  ...  order   oliver
         7     [Men's Clothing, Men's Accessories, Men's Shoes]      EUR  ...  order      abd
@@ -750,14 +768,15 @@
 
         Examples
         --------
 
         Apply a `geo-distance query`_ to a dataset with a geo-point column ``geoip.location``.
 
          .. _geo-distance query documentation from Elasticsearch: https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-geo-distance-query.html
+        >>> from tests import OPENSEARCH_TEST_CLIENT
 
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce', columns=['customer_first_name', 'geoip.city_name'])
         >>> df.os_query({"bool": {"filter": {"geo_distance": {"distance": "1km", "geoip.location": [55.3, 25.3]}}}}).head()
            customer_first_name geoip.city_name
         1                 Mary           Dubai
         9            Rabbia Al           Dubai
         10           Rabbia Al           Dubai
@@ -827,14 +846,16 @@
         -----
         This copies a lot of code from pandas.DataFrame.info as it is difficult
         to split out the appropriate code or creating a SparseDataFrame gives
         incorrect results on types and counts.
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce', columns=['customer_first_name', 'geoip.city_name'])
         >>> df.info()
         <class 'opensearch_py_ml.dataframe.DataFrame'>
         Index: 4675 entries, 0 to 4674
         Data columns (total 2 columns):
          #   Column               Non-Null Count  Dtype...
         ---  ------               --------------  -----...
@@ -1363,14 +1384,16 @@
         Returns
         -------
         opensearch_py_ml.DataFrame
             DataFrame contains only columns of selected dtypes
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights',
         ... columns=['AvgTicketPrice', 'Dest', 'Cancelled', 'timestamp', 'dayOfWeek'])
         >>> df.dtypes
         AvgTicketPrice           float64
         Dest                      object
         Cancelled                   bool
         timestamp         datetime64[ns]
@@ -1404,14 +1427,16 @@
         Notes
         -----
         - number of rows ``len(df)`` queries OpenSearch
         - number of columns ``len(df.columns)`` is cached. If mappings are updated, DataFrame must be updated.
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce')
         >>> df.shape
         (4675, 45)
         """
         num_rows = len(self)
         num_columns = len(self.columns)
 
@@ -1466,14 +1491,16 @@
 
         See Also
         --------
         opensearch_py_ml.DataFrame.itertuples: Iterate over opensearch_py_ml.DataFrame rows as namedtuples.
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=['AvgTicketPrice', 'Cancelled']).head()
         >>> df
            AvgTicketPrice  Cancelled
         0      841.265642      False
         1      882.982662      False
         2      190.636904      False
         3      181.694216       True
@@ -1531,14 +1558,16 @@
 
         See Also
         --------
         opensearch_py_ml.DataFrame.iterrows: Iterate over opensearch_py_ml.DataFrame rows as (index, pandas.Series) pairs.
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=['AvgTicketPrice', 'Cancelled']).head()
         >>> df
            AvgTicketPrice  Cancelled
         0      841.265642      False
         1      882.982662      False
         2      190.636904      False
         3      181.694216       True
@@ -1627,14 +1656,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.aggregate`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=['AvgTicketPrice', 'DistanceKilometers', 'timestamp', 'DestCountry'])
         >>> df.aggregate(['sum', 'min', 'std'], numeric_only=True).astype(int)
              AvgTicketPrice  DistanceKilometers
         sum         8204364            92616288
         min             100                   0
         std             266                4578
 
@@ -1702,16 +1733,18 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.groupby`
 
         Examples
         --------
-        >>> ed_flights = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"])
-        >>> ed_flights.groupby(["DestCountry", "Cancelled"]).agg(["min", "max"], numeric_only=True) # doctest: +NORMALIZE_WHITESPACE
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
+        >>> oml_flights = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"])
+        >>> oml_flights.groupby(["DestCountry", "Cancelled"]).agg(["min", "max"], numeric_only=True) # doctest: +NORMALIZE_WHITESPACE
                               AvgTicketPrice              dayOfWeek
                                          min          max       min  max
         DestCountry Cancelled
         AE          False         110.799911  1126.148682       0.0  6.0
                     True          132.443756   817.931030       0.0  6.0
         AR          False         125.589394  1199.642822       0.0  6.0
                     True          251.389603  1172.382568       0.0  6.0
@@ -1721,15 +1754,15 @@
         US          False         100.145966  1199.729004       0.0  6.0
                     True          102.153069  1192.429932       0.0  6.0
         ZA          False         102.002663  1196.186157       0.0  6.0
                     True          121.280296  1175.709961       0.0  6.0
         <BLANKLINE>
         [63 rows x 4 columns]
 
-        >>> ed_flights.groupby(["DestCountry", "Cancelled"]).mean(numeric_only=True) # doctest: +NORMALIZE_WHITESPACE
+        >>> oml_flights.groupby(["DestCountry", "Cancelled"]).mean(numeric_only=True) # doctest: +NORMALIZE_WHITESPACE
                                AvgTicketPrice  dayOfWeek
         DestCountry Cancelled
         AE          False          643.956793   2.717949
                     True           388.828809   2.571429
         AR          False          673.551677   2.746154
                     True           682.197241   2.733333
         AT          False          647.158290   2.819936
@@ -1738,15 +1771,15 @@
         US          False          598.063146   2.752014
                     True           579.799066   2.767068
         ZA          False          636.998605   2.738589
                     True           677.794078   2.928571
         <BLANKLINE>
         [63 rows x 2 columns]
 
-        >>> ed_flights.groupby(["DestCountry", "Cancelled"]).min(numeric_only=False) # doctest: +NORMALIZE_WHITESPACE
+        >>> oml_flights.groupby(["DestCountry", "Cancelled"]).min(numeric_only=False) # doctest: +NORMALIZE_WHITESPACE
                                AvgTicketPrice  dayOfWeek           timestamp
         DestCountry Cancelled
         AE          False          110.799911          0 2018-01-01 19:31:30
                     True           132.443756          0 2018-01-06 13:03:25
         AR          False          125.589394          0 2018-01-01 01:30:47
                     True           251.389603          0 2018-01-01 02:13:17
         AT          False          100.020531          0 2018-01-01 05:24:19
@@ -1797,14 +1830,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.mode`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> oml_ecommerce = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce')
         >>> oml_df = oml_ecommerce.filter(["total_quantity", "geoip.city_name", "customer_birth_date", "day_of_week", "taxful_total_price"])
         >>> oml_df.mode(numeric_only=False)
            total_quantity geoip.city_name customer_birth_date day_of_week  taxful_total_price
         0               2        New York                 NaT    Thursday               53.98
 
         >>> oml_df.mode(numeric_only=True)
@@ -1862,14 +1897,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.quantile`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> oml_df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
         >>> oml_flights = oml_df.filter(["AvgTicketPrice", "FlightDelayMin", "dayOfWeek", "timestamp"])
         >>> oml_flights.quantile() # doctest: +SKIP
         AvgTicketPrice    640.387285
         FlightDelayMin      0.000000
         dayOfWeek           3.000000
         Name: 0.5, dtype: float64
@@ -1905,14 +1942,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.idxmax`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> oml_df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
         >>> oml_flights = oml_df.filter(["AvgTicketPrice", "FlightDelayMin", "dayOfWeek", "timestamp"])
         >>> oml_flights.idxmax()
         AvgTicketPrice    1843
         FlightDelayMin     109
         dayOfWeek         1988
         dtype: object
@@ -1937,14 +1976,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.idxmin`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> oml_df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
         >>> oml_flights = oml_df.filter(["AvgTicketPrice", "FlightDelayMin", "dayOfWeek", "timestamp"])
         >>> oml_flights.idxmin()
         AvgTicketPrice    5454
         FlightDelayMin       0
         dayOfWeek            0
         dtype: object
@@ -1973,14 +2014,16 @@
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.query`
         :pandas_user_guide:`indexing`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
         >>> df.shape
         (13059, 27)
         >>> df.query('FlightDelayMin > 60').shape
         (2730, 27)
         """
         if isinstance(expr, BooleanFilter):
@@ -2017,14 +2060,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.get`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
         >>> df.get('Carrier')
         0         Kibana Airlines
         1        Logstash Airways
         2        Logstash Airways
         3         Kibana Airlines
         4         Kibana Airlines
@@ -2148,14 +2193,16 @@
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.to_numpy`
         opensearch_to_pandas
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> oml_df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=['AvgTicketPrice', 'Carrier']).head(5)
         >>> pd_df = oml.opensearch_to_pandas(oml_df)
         >>> print(f"type(oml_df)={type(oml_df)}\\ntype(pd_df)={type(pd_df)}")
         type(oml_df)=<class 'opensearch_py_ml.dataframe.DataFrame'>
         type(pd_df)=<class 'pandas.core.frame.DataFrame'>
         >>> oml_df
            AvgTicketPrice           Carrier
```

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/etl.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/etl.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from typing import Any, Dict, Generator, List, Mapping, Optional, Tuple, Union
 
 import pandas as pd  # type: ignore
 from opensearchpy import OpenSearch
 from opensearchpy.helpers import parallel_bulk
 
 from opensearch_py_ml import DataFrame
-from opensearch_py_ml.common import OPENSEARCH_TEST_CLIENT  # noqa: F401
 from opensearch_py_ml.common import DEFAULT_CHUNK_SIZE, PANDAS_VERSION
 from opensearch_py_ml.field_mappings import FieldMappings, verify_mapping_compatibility
 
 try:
     from pandas.io.parsers import _c_parser_defaults  # type: ignore
 except ImportError:
     from pandas.io.parsers.readers import _c_parser_defaults  # type: ignore
@@ -95,14 +94,15 @@
     -------
     opensearch_py_ml.Dataframe
         opensearch_py_ml.DataFrame referencing data in destination_index
 
     Examples
     --------
 
+    >>> from tests import OPENSEARCH_TEST_CLIENT
     >>> pd_df = pd.DataFrame(data={'A': 3.141,
     ...                            'B': 1,
     ...                            'C': 'foo',
     ...                            'D': pd.Timestamp('20190102'),
     ...                            'E': [1.0, 2.0, 3.0],
     ...                            'F': False,
     ...                            'G': [1, 2, 3],
@@ -129,14 +129,15 @@
     dtype: object
 
     Convert `pandas.DataFrame` to `opensearch_py_ml.DataFrame` - this creates an OpenSearch index called
     `pandas_to_opensearch`. Overwrite existing OpenSearch index if it exists `if_exists="replace"`, and sync index, so
     it is readable on return `refresh=True`
 
 
+    >>> from tests import OPENSEARCH_TEST_CLIENT
     >>> oml_df = oml.pandas_to_opensearch(pd_df,
     ...                            OPENSEARCH_TEST_CLIENT,
     ...                            'pandas_to_opensearch',
     ...                            os_if_exists="replace",
     ...                            os_refresh=True,
     ...                            os_type_overrides={'H':'text'}) # index field 'H' as text not keyword
     >>> type(oml_df)
@@ -259,14 +260,16 @@
     Returns
     -------
     pandas.Dataframe
         pandas.DataFrame contains all rows and columns in opensearch_py_ml.DataFrame
 
     Examples
     --------
+    >>> from tests import OPENSEARCH_TEST_CLIENT
+
     >>> oml_df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights').head()
     >>> type(oml_df)
     <class 'opensearch_py_ml.dataframe.DataFrame'>
     >>> oml_df
        AvgTicketPrice  Cancelled  ... dayOfWeek           timestamp
     0      841.265642      False  ...         0 2018-01-01 00:00:00
     1      882.982662      False  ...         0 2018-01-01 18:27:00
```

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/field_mappings.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/field_mappings.py`

 * *Files identical despite different names*

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/filter.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/filter.py`

 * *Files identical despite different names*

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/groupby.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/groupby.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
 from typing import TYPE_CHECKING, List, Optional, Union
 
-from opensearch_py_ml.common import OPENSEARCH_TEST_CLIENT  # noqa: F401
 from opensearch_py_ml.query_compiler import QueryCompiler
 
 if TYPE_CHECKING:
     import pandas as pd  # type: ignore
 
 
 class GroupBy:
@@ -72,14 +71,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.core.groupby.GroupBy.mean`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(
         ...   OPENSEARCH_TEST_CLIENT, "flights",
         ...   columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"]
         ... )
         >>> df.groupby("DestCountry").mean(numeric_only=False) # doctest: +SKIP
                      AvgTicketPrice  Cancelled  dayOfWeek                     timestamp
         DestCountry
@@ -123,14 +124,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.core.groupby.GroupBy.var`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(
         ...   OPENSEARCH_TEST_CLIENT, "flights",
         ...   columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"]
         ... )
         >>> df.groupby("DestCountry").var() # doctest: +NORMALIZE_WHITESPACE
                      AvgTicketPrice  Cancelled  dayOfWeek
         DestCountry
@@ -174,14 +177,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.core.groupby.GroupBy.std`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(
         ...   OPENSEARCH_TEST_CLIENT, "flights",
         ...   columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "DestCountry"]
         ... )
         >>> df.groupby("DestCountry").std() # doctest: +NORMALIZE_WHITESPACE
                      AvgTicketPrice  Cancelled  dayOfWeek
         DestCountry
@@ -225,14 +230,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.core.groupby.GroupBy.mad`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(
         ...   OPENSEARCH_TEST_CLIENT, "flights",
         ...   columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"]
         ... )
         >>> df.groupby("DestCountry").mad() # doctest: +SKIP
                      AvgTicketPrice  Cancelled  dayOfWeek
         DestCountry
@@ -276,14 +283,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.core.groupby.GroupBy.median`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(
         ...   OPENSEARCH_TEST_CLIENT, "flights",
         ...   columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"]
         ... )
         >>> df.groupby("DestCountry").median(numeric_only=False) # doctest: +SKIP
                      AvgTicketPrice  Cancelled  dayOfWeek               timestamp
         DestCountry
@@ -327,14 +336,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.core.groupby.GroupBy.sum`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(
         ...   OPENSEARCH_TEST_CLIENT, "flights",
         ...   columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "DestCountry"]
         ... )
         >>> df.groupby("DestCountry").sum() # doctest: +NORMALIZE_WHITESPACE
                      AvgTicketPrice  Cancelled  dayOfWeek
         DestCountry
@@ -378,14 +389,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.core.groupby.GroupBy.min`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(
         ...   OPENSEARCH_TEST_CLIENT, "flights",
         ...   columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"]
         ... )
         >>> df.groupby("DestCountry").min(numeric_only=False) # doctest: +NORMALIZE_WHITESPACE
                      AvgTicketPrice  Cancelled  dayOfWeek           timestamp
         DestCountry
@@ -429,14 +442,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.core.groupby.GroupBy.max`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(
         ...   OPENSEARCH_TEST_CLIENT, "flights",
         ...   columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"]
         ... )
         >>> df.groupby("DestCountry").max(numeric_only=False) # doctest: +NORMALIZE_WHITESPACE
                      AvgTicketPrice  Cancelled  dayOfWeek           timestamp
         DestCountry
@@ -480,14 +495,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.core.groupby.GroupBy.nunique`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(
         ...   OPENSEARCH_TEST_CLIENT, "flights",
         ...   columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "DestCountry"]
         ... )
         >>> df.groupby("DestCountry").nunique() # doctest: +NORMALIZE_WHITESPACE
                      AvgTicketPrice  Cancelled  dayOfWeek
         DestCountry
@@ -531,14 +548,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.core.groupby.GroupBy.quantile`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> oml_df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
         >>> oml_flights = oml_df.filter(["AvgTicketPrice", "FlightDelayMin", "dayOfWeek", "timestamp"])
         >>> oml_flights.groupby(["dayOfWeek", "Cancelled"]).quantile() # doctest: +SKIP
                              AvgTicketPrice  FlightDelayMin
         dayOfWeek Cancelled
         0         False          572.290384             0.0
                   True           578.140564             0.0
@@ -620,14 +639,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.core.groupby.GroupBy.aggregate`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(
         ...   OPENSEARCH_TEST_CLIENT, "flights",
         ...   columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "DestCountry"]
         ... )
         >>> df.groupby("DestCountry").aggregate(["min", "max"]) # doctest: +NORMALIZE_WHITESPACE
                     AvgTicketPrice               ... dayOfWeek
                                min          max  ...       min max
@@ -674,14 +695,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.core.groupby.GroupBy.count`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(
         ...   OPENSEARCH_TEST_CLIENT, "flights",
         ...   columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "DestCountry"]
         ... )
         >>> df.groupby("DestCountry").count() # doctest: +NORMALIZE_WHITESPACE
                      AvgTicketPrice  Cancelled  dayOfWeek
         DestCountry
```

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/index.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/index.py`

 * *Files identical despite different names*

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/ml_commons_integration/upload/ml_common_model_uploader.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/ml_commons/model_uploader.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,96 +9,122 @@
 import json
 import os
 from math import ceil
 from typing import Any, Iterable, Union
 
 from opensearchpy import OpenSearch
 
-from opensearch_py_ml.ml_commons_integration.ml_common_utils import (
+from opensearch_py_ml.ml_commons.ml_common_utils import (
     BUF_SIZE,
+    EMBEDDING_DIMENSION,
+    FRAMEWORK_TYPE,
+    META_API_ENDPOINT,
     ML_BASE_URI,
+    MODEL_CHUNK_MAX_SIZE,
+    MODEL_CONFIG_FIELD,
+    MODEL_CONTENT_HASH_VALUE,
+    MODEL_CONTENT_SIZE_IN_BYTES_FIELD,
+    MODEL_FORMAT_FIELD,
+    MODEL_GROUP_ID,
     MODEL_MAX_SIZE,
-    MODEL_UPLOAD_CHUNK_SIZE,
+    MODEL_NAME_FIELD,
+    MODEL_TYPE,
+    MODEL_VERSION_FIELD,
+    TOTAL_CHUNKS_FIELD,
 )
 
 
-class MLCommonModelUploader:
+class ModelUploader:
     """
-    Class for uploading model using ml-commons apis in opensearch cluster.
+    Class for registering a model using ml-commons apis in opensearch cluster.
     """
 
-    META_API_ENDPOINT = "models/meta"
-    MODEL_NAME_FIELD = "name"
-    MODEL_VERSION_FIELD = "version"
-    MODEL_FORMAT_FIELD = "model_format"
-    TOTAL_CHUNKS_FIELD = "total_chunks"
-    MODEL_CONFIG_FIELD = "model_config"
-    MODEL_TYPE = "model_type"
-    EMBEDDING_DIMENSION = "embedding_dimension"
-    FRAMEWORK_TYPE = "framework_type"
-    MODEL_CONTENT_HASH_VALUE = "model_content_hash_value"
-
     def __init__(self, os_client: OpenSearch):
         self._client = os_client
 
-    def upload_model(
-        self, model_path: str, model_meta_path: str, isVerbose: bool
-    ) -> None:
-
+    def _register_model(
+        self,
+        model_path: str,
+        model_meta_path: str,
+        model_group_id: str = "",
+        isVerbose: bool = False,
+    ) -> str:
         """
-        This method uploads model into opensearch cluster using ml-common plugin's api.
-        first this method creates a model id to store model metadata and then breaks the model zip file into
+        This method registers the model in the opensearch cluster using ml-common plugin's register model api.
+        First, this method creates a model id to store model metadata and then breaks the model zip file into
         multiple chunks and then upload chunks into cluster.
 
-        @param model_path         string     path of the zip file of the model
-        @param model_meta_path    string     filepath of the model metadata. A json file of model metadata is expected
-        @param isVerbose          bool       if isVerbose is true method will print more messages.
+        :param model_path: path of the zip file of the model
+        :type model_path: string
+        :param model_meta_path:
+            filepath of the model metadata. A json file of model metadata is expected
+            Model metadata format example:
+                {
+                    "name": "all-MiniLM-L6-v2",
+                    "version": 1,
+                    "model_format": "TORCH_SCRIPT",
+                    "model_config": {
+                        "model_type": "bert",
+                        "embedding_dimension": 384,
+                        "framework_type": "sentence_transformers",
+                        "all_config": '{"_name_or_path":"nreimers/MiniLM-L6-H384-uncased","architectures":["BertModel"],"attention_probs_dropout_prob":0.1,"gradient_checkpointing":false,"hidden_act":"gelu","hidden_dropout_prob":0.1,"hidden_size":384,"initializer_range":0.02,"intermediate_size":1536,"layer_norm_eps":1e-12,"max_position_embeddings":512,"model_type":"bert","num_attention_heads":12,"num_hidden_layers":6,"pad_token_id":0,"position_embedding_type":"absolute","transformers_version":"4.8.2","type_vocab_size":2,"use_cache":true,"vocab_size":30522}',
+                    },
+                }
+            refer to:
+                https://opensearch.org/docs/latest/ml-commons-plugin/model-serving-framework/#upload-model-to-opensearch
+        :type model_meta_path: string
+        :param model_group_id: Model group id
+        :type model_group_id: string
+        :param isVerbose: if isVerbose is true method will print more messages
+        :type isVerbose: bool
+        :return: returns model id which is created by the model metadata
+        :rtype: string
         """
         if os.stat(model_path).st_size > MODEL_MAX_SIZE:
             raise Exception("Model file size exceeds the limit of 4GB")
 
-        total_num_chunks: int = ceil(
-            os.stat(model_path).st_size / MODEL_UPLOAD_CHUNK_SIZE
-        )
+        model_content_size_in_bytes = os.stat(model_path).st_size
+        total_num_chunks: int = ceil(model_content_size_in_bytes / MODEL_CHUNK_MAX_SIZE)
 
         # we are generating the sha1 hash for the model zip file
-        hash_val_model_file = self.generate_hash(model_path)
+        hash_val_model_file = self._generate_hash(model_path)
 
         if isVerbose:
             print("Total number of chunks", total_num_chunks)
             print("Sha1 value of the model file: ", hash_val_model_file)
 
         model_meta_json_file = open(model_meta_path)
 
         model_meta_json: dict[str, Union[str, dict[str, str]]] = json.load(
             model_meta_json_file
         )
-        model_meta_json[self.TOTAL_CHUNKS_FIELD] = total_num_chunks
-        model_meta_json[self.MODEL_CONTENT_HASH_VALUE] = hash_val_model_file
+        model_meta_json[TOTAL_CHUNKS_FIELD] = total_num_chunks
+        model_meta_json[MODEL_CONTENT_SIZE_IN_BYTES_FIELD] = model_content_size_in_bytes
+        model_meta_json[MODEL_CONTENT_HASH_VALUE] = hash_val_model_file
+        model_meta_json[MODEL_GROUP_ID] = model_group_id
 
-        if self.check_mandatory_field(model_meta_json):
+        if self._check_mandatory_field(model_meta_json):
             meta_output: Union[bool, Any] = self._client.transport.perform_request(
                 method="POST",
-                url=f"{ML_BASE_URI}/{self.META_API_ENDPOINT}",
+                url=f"{ML_BASE_URI}/{META_API_ENDPOINT}",
                 body=model_meta_json,
             )
-
             print(
                 "Model meta data was created successfully. Model Id: ",
                 meta_output.get("model_id"),
             )
 
             # model meta doc is created successfully, and now we can upload model chunks to the model id
             if meta_output.get("status") == "CREATED" and meta_output.get("model_id"):
                 model_id = meta_output.get("model_id")
 
                 def model_file_chunk_generator() -> Iterable[str]:
                     with open(model_path, "rb") as f:
                         while True:
-                            data = f.read(MODEL_UPLOAD_CHUNK_SIZE)
+                            data = f.read(MODEL_CHUNK_MAX_SIZE)
                             if not data:
                                 break
                             yield data  # type: ignore # check if we actually need to do base64 encoding
 
                 to_iterate_over = enumerate(model_file_chunk_generator())
 
                 for i, chunk in to_iterate_over:
@@ -106,68 +132,83 @@
                         print(f"uploading chunk {i + 1} of {total_num_chunks}")
                     output = self._client.transport.perform_request(
                         method="POST",
                         url=f"{ML_BASE_URI}/models/{model_id}/chunk/{i}",
                         body=chunk,
                     )
                     if isVerbose:
-                        print(output)
-                print("Model uploaded successfully")
+                        print("Model id:", output)
+
+                print("Model registered successfully")
+                return model_id
             else:
                 raise Exception(
                     "Model meta doc creation wasn't successful. Please check the errors"
                 )
 
-    def check_mandatory_field(self, model_meta: dict) -> bool:
+    def _check_mandatory_field(self, model_meta: dict) -> bool:
         """
-        This method checks if model meta doc has all the required fields to create a model meta doc in opensearch.
+        This method checks if model meta doc has all the required fields to create a model meta doc in opensearch
 
-        @param model_meta         dict     content of the model meta file
-
-        @return                   boolean  if all the required fields are present returns True otherwise
+        Parameters
+        ----------
+        :param model_meta: content of the model meta file
+        :type model_meta: dict
+
+        Returns
+        -------
+        :return: if all the required fields are present returns True otherwise
                                             raise exception
+        :rtype: bool
         """
 
         if model_meta:
-            if not model_meta.get(self.MODEL_NAME_FIELD):
-                raise ValueError(f"{self.MODEL_NAME_FIELD} can not be empty")
-            if not model_meta.get(self.MODEL_VERSION_FIELD):
-                raise ValueError(f"{self.MODEL_VERSION_FIELD} can not be empty")
-            if not model_meta.get(self.MODEL_FORMAT_FIELD):
-                raise ValueError(f"{self.MODEL_FORMAT_FIELD} can not be empty")
-            if not model_meta.get(self.MODEL_CONTENT_HASH_VALUE):
-                raise ValueError(f"{self.MODEL_CONTENT_HASH_VALUE} can not be empty")
-            if not model_meta.get(self.TOTAL_CHUNKS_FIELD):
-                raise ValueError(f"{self.TOTAL_CHUNKS_FIELD} can not be empty")
-            if not model_meta.get(self.MODEL_CONFIG_FIELD):
-                raise ValueError(f"{self.MODEL_CONFIG_FIELD} can not be empty")
+            if not model_meta.get(MODEL_NAME_FIELD):
+                raise ValueError(f"{MODEL_NAME_FIELD} can not be empty")
+            if not model_meta.get(MODEL_VERSION_FIELD):
+                raise ValueError(f"{MODEL_VERSION_FIELD} can not be empty")
+            if not model_meta.get(MODEL_FORMAT_FIELD):
+                raise ValueError(f"{MODEL_FORMAT_FIELD} can not be empty")
+            if not model_meta.get(MODEL_CONTENT_HASH_VALUE):
+                raise ValueError(f"{MODEL_CONTENT_HASH_VALUE} can not be empty")
+            if not model_meta.get(TOTAL_CHUNKS_FIELD):
+                raise ValueError(f"{TOTAL_CHUNKS_FIELD} can not be empty")
+            if not model_meta.get(MODEL_CONFIG_FIELD):
+                raise ValueError(f"{MODEL_CONFIG_FIELD} can not be empty")
             else:
-                if not isinstance(model_meta.get(self.MODEL_CONFIG_FIELD), dict):
+                if not isinstance(model_meta.get(MODEL_CONFIG_FIELD), dict):
                     raise TypeError(
-                        f"{self.MODEL_CONFIG_FIELD} is expecting to be an object"
+                        f"{MODEL_CONFIG_FIELD} is expecting to be an object"
                     )
-                model_config = model_meta.get(self.MODEL_CONFIG_FIELD)
-                if not model_config.get(self.MODEL_TYPE):
-                    raise ValueError(f"{self.MODEL_TYPE} can not be empty")
-                if not model_config.get(self.EMBEDDING_DIMENSION):
-                    raise ValueError(f"{self.EMBEDDING_DIMENSION} can not be empty")
-                if not model_config.get(self.FRAMEWORK_TYPE):
-                    raise ValueError(f"{self.FRAMEWORK_TYPE} can not be empty")
+                model_config = model_meta.get(MODEL_CONFIG_FIELD)
+                if not model_config.get(MODEL_TYPE):
+                    raise ValueError(f"{MODEL_TYPE} can not be empty")
+                if not model_config.get(EMBEDDING_DIMENSION):
+                    raise ValueError(f"{EMBEDDING_DIMENSION} can not be empty")
+                if not model_config.get(FRAMEWORK_TYPE):
+                    raise ValueError(f"{FRAMEWORK_TYPE} can not be empty")
             return True
         else:
             raise ValueError("Model metadata can't be empty")
 
-    def generate_hash(self, model_file_path: str) -> str:
+    def _generate_hash(self, model_file_path: str) -> str:
         """
         Generate sha1 hash value for the model zip file.
 
-        @param model_meta         dict     content of the model meta file
+        Parameters
+        ----------
+        :param model_file_path: file path of the model file
+        :type model_file_path: string
+
+
+        Returns
+        -------
+        :return: sha256 hash
+        :rtype: string
 
-        @return                   boolean  if all the required fields are present returns True otherwise
-                                            raise exception
         """
 
         sha256 = hashlib.sha256()
         with open(model_file_path, "rb") as file:
             while True:
                 chunk = file.read(BUF_SIZE)
                 if not chunk:
```

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/ndframe.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/ndframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
 import sys
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, List, Optional, TextIO, Tuple, Union
 
 import pandas as pd  # type: ignore
 
-from opensearch_py_ml.common import OPENSEARCH_TEST_CLIENT  # noqa: F401
 from opensearch_py_ml.query_compiler import QueryCompiler
 
 if TYPE_CHECKING:
     from opensearchpy import OpenSearch
 
     from opensearch_py_ml.index import Index
 
@@ -104,14 +103,16 @@
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.index`
         :pandas_api_docs:`pandas.Series.index`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
         >>> assert isinstance(df.index, oml.Index)
         >>> df.index.os_index_field
         '_id'
         >>> s = df['Carrier']
         >>> assert isinstance(s.index, oml.Index)
         >>> s.index.os_index_field
@@ -132,14 +133,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.dtypes`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=['Origin', 'AvgTicketPrice', 'timestamp', 'dayOfWeek'])
         >>> df.dtypes
         Origin                    object
         AvgTicketPrice           float64
         timestamp         datetime64[ns]
         dayOfWeek                  int64
         dtype: object
@@ -154,14 +157,16 @@
         Returns
         -------
         pandas.Series
             The data type of each column.
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=['Origin', 'AvgTicketPrice', 'timestamp', 'dayOfWeek'])
         >>> df.os_dtypes
         Origin            keyword
         AvgTicketPrice      float
         timestamp            date
         dayOfWeek            byte
         dtype: object
@@ -218,14 +223,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.mean`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"])
         >>> df.mean()  # doctest: +SKIP
         AvgTicketPrice                          628.254
         Cancelled                              0.128494
         dayOfWeek                               2.83598
         timestamp         2018-01-21 19:20:45.564438232
         dtype: object
@@ -267,14 +274,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.sum`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"])
         >>> df.sum()  # doctest: +SKIP
         AvgTicketPrice    8.20436e+06
         Cancelled                1678
         dayOfWeek               37035
         dtype: object
 
@@ -315,14 +324,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.min`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"])
         >>> df.min()  # doctest: +SKIP
         AvgTicketPrice                100.021
         Cancelled                       False
         dayOfWeek                           0
         timestamp         2018-01-01 00:00:00
         dtype: object
@@ -362,14 +373,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.var`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"])
         >>> df.var()  # doctest: +SKIP
         AvgTicketPrice    70964.570234
         Cancelled             0.111987
         dayOfWeek             3.761279
         dtype: float64
 
@@ -408,14 +421,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.std`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"])
         >>> df.std()  # doctest: +SKIP
         AvgTicketPrice    266.407061
         Cancelled           0.334664
         dayOfWeek           1.939513
         dtype: float64
 
@@ -454,14 +469,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.median`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"])
         >>> df.median() # doctest: +SKIP
         AvgTicketPrice                          640.363
         Cancelled                                 False
         dayOfWeek                                     3
         timestamp         2018-01-21 23:54:06.624776611
         dtype: object
@@ -503,14 +520,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.max`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"])
         >>> df.max()  # doctest: +SKIP
         AvgTicketPrice                1199.73
         Cancelled                        True
         dayOfWeek                           6
         timestamp         2018-02-11 23:50:12
         dtype: object
@@ -561,14 +580,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.nunique`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> columns = ['category', 'currency', 'customer_birth_date', 'customer_first_name', 'user']
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce', columns=columns)
         >>> df.nunique()
         category                6
         currency                1
         customer_birth_date     0
         customer_first_name    46
@@ -588,14 +609,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.std`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=["AvgTicketPrice", "Cancelled", "dayOfWeek", "timestamp", "DestCountry"])
         >>> df.mad() # doctest: +SKIP
         AvgTicketPrice    213.35497
         dayOfWeek           2.00000
         dtype: float64
 
         >>> df.mad(numeric_only=True) # doctest: +SKIP
@@ -633,14 +656,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.describe`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights', columns=['AvgTicketPrice', 'FlightDelayMin']) # ignoring percentiles
         >>> df.describe() # doctest: +SKIP
                AvgTicketPrice  FlightDelayMin
         count    13059.000000    13059.000000
         mean       628.253689       47.335171
         std        266.386661       96.743006
         min        100.020531        0.000000
```

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/operations.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,14 @@
         self, query_compiler: "QueryCompiler", bins: int
     ) -> Tuple[pd.DataFrame, pd.DataFrame]:
         return self._hist_aggs(query_compiler, bins)
 
     def idx(
         self, query_compiler: "QueryCompiler", axis: int, sort_order: str
     ) -> pd.Series:
-
         if axis == 1:
             # Fetch idx on Columns
             raise NotImplementedError(
                 "This feature is not implemented yet for 'axis = 1'"
             )
 
         # Fetch idx on Index
@@ -282,15 +281,14 @@
         query_compiler: "QueryCompiler",
         pd_aggs: List[str],
         is_dataframe: bool,
         os_size: int,
         numeric_only: bool = False,
         dropna: bool = True,
     ) -> Union[pd.DataFrame, pd.Series]:
-
         results = self._metric_aggs(
             query_compiler,
             pd_aggs=pd_aggs,
             numeric_only=numeric_only,
             dropna=dropna,
             os_mode_size=os_size,
         )
@@ -533,15 +531,14 @@
         # weights = [10066.,   263.,   386.,   264.,   273.,   390.,   324.,   438.,   261.,   394.]
         # len(weights) == 10
 
         # ES returns
         # weights = [10066.,   263.,   386.,   264.,   273.,   390.,   324.,   438.,   261.,   252.,    142.]
         # So sum last 2 buckets
         for field in numeric_source_fields:
-
             # in case of series let plotting.oml_hist_series thrown an exception
             if not response.get("aggregations"):
                 continue
 
             # in case of dataframe, throw warning that field is excluded
             if not response["aggregations"].get(field):
                 warnings.warn(
@@ -770,15 +767,14 @@
         self,
         query_compiler: "QueryCompiler",
         pd_aggs: List[str],
         quantiles: Union[int, float, List[int], List[float]],
         is_dataframe: bool = True,
         numeric_only: Optional[bool] = True,
     ) -> Union[pd.DataFrame, pd.Series]:
-
         percentiles = [
             quantile_to_percentile(x)
             for x in (
                 (quantiles,) if not isinstance(quantiles, (list, tuple)) else quantiles
             )
         ]
 
@@ -800,15 +796,14 @@
         # Display Output same as pandas does
         if isinstance(quantiles, float):
             return df.squeeze()
         else:
             return df if is_dataframe else df.transpose().iloc[0]
 
     def unique(self, query_compiler: "QueryCompiler") -> pd.Series:
-
         query_params, _ = self._resolve_tasks(query_compiler)
         body = Query(query_params.query)
 
         fields = query_compiler._mappings.all_source_fields()
         assert len(fields) == 1  # Unique is only for opensearch_py_ml.Series
         field = fields[0]
         bucket_key = f"unique_{field.column}"
@@ -1051,15 +1046,14 @@
 
             after_key: Optional[Dict[str, Any]] = composite_buckets.get(
                 "after_key", None
             )
             buckets: Sequence[Dict[str, Any]] = composite_buckets["buckets"]
 
             if after_key:
-
                 # yield the bucket which contains the result
                 yield buckets
 
                 body.composite_agg_after_key(
                     name=agg_name,
                     after_key=after_key,
                 )
@@ -1226,15 +1220,14 @@
         return pd.concat([df1, df2]).reindex(
             ["count", "mean", "std", "min", "25%", "50%", "75%", "max"]
         )
 
     def to_pandas(
         self, query_compiler: "QueryCompiler", show_progress: bool = False
     ) -> pd.DataFrame:
-
         df_list: List[pd.DataFrame] = []
         i = 0
         for df in self.search_yield_pandas_dataframes(query_compiler=query_compiler):
             if show_progress:
                 i = i + df.shape[0]
                 if i % DEFAULT_PROGRESS_REPORTING_NUM_ROWS == 0:
                     print(f"{datetime.now()}: read {i} rows")
```

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/plotting/__init__.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/plotting/_core.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/plotting/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-from opensearch_py_ml.common import OPENSEARCH_TEST_CLIENT  # noqa: F401
 from opensearch_py_ml.plotting._matplotlib.hist import hist_frame, hist_series
 
 
 def oml_hist_series(
     self,
     by=None,
     ax=None,
@@ -48,14 +47,15 @@
     Notes
     -----
     Derived from ``pandas.plotting._core.hist_frame 0.25.3``
 
     Examples
     --------
     >>> import matplotlib.pyplot as plt
+    >>> from tests import OPENSEARCH_TEST_CLIENT  # noqa: F401
     >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
     >>> df[df.OriginWeather == 'Sunny']['FlightTimeMin'].hist(alpha=0.5, density=True) # doctest: +SKIP
     >>> df[df.OriginWeather != 'Sunny']['FlightTimeMin'].hist(alpha=0.5, density=True) # doctest: +SKIP
     >>> plt.show() # doctest: +SKIP
 
     """
     return hist_series(
@@ -114,14 +114,16 @@
 
         ax.hist(data[col].dropna().values, bins=bins, **kwds)
 
     is for ``[col]`` and weights are a single array.
 
     Examples
     --------
+    >>> from tests import OPENSEARCH_TEST_CLIENT
+
     >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
     >>> hist = df.select_dtypes(include=[np.number]).hist(figsize=[10,10]) # doctest: +SKIP
     """
     return hist_frame(
         data,
         column=column,
         by=by,
```

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/plotting/_matplotlib/__init__.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/plotting/_matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/plotting/_matplotlib/hist.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/plotting/_matplotlib/hist.py`

 * *Files identical despite different names*

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/query.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,14 @@
     def top_hits_agg(
         self,
         name: str,
         source_columns: List[str],
         sort_order: str,
         size: int = 1,
     ) -> None:
-
         top_hits: Any = {}
         if sort_order:
             top_hits["sort"] = [{i: {"order": sort_order}} for i in source_columns]
         if source_columns:
             top_hits["_source"] = {"includes": source_columns}
         top_hits["size"] = size
         self._aggs[name] = {"top_hits": top_hits}
```

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/query_compiler.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/query_compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,14 @@
         field_mapping_cache = FieldMappingCache(self._mappings)
 
         rows = []
         index = []
 
         i = 0
         for i, hit in enumerate(results, 1):
-
             if "_source" in hit:
                 row = hit["_source"]
             else:
                 row = {}
 
             # script_fields appear in 'fields'
             if "fields" in hit:
```

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/series.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/series.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 
 import opensearch_py_ml.plotting
 from opensearch_py_ml.arithmetics import (
     ArithmeticNumber,
     ArithmeticSeries,
     ArithmeticString,
 )
-from opensearch_py_ml.common import OPENSEARCH_TEST_CLIENT  # noqa: F401
 from opensearch_py_ml.common import DEFAULT_NUM_ROWS_DISPLAYED, docstring_parameter
 from opensearch_py_ml.filter import (
     BooleanFilter,
     Equal,
     Greater,
     GreaterEqual,
     IsIn,
@@ -107,14 +106,15 @@
 
     See Also
     --------
     :pandas_api_docs:`pandas.Series`
 
     Examples
     --------
+    >>> from tests import OPENSEARCH_TEST_CLIENT
     >>> oml.Series(os_client=OPENSEARCH_TEST_CLIENT, os_index_pattern='flights', name='Carrier')
     0         Kibana Airlines
     1        Logstash Airways
     2        Logstash Airways
     3         Kibana Airlines
     4         Kibana Airlines
                    ...
@@ -175,14 +175,16 @@
         Notes
         -----
         - number of rows ``len(series)`` queries OpenSearch
         - number of columns == 1
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.Series(OPENSEARCH_TEST_CLIENT, 'ecommerce', name='total_quantity')
         >>> df.shape
         (4675, 1)
         """
         num_rows = len(self)
         num_columns = 1
 
@@ -224,14 +226,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.Series.rename`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
         >>> df.Carrier
         0         Kibana Airlines
         1        Logstash Airways
         2        Logstash Airways
         3         Kibana Airlines
         4         Kibana Airlines
@@ -300,14 +304,16 @@
         See Also
         --------
         :pandas_api_docs:`pandas.Series.value_counts`
         :os_api_docs:`search-aggregations-bucket-terms-aggregation`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
         >>> df['Carrier'].value_counts()
         Logstash Airways    3331
         JetBeats            3274
         Kibana Airlines     3234
         ES-Air              3220
         Name: Carrier, dtype: int64
@@ -616,14 +622,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.Series.quantile`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> oml_flights = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')
         >>> oml_flights["timestamp"].quantile([.2,.5,.75]) # doctest: +SKIP
         0.20   2018-01-09 04:30:57.289159912
         0.50   2018-01-21 23:39:27.031627441
         0.75   2018-02-01 04:54:59.256136963
         Name: timestamp, dtype: datetime64[ns]
 
@@ -720,14 +728,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.Series.mode`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> oml_ecommerce = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce')
         >>> oml_ecommerce["day_of_week"].mode()
         0    Thursday
         Name: day_of_week, dtype: object
 
         >>> oml_ecommerce["order_date"].mode()
         0   2016-12-02 20:36:58
@@ -788,14 +798,16 @@
         -------
         QueryFilter
             Boolean filter to be combined with other filters and
             then passed to DataFrame[...].
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(
         ...   OPENSEARCH_TEST_CLIENT, "ecommerce",
         ...   columns=["category", "taxful_total_price"]
         ... )
         >>> df[
         ...     df.category.os_match("Men's")
         ...     & (df.taxful_total_price > 200.0)
@@ -836,14 +848,16 @@
 
         Returns
         -------
         opensearch_py_ml.Series
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce').head(5)
         >>> df.taxful_total_price
         0     36.98
         1     53.98
         2    199.98
         3    174.98
         4     80.98
@@ -896,14 +910,16 @@
 
         Returns
         -------
         opensearch_py_ml.Series
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce').head(5)
         >>> df.taxful_total_price
         0     36.98
         1     53.98
         2    199.98
         3    174.98
         4     80.98
@@ -935,14 +951,16 @@
 
         Returns
         -------
         opensearch_py_ml.Series
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce').head(5)
         >>> df.taxful_total_price
         0     36.98
         1     53.98
         2    199.98
         3    174.98
         4     80.98
@@ -974,14 +992,16 @@
 
         Returns
         -------
         opensearch_py_ml.Series
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce').head(5)
         >>> df.taxful_total_price
         0     36.98
         1     53.98
         2    199.98
         3    174.98
         4     80.98
@@ -1013,14 +1033,16 @@
 
         Returns
         -------
         opensearch_py_ml.Series
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce').head(5)
         >>> df.taxful_total_price
         0     36.98
         1     53.98
         2    199.98
         3    174.98
         4     80.98
@@ -1052,14 +1074,16 @@
 
         Returns
         -------
         opensearch_py_ml.Series
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce').head(5)
         >>> df.taxful_total_price
         0     36.98
         1     53.98
         2    199.98
         3    174.98
         4     80.98
@@ -1091,14 +1115,16 @@
 
         Returns
         -------
         opensearch_py_ml.Series
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce').head(5)
         >>> df.taxful_total_price
         0     36.98
         1     53.98
         2    199.98
         3    174.98
         4     80.98
@@ -1130,14 +1156,16 @@
 
         Returns
         -------
         opensearch_py_ml.Series
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce').head(5)
         >>> df.taxful_total_price
         0     36.98
         1     53.98
         2    199.98
         3    174.98
         4     80.98
@@ -1162,14 +1190,16 @@
 
         Returns
         -------
         opensearch_py_ml.Series
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce').head(5)
         >>> df.taxful_total_price
         0     36.98
         1     53.98
         2    199.98
         3    174.98
         4     80.98
@@ -1194,14 +1224,16 @@
 
         Returns
         -------
         opensearch_py_ml.Series
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce').head(5)
         >>> df.taxful_total_price
         0     36.98
         1     53.98
         2    199.98
         3    174.98
         4     80.98
@@ -1226,14 +1258,16 @@
 
         Returns
         -------
         opensearch_py_ml.Series
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce').head(5)
         >>> df.taxful_total_price
         0     36.98
         1     53.98
         2    199.98
         3    174.98
         4     80.98
@@ -1258,14 +1292,16 @@
 
         Returns
         -------
         opensearch_py_ml.Series
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce').head(5)
         >>> df.taxful_total_price
         0     36.98
         1     53.98
         2    199.98
         3    174.98
         4     80.98
@@ -1290,14 +1326,16 @@
 
         Returns
         -------
         opensearch_py_ml.Series
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce').head(5)
         >>> df.total_quantity
         0    2
         1    2
         2    2
         3    2
         4    2
@@ -1322,14 +1360,16 @@
 
         Returns
         -------
         opensearch_py_ml.Series
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'ecommerce').head(5)
         >>> df.taxful_total_price
         0     36.98
         1     53.98
         2    199.98
         3    174.98
         4     80.98
@@ -1444,14 +1484,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.Series.max`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> s = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')['AvgTicketPrice']
         >>> int(s.max())
         1199
         """
         results = super().max(numeric_only=numeric_only)
         return results.squeeze()
 
@@ -1468,14 +1510,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.Series.mean`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> s = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')['AvgTicketPrice']
         >>> int(s.mean())
         628
         """
         results = super().mean(numeric_only=numeric_only)
         return results.squeeze()
 
@@ -1492,14 +1536,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.Series.median`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> s = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')['AvgTicketPrice']
         >>> int(s.median())
         640
         """
         results = super().median(numeric_only=numeric_only)
         return results.squeeze()
 
@@ -1516,14 +1562,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.Series.min`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> s = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')['AvgTicketPrice']
         >>> int(s.min())
         100
         """
         results = super().min(numeric_only=numeric_only)
         return results.squeeze()
 
@@ -1540,14 +1588,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.Series.sum`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> s = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')['AvgTicketPrice']
         >>> int(s.sum())
         8204364
         """
         results = super().sum(numeric_only=numeric_only)
         return results.squeeze()
 
@@ -1562,14 +1612,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.Series.nunique`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> s = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')['Carrier']
         >>> s.nunique()
         4
         """
         results = super().nunique()
         return results.squeeze()
 
@@ -1602,14 +1654,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.Series.var`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> s = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')['AvgTicketPrice']
         >>> int(s.var())
         70964
         """
         results = super().var(numeric_only=numeric_only)
         return results.squeeze()
 
@@ -1624,14 +1678,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.Series.var`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> s = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')['AvgTicketPrice']
         >>> int(s.std())
         266
         """
         results = super().std(numeric_only=numeric_only)
         return results.squeeze()
 
@@ -1646,14 +1702,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.Series.mad`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> s = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights')['AvgTicketPrice']
         >>> int(s.mad())
         213
         """
         results = super().mad(numeric_only=numeric_only)
         return results.squeeze()
 
@@ -1674,14 +1732,16 @@
 
         See Also
         --------
         :pandas_api_docs:`pandas.Series.describe`
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> df = oml.DataFrame(OPENSEARCH_TEST_CLIENT, 'flights') # ignoring percentiles as they don't generate consistent results
         >>> df.AvgTicketPrice.describe()  # doctest: +SKIP
         count    13059.000000
         mean       628.253689
         std        266.386661
         min        100.020531
         ...
@@ -1707,14 +1767,16 @@
         See Also
         --------
         :pandas_api_docs:`pandas.DataFrame.to_numpy`
         opensearch_to_pandas
 
         Examples
         --------
+        >>> from tests import OPENSEARCH_TEST_CLIENT
+
         >>> oml_s = oml.Series(OPENSEARCH_TEST_CLIENT, 'flights', name='Carrier').head(5)
         >>> pd_s = oml.opensearch_to_pandas(oml_s)
         >>> print(f"type(oml_s)={type(oml_s)}\\ntype(pd_s)={type(pd_s)}")
         type(oml_s)=<class 'opensearch_py_ml.series.Series'>
         type(pd_s)=<class 'pandas.core.series.Series'>
         >>> oml_s
         0     Kibana Airlines
```

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/tasks.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/tasks.py`

 * *Files identical despite different names*

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml/utils.py` & `opensearch_py_ml-1.1.0/opensearch_py_ml/utils.py`

 * *Files identical despite different names*

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml.egg-info/PKG-INFO` & `opensearch_py_ml-1.1.0/opensearch_py_ml.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: opensearch-py-ml
-Version: 1.0.0b1
+Version: 1.1.0
 Summary: Python Client and Toolkit for DataFrames, Big Data, Machine Learning and ETL in OpenSearch
 Home-page: https://github.com/opensearch-project/opensearch-py-ml
 Author: Dhrubo Saha
 Author-email: dhrubo@amazon.com, 
-Maintainer: Dhrubo Saha, Yaliang Wu
-Maintainer-email: dhrubo@amazon.com, ylwu@amazon.com
+Maintainer: Dhrubo Saha, Yaliang Wu, Alexander Greaves-Tunnell, Sicheng Song, Jing Zhang, Bhavana Goud Ramaram
+Maintainer-email: dhrubo@amazon.com, ylwu@amazon.com, greaa@amazon.com, seasonsg@amazon.com, jngz@amazon.com, rbhavna@amazon.com
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/opensearch-project/opensearch-py-ml
 Project-URL: Issue Tracker, https://github.com/opensearch-project/opensearch-py-ml/issues
 Keywords: Opensearch opensearch_py_ml pandas python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Environment :: Console
@@ -46,23 +46,35 @@
 - [Code of Conduct](https://github.com/opensearch-project/opensearch-py-ml#code-of-conduct)
 - [License](https://github.com/opensearch-project/opensearch-py-ml#license)
 - [Copyright](https://github.com/opensearch-project/opensearch-py-ml#copyright)
 
 ## Welcome!
 
 **opensearch-py-ml** is a Python client that provides a suite of data analytics and machine learning tools for OpenSearch.
-**Opensearch-py-ml is an experimental project**
+
 It is [a community-driven, open source fork](https://aws.amazon.com/blogs/opensource/introducing-opensearch/) a fork of [eland](https://github.com/elastic/eland), which provides data analysis and machine learning
 licensed under the [Apache v2.0 License](https://github.com/opensearch-project/opensearch-py/blob/main/LICENSE.txt). 
 
 **opensearch-py-ml** lets users call OpenSearch indices and manipulate them as if they were pandas DataFrames, supporting
 complex filtering and aggregation operations. It also provides rudimentary support for uploading models to OpenSearch
 clusters using the [ml-commons](https://github.com/opensearch-project/ml-commons) plugin.
 
 
+For more information, see [opensearch.org](https://opensearch.org/docs/latest/clients/opensearch-py-ml/) and the [API Doc](https://opensearch-project.github.io/opensearch-py-ml/index.html).
+
+
+##Installing Opensearch-py-ml
+
+
+Opensearch-py-ml can be installed from [PyPI](https://pypi.org/project/opensearch-py-ml) via pip:
+
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+    $ python -m pip install opensearch-py-ml
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
 ## Code of Conduct
 
 This project has adopted the 
 [Amazon Open Source Code of Conduct](https://github.com/opensearch-project/opensearch-py-ml/blob/main/CODE_OF_CONDUCT.md).
 For more information see the [Code of Conduct FAQ](https://aws.github.io/code-of-conduct-faq), or contact 
 [opensource-codeofconduct@amazon.com](mailto:opensource-codeofconduct@amazon.com) with any additional questions or comments.
```

### Comparing `opensearch_py_ml-1.0.0b1/opensearch_py_ml.egg-info/SOURCES.txt` & `opensearch_py_ml-1.1.0/opensearch_py_ml.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -26,22 +26,28 @@
 opensearch_py_ml/utils.py
 opensearch_py_ml.egg-info/PKG-INFO
 opensearch_py_ml.egg-info/SOURCES.txt
 opensearch_py_ml.egg-info/dependency_links.txt
 opensearch_py_ml.egg-info/not-zip-safe
 opensearch_py_ml.egg-info/requires.txt
 opensearch_py_ml.egg-info/top_level.txt
-opensearch_py_ml/ml_commons_integration/__init__.py
-opensearch_py_ml/ml_commons_integration/ml_common_client.py
-opensearch_py_ml/ml_commons_integration/ml_common_utils.py
-opensearch_py_ml/ml_commons_integration/load/__init__.py
-opensearch_py_ml/ml_commons_integration/load/ml_common_load_client.py
-opensearch_py_ml/ml_commons_integration/predict/__init__.py
-opensearch_py_ml/ml_commons_integration/predict/ml_common_predict_client.py
-opensearch_py_ml/ml_commons_integration/upload/__init__.py
-opensearch_py_ml/ml_commons_integration/upload/ml_common_model_uploader.py
+opensearch_py_ml/ml_commons/__init__.py
+opensearch_py_ml/ml_commons/ml_common_utils.py
+opensearch_py_ml/ml_commons/ml_commons_client.py
+opensearch_py_ml/ml_commons/model_execute.py
+opensearch_py_ml/ml_commons/model_uploader.py
+opensearch_py_ml/ml_models/__init__.py
+opensearch_py_ml/ml_models/sentencetransformermodel.py
+opensearch_py_ml/ml_models/metrics_correlation/__init__.py
+opensearch_py_ml/ml_models/metrics_correlation/dip.py
+opensearch_py_ml/ml_models/metrics_correlation/event_detection.py
+opensearch_py_ml/ml_models/metrics_correlation/mcorr.py
+opensearch_py_ml/ml_models/metrics_correlation/nmf.py
+opensearch_py_ml/ml_models/metrics_correlation/utils.py
+opensearch_py_ml/ml_models/metrics_correlation/wavelet_piecewise_const.py
+opensearch_py_ml/ml_models/metrics_correlation/wavelet_tools.py
 opensearch_py_ml/plotting/__init__.py
 opensearch_py_ml/plotting/_core.py
 opensearch_py_ml/plotting/_matplotlib/__init__.py
 opensearch_py_ml/plotting/_matplotlib/hist.py
-opensearch_py_ml/sentence_transformer_model/__init__.py
-opensearch_py_ml/sentence_transformer_model/sentencetransformermodel.py
+tests/test_common_pytest.py
+tests/test_utils_pytest.py
```

### Comparing `opensearch_py_ml-1.0.0b1/setup.py` & `opensearch_py_ml-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,17 @@
     packages=find_packages(include=["opensearch_py_ml", "opensearch_py_ml.*"]),
     project_urls={
         "Source Code": "https://github.com/opensearch-project/opensearch-py-ml",
         "Issue Tracker": "https://github.com/opensearch-project/opensearch-py-ml/issues",
     },
     install_requires=[
         "opensearch-py>=2",
-        "pandas>=1.5,<2",
+        "pandas>=1.5,<3",
         "matplotlib>=3.6.0,<4",
-        "numpy>=1.23.3,<2",
+        "numpy>=1.24.0,<2",
     ],
     python_requires=">=3.8",
     package_data={"opensearch_py_ml": ["py.typed"]},
     include_package_data=True,
     zip_safe=False,
     extras_require=extras,
 )
```

