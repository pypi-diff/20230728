# Comparing `tmp/arfs-1.1.4.tar.gz` & `tmp/arfs-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arfs-1.1.4.tar", last modified: Mon Jul  3 15:51:50 2023, max compression
+gzip compressed data, was "arfs-2.0.0.tar", last modified: Fri Jul 28 10:36:17 2023, max compression
```

## Comparing `arfs-1.1.4.tar` & `arfs-2.0.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 15:51:50.114192 arfs-1.1.4/
--rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-1.1.4/LICENSE.md
--rw-rw-rw-   0        0        0    11069 2023-07-03 15:51:50.115159 arfs-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    10379 2023-01-09 09:31:15.000000 arfs-1.1.4/README.md
--rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0     1389 2023-07-03 15:51:50.133158 arfs-1.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 15:51:49.264744 arfs-1.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 15:51:49.465745 arfs-1.1.4/src/arfs/
--rw-rw-rw-   0        0        0       92 2023-07-03 15:48:57.000000 arfs-1.1.4/src/arfs/__init__.py
--rw-rw-rw-   0        0        0    86574 2023-04-27 11:30:49.000000 arfs-1.1.4/src/arfs/association.py
--rw-rw-rw-   0        0        0     6677 2023-01-06 14:55:48.000000 arfs-1.1.4/src/arfs/benchmark.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:51:49.267756 arfs-1.1.4/src/arfs/dataset/
-drwxrwxrwx   0        0        0        0 2023-07-03 15:51:49.710749 arfs-1.1.4/src/arfs/dataset/data/
--rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-1.1.4/src/arfs/dataset/data/boston_bunch.joblib
--rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-1.1.4/src/arfs/dataset/data/housing.zip
-drwxrwxrwx   0        0        0        0 2023-07-03 15:51:50.029157 arfs-1.1.4/src/arfs/feature_selection/
--rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-1.1.4/src/arfs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0    90379 2023-06-09 19:54:49.000000 arfs-1.1.4/src/arfs/feature_selection/allrelevant.py
--rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-1.1.4/src/arfs/feature_selection/base.py
--rw-rw-rw-   0        0        0    13420 2023-05-21 19:11:19.000000 arfs-1.1.4/src/arfs/feature_selection/mrmr.py
--rw-rw-rw-   0        0        0     2457 2023-05-21 19:11:19.000000 arfs-1.1.4/src/arfs/feature_selection/summary.py
--rw-rw-rw-   0        0        0    15454 2023-07-03 11:13:30.000000 arfs-1.1.4/src/arfs/feature_selection/unsupervised.py
--rw-rw-rw-   0        0        0    14769 2023-07-03 11:13:51.000000 arfs-1.1.4/src/arfs/feature_selection/variable_importance.py
--rw-rw-rw-   0        0        0    21927 2023-06-16 08:19:41.000000 arfs-1.1.4/src/arfs/gbm.py
--rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-1.1.4/src/arfs/parallel.py
--rw-rw-rw-   0        0        0    30283 2023-05-31 17:10:21.000000 arfs-1.1.4/src/arfs/preprocessing.py
--rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-1.1.4/src/arfs/sampling.py
--rw-rw-rw-   0        0        0    24872 2023-05-21 19:11:19.000000 arfs-1.1.4/src/arfs/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:51:49.590746 arfs-1.1.4/src/arfs.egg-info/
--rw-rw-rw-   0        0        0    11069 2023-07-03 15:51:49.000000 arfs-1.1.4/src/arfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-07-03 15:51:49.000000 arfs-1.1.4/src/arfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 15:51:49.000000 arfs-1.1.4/src/arfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-1.1.4/src/arfs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      365 2023-07-03 15:51:49.000000 arfs-1.1.4/src/arfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-03 15:51:49.000000 arfs-1.1.4/src/arfs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 15:51:50.086156 arfs-1.1.4/tests/
--rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-1.1.4/tests/test_allrelevant.py
--rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-1.1.4/tests/test_featselect.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.816036 arfs-2.0.0/
+-rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-2.0.0/LICENSE.md
+-rw-rw-rw-   0        0        0    11965 2023-07-28 10:36:17.819028 arfs-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11275 2023-07-28 10:30:07.000000 arfs-2.0.0/README.md
+-rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1433 2023-07-28 10:36:17.831029 arfs-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.380027 arfs-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.531030 arfs-2.0.0/src/arfs/
+-rw-rw-rw-   0        0        0       92 2023-07-28 09:19:12.000000 arfs-2.0.0/src/arfs/__init__.py
+-rw-rw-rw-   0        0        0    86458 2023-07-27 13:54:59.000000 arfs-2.0.0/src/arfs/association.py
+-rw-rw-rw-   0        0        0     6689 2023-07-24 20:31:43.000000 arfs-2.0.0/src/arfs/benchmark.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.382040 arfs-2.0.0/src/arfs/dataset/
+drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.624028 arfs-2.0.0/src/arfs/dataset/data/
+-rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-2.0.0/src/arfs/dataset/data/boston_bunch.joblib
+-rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-2.0.0/src/arfs/dataset/data/housing.zip
+drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.758029 arfs-2.0.0/src/arfs/feature_selection/
+-rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-2.0.0/src/arfs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0    94894 2023-07-28 09:23:30.000000 arfs-2.0.0/src/arfs/feature_selection/allrelevant.py
+-rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-2.0.0/src/arfs/feature_selection/base.py
+-rw-rw-rw-   0        0        0    19893 2023-07-26 16:20:34.000000 arfs-2.0.0/src/arfs/feature_selection/lasso.py
+-rw-rw-rw-   0        0        0    13397 2023-07-27 13:39:47.000000 arfs-2.0.0/src/arfs/feature_selection/mrmr.py
+-rw-rw-rw-   0        0        0     2457 2023-05-21 19:11:19.000000 arfs-2.0.0/src/arfs/feature_selection/summary.py
+-rw-rw-rw-   0        0        0    15832 2023-07-26 16:49:41.000000 arfs-2.0.0/src/arfs/feature_selection/unsupervised.py
+-rw-rw-rw-   0        0        0    15689 2023-07-24 19:47:35.000000 arfs-2.0.0/src/arfs/feature_selection/variable_importance.py
+-rw-rw-rw-   0        0        0    21927 2023-06-16 08:19:41.000000 arfs-2.0.0/src/arfs/gbm.py
+-rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-2.0.0/src/arfs/parallel.py
+-rw-rw-rw-   0        0        0    40462 2023-07-27 07:24:21.000000 arfs-2.0.0/src/arfs/preprocessing.py
+-rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-2.0.0/src/arfs/sampling.py
+-rw-rw-rw-   0        0        0    25248 2023-07-26 08:46:59.000000 arfs-2.0.0/src/arfs/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.602028 arfs-2.0.0/src/arfs.egg-info/
+-rw-rw-rw-   0        0        0    11965 2023-07-28 10:36:17.000000 arfs-2.0.0/src/arfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2023-07-28 10:36:17.000000 arfs-2.0.0/src/arfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 10:36:17.000000 arfs-2.0.0/src/arfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-2.0.0/src/arfs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      405 2023-07-28 10:36:17.000000 arfs-2.0.0/src/arfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-28 10:36:17.000000 arfs-2.0.0/src/arfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.796031 arfs-2.0.0/tests/
+-rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-2.0.0/tests/test_allrelevant.py
+-rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-2.0.0/tests/test_featselect.py
```

### Comparing `arfs-1.1.4/LICENSE.md` & `arfs-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arfs-1.1.4/PKG-INFO` & `arfs-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 1.1.4
+Version: 2.0.0
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
@@ -28,28 +28,35 @@
 
 # All relevant feature selection
 
 All relevant feature selection means trying to find all features carrying information usable for prediction, rather than finding a possibly compact subset of features on which some particular model has a minimal error. This might include redundant predictors. All relevant feature selection is model agnostic in the sense that it doesn't optimize a scoring function for a *specific* model but rather tries to select all the predictors which are related to the response. 
 
 This package implements 3 different methods (Leshy is an evolution of Boruta, BoostAGroota is an evolution of BoostARoota and GrootCV is a new one). They are sklearn compatible. See hereunder for details about those methods. You can use any sklearn compatible estimator with Leshy and BoostAGroota but I recommend lightGBM. It's fast, accurate and has SHAP values builtin. It also provides a module for performing preprocessing and perform basic feature selection (autobinning, remove columns with too many missing values, zero variance, high-cardinality, highly correlated, etc.). Examples and detailled methods hereunder.
 
-Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method.
+Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for intrucing non-linearities into linear models and perform feature selection.
+
+Please note that one limitation of the lasso is that it treats the levels of a categorical predictor individually. However, this issue can be addressed by utilizing the `TreeDiscretizer`, which automatically bins numerical variables and groups the levels of categorical variables.
 
 ## Installation
 
 `$ pip install arfs`, requires python <3.10
 
 ## Example
 
 Working examples for:
 
  - [Preprocessing](./docs/notebooks/preprocessingipynb)
  - [Basic FS (best before ARFS)](./docs/notebooks/basic_feature_selection.ipynb)
  - [Regression](./docs/notebooks/arfs_regression.ipynb)
  - [Classification](./docs/notebooks/arfs_classification.ipynb)
