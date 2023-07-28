# Comparing `tmp/tensorneko-0.3.0.tar.gz` & `tmp/tensorneko-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorneko-0.3.0.tar", last modified: Thu Jul 27 06:17:28 2023, max compression
+gzip compressed data, was "tensorneko-0.3.1.tar", last modified: Fri Jul 28 09:05:59 2023, max compression
```

## Comparing `tensorneko-0.3.0.tar` & `tensorneko-0.3.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.949462 tensorneko-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-27 06:14:43.000000 tensorneko-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    18248 2023-07-27 06:17:28.949462 tensorneko-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17201 2023-07-27 06:14:43.000000 tensorneko-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-27 06:17:28.949462 tensorneko-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-07-27 06:14:43.000000 tensorneko-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.905461 tensorneko-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.909461 tensorneko-0.3.0/src/tensorneko/
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.909461 tensorneko-0.3.0/src/tensorneko/arch/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/arch/auto_encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)     7205 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/arch/gan.py
--rw-r--r--   0 runner    (1001) docker     (122)     3730 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/arch/vqvae.py
--rw-r--r--   0 runner    (1001) docker     (122)     4712 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/arch/wgan.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.913461 tensorneko-0.3.0/src/tensorneko/backend/
--rw-r--r--   0 runner    (1001) docker     (122)      164 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.917461 tensorneko-0.3.0/src/tensorneko/callback/
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/display_metrics_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/earlystop_lr.py
--rw-r--r--   0 runner    (1001) docker     (122)      456 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/epoch_num_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/epoch_time_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/gpu_stats_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/lr_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/nil_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/system_stats_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.917461 tensorneko-0.3.0/src/tensorneko/dataset/
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      942 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/dataset/nested_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/dataset/round_robin_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.917461 tensorneko-0.3.0/src/tensorneko/debug/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/debug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.921461 tensorneko-0.3.0/src/tensorneko/evaluation/
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/evaluation/enum.py
--rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/evaluation/fid.py
--rw-r--r--   0 runner    (1001) docker     (122)     2914 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/evaluation/iou.py
--rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/evaluation/psnr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/evaluation/ssim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.921461 tensorneko-0.3.0/src/tensorneko/io/
--rw-r--r--   0 runner    (1001) docker     (122)      213 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.925462 tensorneko-0.3.0/src/tensorneko/io/mesh/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/io/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/io/mesh/mesh_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/io/mesh/mesh_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)      705 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/io/reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/io/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.929462 tensorneko-0.3.0/src/tensorneko/layer/
--rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1177 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (122)     6360 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/attention.py
--rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/conv.py
--rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     4796 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/masked_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/noise.py
--rw-r--r--   0 runner    (1001) docker     (122)     6585 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/patching.py
--rw-r--r--   0 runner    (1001) docker     (122)     4283 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/positional_embedding.py
--rw-r--r--   0 runner    (1001) docker     (122)      813 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/reshape.py
--rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/stack.py
--rw-r--r--   0 runner    (1001) docker     (122)     2178 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/vector_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.933462 tensorneko-0.3.0/src/tensorneko/module/
--rw-r--r--   0 runner    (1001) docker     (122)      403 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/module/dense.py
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/module/gated_conv.py
--rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/module/inception.py
--rw-r--r--   0 runner    (1001) docker     (122)     3361 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/module/mlp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/module/residual.py
--rw-r--r--   0 runner    (1001) docker     (122)     7602 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/module/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     9803 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/neko_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/neko_module.py
--rw-r--r--   0 runner    (1001) docker     (122)    10007 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/neko_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.937462 tensorneko-0.3.0/src/tensorneko/notebook/
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.937462 tensorneko-0.3.0/src/tensorneko/optim/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.937462 tensorneko-0.3.0/src/tensorneko/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/optim/lr_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.941462 tensorneko-0.3.0/src/tensorneko/preprocess/
--rw-r--r--   0 runner    (1001) docker     (122)      808 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2732 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/preprocess/crop.py
--rw-r--r--   0 runner    (1001) docker     (122)      874 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/preprocess/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.941462 tensorneko-0.3.0/src/tensorneko/preprocess/face_detector/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/preprocess/face_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3238 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/preprocess/pad.py
--rw-r--r--   0 runner    (1001) docker     (122)     3469 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/preprocess/resize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.945462 tensorneko-0.3.0/src/tensorneko/util/
--rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/util/configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/util/dispatched_misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     4565 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/util/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/util/string_getter.py
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/util/type.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-27 06:17:28.000000 tensorneko-0.3.0/src/tensorneko/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.945462 tensorneko-0.3.0/src/tensorneko/visualization/
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.945462 tensorneko-0.3.0/src/tensorneko/visualization/image_browser/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/visualization/image_browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/visualization/log_graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/visualization/matplotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.949462 tensorneko-0.3.0/src/tensorneko/visualization/watcher/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/visualization/watcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.909461 tensorneko-0.3.0/src/tensorneko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    18248 2023-07-27 06:17:28.000000 tensorneko-0.3.0/src/tensorneko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-27 06:17:28.000000 tensorneko-0.3.0/src/tensorneko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 06:17:28.000000 tensorneko-0.3.0/src/tensorneko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-27 06:17:28.000000 tensorneko-0.3.0/src/tensorneko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-27 06:17:28.000000 tensorneko-0.3.0/src/tensorneko.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.949462 tensorneko-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-27 06:14:43.000000 tensorneko-0.3.0/test/test_library_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-27 06:14:43.000000 tensorneko-0.3.0/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.803948 tensorneko-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-28 09:03:02.000000 tensorneko-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    18248 2023-07-28 09:05:59.799948 tensorneko-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17201 2023-07-28 09:03:02.000000 tensorneko-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-28 09:05:59.803948 tensorneko-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-07-28 09:03:02.000000 tensorneko-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.775948 tensorneko-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.775948 tensorneko-0.3.1/src/tensorneko/
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.783948 tensorneko-0.3.1/src/tensorneko/arch/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/arch/auto_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7205 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/arch/gan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3730 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/arch/vqvae.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4712 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/arch/wgan.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.783948 tensorneko-0.3.1/src/tensorneko/backend/
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.783948 tensorneko-0.3.1/src/tensorneko/callback/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/display_metrics_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/earlystop_lr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      456 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/epoch_num_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/epoch_time_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/gpu_stats_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/lr_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/nil_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/system_stats_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.787948 tensorneko-0.3.1/src/tensorneko/dataset/
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/dataset/nested_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/dataset/round_robin_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.787948 tensorneko-0.3.1/src/tensorneko/debug/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/debug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.787948 tensorneko-0.3.1/src/tensorneko/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/evaluation/enum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/evaluation/fid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2914 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/evaluation/iou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/evaluation/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/evaluation/ssim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.787948 tensorneko-0.3.1/src/tensorneko/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.787948 tensorneko-0.3.1/src/tensorneko/io/mesh/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/io/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/io/mesh/mesh_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/io/mesh/mesh_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      705 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/io/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.791948 tensorneko-0.3.1/src/tensorneko/layer/
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1177 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6360 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4796 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/masked_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/noise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6585 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/patching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4283 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/positional_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/stack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2178 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/vector_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.795948 tensorneko-0.3.1/src/tensorneko/module/
+-rw-r--r--   0 runner    (1001) docker     (122)      403 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/module/dense.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/module/gated_conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/module/inception.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3361 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/module/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/module/residual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7602 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/module/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9927 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/neko_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/neko_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10007 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/neko_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.795948 tensorneko-0.3.1/src/tensorneko/notebook/
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.795948 tensorneko-0.3.1/src/tensorneko/optim/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.795948 tensorneko-0.3.1/src/tensorneko/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/optim/lr_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.795948 tensorneko-0.3.1/src/tensorneko/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (122)      808 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2732 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/preprocess/crop.py
+-rw-r--r--   0 runner    (1001) docker     (122)      874 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/preprocess/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.795948 tensorneko-0.3.1/src/tensorneko/preprocess/face_detector/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/preprocess/face_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3238 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/preprocess/pad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3469 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/preprocess/resize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.799948 tensorneko-0.3.1/src/tensorneko/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/util/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/util/dispatched_misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4565 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/util/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/util/string_getter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/util/type.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-28 09:05:59.000000 tensorneko-0.3.1/src/tensorneko/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.799948 tensorneko-0.3.1/src/tensorneko/visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.799948 tensorneko-0.3.1/src/tensorneko/visualization/image_browser/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/visualization/image_browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/visualization/log_graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/visualization/matplotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.799948 tensorneko-0.3.1/src/tensorneko/visualization/watcher/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/visualization/watcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.775948 tensorneko-0.3.1/src/tensorneko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    18248 2023-07-28 09:05:59.000000 tensorneko-0.3.1/src/tensorneko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-28 09:05:59.000000 tensorneko-0.3.1/src/tensorneko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 09:05:59.000000 tensorneko-0.3.1/src/tensorneko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-28 09:05:59.000000 tensorneko-0.3.1/src/tensorneko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-28 09:05:59.000000 tensorneko-0.3.1/src/tensorneko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.799948 tensorneko-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-28 09:03:02.000000 tensorneko-0.3.1/test/test_library_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-28 09:03:02.000000 tensorneko-0.3.1/test/test_version.py
```

### Comparing `tensorneko-0.3.0/LICENSE` & `tensorneko-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/PKG-INFO` & `tensorneko-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorneko
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 Home-page: https://github.com/ControlNet/tensorneko
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/tensorneko/issues
 Project-URL: Source Code, https://github.com/ControlNet/tensorneko
