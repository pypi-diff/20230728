# Comparing `tmp/arfs-2.0.0.tar.gz` & `tmp/arfs-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arfs-2.0.0.tar", last modified: Fri Jul 28 10:36:17 2023, max compression
+gzip compressed data, was "arfs-2.0.1.tar", last modified: Fri Jul 28 14:34:02 2023, max compression
```

## Comparing `arfs-2.0.0.tar` & `arfs-2.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.816036 arfs-2.0.0/
--rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-2.0.0/LICENSE.md
--rw-rw-rw-   0        0        0    11965 2023-07-28 10:36:17.819028 arfs-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    11275 2023-07-28 10:30:07.000000 arfs-2.0.0/README.md
--rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1433 2023-07-28 10:36:17.831029 arfs-2.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.380027 arfs-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.531030 arfs-2.0.0/src/arfs/
--rw-rw-rw-   0        0        0       92 2023-07-28 09:19:12.000000 arfs-2.0.0/src/arfs/__init__.py
--rw-rw-rw-   0        0        0    86458 2023-07-27 13:54:59.000000 arfs-2.0.0/src/arfs/association.py
--rw-rw-rw-   0        0        0     6689 2023-07-24 20:31:43.000000 arfs-2.0.0/src/arfs/benchmark.py
-drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.382040 arfs-2.0.0/src/arfs/dataset/
-drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.624028 arfs-2.0.0/src/arfs/dataset/data/
--rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-2.0.0/src/arfs/dataset/data/boston_bunch.joblib
--rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-2.0.0/src/arfs/dataset/data/housing.zip
-drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.758029 arfs-2.0.0/src/arfs/feature_selection/
--rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-2.0.0/src/arfs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0    94894 2023-07-28 09:23:30.000000 arfs-2.0.0/src/arfs/feature_selection/allrelevant.py
--rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-2.0.0/src/arfs/feature_selection/base.py
--rw-rw-rw-   0        0        0    19893 2023-07-26 16:20:34.000000 arfs-2.0.0/src/arfs/feature_selection/lasso.py
--rw-rw-rw-   0        0        0    13397 2023-07-27 13:39:47.000000 arfs-2.0.0/src/arfs/feature_selection/mrmr.py
--rw-rw-rw-   0        0        0     2457 2023-05-21 19:11:19.000000 arfs-2.0.0/src/arfs/feature_selection/summary.py
--rw-rw-rw-   0        0        0    15832 2023-07-26 16:49:41.000000 arfs-2.0.0/src/arfs/feature_selection/unsupervised.py
--rw-rw-rw-   0        0        0    15689 2023-07-24 19:47:35.000000 arfs-2.0.0/src/arfs/feature_selection/variable_importance.py
--rw-rw-rw-   0        0        0    21927 2023-06-16 08:19:41.000000 arfs-2.0.0/src/arfs/gbm.py
--rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-2.0.0/src/arfs/parallel.py
--rw-rw-rw-   0        0        0    40462 2023-07-27 07:24:21.000000 arfs-2.0.0/src/arfs/preprocessing.py
--rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-2.0.0/src/arfs/sampling.py
--rw-rw-rw-   0        0        0    25248 2023-07-26 08:46:59.000000 arfs-2.0.0/src/arfs/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.602028 arfs-2.0.0/src/arfs.egg-info/
--rw-rw-rw-   0        0        0    11965 2023-07-28 10:36:17.000000 arfs-2.0.0/src/arfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2023-07-28 10:36:17.000000 arfs-2.0.0/src/arfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 10:36:17.000000 arfs-2.0.0/src/arfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-2.0.0/src/arfs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      405 2023-07-28 10:36:17.000000 arfs-2.0.0/src/arfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-28 10:36:17.000000 arfs-2.0.0/src/arfs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-28 10:36:17.796031 arfs-2.0.0/tests/
--rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-2.0.0/tests/test_allrelevant.py
--rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-2.0.0/tests/test_featselect.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:34:02.274474 arfs-2.0.1/
+-rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-2.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0    11965 2023-07-28 14:34:02.275476 arfs-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11275 2023-07-28 10:30:07.000000 arfs-2.0.1/README.md
+-rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1377 2023-07-28 14:34:02.285475 arfs-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 14:34:01.724457 arfs-2.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-28 14:34:01.879464 arfs-2.0.1/src/arfs/
+-rw-rw-rw-   0        0        0       92 2023-07-28 13:13:55.000000 arfs-2.0.1/src/arfs/__init__.py
+-rw-rw-rw-   0        0        0    86758 2023-07-28 13:17:02.000000 arfs-2.0.1/src/arfs/association.py
+-rw-rw-rw-   0        0        0     6689 2023-07-24 20:31:43.000000 arfs-2.0.1/src/arfs/benchmark.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:34:01.726458 arfs-2.0.1/src/arfs/dataset/
+drwxrwxrwx   0        0        0        0 2023-07-28 14:34:01.994466 arfs-2.0.1/src/arfs/dataset/data/
+-rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-2.0.1/src/arfs/dataset/data/boston_bunch.joblib
+-rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-2.0.1/src/arfs/dataset/data/housing.zip
+drwxrwxrwx   0        0        0        0 2023-07-28 14:34:02.224473 arfs-2.0.1/src/arfs/feature_selection/
+-rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-2.0.1/src/arfs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0    95567 2023-07-28 14:32:16.000000 arfs-2.0.1/src/arfs/feature_selection/allrelevant.py
+-rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-2.0.1/src/arfs/feature_selection/base.py
+-rw-rw-rw-   0        0        0    19893 2023-07-26 16:20:34.000000 arfs-2.0.1/src/arfs/feature_selection/lasso.py
+-rw-rw-rw-   0        0        0    13397 2023-07-27 13:39:47.000000 arfs-2.0.1/src/arfs/feature_selection/mrmr.py
+-rw-rw-rw-   0        0        0     2457 2023-05-21 19:11:19.000000 arfs-2.0.1/src/arfs/feature_selection/summary.py
+-rw-rw-rw-   0        0        0    15832 2023-07-26 16:49:41.000000 arfs-2.0.1/src/arfs/feature_selection/unsupervised.py
+-rw-rw-rw-   0        0        0    15689 2023-07-24 19:47:35.000000 arfs-2.0.1/src/arfs/feature_selection/variable_importance.py
+-rw-rw-rw-   0        0        0    21927 2023-06-16 08:19:41.000000 arfs-2.0.1/src/arfs/gbm.py
+-rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-2.0.1/src/arfs/parallel.py
+-rw-rw-rw-   0        0        0    40462 2023-07-27 07:24:21.000000 arfs-2.0.1/src/arfs/preprocessing.py
+-rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-2.0.1/src/arfs/sampling.py
+-rw-rw-rw-   0        0        0    25248 2023-07-26 08:46:59.000000 arfs-2.0.1/src/arfs/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:34:01.962468 arfs-2.0.1/src/arfs.egg-info/
+-rw-rw-rw-   0        0        0    11965 2023-07-28 14:34:01.000000 arfs-2.0.1/src/arfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2023-07-28 14:34:01.000000 arfs-2.0.1/src/arfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 14:34:01.000000 arfs-2.0.1/src/arfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-2.0.1/src/arfs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      355 2023-07-28 14:34:01.000000 arfs-2.0.1/src/arfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-28 14:34:01.000000 arfs-2.0.1/src/arfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 14:34:02.257474 arfs-2.0.1/tests/
+-rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-2.0.1/tests/test_allrelevant.py
+-rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-2.0.1/tests/test_featselect.py
```

### Comparing `arfs-2.0.0/LICENSE.md` & `arfs-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/PKG-INFO` & `arfs-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 2.0.0
+Version: 2.0.1
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-2.0.0/README.md` & `arfs-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/setup.cfg` & `arfs-2.0.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -41,50 +41,47 @@
 00000280: 696f 6e73 5d0d 0a7a 6970 5f73 6166 6520  ions]..zip_safe 
 00000290: 3d20 4661 6c73 650d 0a70 6163 6b61 6765  = False..package
 000002a0: 5f64 6972 203d 200d 0a09 3d73 7263 0d0a  _dir = ...=src..
 000002b0: 7061 636b 6167 6573 203d 2066 696e 645f  packages = find_
 000002c0: 6e61 6d65 7370 6163 653a 0d0a 7079 7468  namespace:..pyth
 000002d0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
 000002e0: 332e 390d 0a69 6e73 7461 6c6c 5f72 6571  3.9..install_req