+ - [LASSO and (G)LM feature selection](./docs/notebooks/lasso_feature_selection.ipynb)
+ - [Passing custom params](./docs/notebooks/arfs_grootcv_custom_params.ipynb)
+ - [Non-normal loss and sample weights](./docs/notebooks/arfs_non_normal_loss_and_sample_weight.ipynb)
+ - [ARFS on GPU](./docs/notebooks/arfs_on_GPU.ipynb)
+ - [Fast Shap](./docs/notebooks/arfs_shap_vs_fastshap.ipynb)
  - [Categoricals](./docs/notebooks/issue_categoricals.ipynb)
  - [Collinearity](./docs/notebooks/issue_collinearity.ipynb)
  - [Reducing run time for large data](./docs/notebooks/arfs_large_data_sampling.ipynb)
  - [Comparison to Boruta and BorutaShap](./docs/notebooks/arfs_boruta_borutaShap_comparison.ipynb)
  - [MRmr alternative](./docs/notebooks/mrmr_feature_selection.ipynb)
  - [MRmr vs ARFS](./docs/notebooks/mrmr_fs_VS_arfs.ipynb)
```

### Comparing `arfs-1.1.4/README.md` & `arfs-2.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,35 @@
 
 # All relevant feature selection
 
 All relevant feature selection means trying to find all features carrying information usable for prediction, rather than finding a possibly compact subset of features on which some particular model has a minimal error. This might include redundant predictors. All relevant feature selection is model agnostic in the sense that it doesn't optimize a scoring function for a *specific* model but rather tries to select all the predictors which are related to the response. 
 
 This package implements 3 different methods (Leshy is an evolution of Boruta, BoostAGroota is an evolution of BoostARoota and GrootCV is a new one). They are sklearn compatible. See hereunder for details about those methods. You can use any sklearn compatible estimator with Leshy and BoostAGroota but I recommend lightGBM. It's fast, accurate and has SHAP values builtin. It also provides a module for performing preprocessing and perform basic feature selection (autobinning, remove columns with too many missing values, zero variance, high-cardinality, highly correlated, etc.). Examples and detailled methods hereunder.
 
-Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method.
+Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for intrucing non-linearities into linear models and perform feature selection.
+
+Please note that one limitation of the lasso is that it treats the levels of a categorical predictor individually. However, this issue can be addressed by utilizing the `TreeDiscretizer`, which automatically bins numerical variables and groups the levels of categorical variables.
 
 ## Installation
 
 `$ pip install arfs`, requires python <3.10
 
 ## Example
 
 Working examples for:
 
  - [Preprocessing](./docs/notebooks/preprocessingipynb)
  - [Basic FS (best before ARFS)](./docs/notebooks/basic_feature_selection.ipynb)
  - [Regression](./docs/notebooks/arfs_regression.ipynb)
  - [Classification](./docs/notebooks/arfs_classification.ipynb)
+ - [LASSO and (G)LM feature selection](./docs/notebooks/lasso_feature_selection.ipynb)
+ - [Passing custom params](./docs/notebooks/arfs_grootcv_custom_params.ipynb)
+ - [Non-normal loss and sample weights](./docs/notebooks/arfs_non_normal_loss_and_sample_weight.ipynb)
+ - [ARFS on GPU](./docs/notebooks/arfs_on_GPU.ipynb)
+ - [Fast Shap](./docs/notebooks/arfs_shap_vs_fastshap.ipynb)
  - [Categoricals](./docs/notebooks/issue_categoricals.ipynb)
  - [Collinearity](./docs/notebooks/issue_collinearity.ipynb)
  - [Reducing run time for large data](./docs/notebooks/arfs_large_data_sampling.ipynb)
  - [Comparison to Boruta and BorutaShap](./docs/notebooks/arfs_boruta_borutaShap_comparison.ipynb)
  - [MRmr alternative](./docs/notebooks/mrmr_feature_selection.ipynb)
  - [MRmr vs ARFS](./docs/notebooks/mrmr_fs_VS_arfs.ipynb)
```

### Comparing `arfs-1.1.4/setup.cfg` & `arfs-2.0.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -52,36 +52,39 @@
 00000330: 0d0a 096e 756d 7079 3e3d 312e 3231 0d0a  ...numpy>=1.21..
 00000340: 0970 616e 6461 733e 3d31 2e34 0d0a 0970  .pandas>=1.4...p
 00000350: 616e 656c 3e3d 302e 3133 0d0a 0973 6369  anel>=0.13...sci
 00000360: 6b69 745f 6c65 6172 6e3e 3d31 2e30 0d0a  kit_learn>=1.0..
 00000370: 0973 6369 7079 3e3d 312e 382e 300d 0a09  .scipy>=1.8.0...
 00000380: 7365 6162 6f72 6e3e 3d30 2e31 312e 320d  seaborn>=0.11.2.
 00000390: 0a09 7368 6170 3e3d 302e 3430 2e30 0d0a  ..shap>=0.40.0..
