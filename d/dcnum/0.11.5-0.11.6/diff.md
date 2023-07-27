# Comparing `tmp/dcnum-0.11.5.tar.gz` & `tmp/dcnum-0.11.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.11.5.tar", last modified: Thu Jul 27 12:54:01 2023, max compression
+gzip compressed data, was "dcnum-0.11.6.tar", last modified: Thu Jul 27 21:59:23 2023, max compression
```

## Comparing `dcnum-0.11.5.tar` & `dcnum-0.11.6.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.586604 dcnum-0.11.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.578607 dcnum-0.11.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-27 12:53:52.000000 dcnum-0.11.5/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-27 12:53:52.000000 dcnum-0.11.5/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-27 12:53:52.000000 dcnum-0.11.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-27 12:53:52.000000 dcnum-0.11.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-27 12:53:52.000000 dcnum-0.11.5/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 12:53:52.000000 dcnum-0.11.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-27 12:54:01.586604 dcnum-0.11.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-27 12:53:52.000000 dcnum-0.11.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-27 12:54:01.000000 dcnum-0.11.5/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/event_extractor_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/feat/feat_background/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_background/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/feat/feat_brightness/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_brightness/bright_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_brightness/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/feat/feat_moments/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_moments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_moments/ct_opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_moments/mt_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/feat/feat_texture/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_texture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_texture/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_texture/tex_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/queue_event_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/read/hdf5_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/segm/segmenter_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/segm/segmenter_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/segm/segmenter_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.586604 dcnum-0.11.5/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/write/deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/write/queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/write/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-27 12:54:01.000000 dcnum-0.11.5/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-27 12:54:01.000000 dcnum-0.11.5/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:54:01.000000 dcnum-0.11.5/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-27 12:54:01.000000 dcnum-0.11.5/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 12:54:01.000000 dcnum-0.11.5/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.586604 dcnum-0.11.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-27 12:53:52.000000 dcnum-0.11.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.586604 dcnum-0.11.5/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-27 12:53:52.000000 dcnum-0.11.5/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-27 12:53:52.000000 dcnum-0.11.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 12:53:52.000000 dcnum-0.11.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-27 12:53:52.000000 dcnum-0.11.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:54:01.586604 dcnum-0.11.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.586604 dcnum-0.11.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.586604 dcnum-0.11.5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_ppid.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_write_deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_write_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.062649 dcnum-0.11.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.054649 dcnum-0.11.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.054649 dcnum-0.11.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-27 21:59:14.000000 dcnum-0.11.6/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-27 21:59:14.000000 dcnum-0.11.6/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-27 21:59:14.000000 dcnum-0.11.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-27 21:59:14.000000 dcnum-0.11.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-27 21:59:14.000000 dcnum-0.11.6/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 21:59:14.000000 dcnum-0.11.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-27 21:59:23.062649 dcnum-0.11.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-27 21:59:14.000000 dcnum-0.11.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.054649 dcnum-0.11.6/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-27 21:59:22.000000 dcnum-0.11.6/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.058649 dcnum-0.11.6/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/event_extractor_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.058649 dcnum-0.11.6/dcnum/feat/feat_background/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/feat_background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/feat_background/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/feat_background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/feat_background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.058649 dcnum-0.11.6/dcnum/feat/feat_brightness/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/feat_brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/feat_brightness/bright_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/feat_brightness/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.058649 dcnum-0.11.6/dcnum/feat/feat_moments/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/feat_moments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/feat_moments/ct_opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/feat_moments/mt_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.058649 dcnum-0.11.6/dcnum/feat/feat_texture/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/feat_texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/feat_texture/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/feat_texture/tex_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/feat/queue_event_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.058649 dcnum-0.11.6/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.058649 dcnum-0.11.6/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/read/hdf5_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.058649 dcnum-0.11.6/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/segm/segmenter_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/segm/segmenter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/segm/segmenter_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.062649 dcnum-0.11.6/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/write/deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/write/queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-27 21:59:14.000000 dcnum-0.11.6/dcnum/write/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.054649 dcnum-0.11.6/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-27 21:59:23.000000 dcnum-0.11.6/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-27 21:59:23.000000 dcnum-0.11.6/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:59:23.000000 dcnum-0.11.6/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-27 21:59:23.000000 dcnum-0.11.6/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 21:59:23.000000 dcnum-0.11.6/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.062649 dcnum-0.11.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-27 21:59:14.000000 dcnum-0.11.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.062649 dcnum-0.11.6/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-27 21:59:14.000000 dcnum-0.11.6/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-27 21:59:14.000000 dcnum-0.11.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 21:59:14.000000 dcnum-0.11.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-27 21:59:14.000000 dcnum-0.11.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:59:23.066650 dcnum-0.11.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.062649 dcnum-0.11.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:59:23.062649 dcnum-0.11.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/test_ppid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/test_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/test_segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/test_write_deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-27 21:59:14.000000 dcnum-0.11.6/tests/test_write_writer.py
```

### Comparing `dcnum-0.11.5/.github/workflows/check.yml` & `dcnum-0.11.6/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/.github/workflows/deploy_pypi.yml` & `dcnum-0.11.6/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/.gitignore` & `dcnum-0.11.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/CHANGELOG` & `dcnum-0.11.6/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+0.11.6
+ - enh: add more debugging messages for feature extraction workers
 0.11.5
  - setup: fix bad package discovery
 0.11.4
  - fix: properly handle empty logs
 0.11.3
  - fix: make sure values in tables dictionary are one-dimensional
 0.11.2