```

### Comparing `tensorneko-0.3.0/README.md` & `tensorneko-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/setup.py` & `tensorneko-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/__init__.py` & `tensorneko-0.3.1/src/tensorneko/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/arch/auto_encoder.py` & `tensorneko-0.3.1/src/tensorneko/arch/auto_encoder.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/arch/gan.py` & `tensorneko-0.3.1/src/tensorneko/arch/gan.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/arch/vqvae.py` & `tensorneko-0.3.1/src/tensorneko/arch/vqvae.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/arch/wgan.py` & `tensorneko-0.3.1/src/tensorneko/arch/wgan.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/callback/__init__.py` & `tensorneko-0.3.1/src/tensorneko/callback/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/callback/earlystop_lr.py` & `tensorneko-0.3.1/src/tensorneko/callback/earlystop_lr.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/callback/epoch_time_logger.py` & `tensorneko-0.3.1/src/tensorneko/callback/epoch_time_logger.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/callback/gpu_stats_logger.py` & `tensorneko-0.3.1/src/tensorneko/callback/gpu_stats_logger.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/callback/lr_logger.py` & `tensorneko-0.3.1/src/tensorneko/callback/lr_logger.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/callback/system_stats_logger.py` & `tensorneko-0.3.1/src/tensorneko/callback/system_stats_logger.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/dataset/nested_dataset.py` & `tensorneko-0.3.1/src/tensorneko/dataset/nested_dataset.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/dataset/round_robin_dataset.py` & `tensorneko-0.3.1/src/tensorneko/dataset/round_robin_dataset.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/evaluation/fid.py` & `tensorneko-0.3.1/src/tensorneko/evaluation/fid.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/evaluation/iou.py` & `tensorneko-0.3.1/src/tensorneko/evaluation/iou.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/evaluation/psnr.py` & `tensorneko-0.3.1/src/tensorneko/evaluation/psnr.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/evaluation/ssim.py` & `tensorneko-0.3.1/src/tensorneko/evaluation/ssim.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/io/reader.py` & `tensorneko-0.3.1/src/tensorneko/io/reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/io/writer.py` & `tensorneko-0.3.1/src/tensorneko/io/writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/layer/__init__.py` & `tensorneko-0.3.1/src/tensorneko/layer/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/layer/aggregation.py` & `tensorneko-0.3.1/src/tensorneko/layer/aggregation.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/layer/attention.py` & `tensorneko-0.3.1/src/tensorneko/layer/attention.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/layer/concatenate.py` & `tensorneko-0.3.1/src/tensorneko/layer/concatenate.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/layer/conv.py` & `tensorneko-0.3.1/src/tensorneko/layer/conv.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/layer/linear.py` & `tensorneko-0.3.1/src/tensorneko/layer/linear.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/layer/log.py` & `tensorneko-0.3.1/src/tensorneko/layer/log.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/layer/masked_conv2d.py` & `tensorneko-0.3.1/src/tensorneko/layer/masked_conv2d.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/layer/noise.py` & `tensorneko-0.3.1/src/tensorneko/layer/noise.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/layer/patching.py` & `tensorneko-0.3.1/src/tensorneko/layer/patching.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/layer/positional_embedding.py` & `tensorneko-0.3.1/src/tensorneko/layer/positional_embedding.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/layer/reshape.py` & `tensorneko-0.3.1/src/tensorneko/layer/reshape.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/layer/stack.py` & `tensorneko-0.3.1/src/tensorneko/layer/stack.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/layer/vector_quantizer.py` & `tensorneko-0.3.1/src/tensorneko/layer/vector_quantizer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/module/dense.py` & `tensorneko-0.3.1/src/tensorneko/module/dense.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/module/gated_conv.py` & `tensorneko-0.3.1/src/tensorneko/module/gated_conv.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/module/inception.py` & `tensorneko-0.3.1/src/tensorneko/module/inception.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/module/mlp.py` & `tensorneko-0.3.1/src/tensorneko/module/mlp.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/module/residual.py` & `tensorneko-0.3.1/src/tensorneko/module/residual.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/module/transformer.py` & `tensorneko-0.3.1/src/tensorneko/module/transformer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/neko_model.py` & `tensorneko-0.3.1/src/tensorneko/neko_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,24 +167,26 @@
         if not self.trainer:
             return None
         else:
             return self.trainer.logger
 
     def on_train_batch_end(self, outputs: STEP_OUTPUT, batch: Any, batch_idx: int) -> None:
         """For each training step end, log the metrics. Append the outputs of training step to the list"""