-000003a0: 0974 7164 6d3e 3d34 2e36 322e 330d 0a0d  .tqdm>=4.62.3...
-000003b0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-000003c0: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-000003d0: 3d20 7372 630d 0a0d 0a5b 6f70 7469 6f6e  = src....[option
-000003e0: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
-000003f0: 0a61 7266 732e 6461 7461 7365 742e 6461  .arfs.dataset.da
-00000400: 7461 203d 200d 0a09 2a2e 6a6f 626c 6962  ta = ...*.joblib
-00000410: 0d0a 092a 2e7a 6970 0d0a 6172 6673 2e64  ...*.zip..arfs.d
-00000420: 6174 6173 6574 2e64 6573 6372 6970 7469  ataset.descripti
-00000430: 6f6e 203d 200d 0a09 2a2e 7273 740d 0a0d  on = ...*.rst...
-00000440: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
-00000450: 5f72 6571 7569 7265 5d0d 0a64 6f63 7320  _require]..docs 
-00000460: 3d20 0d0a 096e 6273 7068 696e 783e 3d30  = ...nbsphinx>=0
-00000470: 2e38 2e38 0d0a 0969 7079 6b65 726e 656c  .8.8...ipykernel
-00000480: 3e3d 362e 392e 310d 0a09 6970 7974 686f  >=6.9.1...ipytho
-00000490: 6e5f 6765 6e75 7469 6c73 0d0a 0970 616e  n_genutils...pan
-000004a0: 646f 630d 0a09 7370 6869 6e78 3e3d 342e  doc...sphinx>=4.
-000004b0: 342e 300d 0a09 7370 6869 6e78 2d61 7574  4.0...sphinx-aut
-000004c0: 6f64 6f63 2d74 7970 6568 696e 7473 3e3d  odoc-typehints>=
-000004d0: 312e 3136 2e30 0d0a 0973 7068 696e 782d  1.16.0...sphinx-
-000004e0: 636f 7079 6275 7474 6f6e 3e3d 302e 352e  copybutton>=0.5.
-000004f0: 300d 0a09 7370 6869 6e78 2d72 7464 2d74  0...sphinx-rtd-t
-00000500: 6865 6d65 3e3d 312e 302e 300d 0a09 7370  heme>=1.0.0...sp
-00000510: 6869 6e78 2d74 6162 733e 3d33 2e32 2e30  hinx-tabs>=3.2.0
-00000520: 0d0a 7465 7374 203d 200d 0a09 7079 7465  ..test = ...pyte
-00000530: 7374 0d0a 0970 7974 6573 742d 636f 760d  st...pytest-cov.
-00000540: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000550: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000560: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+000003a0: 0974 7164 6d3e 3d34 2e36 322e 330d 0a09  .tqdm>=4.62.3...
+000003b0: 6661 7374 7472 6565 7368 6170 3e3d 302e  fasttreeshap>=0.
+000003c0: 312e 360d 0a09 7374 6174 736d 6f64 656c  1.6...statsmodel
+000003d0: 733e 3d30 2e31 342e 300d 0a0d 0a5b 6f70  s>=0.14.0....[op
+000003e0: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+000003f0: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
+00000400: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  c....[options.pa
+00000410: 636b 6167 655f 6461 7461 5d0d 0a61 7266  ckage_data]..arf
+00000420: 732e 6461 7461 7365 742e 6461 7461 203d  s.dataset.data =
+00000430: 200d 0a09 2a2e 6a6f 626c 6962 0d0a 092a   ...*.joblib...*
+00000440: 2e7a 6970 0d0a 6172 6673 2e64 6174 6173  .zip..arfs.datas
+00000450: 6574 2e64 6573 6372 6970 7469 6f6e 203d  et.description =
+00000460: 200d 0a09 2a2e 7273 740d 0a0d 0a5b 6f70   ...*.rst....[op
+00000470: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
+00000480: 7569 7265 5d0d 0a64 6f63 7320 3d20 0d0a  uire]..docs = ..
+00000490: 096e 6273 7068 696e 783e 3d30 2e38 2e38  .nbsphinx>=0.8.8
+000004a0: 0d0a 0969 7079 6b65 726e 656c 3e3d 362e  ...ipykernel>=6.
+000004b0: 392e 310d 0a09 6970 7974 686f 6e5f 6765  9.1...ipython_ge
+000004c0: 6e75 7469 6c73 0d0a 0970 616e 646f 630d  nutils...pandoc.
+000004d0: 0a09 7370 6869 6e78 3e3d 342e 342e 300d  ..sphinx>=4.4.0.
+000004e0: 0a09 7370 6869 6e78 2d61 7574 6f64 6f63  ..sphinx-autodoc
+000004f0: 2d74 7970 6568 696e 7473 3e3d 312e 3136  -typehints>=1.16
+00000500: 2e30 0d0a 0973 7068 696e 782d 636f 7079  .0...sphinx-copy
+00000510: 6275 7474 6f6e 3e3d 302e 352e 300d 0a09  button>=0.5.0...
+00000520: 7370 6869 6e78 2d72 7464 2d74 6865 6d65  sphinx-rtd-theme
+00000530: 3e3d 312e 302e 300d 0a09 7370 6869 6e78  >=1.0.0...sphinx
+00000540: 2d74 6162 733e 3d33 2e32 2e30 0d0a 7465  -tabs>=3.2.0..te
+00000550: 7374 203d 200d 0a09 7079 7465 7374 0d0a  st = ...pytest..
+00000560: 0970 7974 6573 742d 636f 760d 0a0d 0a5b  .pytest-cov....[
+00000570: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000580: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000590: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `arfs-1.1.4/src/arfs/association.py` & `arfs-2.0.0/src/arfs/association.py`

 * *Files 0% similar despite different names*

```diff
@@ -1556,15 +1556,15 @@
     cat_cols = dtypes_dic["cat"]
 
     if not isinstance(y, pd.Series):
         y = pd.Series(y)
         y.name = "target"
 
     target = y.name
-    X = pd.concat([X, y], axis=1, ignore_index=False)
+    X[target] = y.values
     # sanity checks
     X, sample_weight = _check_association_input(X, sample_weight, handle_na)
 
     y = X[target].copy()
     X = X.drop(target, axis=1)
 
     # define the number of cores
@@ -1630,15 +1630,15 @@
         F-statistic for each feature of shape (n_features,)
     """
     if not isinstance(y, pd.Series):
         y = pd.Series(y)
         y.name = "target"
 
     target = y.name
-    X = pd.concat([X, y], axis=1, ignore_index=False)
+    X[target] = y.values
     # sanity checks
     X, sample_weight = _check_association_input(X, sample_weight, handle_na)
 
     correlation_coefficient = wcorr_series(X, target, sample_weight, n_jobs, handle_na)
 
     deg_of_freedom = y.size - 2
     corr_coef_squared = correlation_coefficient**2
@@ -1801,15 +1801,15 @@
     num_cols = dtypes_dic["num"]
 
     if not isinstance(y, pd.Series):
         y = pd.Series(y)
         y.name = "target"
 
     target = y.name
-    X = pd.concat([X, y], axis=1, ignore_index=False)
+    X[target] = y.values
     # sanity checks
     X, sample_weight = _check_association_input(X, sample_weight, handle_na)
 
     y = X[target].copy()
     X = X.drop(target, axis=1)
 
     # define the number of cores
@@ -1872,15 +1872,15 @@
         F-statistic for each feature of shape (n_features,)
     """
     if not isinstance(y, pd.Series):
         y = pd.Series(y)
         y.name = "target"
 
     target = y.name
-    X = pd.concat([X, y], axis=1, ignore_index=False)
+    X[target] = y.values
     # sanity checks
     X, sample_weight = _check_association_input(X, sample_weight, handle_na)
 
     deg_of_freedom = y.size - 2
 
     theils_u_coef = theils_u_series(X, target, sample_weight, n_jobs, handle_na)
     theils_u_coef_squared = theils_u_coef**2
```

### Comparing `arfs-1.1.4/src/arfs/benchmark.py` & `arfs-2.0.0/src/arfs/benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         the predictors frame
     y : pd.Series
         the target (same length as X)
     sample_weight : None or pd.Series, optional
         sample weights if any, by default None
     """
 
-    varimp_list = ["shap", "pimp", "native"]
+    varimp_list = ["shap", "fastshap", "pimp", "native"]
     for model, varimp in itertools.product(models, varimp_list):
         print(
             "=" * 20
             + " "
             + str(feat_selector.__class__.__name__)
             + " - testing: {mod:>25} for var.imp: {vimp:<15} ".format(
                 mod=str(model.__class__.__name__), vimp=varimp
```

### Comparing `arfs-1.1.4/src/arfs/dataset/data/boston_bunch.joblib` & `arfs-2.0.0/src/arfs/dataset/data/boston_bunch.joblib`

 * *Files identical despite different names*

### Comparing `arfs-1.1.4/src/arfs/dataset/data/housing.zip` & `arfs-2.0.0/src/arfs/dataset/data/housing.zip`

 * *Files identical despite different names*

### Comparing `arfs-1.1.4/src/arfs/feature_selection/__init__.py` & `arfs-2.0.0/src/arfs/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.4/src/arfs/feature_selection/allrelevant.py` & `arfs-2.0.0/src/arfs/feature_selection/allrelevant.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 from sklearn.utils.validation import check_is_fitted
 from sklearn.feature_selection._base import SelectorMixin
 from sklearn.model_selection import RepeatedKFold, train_test_split
 from sklearn.inspection import permutation_importance
 from sklearn.utils.validation import _check_sample_weight
 from matplotlib.lines import Line2D
 from lightgbm import early_stopping
+from fasttreeshap import TreeExplainer as FastTreeExplainer
 
 from ..utils import (
     check_if_tree_based,
     is_lightgbm,
     is_catboost,
     create_dtype_dict,
     get_pandas_cat_codes,
@@ -166,15 +167,15 @@
         Level at which the corrected p-values will get rejected in both
         correction steps.
     importance : str, default = 'shap'
         The kind of variable importance used to compare and discriminate original
         vs shadow predictors. Note that the builtin tree importance (gini/impurity based
         importance) is biased towards numerical and large cardinality predictors, even
         if they are random. Shapley values and permutation imp. are robust w.r.t those predictors.
-        Possible values: 'shap' (Shapley values),
+        Possible values: 'shap' (Shapley values), 'fastshap' (FastTreeShap implementation),
         'pimp' (permutation importance) and 'native' (Gini/impurity)
     two_step : Boolean, default = True
         If you want to use the original implementation of Boruta with Bonferroni
         correction only set this to False.
     max_iter : int, default = 100
         The number of maximum iterations to perform.
     random_state : int, RandomState instance or None; default=None
@@ -261,15 +262,15 @@
 
     def __init__(
         self,
         estimator,
         n_estimators=1000,
         perc=90,
         alpha=0.05,
-        importance="shap",
+        importance="fastshap",
         two_step=True,
         max_iter=100,
         random_state=None,
         verbose=0,
         keep_weak=False,
     ):
         self.estimator = estimator
@@ -538,14 +539,18 @@
         x_sha = x_sha.apply(self.random_state.permutation, axis=0)
         x_sha.columns = [f"Shadow_{i}" for i in range(x_sha.shape[1])]
         # get importance of the merged matrix
         if self.importance == "shap":
             imp = _get_shap_imp(
                 self.estimator, pd.concat([x_cur, x_sha], axis=1), y, sample_weight
             )
+        elif self.importance == "fastshap":
+            imp = _get_shap_imp_fast(
+                self.estimator, pd.concat([x_cur, x_sha], axis=1), y, sample_weight
+            )
         elif self.importance == "pimp":
             imp = _get_perm_imp(
                 self.estimator, pd.concat([x_cur, x_sha], axis=1), y, sample_weight
             )
         else:
             imp = _get_imp(
                 self.estimator, pd.concat([x_cur, x_sha], axis=1), y, sample_weight
@@ -1210,15 +1215,14 @@
     # Clone the estimator to avoid modifying the original one
     estimator = clone(estimator)
 
     # Split the data into train and test sets and fit the model
     model, X_tt, y_tt, w_tt = _split_fit_estimator(
         estimator, X, y, sample_weight=sample_weight, cat_feature=cat_feature
     )
-
     # Compute the SHAP values
     if is_lightgbm(estimator):
         # For LightGBM models use the built-in SHAP method
         shap_matrix = model.predict(X_tt, pred_contrib=True)
 
         # The shape of the shap_matrix depends on whether the estimator is a classifier or a regressor
         if is_classifier(estimator) and (len(np.unique(y_tt)) > 2):
@@ -1234,30 +1238,68 @@
             shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
     else:
         # For other tree-based models, use the shap.TreeExplainer method to compute SHAP values
         explainer = shap.TreeExplainer(
             model, feature_perturbation="tree_path_dependent"
         )
         shap_values = explainer.shap_values(X_tt)
-
         # For multi-class classifiers, reshape the shap_values
         if is_classifier(estimator):
             if isinstance(shap_values, list):
                 # For LightGBM classifier in sklearn API, SHAP returns a list of arrays
                 # https://github.com/slundberg/shap/issues/526
-                class_inds = range(len(shap_values))
-                shap_imp = np.zeros(shap_values[0].shape[1])
-                for i, ind in enumerate(class_inds):
-                    shap_imp += np.abs(shap_values[ind]).mean(0)
-                shap_imp /= len(shap_values)
+                shap_imp = np.mean([np.abs(sv).mean(0) for sv in shap_values], axis=0)
             else:
                 shap_imp = np.abs(shap_values).mean(0)
         else:
             shap_imp = np.abs(shap_values).mean(0)
+    return shap_imp
+        
+def _get_shap_imp_fast(estimator, X, y, sample_weight=None, cat_feature=None):
+    """Get the SHAP feature importance using the fasttreeshap implementation
 
+    Parameters
+    ----------
+    estimator : estimator object
+        An estimator object implementing `fit` and `predict` methods.
+    X : pd.DataFrame of shape [n_samples, n_features]
+        Predictor matrix.
+    y : pd.Series of shape [n_samples]
+        Target variable.
+    sample_weight : array-like, shape = [n_samples], default=None
+        Individual weights for each sample.
+    cat_feature : list of int or None, default=None
+        The list of integers, columns loc, of the categorical predictors. Avoids detecting and encoding
+        each iteration if the exact same columns are passed to the selection methods.
+
+    Returns
+    -------
+    shap_imp : array
+        The SHAP importance array.
+    """
+    # Clone the estimator to avoid modifying the original one
+    estimator = clone(estimator)
+
+    # Split the data into train and test sets and fit the model
+    model, X_tt, y_tt, w_tt = _split_fit_estimator(
+        estimator, X, y, sample_weight=sample_weight, cat_feature=cat_feature
+    )
+    explainer = FastTreeExplainer(model, algorithm="auto", shortcut=False, feature_perturbation="tree_path_dependent")
+    shap_matrix = explainer.shap_values(X_tt)
+    # multiclass returns a list
+    # for binary and for some models, shap is still returning a list
+    if is_classifier(estimator):
+        if isinstance(shap_matrix, list):
+            # For LightGBM classifier, RF, in sklearn API, SHAP returns a list of arrays
+            # https://github.com/slundberg/shap/issues/526
+            shap_imp = np.mean([np.abs(sv).mean(0) for sv in shap_matrix], axis=0)
+        else:
+            shap_imp = np.abs(shap_matrix).mean(0)
+    else:
+        shap_imp = np.abs(shap_matrix).mean(0)
     return shap_imp
 
 
 def _get_perm_imp(estimator, X, y, sample_weight, cat_feature=None):
     """Private function, Get the SHAP feature importance
 
     Parameters
@@ -1424,15 +1466,15 @@
         self,
         estimator=None,
         cutoff=4,
         iters=10,
         max_rounds=500,
         delta=0.1,
         silent=True,
-        importance="shap",
+        importance="fastshap",
     ):
         self.estimator = estimator
         self.cutoff = cutoff
         self.iters = iters
         self.max_rounds = max_rounds
         self.delta = delta
         self.silent = silent
@@ -1672,15 +1714,15 @@
         Stopping criteria for whether another round is started
     silent : bool
         Set to True if don't want to see the BoostARoota output printed.
         Will still show any errors or warnings that may occur
     weight : pd.series
         sample_weight, if any
     imp_kind : str
-        whether if native, shap or permutation importance should be used
+        whether if native, shap, fastshap or permutation importance should be used
     cat_feature : list of int or None
         the list of integers, cols loc, of the categorical predictors. Avoids to detect and encode
         each iteration if the exact same columns are passed to the selection methods.
 
     Returns
     -------
     criteria : bool
@@ -1697,15 +1739,15 @@
     ValueError
         error if the feature importance type is not
     """
     # Set up the parameters for running the model in XGBoost - split is on multi log loss
     for i in range(1, n_iterations + 1):
         # Create the shadow variables and run the model to obtain importances
         new_x, shadow_names = _create_shadow(X)
-        imp_func = {"shap": _get_shap_imp, "pimp": _get_perm_imp, "native": _get_imp}
+        imp_func = {"shap": _get_shap_imp, "fastshap": _get_shap_imp, "pimp": _get_perm_imp, "native": _get_imp}
         importance = imp_func[imp_kind](
             estimator, new_x, y, sample_weight=weight, cat_feature=cat_feature
         )
 
         # Create a dataframe to store the feature importances
         if i == 1:
             df = pd.DataFrame({"feature": new_x.columns})
@@ -1857,28 +1899,40 @@
     - Cross-validated feature importance to smooth out the noise, based on lightGBM only
       (which is, most of the time, the fastest and more accurate Boosting).
     - the feature importance is derived using SHAP importance
     - Taking the max of median of the shadow var. imp over folds otherwise not enough conservative and
       it improves the convergence (needs less evaluation to find a threshold)
     - Not based on a given percentage of cols needed to be deleted
     - Plot method for var. imp
+    
     Parameters
     ----------
     objective: str
         the lightGBM objective
     cutoff: float
         the value by which the max of shadow imp is divided, to compare to real importance
     n_folds: int, default=5
         the number of folds for the cross-val
     n_iter: int, default=5
         the number of times the cross-validation is repeated
     silent: bool, default=False
         print out details or not
     rf: bool, default=False
         the lightGBM implementation of the random forest
+    fastshap: bool, default=True
+        enable or not the fasttreeshap (LinkedIn) implementation of the shap values
+    lgbm_params: dict, Optional
+        the parameters to pass to the lightGBM algorithm (python API). Note that some of
+        those parameters will be overridden by the algorithm. Namely:
+        objective, verbose, is_balanced
+    n_jobs: int, default 0
+        0 means default number of threads in OpenMP
+        for the best speed, set this to the number of real CPU cores, not the number of threads
+    
+    
     Attributes
     ----------
     selected_features_: list of str
         the list of columns to keep
     ranking_ : array of shape [n_features]
         The feature ranking, such that ``ranking_[i]`` corresponds to the
         ranking position of the i-th feature. Selected (i.e., estimated
@@ -1900,26 +1954,29 @@
     >>>
     >>> feat_selector = arfsgroot.GrootCV(objective='rmse', cutoff = 1, n_folds=5, n_iter=5)
     >>> feat_selector.fit(X, y, sample_weight=None)
     >>> feat_selector.plot_importance(n_feat_per_inch=5)
     """
 
     def __init__(
-        self, objective=None, cutoff=1, n_folds=5, n_iter=5, silent=True, rf=False
+        self, objective=None, cutoff=1, n_folds=5, n_iter=5, silent=True, rf=False, fastshap=True, n_jobs=0, lgbm_params=None
     ):
         self.objective = objective
         self.cutoff = cutoff
         self.n_folds = n_folds
         self.n_iter = n_iter
         self.silent = silent
         self.rf = rf
+        self.fastshap = fastshap 
         self.cv_df = None
         self.sha_cutoff = None
         self.ranking_absolutes_ = None
         self.ranking_ = None
+        self.lgbm_params = lgbm_params
+        self.n_jobs=n_jobs
 
         # Throw errors if the inputted parameters don't meet the necessary criteria
         # Ensure parameters meet necessary criteria
         if cutoff <= 0 or n_iter <= 0 or n_folds <= 0:
             raise ValueError("cutoff, n_iter, and n_folds should be greater than 0.")
 
     def fit(self, X, y, sample_weight=None):
@@ -1958,14 +2015,17 @@
             objective=self.objective,
             cutoff=self.cutoff,
             n_folds=self.n_folds,
             n_iter=self.n_iter,
             silent=self.silent,
             weight=sample_weight,
             rf=self.rf,
+            fastshap=self.fastshap,
+            lgbm_params=self.lgbm_params,
+            n_jobs=self.n_jobs
         )
 
         self.selected_features_ = self.selected_features_.values
         self.support_ = np.asarray(
             [c in self.selected_features_ for c in self.feature_names_in_]
         )
         self.ranking_ = np.where(self.support_, 2, 1)