```

### Comparing `dcnum-0.11.5/LICENSE` & `dcnum-0.11.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/PKG-INFO` & `dcnum-0.11.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.11.5
+Version: 0.11.6
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.11.5/README.rst` & `dcnum-0.11.6/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/feat/event_extractor_manager_thread.py` & `dcnum-0.11.6/dcnum/feat/event_extractor_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/feat/feat_background/base.py` & `dcnum-0.11.6/dcnum/feat/feat_background/base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/feat/feat_background/bg_roll_median.py` & `dcnum-0.11.6/dcnum/feat/feat_background/bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/feat/feat_background/bg_sparse_median.py` & `dcnum-0.11.6/dcnum/feat/feat_background/bg_sparse_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/feat/feat_brightness/bright_all.py` & `dcnum-0.11.6/dcnum/feat/feat_brightness/bright_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/feat/feat_moments/mt_legacy.py` & `dcnum-0.11.6/dcnum/feat/feat_moments/mt_legacy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/feat/feat_texture/tex_all.py` & `dcnum-0.11.6/dcnum/feat/feat_texture/tex_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/feat/gate.py` & `dcnum-0.11.6/dcnum/feat/gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/feat/queue_event_extractor.py` & `dcnum-0.11.6/dcnum/feat/queue_event_extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -253,15 +253,29 @@
             try:
                 chunk_index, label_index = self.raw_queue.get(timeout=.03)
                 index = chunk_index * self.data.image.chunk_size + label_index
             except queue.Empty:
                 if self.finalize_extraction.value:
                     # The manager told us that there is nothing more coming.
                     self.logger.debug(
-                        f"Finalizing worker {self} with PID {os.getpid()}")
+                        f"Finalizing worker {self} with PID {os.getpid()}. "
+                        f"{self.event_queue.qsize()} events are still queued.")
+                    # Tell the queue background thread to flush all data to
+                    # the queue. The background thread will quit once it has
+                    # flushed all buffered data to the pipe.
+                    self.event_queue.close()
+                    self.logger.debug(
+                        f"Closed event queue from Process PID {os.getpid()}")
+                    # Join the queue background thread. It blocks until the
+                    # background thread exits, ensuring that all data in the
+                    # buffer has been flushed to the pipe.
+                    self.event_queue.join_thread()
+                    self.logger.debug(
+                        f"Joined event queue background thread from"
+                        f"Process PID {os.getpid()}")
                     break
             else:
                 try:
                     events = self.process_label(
                         label=mp_array[label_index],
                         index=index)
                 except BaseException:
```

### Comparing `dcnum-0.11.5/dcnum/meta/ppid.py` & `dcnum-0.11.6/dcnum/meta/ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/read/cache.py` & `dcnum-0.11.6/dcnum/read/cache.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/read/hdf5_data.py` & `dcnum-0.11.6/dcnum/read/hdf5_data.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/segm/segm_thresh.py` & `dcnum-0.11.6/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/segm/segmenter.py` & `dcnum-0.11.6/dcnum/segm/segmenter.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/segm/segmenter_cpu.py` & `dcnum-0.11.6/dcnum/segm/segmenter_cpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/segm/segmenter_gpu.py` & `dcnum-0.11.6/dcnum/segm/segmenter_gpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/segm/segmenter_manager_thread.py` & `dcnum-0.11.6/dcnum/segm/segmenter_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/write/deque_writer_thread.py` & `dcnum-0.11.6/dcnum/write/deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum/write/queue_collector_thread.py` & `dcnum-0.11.6/dcnum/write/queue_collector_thread.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,15 +179,17 @@
                           cur_frame:cur_frame + self.write_threshold]
             if np.any(np.array(cur_nevents) < 0):
                 # We are not yet ready to write any new data to the queue.
                 time.sleep(.01)
                 continue
 
             if len(cur_nevents) == 0:
-                self.logger.warning("Encountered empty nevents array!")
+                self.logger.info(
+                    "Reached the end of the current dataset (frame "
+                    f"{cur_frame + 1} of {len(self.feat_nevents)}).")
                 break
 
             # We have reached the writer threshold. This means the extractor
             # has analyzed at least `write_threshold` frames (not events).
             self.logger.debug(f"Current frame: {cur_frame}")
 
             # Create an event stash
@@ -210,14 +212,15 @@
 
             # Now, get the data from the queue until we have everything
             # that belongs to our chunk (this might also populate buffer_dq).
             while True:
                 try:
                     idx, events = self.event_queue.get(timeout=.3)
                 except queue.Empty:
+                    # No time.sleep here, because we are using timeout above.
                     continue
                 if cur_frame <= idx < cur_frame + self.write_threshold:
                     stash.add_events(index=idx, events=events)
                 else:
                     # Goes onto the buffer stack (might happen if some other
                     # processes were faster)
                     self.buffer_dq.append((idx, events))
@@ -249,16 +252,18 @@
                 imdat[ii] = self.data.image[idx]
                 bgdat[ii] = self.data.image_bg[idx]
             self.writer_dq.append(("image", imdat))
             self.writer_dq.append(("image_bg", bgdat))
 
             # Write the number of events.
             self.writer_dq.append(("nevents",
+                                   # Get nevents for each event from the
+                                   # frame-based cur_nevents array.
                                    np.array(stash.feat_nevents)[
                                        indices - stash.index_offset]
                                    ))
             # Update events/frames written (used for monitoring)
             self.written_events += stash.size
             self.written_frames += stash.num_frames
 
             # Increment current frame index.
-            cur_frame += self.write_threshold
+            cur_frame += len(cur_nevents)
```

### Comparing `dcnum-0.11.5/dcnum/write/writer.py` & `dcnum-0.11.6/dcnum/write/writer.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/dcnum.egg-info/PKG-INFO` & `dcnum-0.11.6/dcnum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.11.5
+Version: 0.11.6
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.11.5/dcnum.egg-info/SOURCES.txt` & `dcnum-0.11.6/dcnum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/docs/conf.py` & `dcnum-0.11.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/docs/extensions/github_changelog.py` & `dcnum-0.11.6/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/pyproject.toml` & `dcnum-0.11.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/tests/conftest.py` & `dcnum-0.11.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.11.6/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.11.6/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/tests/helper_methods.py` & `dcnum-0.11.6/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.11.6/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/tests/test_feat_brightness.py` & `dcnum-0.11.6/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/tests/test_feat_haralick.py` & `dcnum-0.11.6/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/tests/test_feat_moments_based.py` & `dcnum-0.11.6/tests/test_feat_moments_based.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/tests/test_ppid.py` & `dcnum-0.11.6/tests/test_ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/tests/test_read_concat_hdf5.py` & `dcnum-0.11.6/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/tests/test_read_hdf5.py` & `dcnum-0.11.6/tests/test_read_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/tests/test_segm_thresh.py` & `dcnum-0.11.6/tests/test_segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/tests/test_segmenter.py` & `dcnum-0.11.6/tests/test_segmenter.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/tests/test_write_deque_writer_thread.py` & `dcnum-0.11.6/tests/test_write_deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.5/tests/test_write_writer.py` & `dcnum-0.11.6/tests/test_write_writer.py`

 * *Files identical despite different names*

