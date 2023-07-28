# Comparing `tmp/ml-starter-0.1.40.tar.gz` & `tmp/ml-starter-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.40.tar", last modified: Thu Jul 27 01:14:42 2023, max compression
+gzip compressed data, was "ml-starter-0.1.41.tar", last modified: Fri Jul 28 21:52:34 2023, max compression
```

## Comparing `ml-starter-0.1.40.tar` & `ml-starter-0.1.41.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.993226 ml-starter-0.1.40/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-27 01:14:30.000000 ml-starter-0.1.40/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 01:14:30.000000 ml-starter-0.1.40/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-27 01:14:42.993226 ml-starter-0.1.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-27 01:14:30.000000 ml-starter-0.1.40/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.973225 ml-starter-0.1.40/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.973225 ml-starter-0.1.40/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.973225 ml-starter-0.1.40/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/launchers/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.977226 ml-starter-0.1.40/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.977226 ml-starter-0.1.40/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.977226 ml-starter-0.1.40/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.977226 ml-starter-0.1.40/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.977226 ml-starter-0.1.40/ml/models/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/architectures/bifpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/architectures/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/codebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.981226 ml-starter-0.1.40/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.981226 ml-starter-0.1.40/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.981226 ml-starter-0.1.40/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.981226 ml-starter-0.1.40/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.981226 ml-starter-0.1.40/ml/tasks/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/diffusion/beta_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/diffusion/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.985226 ml-starter-0.1.40/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.985226 ml-starter-0.1.40/ml/tasks/gan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/gan/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.985226 ml-starter-0.1.40/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/losses/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/losses/kl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/losses/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.985226 ml-starter-0.1.40/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.985226 ml-starter-0.1.40/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.985226 ml-starter-0.1.40/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24976 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.985226 ml-starter-0.1.40/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.993226 ml-starter-0.1.40/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    35281 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.993226 ml-starter-0.1.40/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.993226 ml-starter-0.1.40/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.993226 ml-starter-0.1.40/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-27 01:14:42.000000 ml-starter-0.1.40/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-27 01:14:42.000000 ml-starter-0.1.40/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 01:14:42.000000 ml-starter-0.1.40/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-27 01:14:42.000000 ml-starter-0.1.40/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-27 01:14:42.000000 ml-starter-0.1.40/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-27 01:14:30.000000 ml-starter-0.1.40/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-27 01:14:42.993226 ml-starter-0.1.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-27 01:14:30.000000 ml-starter-0.1.40/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.550255 ml-starter-0.1.41/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-28 21:52:19.000000 ml-starter-0.1.41/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-28 21:52:19.000000 ml-starter-0.1.41/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-28 21:52:34.550255 ml-starter-0.1.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-28 21:52:19.000000 ml-starter-0.1.41/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.530255 ml-starter-0.1.41/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.530255 ml-starter-0.1.41/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.534255 ml-starter-0.1.41/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/launchers/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.534255 ml-starter-0.1.41/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.534255 ml-starter-0.1.41/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.534255 ml-starter-0.1.41/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.534255 ml-starter-0.1.41/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.534255 ml-starter-0.1.41/ml/models/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/architectures/bifpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/architectures/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/codebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.538255 ml-starter-0.1.41/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.538255 ml-starter-0.1.41/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.538255 ml-starter-0.1.41/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.538255 ml-starter-0.1.41/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.538255 ml-starter-0.1.41/ml/tasks/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/diffusion/beta_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/diffusion/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.542255 ml-starter-0.1.41/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.542255 ml-starter-0.1.41/ml/tasks/gan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/gan/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.542255 ml-starter-0.1.41/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/losses/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/losses/kl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/losses/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.542255 ml-starter-0.1.41/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.542255 ml-starter-0.1.41/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.542255 ml-starter-0.1.41/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24976 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.542255 ml-starter-0.1.41/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.546255 ml-starter-0.1.41/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38804 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.550255 ml-starter-0.1.41/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.550255 ml-starter-0.1.41/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.550255 ml-starter-0.1.41/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-28 21:52:34.000000 ml-starter-0.1.41/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-28 21:52:34.000000 ml-starter-0.1.41/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 21:52:34.000000 ml-starter-0.1.41/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-28 21:52:34.000000 ml-starter-0.1.41/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-28 21:52:34.000000 ml-starter-0.1.41/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-28 21:52:19.000000 ml-starter-0.1.41/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-28 21:52:34.550255 ml-starter-0.1.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-28 21:52:19.000000 ml-starter-0.1.41/setup.py
```

### Comparing `ml-starter-0.1.40/LICENSE` & `ml-starter-0.1.41/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/PKG-INFO` & `ml-starter-0.1.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.40
+Version: 0.1.41
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.40/README.md` & `ml-starter-0.1.41/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/api.py` & `ml-starter-0.1.41/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/core/common_types.py` & `ml-starter-0.1.41/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/core/config.py` & `ml-starter-0.1.41/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/core/env.py` & `ml-starter-0.1.41/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/core/registry.py` & `ml-starter-0.1.41/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/core/state.py` & `ml-starter-0.1.41/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/launchers/base.py` & `ml-starter-0.1.41/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/launchers/mp.py` & `ml-starter-0.1.41/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/launchers/sagemaker.py` & `ml-starter-0.1.41/ml/launchers/sagemaker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/launchers/slurm.py` & `ml-starter-0.1.41/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/launchers/torchrun.py` & `ml-starter-0.1.41/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/loggers/base.py` & `ml-starter-0.1.41/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/loggers/meter.py` & `ml-starter-0.1.41/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/loggers/multi.py` & `ml-starter-0.1.41/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/loggers/stdout.py` & `ml-starter-0.1.41/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/loggers/tensorboard.py` & `ml-starter-0.1.41/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/lr_schedulers/base.py` & `ml-starter-0.1.41/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/lr_schedulers/constant.py` & `ml-starter-0.1.41/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.41/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.41/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/lr_schedulers/gan.py` & `ml-starter-0.1.41/ml/lr_schedulers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/lr_schedulers/linear.py` & `ml-starter-0.1.41/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.41/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.41/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/models/activations.py` & `ml-starter-0.1.41/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/models/architectures/bifpn.py` & `ml-starter-0.1.41/ml/models/architectures/bifpn.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/models/architectures/unet.py` & `ml-starter-0.1.41/ml/models/architectures/unet.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/models/base.py` & `ml-starter-0.1.41/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/models/codebook.py` & `ml-starter-0.1.41/ml/models/codebook.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/models/embeddings.py` & `ml-starter-0.1.41/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/models/gan.py` & `ml-starter-0.1.41/ml/models/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/models/init.py` & `ml-starter-0.1.41/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/models/kmeans.py` & `ml-starter-0.1.41/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/models/lora.py` & `ml-starter-0.1.41/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/models/modules.py` & `ml-starter-0.1.41/ml/models/modules.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/models/norms.py` & `ml-starter-0.1.41/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/models/parallel.py` & `ml-starter-0.1.41/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/optimizers/adam.py` & `ml-starter-0.1.41/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/optimizers/adan.py` & `ml-starter-0.1.41/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/optimizers/base.py` & `ml-starter-0.1.41/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/optimizers/common.py` & `ml-starter-0.1.41/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/optimizers/gan.py` & `ml-starter-0.1.41/ml/optimizers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/optimizers/lion.py` & `ml-starter-0.1.41/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/optimizers/sgd.py` & `ml-starter-0.1.41/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/optimizers/shampoo.py` & `ml-starter-0.1.41/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/scripts/cli.py` & `ml-starter-0.1.41/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/scripts/stage.py` & `ml-starter-0.1.41/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/scripts/train.py` & `ml-starter-0.1.41/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/base.py` & `ml-starter-0.1.41/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.41/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.41/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/datasets/collate.py` & `ml-starter-0.1.41/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.41/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.41/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.41/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.41/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.41/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.41/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/diffusion/beta_schedule.py` & `ml-starter-0.1.41/ml/tasks/diffusion/beta_schedule.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/diffusion/gaussian.py` & `ml-starter-0.1.41/ml/tasks/diffusion/gaussian.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/environments/base.py` & `ml-starter-0.1.41/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/environments/utils.py` & `ml-starter-0.1.41/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/environments/worker.py` & `ml-starter-0.1.41/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/gan/base.py` & `ml-starter-0.1.41/ml/tasks/gan/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/losses/audio.py` & `ml-starter-0.1.41/ml/tasks/losses/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Defines some loss functions which are suitable for audio."""
 
+import warnings
 from typing import Literal, cast
 
 import torch
 import torch.nn.functional as F
 from torch import Tensor
 
 WindowFn = Literal["hann", "hamming", "blackman"]
@@ -59,14 +60,19 @@
             ``(B, num_frames, #=num_freq_bins)``.
         y_mag: Magnitude spectrogram of groundtruth signal, with shape
             ``(B, num_frames, num_freq_bins)``.
 
     Returns:
         Spectral convergence loss value.
     """