@@ -2063,53 +2123,64 @@
 #
 # GrootCV. In principle, you cannot/don't need to access those methods (reason of
 # the _ in front of the function name, they're internal functions)
 #
 ########################################################################################
 
 
-def _reduce_vars_lgb_cv(X, y, objective, n_folds, cutoff, n_iter, silent, weight, rf):
-    """Private function, reduce the number of predictors using a lightgbm (python API)
+def _reduce_vars_lgb_cv(X, y, objective, n_folds, cutoff, n_iter, silent, weight, rf, fastshap, lgbm_params=None, n_jobs=0):
+    """
+    Reduce the number of predictors using a lightgbm (python API)
+
     Parameters
     ----------
-    x : pd.DataFrame
-        the dataframe to create shadow features on
+    X : pd.DataFrame
+            the dataframe to create shadow features on
     y : pd.Series
-        the target
+            the target
     objective : str
-        the lightGBM objective
+            the lightGBM objective
     cutoff : float
-        the value by which the max of shadow imp is divided, to compare to real importance
+            the value by which the max of shadow imp is divided, to compare to real importance
     n_iter : int
-        The number of repetition of the cross-validation, smooth out the feature importance noise
+            The number of repetition of the cross-validation, smooth out the feature importance noise
     silent : bool
-        Set to True if don't want to see the BoostARoota output printed.
-        Will still show any errors or warnings that may occur
+            Set to True if don't want to see the BoostARoota output printed.
+            Will still show any errors or warnings that may occur
     weight : pd.series