+        outputs = {k: v.detach() for k, v in outputs.items()}
         self.training_step_outputs.append(outputs)
         if self.trainer.log_on_step \
             and self.logger is not None \
             and self.trainer.global_step % self.trainer.log_every_n_steps == 0:
             self.log_on_training_step_end(outputs)
 
     def on_validation_batch_end(
         self, outputs: Optional[STEP_OUTPUT], batch: Any, batch_idx: int, dataloader_idx: int = 0
     ) -> None:
         """Append the outputs of validation step to the list"""
+        outputs = {k: v.detach() for k, v in outputs.items()}
         self.validation_step_outputs.append(outputs)
 
     def on_train_epoch_end(self) -> None:
         """For each training epoch end, log the metrics"""
         if self.trainer.log_on_epoch and self.logger is not None:
             self.log_on_training_epoch_end(self.training_step_outputs)
         self.training_step_outputs.clear()
```

### Comparing `tensorneko-0.3.0/src/tensorneko/neko_module.py` & `tensorneko-0.3.1/src/tensorneko/neko_module.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/neko_trainer.py` & `tensorneko-0.3.1/src/tensorneko/neko_trainer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/preprocess/__init__.py` & `tensorneko-0.3.1/src/tensorneko/preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/preprocess/crop.py` & `tensorneko-0.3.1/src/tensorneko/preprocess/crop.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/preprocess/enum.py` & `tensorneko-0.3.1/src/tensorneko/preprocess/enum.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/preprocess/pad.py` & `tensorneko-0.3.1/src/tensorneko/preprocess/pad.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/preprocess/resize.py` & `tensorneko-0.3.1/src/tensorneko/preprocess/resize.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/util/__init__.py` & `tensorneko-0.3.1/src/tensorneko/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/util/configuration.py` & `tensorneko-0.3.1/src/tensorneko/util/configuration.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/util/dispatched_misc.py` & `tensorneko-0.3.1/src/tensorneko/util/dispatched_misc.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/util/misc.py` & `tensorneko-0.3.1/src/tensorneko/util/misc.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/util/reproducibility.py` & `tensorneko-0.3.1/src/tensorneko/util/reproducibility.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/util/string_getter.py` & `tensorneko-0.3.1/src/tensorneko/util/string_getter.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/util/type.py` & `tensorneko-0.3.1/src/tensorneko/util/type.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/visualization/__init__.py` & `tensorneko-0.3.1/src/tensorneko/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/visualization/log_graph.py` & `tensorneko-0.3.1/src/tensorneko/visualization/log_graph.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko/visualization/matplotlib.py` & `tensorneko-0.3.1/src/tensorneko/visualization/matplotlib.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/src/tensorneko.egg-info/PKG-INFO` & `tensorneko-0.3.1/src/tensorneko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorneko
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 Home-page: https://github.com/ControlNet/tensorneko
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/tensorneko/issues
 Project-URL: Source Code, https://github.com/ControlNet/tensorneko
```

### Comparing `tensorneko-0.3.0/src/tensorneko.egg-info/SOURCES.txt` & `tensorneko-0.3.1/src/tensorneko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.0/test/test_version.py` & `tensorneko-0.3.1/test/test_version.py`

 * *Files identical despite different names*