+    if y_mag.requires_grad:
+        warnings.warn(
+            "`y_mag` is the ground truth and should not require a gradient! "
+            "`spectral_convergence_loss` is not a symmetric loss function."
+        )
     return torch.norm(y_mag - x_mag, p="fro", dim=-1) / torch.norm(y_mag, p="fro", dim=-1)
 
 
 def log_stft_magnitude_loss(x_mag: Tensor, y_mag: Tensor) -> Tensor:
     """Log STFT magnitude loss module.
 
     Args:
```

### Comparing `ml-starter-0.1.40/ml/tasks/losses/image.py` & `ml-starter-0.1.41/ml/tasks/losses/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/losses/kl.py` & `ml-starter-0.1.41/ml/tasks/losses/kl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/losses/loss.py` & `ml-starter-0.1.41/ml/tasks/losses/loss.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/rl/base.py` & `ml-starter-0.1.41/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/rl/replay.py` & `ml-starter-0.1.41/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/tasks/sl/base.py` & `ml-starter-0.1.41/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/trainers/base.py` & `ml-starter-0.1.41/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/trainers/gan.py` & `ml-starter-0.1.41/ml/trainers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/trainers/learning.py` & `ml-starter-0.1.41/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/trainers/mixins/compile.py` & `ml-starter-0.1.41/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.41/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.41/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.41/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.41/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.41/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.41/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.41/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.41/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/trainers/rl.py` & `ml-starter-0.1.41/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/trainers/sl.py` & `ml-starter-0.1.41/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/amp.py` & `ml-starter-0.1.41/ml/utils/amp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/argparse.py` & `ml-starter-0.1.41/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/atomic.py` & `ml-starter-0.1.41/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/attention.py` & `ml-starter-0.1.41/ml/utils/attention.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/audio.py` & `ml-starter-0.1.41/ml/utils/audio.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
     from ml.utils.audio import read_audio, write_audio
 
 This just uses FFMPEG so it should be rasonably quick.
 """
 
 import fractions