-        sample_weight, if any
+            sample_weight, if any
     rf : bool, default=False
-        the lightGBM implementation of the random forest
-    returns
+            the lightGBM implementation of the random forest
+    fastshap : bool
+            enable or not the fasttreeshap implementation
+    lgbm_params : dict, optional
+            dictionary of lightgbm parameters
+    n_jobs: int, default 0
+        0 means default number of threads in OpenMP
+        for the best speed, set this to the number of real CPU cores, not the number of threads
+
+    Returns
     -------
-     real_vars['feature'] : pd.dataframe
-        feature importance of the real predictors over iter
-     df : pd.DataFrame
-        feature importance of the real+shadow predictors over iter
-     cutoff_shadow : float
-        the feature importance threshold, to reject or not the predictors
+    real_vars['feature'] : pd.dataframe
+            feature importance of the real predictors over iter
+    df : pd.DataFrame
+            feature importance of the real+shadow predictors over iter
+    cutoff_shadow : float
+            the feature importance threshold, to reject or not the predictors
     """
 
-    param = _set_lgb_parameters(X=X, y=y, objective=objective, rf=rf, silent=silent)
+    params = _set_lgb_parameters(X=X, y=y, objective=objective, rf=rf, silent=silent, n_jobs=n_jobs, lgbm_params=lgbm_params)
 
     dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
     category_cols = dtypes_dic["cat"] + dtypes_dic["time"] + dtypes_dic["unk"]
     cat_idx = [X.columns.get_loc(col) for col in category_cols]
 
     rkf = RepeatedKFold(n_splits=n_folds, n_repeats=n_iter, random_state=2652124)
     iter = 0
+    df = pd.DataFrame({"feature": X.columns})
     for tridx, validx in tqdm(
         rkf.split(X, y), total=rkf.get_n_splits(), desc="Repeated k-fold"
     ):
         X_train, X_val, y_train, y_val, weight_tr, weight_val = _split_data(
             X, y, tridx, validx, weight
         )
 
@@ -2122,20 +2193,19 @@
             y_train,
             weight_tr,
             new_x_val,
             y_val,
             weight_val,
             category_cols=category_cols,
             early_stopping_rounds=20,
-            **param,
+            fastshap=fastshap,
+            **params,
         )
 
-        importance = _compute_importance(new_x_tr, shap_matrix, param, objective)
-        if iter == 0:
-            df = pd.DataFrame({"feature": new_x_tr.columns})
+        importance = _compute_importance(new_x_tr, shap_matrix, params, objective, fastshap)
         df = _merge_importance_df(
             df=df,
             importance=importance,
             iter=iter,
             n_folds=n_folds,
             column_names=new_x_tr.columns,
             silent=silent,
@@ -2152,82 +2222,94 @@
     # Otherwise too conservative (reject too often)
     cutoff_shadow = shadow_vars.select_dtypes(include=[np.number]).max().mean() / cutoff
     real_vars = real_vars[(real_vars.Med.values >= cutoff_shadow)]
 
     return real_vars["feature"], df, cutoff_shadow
 
 
-def _set_lgb_parameters(X, y, objective, rf=False, silent=True):
+def _set_lgb_parameters(
+    X: np.ndarray, y: np.ndarray, objective: str, rf: bool, silent: bool, n_jobs: int = 0, lgbm_params: dict = None
+) -> dict:
     """Set parameters for a LightGBM model based on the input features and the objective.
 
     Parameters
     ----------
     X : numpy array or pandas DataFrame
         The feature matrix of the training data.
     y : numpy array or pandas Series
         The target variable of the training data.
     objective : str
         The objective function to optimize during training.
     rf : bool, default False
         Whether to use random forest boosting.
     silent : bool, default True
         Whether to print messages during parameter setting.
+    n_jobs: int, default 0
+        0 means default number of threads in OpenMP
+        for the best speed, set this to the number of real CPU cores, not the number of threads
 
     Returns
     -------
     dict
         The dictionary of LightGBM parameters.
 
     """
+
     n_feat = X.shape[1]
-    param = {"objective": objective}
-    param.update({"verbosity": -1})
+
+    params = lgbm_params if lgbm_params is not None else {}
+
+    params["objective"] = objective
+    params["verbosity"] = -1
     if objective == "softmax":
-        param["num_class"] = len(np.unique(y))
+        params["num_class"] = len(np.unique(y))
+
     if rf:
         feat_frac = (
             np.sqrt(n_feat) / n_feat
             if objective in ["softmax", "binary"]
             else n_feat / (3 * n_feat)
         )
-        param.update(
+        params.update(
             {
                 "boosting_type": "rf",
-                "bagging_fraction": "0.7",
+                "bagging_fraction": 0.7,
                 "feature_fraction": feat_frac,
-                "bagging_freq": "1",
+                "bagging_freq": 1,
             }
         )
-    clf_losses = [
-        "binary",
-        "softmax",
-        "multi_logloss",
-        "multiclassova",
-        "multiclass",
-        "multiclass_ova",
-        "ova",
-        "ovr",
-        "binary_logloss",
-    ]
+
+    clf_losses = [ "binary", "softmax", "multi_logloss", "multiclassova", "multiclass", "multiclass_ova", "ova", "ovr", "binary_logloss"]
     if objective in clf_losses:
         y = y.astype(int)
         y_freq_table = pd.Series(y.fillna(0)).value_counts(normalize=True)
         n_classes = y_freq_table.size
         if n_classes > 2 and objective != "softmax":
-            param["objective"] = "softmax"
-            param["num_class"] = len(np.unique(y))
+            params["objective"] = "softmax"
+            params["num_class"] = len(np.unique(y))
             if not silent:
                 print("Multi-class task, setting objective to softmax")
         main_class = y_freq_table[0]
         if not silent:
             print("GrootCV: classification with unbalance classes")
         if main_class > 0.8:
-            param.update({"is_unbalance": True})
-    param.update({"num_threads": 0})
-    return param
+            params.update({"is_unbalance": True})
+
+    params.update({"num_threads": n_jobs})
+    
+    # we are using early_stopping
+    # we prevent the overridding of it by popping the n_iterations
+    keys_to_pop = ['num_iterations', 'num_iteration', 'n_iter', 'num_tree', 'num_trees',
+                   'num_round', 'num_rounds', 'nrounds', 'num_boost_round', 'n_estimators', 'max_iter']
+    for key in keys_to_pop:
+        params.pop(key, None)
+    
+    return params
+
+
 
 
 def _split_data(X, y, tridx, validx, weight=None):
     """
     Split data into train and validation sets based on provided indices.
 
     Parameters
@@ -2272,14 +2354,15 @@
     y_train,
     weight_train,
     X_val,
     y_val,
     weight_val,
     category_cols=None,
     early_stopping_rounds=20,
+    fastshap=True,
     **params,
 ):
     """
     Train a LightGBM model with the given training data and hyperparameters and return the trained model and its SHAP values.
 
     Parameters
     ----------
@@ -2296,14 +2379,16 @@
     weight_val : array-like of shape (n_val_samples,)
         The sample weights for validation data.
     category_cols : array-like or None, optional (default=None)
         The indices of categorical columns. If None, no categorical columns will be considered.
     early_stopping_rounds : int, optional (default=20)
         Activates early stopping. Validation metric needs to improve at least once in every early_stopping_rounds
         round(s) to continue training._train_lgb_model
+    fastshap : bool
+        enable or not fasttreeshap implementation
     **params : dict
         Other parameters passed to the LightGBM model.
 
     Returns
     -------
     tuple of (Booster, numpy.ndarray, int)
         The trained LightGBM model, its SHAP values for X_train, and the best iteration reached during training.
@@ -2322,19 +2407,24 @@
         train_set=d_train,
         num_boost_round=10000,
         valid_sets=watchlist,
         categorical_feature=category_cols,
         callbacks=[early_stopping(early_stopping_rounds, False, False)],
     )
 
-    shap_matrix = bst.predict(X_train, pred_contrib=True)
+    if fastshap:
+        explainer = FastTreeExplainer(bst, algorithm="auto", shortcut=False, feature_perturbation="tree_path_dependent")
+        shap_matrix = explainer.shap_values(X_train)
+    else:
+        shap_matrix = bst.predict(X_train, pred_contrib=True)
+    
     return bst, shap_matrix, bst.best_iteration
 
 
-def _compute_importance(new_x_tr, shap_matrix, param, objective):
+def _compute_importance(new_x_tr, shap_matrix, param, objective, fastshap):
     """
     Compute feature importance scores using SHAP values.
 
     Parameters:
     -----------
     new_x_tr : numpy.ndarray
         The training dataset after being processed.