-000002f0: 7569 7265 7320 3d20 0d0a 0968 6f6c 6f76  uires = ...holov
-00000300: 6965 7773 3e3d 312e 3134 2e38 0d0a 096c  iews>=1.14.8...l
-00000310: 6967 6874 6762 6d3e 3d33 2e33 2e32 0d0a  ightgbm>=3.3.2..
-00000320: 096d 6174 706c 6f74 6c69 623e 3d33 2e35  .matplotlib>=3.5
-00000330: 0d0a 096e 756d 7079 3e3d 312e 3231 0d0a  ...numpy>=1.21..
-00000340: 0970 616e 6461 733e 3d31 2e34 0d0a 0970  .pandas>=1.4...p
-00000350: 616e 656c 3e3d 302e 3133 0d0a 0973 6369  anel>=0.13...sci
-00000360: 6b69 745f 6c65 6172 6e3e 3d31 2e30 0d0a  kit_learn>=1.0..
-00000370: 0973 6369 7079 3e3d 312e 382e 300d 0a09  .scipy>=1.8.0...
-00000380: 7365 6162 6f72 6e3e 3d30 2e31 312e 320d  seaborn>=0.11.2.
-00000390: 0a09 7368 6170 3e3d 302e 3430 2e30 0d0a  ..shap>=0.40.0..
-000003a0: 0974 7164 6d3e 3d34 2e36 322e 330d 0a09  .tqdm>=4.62.3...
-000003b0: 6661 7374 7472 6565 7368 6170 3e3d 302e  fasttreeshap>=0.
-000003c0: 312e 360d 0a09 7374 6174 736d 6f64 656c  1.6...statsmodel
-000003d0: 733e 3d30 2e31 342e 300d 0a0d 0a5b 6f70  s>=0.14.0....[op
-000003e0: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-000003f0: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-00000400: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  c....[options.pa
-00000410: 636b 6167 655f 6461 7461 5d0d 0a61 7266  ckage_data]..arf
-00000420: 732e 6461 7461 7365 742e 6461 7461 203d  s.dataset.data =
-00000430: 200d 0a09 2a2e 6a6f 626c 6962 0d0a 092a   ...*.joblib...*
-00000440: 2e7a 6970 0d0a 6172 6673 2e64 6174 6173  .zip..arfs.datas
-00000450: 6574 2e64 6573 6372 6970 7469 6f6e 203d  et.description =
-00000460: 200d 0a09 2a2e 7273 740d 0a0d 0a5b 6f70   ...*.rst....[op
-00000470: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
-00000480: 7569 7265 5d0d 0a64 6f63 7320 3d20 0d0a  uire]..docs = ..
-00000490: 096e 6273 7068 696e 783e 3d30 2e38 2e38  .nbsphinx>=0.8.8
-000004a0: 0d0a 0969 7079 6b65 726e 656c 3e3d 362e  ...ipykernel>=6.
-000004b0: 392e 310d 0a09 6970 7974 686f 6e5f 6765  9.1...ipython_ge
-000004c0: 6e75 7469 6c73 0d0a 0970 616e 646f 630d  nutils...pandoc.
-000004d0: 0a09 7370 6869 6e78 3e3d 342e 342e 300d  ..sphinx>=4.4.0.
-000004e0: 0a09 7370 6869 6e78 2d61 7574 6f64 6f63  ..sphinx-autodoc
-000004f0: 2d74 7970 6568 696e 7473 3e3d 312e 3136  -typehints>=1.16
-00000500: 2e30 0d0a 0973 7068 696e 782d 636f 7079  .0...sphinx-copy
-00000510: 6275 7474 6f6e 3e3d 302e 352e 300d 0a09  button>=0.5.0...
-00000520: 7370 6869 6e78 2d72 7464 2d74 6865 6d65  sphinx-rtd-theme
-00000530: 3e3d 312e 302e 300d 0a09 7370 6869 6e78  >=1.0.0...sphinx
-00000540: 2d74 6162 733e 3d33 2e32 2e30 0d0a 7465  -tabs>=3.2.0..te
-00000550: 7374 203d 200d 0a09 7079 7465 7374 0d0a  st = ...pytest..
-00000560: 0970 7974 6573 742d 636f 760d 0a0d 0a5b  .pytest-cov....[
-00000570: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000580: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000590: 6520 3d20 300d 0a0d 0a                   e = 0....
+000002f0: 7569 7265 7320 3d20 0d0a 096c 6967 6874  uires = ...light
+00000300: 6762 6d3e 3d33 2e33 2e32 0d0a 096d 6174  gbm>=3.3.2...mat
+00000310: 706c 6f74 6c69 623e 3d33 2e35 0d0a 096e  plotlib>=3.5...n
+00000320: 756d 7079 3e3d 312e 3231 0d0a 0970 616e  umpy>=1.21...pan
+00000330: 6461 733e 3d31 2e34 0d0a 0973 6369 6b69  das>=1.4...sciki
+00000340: 745f 6c65 6172 6e3e 3d31 2e30 0d0a 0973  t_learn>=1.0...s
+00000350: 6369 7079 3e3d 312e 382e 300d 0a09 7365  cipy>=1.8.0...se
+00000360: 6162 6f72 6e3e 3d30 2e31 312e 320d 0a09  aborn>=0.11.2...
+00000370: 7368 6170 3e3d 302e 3430 2e30 0d0a 0974  shap>=0.40.0...t
+00000380: 7164 6d3e 3d34 2e36 322e 330d 0a09 7374  qdm>=4.62.3...st
+00000390: 6174 736d 6f64 656c 733e 3d30 2e31 342e  atsmodels>=0.14.
+000003a0: 300d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  0....[options.pa
+000003b0: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
+000003c0: 6572 6520 3d20 7372 630d 0a0d 0a5b 6f70  ere = src....[op
+000003d0: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
+000003e0: 7461 5d0d 0a61 7266 732e 6461 7461 7365  ta]..arfs.datase
+000003f0: 742e 6461 7461 203d 200d 0a09 2a2e 6a6f  t.data = ...*.jo
+00000400: 626c 6962 0d0a 092a 2e7a 6970 0d0a 6172  blib...*.zip..ar
+00000410: 6673 2e64 6174 6173 6574 2e64 6573 6372  fs.dataset.descr
+00000420: 6970 7469 6f6e 203d 200d 0a09 2a2e 7273  iption = ...*.rs
+00000430: 740d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  t....[options.ex
+00000440: 7472 6173 5f72 6571 7569 7265 5d0d 0a64  tras_require]..d
+00000450: 6f63 7320 3d20 0d0a 096e 6273 7068 696e  ocs = ...nbsphin
+00000460: 783e 3d30 2e38 2e38 0d0a 0969 7079 6b65  x>=0.8.8...ipyke
+00000470: 726e 656c 3e3d 362e 392e 310d 0a09 6970  rnel>=6.9.1...ip
+00000480: 7974 686f 6e5f 6765 6e75 7469 6c73 0d0a  ython_genutils..
+00000490: 0970 616e 646f 630d 0a09 7370 6869 6e78  .pandoc...sphinx
+000004a0: 3e3d 342e 342e 300d 0a09 7370 6869 6e78  >=4.4.0...sphinx
+000004b0: 2d61 7574 6f64 6f63 2d74 7970 6568 696e  -autodoc-typehin
+000004c0: 7473 3e3d 312e 3136 2e30 0d0a 0973 7068  ts>=1.16.0...sph
+000004d0: 696e 782d 636f 7079 6275 7474 6f6e 3e3d  inx-copybutton>=
+000004e0: 302e 352e 300d 0a09 7370 6869 6e78 2d72  0.5.0...sphinx-r
+000004f0: 7464 2d74 6865 6d65 3e3d 312e 302e 300d  td-theme>=1.0.0.
+00000500: 0a09 7370 6869 6e78 2d74 6162 733e 3d33  ..sphinx-tabs>=3
+00000510: 2e32 2e30 0d0a 7465 7374 203d 200d 0a09  .2.0..test = ...
+00000520: 7079 7465 7374 0d0a 0970 7974 6573 742d  pytest...pytest-
+00000530: 636f 760d 0a0d 0a5b 6567 675f 696e 666f  cov....[egg_info
+00000540: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000550: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000560: 0a                                       .
```

### Comparing `arfs-2.0.0/src/arfs/association.py` & `arfs-2.0.1/src/arfs/association.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 import numpy as np
 import gc
 import pandas as pd
 import scipy.stats as ss
 import matplotlib.pyplot as plt
 import scipy.cluster.hierarchy as sch
 import scipy.stats as ss
-import holoviews as hv
-import panel as pn
+
 
 
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from sklearn.utils import as_float_array, safe_sqr, safe_mask
 from multiprocessing import cpu_count
 from itertools import combinations, permutations, product
 from pandas.api.types import is_numeric_dtype
@@ -2399,14 +2398,23 @@
         whether or not to cluster the square matrix, by default True
 
     Returns
     -------
     panel.Column
         the panel object
     """
+    try:
+        import holoviews as hv
+    except ImportError:
+        raise ImportError("Holoviews is not installed. Please install it using 'pip install holoviews'.")
+    
+    try:
+        import panel as pn
+    except ImportError:
+        raise ImportError("Panel is not installed. Please install it using 'pip install panel'.")
 
     cmap = cmap if cmap is not None else "coolwarm"
 
     # rename the columns for keeping track of num vs cat columns
     if suffix_dic is not None:
         rename_dic = {c: f"{c}_{suffix_dic[c]}" for c in assoc_mat.columns}
         assoc_mat = assoc_mat.rename(columns=rename_dic)
```

### Comparing `arfs-2.0.0/src/arfs/benchmark.py` & `arfs-2.0.1/src/arfs/benchmark.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/src/arfs/dataset/data/boston_bunch.joblib` & `arfs-2.0.1/src/arfs/dataset/data/boston_bunch.joblib`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/src/arfs/dataset/data/housing.zip` & `arfs-2.0.1/src/arfs/dataset/data/housing.zip`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/src/arfs/feature_selection/__init__.py` & `arfs-2.0.1/src/arfs/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/src/arfs/feature_selection/allrelevant.py` & `arfs-2.0.1/src/arfs/feature_selection/allrelevant.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 from sklearn.utils.validation import check_is_fitted
 from sklearn.feature_selection._base import SelectorMixin
 from sklearn.model_selection import RepeatedKFold, train_test_split
 from sklearn.inspection import permutation_importance
 from sklearn.utils.validation import _check_sample_weight
 from matplotlib.lines import Line2D
 from lightgbm import early_stopping
-from fasttreeshap import TreeExplainer as FastTreeExplainer
+
 
 from ..utils import (
     check_if_tree_based,
     is_lightgbm,
     is_catboost,
     create_dtype_dict,
     get_pandas_cat_codes,
@@ -262,15 +262,15 @@
 
     def __init__(
         self,
         estimator,
         n_estimators=1000,
         perc=90,
         alpha=0.05,
-        importance="fastshap",
+        importance="shap",
         two_step=True,
         max_iter=100,
         random_state=None,
         verbose=0,
         keep_weak=False,
     ):
         self.estimator = estimator
@@ -310,14 +310,20 @@
 
         Returns
         -------
         self : object
             Nothing but attributes
 
         """
+        try:
+            from fasttreeshap import TreeExplainer as FastTreeExplainer
+        except ImportError:
+            warnings.warn("fasttreeshap is not installed. Fallback to shap.")
+            self.importance = "shap"
+        
         if isinstance(X, pd.DataFrame):
             self.feature_names_in_ = X.columns.to_numpy()
         else:
             raise TypeError("X is not a dataframe")
 
         self.imp_real_hist = np.empty((0, X.shape[1]), float)
         self._fit(X, y, sample_weight=sample_weight)
@@ -1466,15 +1472,15 @@
         self,
         estimator=None,
         cutoff=4,
         iters=10,
         max_rounds=500,
         delta=0.1,
         silent=True,
-        importance="fastshap",
+        importance="shap",
     ):
         self.estimator = estimator
         self.cutoff = cutoff
         self.iters = iters
         self.max_rounds = max_rounds
         self.delta = delta
         self.silent = silent
@@ -1536,14 +1542,20 @@
         X : pd.DataFrame
             the predictors matrix
         y : pd.Series
             the target
         sample_weight : pd.series
             sample_weight, if any
         """
+        try:
+            from fasttreeshap import TreeExplainer as FastTreeExplainer
+        except ImportError:
+            warnings.warn("fasttreeshap is not installed. Fallback to shap.")
+            self.importance = "shap"
+            
         if isinstance(X, pd.DataFrame):
             self.feature_names_in_ = X.columns.to_numpy()
         else:
             raise TypeError("X is not a dataframe")
 
         if sample_weight is not None:
             sample_weight = pd.Series(_check_sample_weight(sample_weight, X))
@@ -1954,15 +1966,15 @@
     >>>
     >>> feat_selector = arfsgroot.GrootCV(objective='rmse', cutoff = 1, n_folds=5, n_iter=5)
     >>> feat_selector.fit(X, y, sample_weight=None)
     >>> feat_selector.plot_importance(n_feat_per_inch=5)
     """
 
     def __init__(
-        self, objective=None, cutoff=1, n_folds=5, n_iter=5, silent=True, rf=False, fastshap=True, n_jobs=0, lgbm_params=None
+        self, objective=None, cutoff=1, n_folds=5, n_iter=5, silent=True, rf=False, fastshap=False, n_jobs=0, lgbm_params=None
     ):
         self.objective = objective
         self.cutoff = cutoff
         self.n_folds = n_folds
         self.n_iter = n_iter
         self.silent = silent
         self.rf = rf
@@ -2408,14 +2420,19 @@
         num_boost_round=10000,
         valid_sets=watchlist,
         categorical_feature=category_cols,
         callbacks=[early_stopping(early_stopping_rounds, False, False)],
     )
 
     if fastshap:
+        try:
+            from fasttreeshap import TreeExplainer as FastTreeExplainer
+        except ImportError:
+            raise ImportError("fasttreeshap is not installed. Please install it using 'pip/conda install fasttreeshap'.")
+        
         explainer = FastTreeExplainer(bst, algorithm="auto", shortcut=False, feature_perturbation="tree_path_dependent")
         shap_matrix = explainer.shap_values(X_train)
     else:
         shap_matrix = bst.predict(X_train, pred_contrib=True)
     
     return bst, shap_matrix, bst.best_iteration
```

### Comparing `arfs-2.0.0/src/arfs/feature_selection/base.py` & `arfs-2.0.1/src/arfs/feature_selection/base.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/src/arfs/feature_selection/lasso.py` & `arfs-2.0.1/src/arfs/feature_selection/lasso.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/src/arfs/feature_selection/mrmr.py` & `arfs-2.0.1/src/arfs/feature_selection/mrmr.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/src/arfs/feature_selection/summary.py` & `arfs-2.0.1/src/arfs/feature_selection/summary.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/src/arfs/feature_selection/unsupervised.py` & `arfs-2.0.1/src/arfs/feature_selection/unsupervised.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/src/arfs/feature_selection/variable_importance.py` & `arfs-2.0.1/src/arfs/feature_selection/variable_importance.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/src/arfs/gbm.py` & `arfs-2.0.1/src/arfs/gbm.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/src/arfs/parallel.py` & `arfs-2.0.1/src/arfs/parallel.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/src/arfs/preprocessing.py` & `arfs-2.0.1/src/arfs/preprocessing.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/src/arfs/sampling.py` & `arfs-2.0.1/src/arfs/sampling.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/src/arfs/utils.py` & `arfs-2.0.1/src/arfs/utils.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/src/arfs.egg-info/PKG-INFO` & `arfs-2.0.1/src/arfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 2.0.0
+Version: 2.0.1
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-2.0.0/src/arfs.egg-info/SOURCES.txt` & `arfs-2.0.1/src/arfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/tests/test_allrelevant.py` & `arfs-2.0.1/tests/test_allrelevant.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.0/tests/test_featselect.py` & `arfs-2.0.1/tests/test_featselect.py`

 * *Files identical despite different names*