+import functools
 import itertools
 import logging
 import multiprocessing as mp
 import os
 import random
 import re
 import shutil
@@ -35,14 +36,15 @@
 from torch.utils.data.dataset import ConcatDataset, Dataset, IterableDataset
 
 from ml.utils.data import get_worker_info
 from ml.utils.distributed import get_world_size
 from ml.utils.io import prefetch_samples
 from ml.utils.numpy import as_numpy_array
 from ml.utils.timer import Timer
+from ml.utils.tokens import TokenReader, TokenWriter
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 DEFAULT_BLOCKSIZE = 16_000
 
@@ -531,30 +533,72 @@
             sample_rate=sample_rate,
             channels=channels,
             num_frames=num_frames,
         ),
     )
 
 
-def get_files_cached(root_dir: Path, processes: int = 16) -> list[AudioFile]:
+class AudioFileCache:
+    def __init__(self, cache_path: Path, props_path: Path) -> None:
+        super().__init__()
+
+        self.cache_path = cache_path
+        self.props_path = props_path
+
+    @functools.cached_property
+    def _props_and_offsets(self) -> tuple[list[AudioProps], list[int]]:
+        tr = TokenReader(self.props_path, None)
+        sample_rates = tr[0]
+        channels = tr[1]
+        num_frames = tr[2]
+        lengths = tr[3]
+        offsets = [0]
+        for length in lengths:
+            offsets.append(offsets[-1] + length)
+        return (
+            [AudioProps(*values) for values in zip(sample_rates, channels, num_frames)],
+            offsets,
+        )
+
+    @property
+    def props(self) -> list[AudioProps]:
+        return self._props_and_offsets[0]
+
+    @property
+    def offsets(self) -> list[int]:
+        return self._props_and_offsets[1]
+
+    def __getitem__(self, index: int) -> AudioFile:
+        offset, next_offset = self.offsets[index], self.offsets[index + 1]
+
+        with open(self.cache_path, "r", encoding="utf-8") as f:
+            f.seek(offset)
+            line = f.read(next_offset - offset)
+            return AudioFile.parse(line)
+
+    def __len__(self) -> int:
+        return len(self.offsets) - 1
+
+
+def get_files_cached_path(root_dir: Path, processes: int = 16) -> Path:
     """Gets all audio files in the given directory.
 
     Args:
         root_dir: The root directory.
         extensions: The file extensions to look for.
         processes: The number of processes to use.
 
     Returns:
         A list of files (relative to the root directory).
     """
     cache_path = (root_dir / ".audio_files_cache").resolve()
 
     if cache_path.exists():