@@ -2346,24 +2436,29 @@
         The objective function of the LightGBM model.
 
     Returns:
     --------
     list
         A list of tuples containing feature names and their corresponding importance scores.
     """
-    if objective == "softmax":
-        n_feat = new_x_tr.shape[1]
-        shap_matrix = np.delete(
-            shap_matrix,
-            list(range(n_feat, (n_feat + 1) * param["num_class"], n_feat + 1)),
-            axis=1,
-        )
-        shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
+    if fastshap:
+        if objective == "softmax":
+            shap_matrix = np.abs(np.concatenate(shap_matrix, axis=1))
+        shap_imp = np.mean(np.abs(shap_matrix), axis=0)
     else:
-        shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
+        if objective == "softmax":
+            n_feat = new_x_tr.shape[1]
+            shap_matrix = np.delete(
+                shap_matrix,
+                list(range(n_feat, (n_feat + 1) * param["num_class"], n_feat + 1)),
+                axis=1,
+            )
+            shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
+        else:
+            shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
     importance = dict(zip(new_x_tr.columns, shap_imp))
     return sorted(importance.items(), key=operator.itemgetter(1))
 
 
 def _merge_importance_df(df, importance, iter, n_folds, column_names, silent=True):
     """
     Merge the feature importance dataframe `df` with the importance
```

### Comparing `arfs-1.1.4/src/arfs/feature_selection/base.py` & `arfs-2.0.0/src/arfs/feature_selection/base.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.4/src/arfs/feature_selection/mrmr.py` & `arfs-2.0.0/src/arfs/feature_selection/mrmr.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,18 +156,18 @@
         """
 
         if isinstance(X, pd.DataFrame):
             self.feature_names_in_ = X.columns.to_numpy()
         else:
             raise TypeError("X is not a pd.DataFrame")
 
-        if isinstance(y, pd.Series):
-            y.name = "target"
-        else:
-            raise TypeError("yis not a pd.Series")
+        if not isinstance(y, pd.Series):
+            y = pd.Series(y)
+            
+        y.name = "target"
 
         target = y.copy()
         if self.task == "classification":
             target = target.astype("category")
 
         self.relevance_args = {"X": X, "y": target, "sample_weight": sample_weight}
         self.redundancy_args = {"X": X, "sample_weight": sample_weight}
```

### Comparing `arfs-1.1.4/src/arfs/feature_selection/summary.py` & `arfs-2.0.0/src/arfs/feature_selection/summary.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.4/src/arfs/feature_selection/unsupervised.py` & `arfs-2.0.0/src/arfs/feature_selection/unsupervised.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,27 @@
 from ..preprocessing import OrdinalEncoderPandas
 
 
 # fix random seed for reproducibility
 np.random.seed(7)
 
 
-def _missing_ratio(X):
-    if not isinstance(X, pd.DataFrame):
-        raise TypeError("X should be a pandas DataFrame")
-    return X.isnull().sum() / X.shape[0]
+def _missing_ratio(df):
+    if not isinstance(df, pd.DataFrame):
+        raise TypeError("df should be a pandas DataFrame")
+    numeric_columns = df.select_dtypes(np.number).columns
+    n_samples = len(df)
+    
+    missing_counts = {}
+    for column in df.columns:
+        if column in numeric_columns:
+            missing_counts[column] = (df[column].isnull().sum() + np.isinf(df[column]).sum())/n_samples
+        else:
+            missing_counts[column] = df[column].isnull().sum()/n_samples
+    return pd.Series(missing_counts)
 
 
 class MissingValueThreshold(BaseThresholdSelector):
     """Feature selector that removes all high missing percentage features.
     This feature selection algorithm looks only at the features (X),
     not the desired outputs (y), and can thus be used for unsupervised learning.
```

### Comparing `arfs-1.1.4/src/arfs/feature_selection/variable_importance.py` & `arfs-2.0.0/src/arfs/feature_selection/variable_importance.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 
 # sklearn
 from sklearn.utils.validation import check_is_fitted
 from sklearn.base import BaseEstimator
 from sklearn.feature_selection._base import SelectorMixin
+from fasttreeshap import TreeExplainer as FastTreeExplainer
 
 # ARFS
 from ..utils import reset_plot
 from ..gbm import GradientBoosting
 from ..preprocessing import OrdinalEncoderPandas
 
 
@@ -75,14 +76,16 @@
         the pairs of collinear features and the association values
     support_ : list of bool
         the list of the selected X-columns
     selected_features_ : list of str
         the list of names of selected features
     not_selected_features_ : list of str
         the list of names of rejected features
+    fastshap : boolean
+        enable or not the fasttreeshap implementation
     verbose : int, default = -1
         controls the progress bar, > 1 print out progress
 
     Example
     -------
     >>> from sklearn.datasets import make_classification, make_regression
     >>> X, y = make_regression(n_samples = 1000, n_features = 50, n_informative = 5, shuffle=False) # , n_redundant = 5
@@ -98,23 +101,25 @@
         self,
         task="regression",
         encode=True,
         n_iterations=10,
         threshold=0.99,
         lgb_kwargs={"objective": "rmse", "zero_as_missing": False},
         encoder_kwargs=None,
+        fastshap=True,
         verbose=-1,
     ):
         self.task = task
         self.encode = encode
         self.n_iterations = n_iterations
         self.threshold = threshold
         self.lgb_kwargs = lgb_kwargs
         self.encoder_kwargs = encoder_kwargs
         self.verbose = verbose
