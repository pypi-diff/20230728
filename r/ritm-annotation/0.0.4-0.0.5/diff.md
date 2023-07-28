# Comparing `tmp/ritm_annotation-0.0.4.tar.gz` & `tmp/ritm_annotation-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ritm_annotation-0.0.4.tar", last modified: Thu Jul 27 20:53:42 2023, max compression
+gzip compressed data, was "ritm_annotation-0.0.5.tar", last modified: Fri Jul 28 12:29:20 2023, max compression
```

## Comparing `ritm_annotation-0.0.4.tar` & `ritm_annotation-0.0.5.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.411370 ritm_annotation-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-27 20:53:42.411370 ritm_annotation-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.403370 ritm_annotation-0.0.4/ritm_annotation/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.407370 ritm_annotation-0.0.4/ritm_annotation/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.407370 ritm_annotation-0.0.4/ritm_annotation/cli/annotate/
--rw-r--r--   0 runner    (1001) docker     (123)    24767 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/cli/annotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/cli/annotate/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/cli/annotate/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/cli/annotate/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.407370 ritm_annotation-0.0.4/ritm_annotation/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.407370 ritm_annotation-0.0.4/ritm_annotation/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/datasets/berkeley.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/datasets/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/datasets/coco_lvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/datasets/davis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/datasets/grabcut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/datasets/images_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/datasets/lvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/datasets/openimages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/datasets/pascalvoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/datasets/sbd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/data/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.407370 ritm_annotation-0.0.4/ritm_annotation/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/engine/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20214 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/engine/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.407370 ritm_annotation-0.0.4/ritm_annotation/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/inference/clicker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/inference/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.407370 ritm_annotation-0.0.4/ritm_annotation/inference/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/inference/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/inference/predictors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/inference/predictors/brs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/inference/predictors/brs_functors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/inference/predictors/brs_losses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.407370 ritm_annotation-0.0.4/ritm_annotation/inference/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/inference/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/inference/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/inference/transforms/crops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/inference/transforms/flip.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/inference/transforms/limit_longest_side.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/inference/transforms/zoom_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/inference/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.411370 ritm_annotation-0.0.4/ritm_annotation/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/is_deeplab_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/is_hrnet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/is_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.411370 ritm_annotation-0.0.4/ritm_annotation/model/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/modeling/basic_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/modeling/deeplab_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/modeling/hrnet_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/modeling/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/modeling/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/modeling/resnetv1b.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/modifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/model/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.411370 ritm_annotation-0.0.4/ritm_annotation/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.411370 ritm_annotation-0.0.4/ritm_annotation/utils/cython/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/utils/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/utils/cython/_get_dist_maps.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/utils/cython/_get_dist_maps.pyxbld
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/utils/cython/dist_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/utils/exp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.411370 ritm_annotation-0.0.4/ritm_annotation/utils/exp_imports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/utils/exp_imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/utils/exp_imports/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/ritm_annotation/utils/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.403370 ritm_annotation-0.0.4/ritm_annotation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-27 20:53:42.000000 ritm_annotation-0.0.4/ritm_annotation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-27 20:53:42.000000 ritm_annotation-0.0.4/ritm_annotation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:53:42.000000 ritm_annotation-0.0.4/ritm_annotation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-27 20:53:42.000000 ritm_annotation-0.0.4/ritm_annotation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-27 20:53:42.000000 ritm_annotation-0.0.4/ritm_annotation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 20:53:42.000000 ritm_annotation-0.0.4/ritm_annotation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:53:42.411370 ritm_annotation-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:42.411370 ritm_annotation-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 20:53:32.000000 ritm_annotation-0.0.4/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.405578 ritm_annotation-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-28 12:29:20.405578 ritm_annotation-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.393578 ritm_annotation-0.0.5/ritm_annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.393578 ritm_annotation-0.0.5/ritm_annotation/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.397578 ritm_annotation-0.0.5/ritm_annotation/cli/annotate/
+-rw-r--r--   0 runner    (1001) docker     (123)    24767 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/cli/annotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/cli/annotate/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/cli/annotate/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/cli/annotate/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.397578 ritm_annotation-0.0.5/ritm_annotation/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.397578 ritm_annotation-0.0.5/ritm_annotation/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/datasets/berkeley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/datasets/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/datasets/coco_lvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/datasets/davis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/datasets/grabcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/datasets/images_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/datasets/lvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/datasets/openimages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/datasets/pascalvoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/datasets/sbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/data/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.397578 ritm_annotation-0.0.5/ritm_annotation/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/engine/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20214 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/engine/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.397578 ritm_annotation-0.0.5/ritm_annotation/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/inference/clicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/inference/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.401578 ritm_annotation-0.0.5/ritm_annotation/inference/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/inference/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/inference/predictors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/inference/predictors/brs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/inference/predictors/brs_functors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/inference/predictors/brs_losses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.401578 ritm_annotation-0.0.5/ritm_annotation/inference/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/inference/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/inference/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/inference/transforms/crops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/inference/transforms/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/inference/transforms/limit_longest_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/inference/transforms/zoom_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/inference/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.401578 ritm_annotation-0.0.5/ritm_annotation/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/is_deeplab_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/is_hrnet_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/is_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.401578 ritm_annotation-0.0.5/ritm_annotation/model/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/modeling/basic_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/modeling/deeplab_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/modeling/hrnet_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/modeling/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/modeling/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/modeling/resnetv1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/model/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.405578 ritm_annotation-0.0.5/ritm_annotation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.405578 ritm_annotation-0.0.5/ritm_annotation/utils/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/utils/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/utils/cython/_get_dist_maps.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/utils/cython/_get_dist_maps.pyxbld
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/utils/cython/dist_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/utils/exp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.405578 ritm_annotation-0.0.5/ritm_annotation/utils/exp_imports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/utils/exp_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/utils/exp_imports/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/ritm_annotation/utils/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.393578 ritm_annotation-0.0.5/ritm_annotation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-28 12:29:20.000000 ritm_annotation-0.0.5/ritm_annotation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-28 12:29:20.000000 ritm_annotation-0.0.5/ritm_annotation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:29:20.000000 ritm_annotation-0.0.5/ritm_annotation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 12:29:20.000000 ritm_annotation-0.0.5/ritm_annotation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-28 12:29:20.000000 ritm_annotation-0.0.5/ritm_annotation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 12:29:20.000000 ritm_annotation-0.0.5/ritm_annotation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 12:29:20.405578 ritm_annotation-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:20.405578 ritm_annotation-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 12:29:04.000000 ritm_annotation-0.0.5/tests/test_base.py
```

### Comparing `ritm_annotation-0.0.4/ritm_annotation/cli/__init__.py` & `ritm_annotation-0.0.5/ritm_annotation/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/cli/annotate/__init__.py` & `ritm_annotation-0.0.5/ritm_annotation/cli/annotate/__init__.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/cli/annotate/canvas.py` & `ritm_annotation-0.0.5/ritm_annotation/cli/annotate/canvas.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/cli/annotate/controller.py` & `ritm_annotation-0.0.5/ritm_annotation/cli/annotate/controller.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/cli/annotate/wrappers.py` & `ritm_annotation-0.0.5/ritm_annotation/cli/annotate/wrappers.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/base.py` & `ritm_annotation-0.0.5/ritm_annotation/data/base.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/compose.py` & `ritm_annotation-0.0.5/ritm_annotation/data/compose.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/datasets/__init__.py` & `ritm_annotation-0.0.5/ritm_annotation/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/datasets/ade20k.py` & `ritm_annotation-0.0.5/ritm_annotation/data/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/datasets/coco.py` & `ritm_annotation-0.0.5/ritm_annotation/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/datasets/coco_lvis.py` & `ritm_annotation-0.0.5/ritm_annotation/data/datasets/coco_lvis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/datasets/davis.py` & `ritm_annotation-0.0.5/ritm_annotation/data/datasets/davis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/datasets/grabcut.py` & `ritm_annotation-0.0.5/ritm_annotation/data/datasets/grabcut.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/datasets/images_dir.py` & `ritm_annotation-0.0.5/ritm_annotation/data/datasets/images_dir.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/datasets/lvis.py` & `ritm_annotation-0.0.5/ritm_annotation/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/datasets/openimages.py` & `ritm_annotation-0.0.5/ritm_annotation/data/datasets/openimages.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/datasets/pascalvoc.py` & `ritm_annotation-0.0.5/ritm_annotation/data/datasets/pascalvoc.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/datasets/sbd.py` & `ritm_annotation-0.0.5/ritm_annotation/data/datasets/sbd.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/points_sampler.py` & `ritm_annotation-0.0.5/ritm_annotation/data/points_sampler.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/sample.py` & `ritm_annotation-0.0.5/ritm_annotation/data/sample.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/data/transforms.py` & `ritm_annotation-0.0.5/ritm_annotation/data/transforms.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/engine/optimizer.py` & `ritm_annotation-0.0.5/ritm_annotation/engine/optimizer.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/engine/trainer.py` & `ritm_annotation-0.0.5/ritm_annotation/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/inference/clicker.py` & `ritm_annotation-0.0.5/ritm_annotation/inference/clicker.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/inference/evaluation.py` & `ritm_annotation-0.0.5/ritm_annotation/inference/evaluation.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/inference/predictors/__init__.py` & `ritm_annotation-0.0.5/ritm_annotation/inference/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/inference/predictors/base.py` & `ritm_annotation-0.0.5/ritm_annotation/inference/predictors/base.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/inference/predictors/brs.py` & `ritm_annotation-0.0.5/ritm_annotation/inference/predictors/brs.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/inference/predictors/brs_functors.py` & `ritm_annotation-0.0.5/ritm_annotation/inference/predictors/brs_functors.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/inference/predictors/brs_losses.py` & `ritm_annotation-0.0.5/ritm_annotation/inference/predictors/brs_losses.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/inference/transforms/base.py` & `ritm_annotation-0.0.5/ritm_annotation/inference/transforms/base.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/inference/transforms/crops.py` & `ritm_annotation-0.0.5/ritm_annotation/inference/transforms/crops.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/inference/transforms/flip.py` & `ritm_annotation-0.0.5/ritm_annotation/inference/transforms/flip.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/inference/transforms/limit_longest_side.py` & `ritm_annotation-0.0.5/ritm_annotation/inference/transforms/limit_longest_side.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/inference/transforms/zoom_in.py` & `ritm_annotation-0.0.5/ritm_annotation/inference/transforms/zoom_in.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/inference/utils.py` & `ritm_annotation-0.0.5/ritm_annotation/inference/utils.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/model/initializer.py` & `ritm_annotation-0.0.5/ritm_annotation/model/initializer.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/model/is_deeplab_model.py` & `ritm_annotation-0.0.5/ritm_annotation/model/is_deeplab_model.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/model/is_hrnet_model.py` & `ritm_annotation-0.0.5/ritm_annotation/model/is_hrnet_model.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/model/is_model.py` & `ritm_annotation-0.0.5/ritm_annotation/model/is_model.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/model/losses.py` & `ritm_annotation-0.0.5/ritm_annotation/model/losses.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/model/metrics.py` & `ritm_annotation-0.0.5/ritm_annotation/model/metrics.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/model/modeling/basic_blocks.py` & `ritm_annotation-0.0.5/ritm_annotation/model/modeling/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/model/modeling/deeplab_v3.py` & `ritm_annotation-0.0.5/ritm_annotation/model/modeling/deeplab_v3.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/model/modeling/hrnet_ocr.py` & `ritm_annotation-0.0.5/ritm_annotation/model/modeling/hrnet_ocr.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/model/modeling/ocr.py` & `ritm_annotation-0.0.5/ritm_annotation/model/modeling/ocr.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/model/modeling/resnet.py` & `ritm_annotation-0.0.5/ritm_annotation/model/modeling/resnet.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/model/modeling/resnetv1b.py` & `ritm_annotation-0.0.5/ritm_annotation/model/modeling/resnetv1b.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/model/ops.py` & `ritm_annotation-0.0.5/ritm_annotation/model/ops.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/utils/cython/_get_dist_maps.pyx` & `ritm_annotation-0.0.5/ritm_annotation/utils/cython/_get_dist_maps.pyx`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/utils/distributed.py` & `ritm_annotation-0.0.5/ritm_annotation/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/utils/exp.py` & `ritm_annotation-0.0.5/ritm_annotation/utils/exp.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/utils/exp_imports/default.py` & `ritm_annotation-0.0.5/ritm_annotation/utils/exp_imports/default.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/utils/log.py` & `ritm_annotation-0.0.5/ritm_annotation/utils/log.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/utils/misc.py` & `ritm_annotation-0.0.5/ritm_annotation/utils/misc.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/utils/serialization.py` & `ritm_annotation-0.0.5/ritm_annotation/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation/utils/vis.py` & `ritm_annotation-0.0.5/ritm_annotation/utils/vis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/ritm_annotation.egg-info/SOURCES.txt` & `ritm_annotation-0.0.5/ritm_annotation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.4/setup.py` & `ritm_annotation-0.0.5/setup.py`

 * *Files identical despite different names*