-        with Timer("reading cached audio files", spinner=True), open(cache_path, "r", encoding="utf-8") as f:
-            return [AudioFile.parse(line) for line in f]
+        with Timer("reading cached audio files", spinner=True):
+            return cache_path
 
     logger.info("Caching audio files to %s", cache_path)
     audio_files: list[AudioFile] = []
 
     with Timer("listing files", spinner=True):
         files = [f for f in root_dir.rglob("*.*") if f.suffix.lower() in AUDIO_FILE_EXTENSIONS]
         assert files, f"No files found in {root_dir}!"
@@ -567,38 +611,85 @@
             audio_file.path = audio_file.path.relative_to(root_dir)
             audio_files.append(audio_file)
 
     with Timer("writing cached audio files", spinner=True), open(cache_path, "w", encoding="utf-8") as f:
         for audio_file in audio_files:
             f.write(f"{audio_file}\n")
 
-    return audio_files
+    return cache_path
+
+
+def get_files_cached(root_dir: Path, processes: int = 16) -> AudioFileCache:
+    cache_path = get_files_cached_path(root_dir, processes=processes)
+
+    props_path = root_dir / ".audio_files_props"
+    if not props_path.exists():
+        with Timer("getting offsets", spinner=True):
+            offsets = [0]
+            props: list[AudioProps] = []
+
+            with open(cache_path, "r", encoding="utf-8") as f:
+                line = f.readline()
+                while line:
+                    props.append(AudioFile.parse(line).props)
+                    offsets.append(f.tell())
+                    line = f.readline()
+
+            lengths = [offsets[i + 1] - offsets[i] for i in range(len(offsets) - 1)]
+            assert len(lengths) == len(props)
+
+        with Timer("writing props file", spinner=True):
+            sample_rates = [p.sample_rate for p in props]
+            channels = [p.channels for p in props]
+            num_frames = [p.num_frames for p in props]
+            num_tokens = max(*lengths, *sample_rates, *channels, *num_frames) + 1
+
+            with TokenWriter(props_path, num_tokens=num_tokens) as tw:
+                tw.write(sample_rates)
+                tw.write(channels)
+                tw.write(num_frames)
+                tw.write(lengths)
+
+    return AudioFileCache(cache_path, props_path)
 
 
 class AudioFolderFilesDataset(Dataset[tuple[AudioFile, Path]]):
     def __init__(
         self,
         root_dir: str | Path,
         min_frames_quantile: float = 0.01,
         max_frames_quantile: float = 0.99,
     ) -> None:
         super().__init__()
 
         self.root_dir = Path(root_dir).resolve()