+        self.fastshap = fastshap
 
         if (self.threshold > 1.0) or (self.threshold < 0.0):
             raise ValueError("``threshold`` should be larger than 0 and smaller than 1")
 
     def fit(self, X, y, sample_weight=None):
         """Learn variable importance from X and y, supervised learning.
 
@@ -146,14 +151,15 @@
             sample_weight=sample_weight,
             encode=self.encode,
             task=self.task,
             n_iterations=self.n_iterations,
             verbose=self.verbose,
             encoder_kwargs=self.encoder_kwargs,
             lgb_kwargs=self.lgb_kwargs,
+            fastshap=self.fastshap
         )
 
         self.feature_importances_summary_ = feature_importances
 
         support_ordered = (
             self.feature_importances_summary_["cumulative_importance"] >= self.threshold
         )
@@ -315,14 +321,15 @@
     X,
     y,
     sample_weight=None,
     encode=False,
     task="regression",
     n_iterations=10,
     verbose=-1,
+    fastshap=True,
     encoder_kwargs=None,
     lgb_kwargs={"objective": "rmse", "zero_as_missing": False},
 ):
     if task not in ["regression", "classification", "multiclass"]:
         raise ValueError('Task must be either "classification" or "regression"')
 
     if y is None:
@@ -360,34 +367,42 @@
         gbm_model.fit(X=X, y=y, sample_weight=sample_weight)
 
         # pimp cool but too slow
         # perm_imp =  permutation_importance(
         # model, valid_features, valid_labels, n_repeats=10, random_state=42, n_jobs=-1
         # )
         # perm_imp = perm_imp.importances_mean
-        shap_matrix = gbm_model.model.predict(
-            gbm_model.valid_features, pred_contrib=True
-        )
-        # the dim changed in lightGBM >= 3.0.0
-        if task == "multiclass":
-            # X_SHAP_values (array-like of shape = [n_samples, n_features + 1]
-            # or shape = [n_samples, (n_features + 1) * n_classes])
-            # index starts from 0
-            n_feat = gbm_model.valid_features.shape[1]
-            y_freq_table = pd.Series(y.fillna(0)).value_counts(normalize=True)
-            n_classes = y_freq_table.size
-            shap_matrix = np.delete(
-                shap_matrix,
-                list(range(n_feat, (n_feat + 1) * n_classes, n_feat + 1)),
-                axis=1,
-            )
-            shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
+        if fastshap:
+            explainer = FastTreeExplainer(gbm_model.model, algorithm="auto", shortcut=False, feature_perturbation="tree_path_dependent")
+            shap_matrix = explainer.shap_values(gbm_model.valid_features)
+            if isinstance(shap_matrix, list):
+                # For LightGBM classifier, RF, in sklearn API, SHAP returns a list of arrays
+                # https://github.com/slundberg/shap/issues/526
+                shap_imp = np.mean([np.abs(sv).mean(0) for sv in shap_matrix], axis=0)
+            else:
+                shap_imp = np.abs(shap_matrix).mean(0)
         else:
-            # for binary, only one class is returned, for regression a single column added as well
-            shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
+            shap_matrix = gbm_model.model.predict(gbm_model.valid_features, pred_contrib=True)
+            # the dim changed in lightGBM >= 3.0.0
+            if task == "multiclass":
+                # X_SHAP_values (array-like of shape = [n_samples, n_features + 1]
+                # or shape = [n_samples, (n_features + 1) * n_classes])
+                # index starts from 0
+                n_feat = gbm_model.valid_features.shape[1]
+                y_freq_table = pd.Series(y.fillna(0)).value_counts(normalize=True)
+                n_classes = y_freq_table.size
+                shap_matrix = np.delete(
+                    shap_matrix,
+                    list(range(n_feat, (n_feat + 1) * n_classes, n_feat + 1)),
+                    axis=1,
+                )
+                shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
+            else:
+                # for binary, only one class is returned, for regression a single column added as well
+                shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
 
         # Record the feature importances
         feature_importance_values += (
             shap_imp / n_iterations
         )  # model.feature_importances_ / n_iterations
     feature_importances = pd.DataFrame(
         {"feature": feature_names, "importance": feature_importance_values}
```

### Comparing `arfs-1.1.4/src/arfs/gbm.py` & `arfs-2.0.0/src/arfs/gbm.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.4/src/arfs/parallel.py` & `arfs-2.0.0/src/arfs/parallel.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.4/src/arfs/preprocessing.py` & `arfs-2.0.0/src/arfs/preprocessing.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,20 +16,30 @@
 # pandas
 import pandas as pd
 from pandas.api.types import IntervalDtype
 
 # numpy
 import numpy as np
 
+# regular expression
+import re
+
 # sklearn
 from sklearn.preprocessing import OrdinalEncoder
 from sklearn.base import BaseEstimator, TransformerMixin
 
+# patsy
+from patsy import dmatrix, EvalEnvironment, ModelDesc, INTERCEPT
+
+# typing
+from typing import Any, Callable, Union, List, Tuple, Optional, Dict
+
 # ARFS
 from .gbm import GradientBoosting
+from .utils import create_dtype_dict
 
 
 # fix random seed for reproducibility
 np.random.seed(7)
 
 __all__ = [
     "OrdinalEncoderPandas",
@@ -513,14 +523,20 @@
         Returns
         -------
         X :
             pd.DataFrame with the binned and grouped columns
         """
         X = X.copy()
         
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+            X.columns = [f"pred_{i}" for i in range(X.shape[1])]
+        
+        self.feature_names_in_ = X.columns.to_numpy()
+        
         if self.bin_features is None:
             self.bin_features = list(X.select_dtypes("number").columns)
             self.cat_features = []
         elif isinstance(self.bin_features, list):
             self.cat_features = list(
                 set(self.bin_features)
                 - set(list(X[self.bin_features].select_dtypes("number").columns))
@@ -736,7 +752,291 @@
     col_to_apply_style = tag_df.columns[1:]
     tag_df = (
         tag_df.style.apply(highlight_discarded, subset=col_to_apply_style)
         .applymap(lambda x: "" if x == x else "background-color: #ffa500")
         .format(precision=0)
     )
     return tag_df
+
+class IntervalToMidpoint(BaseEstimator, TransformerMixin):
+    """
+    IntervalToMidpoint is a transformer that converts numerical intervals in a pandas DataFrame to their midpoints.
+
+    Parameters
+    ----------
+    cols : list of str or str, default "all"
+        The column(s) to transform. If "all", all columns with numerical intervals will be transformed.
+
+    Attributes
+    ----------
+    cols : list of str or str
+        The column(s) to transform.
+    float_interval_cols_ : list of str
+        The columns with numerical interval data types in the input DataFrame.
+    columns_to_transform_ : list of str
+        The columns to be transformed based on the specified `cols` attribute.
+
+    Methods
+    -------
+    fit(X, y=None)
+        Fit the transformer on the input data.
+    transform(X)
+        Transform the input data by converting numerical intervals to midpoints.
+    inverse_transform(X)
+        Inverse transform is not implemented for this transformer.
+    """
+
+    def __init__(self, cols: Union[List[str], str]="all"):
+
+        self.cols = cols
+
+    def fit(self, X: pd.DataFrame = None, y: pd.Series = None):
+        """
+        Fit the transformer on the input data.
+
+        Parameters
+        ----------
+        X : 
+            The input data to fit the transformer on.
+        y : 
+            Ignored parameter.
+
+        Returns
+        -------
+        self : IntervalToMidpoint
+            The fitted transformer object.
+        """
+        data = X.copy()
+        
+        if self.cols == "all":
+            self.cols = data.columns
+        
+        self.float_interval_cols_ = create_dtype_dict(X, dic_keys="dtypes")["num_interval"]
+        self.columns_to_transform_ = list(set(self.cols).intersection(set(self.float_interval_cols_)))
+        return self
+
+    def transform(self, X: pd.DataFrame):
+        """
+        Transform the input data by converting numerical intervals to midpoints.
+
+        Parameters
+        ----------
+        X : pd.DataFrame
+            The input data to transform.
+
+        Returns
+        -------
+        X : pd.DataFrame
+            The transformed data with numerical intervals replaced by their midpoints.
+        """
+        X = X.copy()
+        for c in self.columns_to_transform_:
+            X.loc[:, c] = find_interval_midpoint(X[c])
+            X.loc[:, c] = X[c].astype(float)
+        return X
+
+    def inverse_transform(self, X: pd.DataFrame):
+        """
+        Inverse transform is not implemented for this transformer.
+
+        Parameters
+        ----------
+        X : pd.DataFrame
+            The input data to perform inverse transform on.
+
+        Raises
+        ------
+        NotImplementedError
+            Raised since inverse transform is not implemented for this transformer.
+        """
+        raise NotImplementedError(
+            "inverse_transform is not implemented for this transformer."
+        )
+        
+def transform_interval_to_midpoint(X: pd.DataFrame, cols: Union[List[str], str] = "all") -> pd.DataFrame:
+    """
+    Transforms interval columns in a pandas DataFrame to their midpoint values.
+    
+    Notes
+    -----
+    Equivalent function to ``IntervalToMidpoint`` without the estimator API
+
+    Parameters
+    ----------
+    X : pd.DataFrame
+        The input DataFrame containing the data to be transformed.
+    cols : list of str or str
+        The columns to be transformed. Defaults to "all" which transforms all columns.
+
+    Returns
+    -------
+    pd.DataFrame : 
+        The transformed DataFrame with interval columns replaced by their midpoint values.
+
+    Raises
+    ------
+    TypeError : 
+        If the input data is not a pandas DataFrame.
+    """
+    if cols == "all":
+        cols = X.columns
+    
+    X = X.copy()
+    float_interval_cols_ = create_dtype_dict(X, dic_keys="dtypes")["num_interval"]
+    columns_to_transform_ = list(set(cols).intersection(set(float_interval_cols_)))
+    for c in columns_to_transform_:
+        X.loc[:, c] = find_interval_midpoint(X[c])
+    return X
+
+
+def find_interval_midpoint(interval_series: pd.Series) -> np.ndarray:
+    """Find the midpoint (or left/right bound if the interval contains Inf).
+
+    Parameters
+    ----------
+    interval_series : pd.Series
+        series of pandas intervals.
+
+    Returns
+    -------
+    np.ndarray
+        Array of midpoints or bounds of the intervals.
+    """
+    left = interval_series.array.left
+    right = interval_series.array.right
+    mid = interval_series.array.mid
+    left_inf = np.isinf(left)
+    right_inf = np.isinf(right)
+
+    return np.where(left_inf & right_inf, np.inf,
+                        np.where(left_inf, right,
+                                 np.where(right_inf, left, mid)))
+    
+class PatsyTransformer(BaseEstimator, TransformerMixin):
+    """Transformer using patsy-formulas.
+
+    PatsyTransformer transforms a pandas DataFrame (or dict-like)
+    according to the formula and produces a numpy array.
+
+    Parameters
+    ----------
+    formula : string or formula-like
+        Pasty formula used to transform the data.
+
+    add_intercept : boolean, default=False
+        Wether to add an intersept. By default scikit-learn has built-in
+        intercepts for all models, so we don't add an intercept to the data,
+        even if one is specified in the formula.
+
+    eval_env : environment or int, default=0
+        Envirionment in which to evalute the formula.
+        Defaults to the scope in which PatsyModel was instantiated.
+
+    NA_action : string or NAAction, default="drop"
+        What to do with rows that contain missing values. You can ``"drop"``
+        them, ``"raise"`` an error, or for customization, pass an `NAAction`
+        object.  See ``patsy.NAAction`` for details on what values count as
+        'missing' (and how to alter this).
+
+    Attributes
+    ----------
+    feature_names_ : list of string
+        Column names / keys of training data.
+
+    return_type : string, default="dataframe"
+        data type that transform method will return. Default is ``"dataframe"``
+        for numpy array, but if you would like to get Pandas dataframe (for
+        example for using it in scikit transformers with dataframe as input
+        use ``"dataframe"`` and if numpy array use ``"ndarray"``
+
+    Note
+    ----
+    PastyTransformer does by default not add an intercept, even if you
+    specified it in the formula. You need to set add_intercept=True.
+
+    As scikit-learn transformers can not ouput y, the formula
+    should not contain a left hand side.  If you need to transform both
+    features and targets, use PatsyModel.
+    """
+    def __init__(self, formula=None, add_intercept=True, eval_env=0, NA_action="drop",
+                 return_type='dataframe'):
+        self.formula = formula
+        self.eval_env = eval_env
+        self.add_intercept = add_intercept
+        self.NA_action = NA_action
+        self.return_type = return_type
+
+    def fit(self, data, y=None):
+        """Fit the scikit-learn model using the formula.
+
+        Parameters
+        ----------
+        data : dict-like (pandas dataframe)
+            Input data. Column names need to match variables in formula.
+        """
+        self._fit_transform(data, y)
+        return self
+
+    def fit_transform(self, data, y=None):
+        """Fit the scikit-learn model using the formula and transform it.
+
+        Parameters
+        ----------
+        data : dict-like (pandas dataframe)
+            Input data. Column names need to match variables in formula.
+
+        Returns
+        -------
+        X_transform : ndarray
+            Transformed data
+        """
+        return self._fit_transform(data, y)
+
+    def _fit_transform(self, data, y=None):
+        
+        if not isinstance(data, pd.DataFrame):
+            data = pd.DataFrame(data)
+            data.columns = [f"pred_{i}" for i in range(data.shape[1])]
+        
+        if not isinstance(y, pd.Series):
+            y = pd.Series(y)
+            y.name = "target"
+            
+        target_name = y.name if y is not None else "y"
+        self.formula = self.formula or " + ".join(data.columns.difference([target_name]))
+        eval_env = EvalEnvironment.capture(self.eval_env, reference=2)
+        # self.formula = _drop_intercept(self.formula, self.add_intercept)
+
+        design = dmatrix(self.formula, data, NA_action=self.NA_action, return_type='dataframe', eval_env=eval_env)
+        self.design_ = design.design_info
+
+        if self.return_type == 'dataframe':
+            return design
+        else:
+            return np.array(design)
+
+    def transform(self, data):
+        """Transform with estimator using formula.
+
+        Transform the data using formula, then transform it
+        using the estimator.
+
+        Parameters
+        ----------
+        data : dict-like (pandas dataframe)
+            Input data. Column names need to match variables in formula.
+        """
+        if self.return_type == 'dataframe':
+            return dmatrix(self.design_, data, return_type='dataframe')
+        else:
+            return np.array(dmatrix(self.design_, data))
+
+
+def _drop_intercept(formula, add_intercept):
+    """Drop the intercept from formula if not add_intercept"""
+    if not add_intercept:
+        if not isinstance(formula, ModelDesc):
+            formula = ModelDesc.from_formula(formula)
+        if INTERCEPT in formula.rhs_termlist:
+            formula.rhs_termlist.remove(INTERCEPT)
+        return formula
+    return formula
```

### Comparing `arfs-1.1.4/src/arfs/sampling.py` & `arfs-2.0.0/src/arfs/sampling.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.4/src/arfs/utils.py` & `arfs-2.0.0/src/arfs/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 def create_dtype_dict(df: pd.DataFrame, dic_keys: str = "col_names") -> dict:
     """Create a custom dictionary of data type for adding suffixes
     to column names in the plotting utility for association matrix.
 
     Parameters
     ----------
-    df : pandas.DataFrame
+    df : pd.DataFrame
         The dataframe used for computing the association matrix.
     dic_keys : str
         Either "col_names" or "dtypes" for returning either a dictionary
         with column names or dtypes as keys.
 
     Returns
     -------
@@ -100,34 +100,37 @@
     ------
     ValueError
         If `dic_keys` is not either "col_names" or "dtypes".
     """
     if not isinstance(df, pd.DataFrame):
         raise TypeError("df should be a pandas DataFrame")
 
-    cat_cols = df.select_dtypes(include=["object", "category", "bool"]).columns
+    categorical_cols = df.select_dtypes(include=["object", "category", "bool"]).columns
     time_cols = df.select_dtypes(
         include=["datetime", "timedelta", "datetimetz"]
     ).columns
-    num_cols = df.select_dtypes(include=np.number).columns
+    numerical_interval_cols = df.select_dtypes(["Interval[float]", "Interval[int]"]).columns
+    numerical_cols = df.select_dtypes(include=np.number).columns
     remaining_cols = (
-        df.columns.difference(cat_cols).difference(num_cols).difference(time_cols)
+        df.columns.difference(categorical_cols).difference(numerical_cols).difference(time_cols).difference(numerical_interval_cols)
     )
 
     if dic_keys == "col_names":
-        cat_dict = dict.fromkeys(cat_cols, "cat")
-        num_dict = dict.fromkeys(num_cols, "num")
+        cat_dict = dict.fromkeys(categorical_cols, "cat")
+        num_dict = dict.fromkeys(numerical_cols, "num")
+        num_interval_dict = dict.fromkeys(numerical_interval_cols, "num_interval")
         time_dict = dict.fromkeys(time_cols, "time")
         remaining_dict = dict.fromkeys(remaining_cols, "unk")
-        return {**cat_dict, **num_dict, **time_dict, **remaining_dict}
+        return {**cat_dict, **num_dict, **num_interval_dict, **time_dict, **remaining_dict}
 
     if dic_keys == "dtypes":
         return {
-            "cat": cat_cols.tolist(),
-            "num": num_cols.tolist(),
+            "cat": categorical_cols.tolist(),
+            "num": numerical_cols.tolist(),
+            "num_interval": numerical_interval_cols.tolist(),
             "time": time_cols.tolist(),
             "unk": remaining_cols.tolist(),
         }
 
     raise ValueError("dic_keys should be either 'col_names' or 'dtypes'")
 
 
@@ -852,7 +855,9 @@
         "Gruber",
         "KeyserSoze",
         "Luthor",
         "Klaue",
         "Bane",
         "MarkZ",
     ]
+    
+    return X, y, w
```

### Comparing `arfs-1.1.4/src/arfs.egg-info/PKG-INFO` & `arfs-2.0.0/src/arfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 1.1.4
+Version: 2.0.0
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
@@ -28,28 +28,35 @@
 
 # All relevant feature selection
 
 All relevant feature selection means trying to find all features carrying information usable for prediction, rather than finding a possibly compact subset of features on which some particular model has a minimal error. This might include redundant predictors. All relevant feature selection is model agnostic in the sense that it doesn't optimize a scoring function for a *specific* model but rather tries to select all the predictors which are related to the response. 
 
 This package implements 3 different methods (Leshy is an evolution of Boruta, BoostAGroota is an evolution of BoostARoota and GrootCV is a new one). They are sklearn compatible. See hereunder for details about those methods. You can use any sklearn compatible estimator with Leshy and BoostAGroota but I recommend lightGBM. It's fast, accurate and has SHAP values builtin. It also provides a module for performing preprocessing and perform basic feature selection (autobinning, remove columns with too many missing values, zero variance, high-cardinality, highly correlated, etc.). Examples and detailled methods hereunder.
 
-Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method.
+Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for intrucing non-linearities into linear models and perform feature selection.
+
+Please note that one limitation of the lasso is that it treats the levels of a categorical predictor individually. However, this issue can be addressed by utilizing the `TreeDiscretizer`, which automatically bins numerical variables and groups the levels of categorical variables.
 
 ## Installation
 
 `$ pip install arfs`, requires python <3.10
 
 ## Example
 
 Working examples for:
 
  - [Preprocessing](./docs/notebooks/preprocessingipynb)
  - [Basic FS (best before ARFS)](./docs/notebooks/basic_feature_selection.ipynb)
  - [Regression](./docs/notebooks/arfs_regression.ipynb)
  - [Classification](./docs/notebooks/arfs_classification.ipynb)
+ - [LASSO and (G)LM feature selection](./docs/notebooks/lasso_feature_selection.ipynb)
+ - [Passing custom params](./docs/notebooks/arfs_grootcv_custom_params.ipynb)
+ - [Non-normal loss and sample weights](./docs/notebooks/arfs_non_normal_loss_and_sample_weight.ipynb)
+ - [ARFS on GPU](./docs/notebooks/arfs_on_GPU.ipynb)
+ - [Fast Shap](./docs/notebooks/arfs_shap_vs_fastshap.ipynb)
  - [Categoricals](./docs/notebooks/issue_categoricals.ipynb)
  - [Collinearity](./docs/notebooks/issue_collinearity.ipynb)
  - [Reducing run time for large data](./docs/notebooks/arfs_large_data_sampling.ipynb)
  - [Comparison to Boruta and BorutaShap](./docs/notebooks/arfs_boruta_borutaShap_comparison.ipynb)
  - [MRmr alternative](./docs/notebooks/mrmr_feature_selection.ipynb)
  - [MRmr vs ARFS](./docs/notebooks/mrmr_fs_VS_arfs.ipynb)
```

### Comparing `arfs-1.1.4/src/arfs.egg-info/SOURCES.txt` & `arfs-2.0.0/src/arfs.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -17,13 +17,14 @@
 src/arfs.egg-info/requires.txt
 src/arfs.egg-info/top_level.txt
 src/arfs/dataset/data/boston_bunch.joblib
 src/arfs/dataset/data/housing.zip
 src/arfs/feature_selection/__init__.py
 src/arfs/feature_selection/allrelevant.py
 src/arfs/feature_selection/base.py
+src/arfs/feature_selection/lasso.py
 src/arfs/feature_selection/mrmr.py
 src/arfs/feature_selection/summary.py
 src/arfs/feature_selection/unsupervised.py
 src/arfs/feature_selection/variable_importance.py
 tests/test_allrelevant.py
 tests/test_featselect.py
```

### Comparing `arfs-1.1.4/tests/test_allrelevant.py` & `arfs-2.0.0/tests/test_allrelevant.py`

 * *Files identical despite different names*

### Comparing `arfs-1.1.4/tests/test_featselect.py` & `arfs-2.0.0/tests/test_featselect.py`

 * *Files identical despite different names*