-        files = [f for f in get_files_cached(self.root_dir)]
-        lengths = torch.tensor([f.props.num_frames / f.props.sample_rate for f in files])
-        min_length = lengths.quantile(min_frames_quantile)
-        max_length = lengths.quantile(max_frames_quantile)
-        self.files = [f for i, f in enumerate(files) if lengths[i] >= min_length and lengths[i] <= max_length]
+        files = get_files_cached(self.root_dir)
+
+        indices_path = self.root_dir / ".audio_files_indices"
+        if not indices_path.exists():
+            with Timer("filtering indices by length", spinner=True):
+                lengths = torch.tensor([p.num_frames / p.sample_rate for p in files.props])
+                min_length = lengths.quantile(min_frames_quantile)
+                max_length = lengths.quantile(max_frames_quantile)
+                indices = [i for i in range(len(files)) if lengths[i] >= min_length and lengths[i] <= max_length]
+                num_tokens = max(indices) + 1
+
+            with Timer("writing indices file", spinner=True), TokenWriter(indices_path, num_tokens=num_tokens) as tw:
+                for index in indices:
+                    tw.write([index])
+
+        self.files = files
+        self.indices = TokenReader(indices_path, self.root_dir / ".audio_files_indices_offsets")
 
     def __getitem__(self, index: int) -> tuple[AudioFile, Path]:
+        index = self.indices[index][0]
         return self.files[index], self.root_dir
 
     def __len__(self) -> int:
-        return len(self.files)
+        return len(self.indices)
 
 
 class AudioFoldersFilesDataset(ConcatDataset[tuple[AudioFile, Path]]):
     """Defines a dataset for reading audio files from a list of folders.
 
     This dataset just indexes the audio files in some given directories and
     returns some information about them. It is a good idea to use this dataset
@@ -872,41 +963,49 @@
         self.normalize = normalize
         self.num_simultaneous = num_simultaneous
 
         # Indexes the files in the root directory.
         self.files_ds = AudioFolderFilesDataset(root_dir)
         self.audio_ds_queue: Deque[Item] = deque()
 
+        all_indices = list(range(len(self.files_ds)))
+
+        # Filters all indices by length.
+        # props = [self.files_ds[i][0].props for i in all_indices]
+        # lengths = [p.num_frames / p.sample_rate for p in props]
+        # min_length = (length_ms / 1000) * num_samples_per_clip
+        # all_indices = [i for i in all_indices if lengths[i] >= min_length]
+
         # Gets the mapping from the speaker ID to the index.
-        speakers = [self.get_speaker(*self.files_ds[i]) for i in range(len(self.files_ds))]
-        speaker_to_id: dict[SpeakerT, int] = {s: i for i, s in enumerate(sorted(set(speakers)))}
+        speakers = {i: self.get_speaker(i) for i in all_indices}
+        speaker_to_id: dict[SpeakerT, int] = {s: i for i, s in enumerate(sorted(set(speakers.values())))}
 
         # Filters the file dataset indices to only some subset.
-        all_indices = list(range(len(self.files_ds)))
         if specific_speakers is not None and top_n_speakers is not None:
             raise ValueError("Cannot specify both `specific_speakers` and `top_n_speakers`.")
         if top_n_speakers is not None:
-            speaker_counts = Counter(speakers)
+            speaker_counts = Counter(speakers.values())
             specific_speakers = [s for s, _ in speaker_counts.most_common(top_n_speakers)]
         if specific_speakers is not None:
             speaker_set = set(specific_speakers)
             all_indices = [i for i in all_indices if speakers[i] in speaker_set]
             speaker_to_id = {s: i for i, s in enumerate(sorted(specific_speakers))}
 
         self.indices = self.all_indices = all_indices
         self.speaker_to_id: dict[SpeakerT, int] = speaker_to_id
 
     @abstractmethod
-    def get_speaker(self, audio_file: AudioFile, root_dir: Path) -> SpeakerT:
+    def get_speaker(self, index: int) -> SpeakerT:
         """Returns the speaker for a given audio file.
 
+        You can access the current file with ``self.files_ds[index]``. This is
+        avoided in the function signature for performance reasons.
+
         Args:
-            audio_file: The audio file relative to the root directory, with
-                its associated properties.
-            root_dir: The root directory of the dataset.
+            index: The index of the audio file.
 
         Returns:
             The speaker identifier.
         """
 
     def num_speakers(self) -> int:
         return len(self.speaker_to_id)
@@ -918,15 +1017,15 @@
             audio_file=root_dir / audio_file.path,
             sample_rate=self.sample_rate,
             length_ms=self.length_ms,
             num_samples_per_clip=self.num_samples_per_clip,
             max_iters=self.max_iters,
         )
 
-        speaker = self.get_speaker(audio_file, root_dir)
+        speaker = self.get_speaker(index)
         speaker_id = self.speaker_to_id[speaker]
 
         return Item(
             index=index,
             audio_path=audio_file.path,
             speaker_id=speaker_id,
             iterator=iter(ds),
@@ -985,14 +1084,17 @@
 
         self._datasets = list(datasets)
         self._num_speakers = [ds.num_speakers() for ds in self._datasets]
         self._speaker_offset = [0] + list(itertools.accumulate(self._num_speakers))[:-1]
 
         self.finish_all = finish_all
 
+    def num_speakers(self) -> int:
+        return sum(self._num_speakers)
+
     def __iter__(self) -> Iterator[tuple[Tensor, int]]:
         self.iterators = [iter(ds) for ds in self._datasets]
         return self
 
     def __next__(self) -> tuple[Tensor, int]:
         if not self.iterators:
             raise StopIteration
```

### Comparing `ml-starter-0.1.40/ml/utils/augmentation.py` & `ml-starter-0.1.41/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/caching.py` & `ml-starter-0.1.41/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/checkpoint.py` & `ml-starter-0.1.41/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/cli.py` & `ml-starter-0.1.41/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/colors.py` & `ml-starter-0.1.41/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/containers.py` & `ml-starter-0.1.41/ml/utils/containers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/data.py` & `ml-starter-0.1.41/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/datetime.py` & `ml-starter-0.1.41/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/device/auto.py` & `ml-starter-0.1.41/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/device/base.py` & `ml-starter-0.1.41/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/device/cpu.py` & `ml-starter-0.1.41/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/device/gpu.py` & `ml-starter-0.1.41/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/device/metal.py` & `ml-starter-0.1.41/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/distributed.py` & `ml-starter-0.1.41/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/exceptions.py` & `ml-starter-0.1.41/ml/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/image.py` & `ml-starter-0.1.41/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/io.py` & `ml-starter-0.1.41/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/large_models.py` & `ml-starter-0.1.41/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/logging.py` & `ml-starter-0.1.41/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/meter.py` & `ml-starter-0.1.41/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/mixed_precision.py` & `ml-starter-0.1.41/ml/utils/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/networking.py` & `ml-starter-0.1.41/ml/utils/networking.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/numpy.py` & `ml-starter-0.1.41/ml/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/parallel.py` & `ml-starter-0.1.41/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/spectrogram.py` & `ml-starter-0.1.41/ml/utils/spectrogram.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/staging.py` & `ml-starter-0.1.41/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/testing.py` & `ml-starter-0.1.41/ml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/timer.py` & `ml-starter-0.1.41/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/tokens.py` & `ml-starter-0.1.41/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/torch_distributed.py` & `ml-starter-0.1.41/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/triton/kmeans.py` & `ml-starter-0.1.41/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/triton/lion.py` & `ml-starter-0.1.41/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml/utils/video.py` & `ml-starter-0.1.41/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.41/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.40
+Version: 0.1.41
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.40/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.41/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/pyproject.toml` & `ml-starter-0.1.41/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.40/setup.py` & `ml-starter-0.1.41/setup.py`

 * *Files identical despite different names*

