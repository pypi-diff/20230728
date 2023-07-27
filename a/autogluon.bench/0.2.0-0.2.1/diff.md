# Comparing `tmp/autogluon.bench-0.2.0.tar.gz` & `tmp/autogluon.bench-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.bench-0.2.0.tar", last modified: Thu Jul 13 21:28:23 2023, max compression
+gzip compressed data, was "autogluon.bench-0.2.1.tar", last modified: Thu Jul 27 22:25:26 2023, max compression
```

## Comparing `autogluon.bench-0.2.0.tar` & `autogluon.bench-0.2.1.tar`

### file list

```diff
@@ -1,127 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/.github/workflows/continuous_integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/.github/workflows/pypi_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26736 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12290 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/sample_configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/sample_configs/multimodal_cloud_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/sample_configs/multimodal_local_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/sample_configs/tabular_cloud_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/sample_configs/tabular_local_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.910014 autogluon.bench-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.910014 autogluon.bench-0.2.0/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/src/autogluon/bench/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/src/autogluon/bench/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/default_config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1803 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/deploy.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/destroy.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/docker/entrypoint.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/docker/gpu_utilization.sh
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/stack_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/datasets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/datasets/dataset_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    20034 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/datasets/multimodal_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/datasets/object_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/datasets/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/eval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/eval/aggregate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/aggregate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/aggregate/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/eval/benchmark_context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/benchmark_context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/benchmark_context/output_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/benchmark_context/output_suite_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/benchmark_context/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/benchmark_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/evaluate_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/evaluate_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/metadata/metadata_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1441 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/metadata/metadata_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/preprocess/preprocess_openml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/preprocess/preprocess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/eval/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/scripts/aggregate_amlb_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    15468 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/scripts/run_evaluation_openml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/scripts/run_generate_clean_openml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/multimodal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/multimodal/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1358 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/multimodal/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/tabular/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      750 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/tabular/exec.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      464 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/tabular/setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/runbenchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/src/autogluon/bench/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/scripts/generate_cloud_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/src/autogluon/bench/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/utils/general_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 21:28:23.000000 autogluon.bench-0.2.0/src/autogluon/bench/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/src/autogluon.bench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26736 2023-07-13 21:28:23.000000 autogluon.bench-0.2.0/src/autogluon.bench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-07-13 21:28:23.000000 autogluon.bench-0.2.0/src/autogluon.bench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 21:28:23.000000 autogluon.bench-0.2.0/src/autogluon.bench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 21:28:23.000000 autogluon.bench-0.2.0/src/autogluon.bench.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-13 21:28:23.000000 autogluon.bench-0.2.0/src/autogluon.bench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 21:28:23.000000 autogluon.bench-0.2.0/src/autogluon.bench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.910014 autogluon.bench-0.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.910014 autogluon.bench-0.2.0/tests/unittests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/tests/unittests/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/benchmark/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/benchmark/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/benchmark/test_runbenchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.910014 autogluon.bench-0.2.0/tests/unittests/cloud/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/tests/unittests/cloud/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/cloud/aws/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/cloud/aws/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/cloud/aws/test_stack_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/tests/unittests/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/datasets/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/datasets/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/.github/workflows/continuous_integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/.github/workflows/pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27613 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/sample_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/sample_configs/amlb_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/amlb_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/amlb_configs/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/amlb_configs/constraints.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/amlb_configs/frameworks_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/multimodal_cloud_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/multimodal_local_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/tabular_cloud_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/tabular_local_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.252851 autogluon.bench-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/constructs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/lambdas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/lambdas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/lambdas/amlb_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/lambdas/amlb_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18378 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/lambdas/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/default_config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1803 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/deploy.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/destroy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/stack_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/src/autogluon/bench/custom_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/custom_configs/amlb_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/custom_configs/amlb_configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/datasets/dataset_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20034 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/datasets/multimodal_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/datasets/object_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/datasets/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/eval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/eval/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/aggregate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/aggregate/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/eval/benchmark_context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/benchmark_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/benchmark_context/output_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/benchmark_context/output_suite_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/benchmark_context/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/benchmark_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/evaluate_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/evaluate_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/metadata/metadata_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1441 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/metadata/metadata_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/preprocess/preprocess_openml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/preprocess/preprocess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/aggregate_amlb_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15468 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/run_evaluation_openml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/run_generate_clean_openml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/multimodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/multimodal/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1698 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/multimodal/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/tabular/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/tabular/exec.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      928 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/tabular/setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17422 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/runbenchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/src/autogluon/bench/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/scripts/generate_cloud_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/src/autogluon/bench/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/utils/general_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/utils/gpu_utilization.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 22:25:26.000000 autogluon.bench-0.2.1/src/autogluon/bench/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon.bench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27613 2023-07-27 22:25:26.000000 autogluon.bench-0.2.1/src/autogluon.bench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-27 22:25:26.000000 autogluon.bench-0.2.1/src/autogluon.bench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:25:26.000000 autogluon.bench-0.2.1/src/autogluon.bench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 22:25:26.000000 autogluon.bench-0.2.1/src/autogluon.bench.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-27 22:25:26.000000 autogluon.bench-0.2.1/src/autogluon.bench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 22:25:26.000000 autogluon.bench-0.2.1/src/autogluon.bench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/tests/unittests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/tests/unittests/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/benchmark/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/benchmark/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/benchmark/test_runbenchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/tests/unittests/cloud/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/tests/unittests/cloud/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/cloud/aws/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/cloud/aws/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/cloud/aws/test_stack_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/tests/unittests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/datasets/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/tests/unittests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/utils/test_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/utils/test_general_utils.py
```

### Comparing `autogluon.bench-0.2.0/.github/workflows/continuous_integration.yml` & `autogluon.bench-0.2.1/.github/workflows/continuous_integration.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 
 jobs:
   lint_check:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout repository
         uses: actions/checkout@v3
-      - name: Set up Python 3.8
+      - name: Set up Python 3.9
         uses: actions/setup-python@v4
         with:
-          python-version: '3.8'
+          python-version: '3.9'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install tox
       - name: Lint Check
         run: tox -e lint
   
   run_tests:
     needs: lint_check
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.9", "3.10"]
 
     steps:
       - name: Checkout repository
         uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
```

### Comparing `autogluon.bench-0.2.0/.github/workflows/pypi_release.yml` & `autogluon.bench-0.2.1/.github/workflows/pypi_release.yml`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/.gitignore` & `autogluon.bench-0.2.1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+# hidden directories
+.*/
+
 AutogluonModels
-.ag_bench_runs
+ag_bench_runs
 data
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
```

### Comparing `autogluon.bench-0.2.0/LICENSE` & `autogluon.bench-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/PKG-INFO` & `autogluon.bench-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.bench
-Version: 0.2.0
+Version: 0.2.1
 Summary: A benchmarking tool for AutoML
 Author: AutoGluon Community
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -217,22 +217,21 @@
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Requires-Python: <3.11,>=3.8
+Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 <div align="left">
   <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
 </div>
@@ -267,15 +266,15 @@
 # install from source in editable mode
 pip install -e ".[tests]"
 ```
 
 For development, please be aware that `autogluon.bench` is installed as a dependency in certain places, such as the [Dockerfile](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/Dockerfile) and [Multimodal Setup](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/frameworks/multimodal/setup.sh). We made it possible to reflect the development changes by pushing the changes to a remote GitHub branch, and providing the URI when testing on benchmark runs:
 
 ```
-agbench run sample_configs/multimodal_cloud_configs.yaml --dev-branch https://github.com/suzhoum/autogluon-bench.git\#add_dev_branch
+agbench run sample_configs/multimodal_cloud_configs.yaml --dev-branch https://github.com/<username>/autogluon-bench.git#<dev_branch>
 ```
 
 
 ## Run benchmarks locally
 
 To run the benchmarks on your local machine, use the following command:
 
@@ -286,19 +285,26 @@
 Check out our [sample local configuration files](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs) for local runs.
 
 The results are stored in the following directory: `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}`.
 
 
 ### Tabular Benchmark
 
-To perform tabular benchmarking, set the module to tabular. You must set both Benchmark Configurations and Tabular Specific configurations, and each should have a single value. Refer to the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for more details.
+To perform tabular benchmarking, set the module to tabular. You must set both Benchmark Configurations and Tabular Specific configurations, and each should have a single value. Refer to the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/tabluar_local_configs.yaml) for more details.
 
 The tabular module leverages the [AMLB](https://github.com/openml/automlbenchmark) benchmarking framework. Required and optional AMLB arguments are specified via the configuration file mentioned previously.
 
-To benchmark a custom branch of AutoGluon on `tabular` module, use `amlb_custom_branch: https://github.com/REPO/autogluon#BRANCH` in the configuration file.
+Custom configuration is supported by providing a local directory to `amlb_user_dir` in the config, by which custom frameworks, constraints and datasets can be overriden. We have a minimum working [custom config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/amlb_configs) setup for benchmarking on a custom framework (a `AutoGluon` dev branch). In the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/tabluar_local_configs.yaml), change the following field to:
+
+```
+framework: AutoGluon_dev:example
+amlb_user_dir: path_to/sample_configs/amlb_configs 
+```
+
+For more customizations, please follow the [example custom configuration folder](https://github.com/openml/automlbenchmark/tree/master/examples/custom) provided by AMLB and their [documentation](https://github.com/openml/automlbenchmark/blob/master/docs/HOWTO.md#custom-configuration). 
 
 
 ### Multimodal Benchmark
 
 For multimodal benchmarking, set the module to multimodal. We currently support benchmarking multimodal on a custom branch. Note that multimodal benchmarking directly calls the MultiModalPredictor, bypassing the extra layer of [AMLB](https://github.com/openml/automlbenchmark). Therefore, the required arguments are different from those for tabular.
 
 You can add more datasets to your benchmarking jobs. We provided sample [multimodal datasets](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/multimodal_dataset.py) and [object detection dataset](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/object_detection_dataset.py). Follow these samples to add custom datasets, then specify dataset_name in your local config file. Please follow the section `Install From Source` for more instructions on how to develop with source.
@@ -307,20 +313,21 @@
 
 AutoGluon-Bench uses the AWS CDK to build an AWS Batch compute environment for benchmarking.
 
 To get started, install [Node.js](https://nodejs.org/) and [AWS CDK](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html#getting_started_install) with the following instructions:
 
 1. Install [Node Version Manager](https://github.com/nvm-sh/nvm#installing-and-updating).
 2. Source profile or restart the terminal.
-3. Follow the `Prerequisites` section on the [AWS CDK Guide](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html) and install an appropriate version for your system:
+3. Follow the `Prerequisites` section on the [AWS CDK Guide](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html) and install an appropriate `Node.js` version for your system:
 ```bash
 nvm install $VERSION  # install Node.js
 npm install -g aws-cdk  # install aws-cdk
 cdk --version  # verify the installation, you might need to update the Node.js version depending on the log.
 ```
+4. Follow the [AWS CLI Installation Guide](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) to install `awscliv2`. 
 
 If it is the first time using CDK to deploy to an AWS environment (An AWS environment is a combination of an AWS account and Region), please run the following:
 
 ```bash
 cdk bootstrap aws://CDK_DEPLOY_ACCOUNT/CDK_DEPLOY_REGION
 ```
```

### Comparing `autogluon.bench-0.2.0/README.md` & `autogluon.bench-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 # install from source in editable mode
 pip install -e ".[tests]"
 ```
 
 For development, please be aware that `autogluon.bench` is installed as a dependency in certain places, such as the [Dockerfile](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/Dockerfile) and [Multimodal Setup](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/frameworks/multimodal/setup.sh). We made it possible to reflect the development changes by pushing the changes to a remote GitHub branch, and providing the URI when testing on benchmark runs:
 
 ```
-agbench run sample_configs/multimodal_cloud_configs.yaml --dev-branch https://github.com/suzhoum/autogluon-bench.git\#add_dev_branch
+agbench run sample_configs/multimodal_cloud_configs.yaml --dev-branch https://github.com/<username>/autogluon-bench.git#<dev_branch>
 ```
 
 
 ## Run benchmarks locally
 
 To run the benchmarks on your local machine, use the following command:
 
@@ -51,19 +51,26 @@
 Check out our [sample local configuration files](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs) for local runs.
 
 The results are stored in the following directory: `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}`.
 
 
 ### Tabular Benchmark
 
-To perform tabular benchmarking, set the module to tabular. You must set both Benchmark Configurations and Tabular Specific configurations, and each should have a single value. Refer to the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for more details.
+To perform tabular benchmarking, set the module to tabular. You must set both Benchmark Configurations and Tabular Specific configurations, and each should have a single value. Refer to the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/tabluar_local_configs.yaml) for more details.
 
 The tabular module leverages the [AMLB](https://github.com/openml/automlbenchmark) benchmarking framework. Required and optional AMLB arguments are specified via the configuration file mentioned previously.
 
-To benchmark a custom branch of AutoGluon on `tabular` module, use `amlb_custom_branch: https://github.com/REPO/autogluon#BRANCH` in the configuration file.
+Custom configuration is supported by providing a local directory to `amlb_user_dir` in the config, by which custom frameworks, constraints and datasets can be overriden. We have a minimum working [custom config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/amlb_configs) setup for benchmarking on a custom framework (a `AutoGluon` dev branch). In the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/tabluar_local_configs.yaml), change the following field to:
+
+```
+framework: AutoGluon_dev:example
+amlb_user_dir: path_to/sample_configs/amlb_configs 
+```
+
+For more customizations, please follow the [example custom configuration folder](https://github.com/openml/automlbenchmark/tree/master/examples/custom) provided by AMLB and their [documentation](https://github.com/openml/automlbenchmark/blob/master/docs/HOWTO.md#custom-configuration). 
 
 
 ### Multimodal Benchmark
 
 For multimodal benchmarking, set the module to multimodal. We currently support benchmarking multimodal on a custom branch. Note that multimodal benchmarking directly calls the MultiModalPredictor, bypassing the extra layer of [AMLB](https://github.com/openml/automlbenchmark). Therefore, the required arguments are different from those for tabular.
 
 You can add more datasets to your benchmarking jobs. We provided sample [multimodal datasets](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/multimodal_dataset.py) and [object detection dataset](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/object_detection_dataset.py). Follow these samples to add custom datasets, then specify dataset_name in your local config file. Please follow the section `Install From Source` for more instructions on how to develop with source.
@@ -72,20 +79,21 @@
 
 AutoGluon-Bench uses the AWS CDK to build an AWS Batch compute environment for benchmarking.
 
 To get started, install [Node.js](https://nodejs.org/) and [AWS CDK](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html#getting_started_install) with the following instructions:
 
 1. Install [Node Version Manager](https://github.com/nvm-sh/nvm#installing-and-updating).
 2. Source profile or restart the terminal.
-3. Follow the `Prerequisites` section on the [AWS CDK Guide](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html) and install an appropriate version for your system:
+3. Follow the `Prerequisites` section on the [AWS CDK Guide](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html) and install an appropriate `Node.js` version for your system:
 ```bash
 nvm install $VERSION  # install Node.js
 npm install -g aws-cdk  # install aws-cdk
 cdk --version  # verify the installation, you might need to update the Node.js version depending on the log.
 ```
+4. Follow the [AWS CLI Installation Guide](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) to install `awscliv2`. 
 
 If it is the first time using CDK to deploy to an AWS environment (An AWS environment is a combination of an AWS account and Region), please run the following:
 
 ```bash
 cdk bootstrap aws://CDK_DEPLOY_ACCOUNT/CDK_DEPLOY_REGION
 ```
```

### Comparing `autogluon.bench-0.2.0/pyproject.toml` & `autogluon.bench-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "autogluon.bench"
 dynamic = ["version"]
 description = "A benchmarking tool for AutoML"
 authors = [{name = "AutoGluon Community"}]
 readme = "README.md"
-requires-python = ">=3.8, <3.11"
+requires-python = ">=3.9, <3.11"
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Education",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Customer Service",
@@ -21,34 +21,34 @@
     "Intended Audience :: Telecommunications Industry",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Software Development",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Image Recognition"
 ]
 dependencies = [
     "autogluon.common >=0.7,<1.0",
     "aws-cdk-lib >=2.0.0,<2.70.0",
     "aws-cdk.aws-batch-alpha >=2.0.0a1,<2.70.0a0",
     "awscliv2 >=2.2.0,<2.3.0",
-    "boto3 >=1.26.0,<1.26.99",
+    "boto3 >=1.26.0,<1.28.0",
     "constructs >=10.0.0,<10.1.289",
     "fsspec >=2023.5.0,<=2023.6.0",
     "matplotlib >=3.4,<3.7",
     "pandas >=1.2.5,<2.0",
+    "pydantic>=1.10.4,<2.0", # https://github.com/ray-project/ray/issues/36990
     "pyyaml >=5.4,<=6.0",
-    "ray >=2.3.0,<2.4.0",
+    "ray[default] >=2.3.0,<2.4.0",
     "s3fs >=2023.5.0,<=2023.6.0",
     "typer >=0.9.0,<1.0.0",
     "wheel >0.38.0,<=0.40.0",
 ]
 
 [project.optional-dependencies]
 tests = ["pytest", "pytest-mock", "tox", "black>=23.1.9, <=23.7.0", "isort>=5.11.0, <=5.12.0"]
@@ -59,15 +59,15 @@
 
 [project.scripts]
 agbench = "autogluon.bench.main:app"
 
 # Testing and formatting configurations
 [tool.black]
 line-length = 119
-target-version = ['py38', 'py39', 'py310']
+target-version = ['py39', 'py310']
 
 [tool.isort]
 known_first_party = "autogluon"
 known_third_party = [
     "numpy",
     "pandas",
     "psutil",
@@ -78,15 +78,15 @@
 line_length = 119
 profile = "black"
 
 [tool.tox]
 legacy_tox_ini = """
     [tox]
     min_version = 4.0
-    envlist = py38, py39, py310
+    envlist = py39, py310
     isolated_build = True
 
     [testenv]
     deps = 
         pytest
         pytest-mock
     commands = pytest
```

### Comparing `autogluon.bench-0.2.0/sample_configs/multimodal_cloud_configs.yaml` & `autogluon.bench-0.2.1/sample_configs/multimodal_cloud_configs.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   # INSTANCE: g4dn.2xlarge  # optional
   # VPC_NAME: existing-vpc-name  # optional
 
 # Benchmark configurations
 module: multimodal  # required
 mode: aws  # required
 benchmark_name: ag_bench  # required
-root_dir: .ag_bench_runs  # optional, default = ".ag_bench_runs"
+root_dir: ag_bench_runs  # optional, default = "ag_bench_runs"
 
 module_configs:
   # Multimodal specific
   multimodal:
     git_uri#branch: # required
       - https://github.com/autogluon/autogluon#master
     dataset_name:  # required
```

### Comparing `autogluon.bench-0.2.0/sample_configs/multimodal_local_configs.yaml` & `autogluon.bench-0.2.1/sample_configs/multimodal_local_configs.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Benchmark configurations
 module: multimodal  # required
 mode: local  # required
 benchmark_name: ag_bench  # required
-root_dir: .ag_bench_runs  # optional, default = ".ag_bench_runs"
+root_dir: ag_bench_runs  # optional, default = "ag_bench_runs"
 # METRICS_BUCKET: autogluon-benchmark-metrics  # optional, required only if you want to upload metrics to S3
 
 # Multimodal specific
 git_uri#branch: https://github.com/autogluon/autogluon#master  # required
 dataset_name: melbourne_airbnb  # required
 presets: medium_quality  # optional
 hyperparameters:  # optional
```

### Comparing `autogluon.bench-0.2.0/sample_configs/tabular_cloud_configs.yaml` & `autogluon.bench-0.2.1/sample_configs/tabular_cloud_configs.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -10,27 +10,32 @@
   # RESERVED_MEMORY_SIZE: 15000  # optional
   # INSTANCE: g4dn.2xlarge  # optional
 
 # Benchmark configurations
 module: tabular  # required
 mode: aws  # required
 benchmark_name: ag_bench  # required
-root_dir: .ag_bench_runs  # optional, default = ".ag_bench_runs"
+root_dir: ag_bench_runs  # optional, default = "ag_bench_runs"
 
 module_configs:
   # Tabular specific
   # You can refer to AMLB (https://github.com/openml/automlbenchmark#quickstart) for more details
   tabular:
-    framework:  # either framework or amlb_custom_branch is required
+    git_uri#branch:  # required, can be any AMLB custom fork and branch, only one value allowed
+      - https://github.com/openml/automlbenchmark.git#master
+    framework:  # required, only one value allowed
       - AutoGluon:stable
     amlb_benchmark:  # required, each benchmark contains a list of datasets, can be subsetted by amlb_task below
-      - test
       - small
     amlb_task:  # optional, value of each key is a subset of dataset names in each 'amlb_benchmark'
-      test: null
       small:
         - credit-g
         - vehicle
-    amlb_constraint:  # optional
+    amlb_constraint:  # optional, only one value allowed
       - test
-    # amlb_custom_branch: 
-    #   - https://github.com/<ACCOUNT>/autogluon#<CUSTOM_BRANCH>  # optional, `framework` is overwritten when this is specified 
+    # fold_to_run:  # optional, capped by `folds` in amlb_constraint
+    #   small:
+    #     credit-g:
+    #       - 3
+    #       - 6
+    # amlb_user_dir:  # optional, local/s3 path where all the amlb customizations are stored, only one value allowed
+    #   - sample_configs/amlb_configs
```

### Comparing `autogluon.bench-0.2.0/sample_configs/tabular_local_configs.yaml` & `autogluon.bench-0.2.1/sample_configs/tabular_local_configs.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Benchmark configurations
 module: tabular  # required
 mode: local  # required
 benchmark_name: ag_bench  # required
-root_dir: .ag_bench_runs  # optional, default = ".ag_bench_runs"
+root_dir: ag_bench_runs  # optional, default = "ag_bench_runs"
 # METRICS_BUCKET: autogluon-benchmark-metrics  # optional, required only if you want to upload metrics to S3
 
 # Tabular specific
+git_uri#branch: https://github.com/openml/automlbenchmark.git#stable  # required, can be any AMLB custom fork and branch
 framework: AutoGluon:stable  # required
-amlb_benchmark: test  # optional
-amlb_task:   # optional
+amlb_benchmark: small  # required
+amlb_task: vehicle # optional
 amlb_constraint: test  # optional
-# amlb_custom_branch: https://github.com/<ACCOUNT>/autogluon#<CUSTOM_BRANCH>  # optional, `framework` and `label` are overwritten when this is specified 
+fold_to_run: 1  # optional, the specific data fold to run
+amlb_user_dir: sample_configs/amlb_configs  # optional, local/s3 path where all the amlb customizations are stored
```

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/app.py` & `autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/app.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py` & `autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py` & `autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/stack.py` & `autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from autogluon.bench.cloud.aws.batch_stack.constructs.instance_profile import InstanceProfile
 
 """
 Sample CDK code for creating the required infrastructure for running a AWS Batch job.
 AWS Batch as the compute enviroment in which a docker image runs the benchmarking script.
 """
 
-with importlib.resources.path("autogluon.bench.cloud.aws.docker", "Dockerfile") as file_path:
+with importlib.resources.path("autogluon.bench", "Dockerfile") as file_path:
     docker_base_dir = os.path.dirname(file_path)
 
 with importlib.resources.path("autogluon.bench.cloud.aws.batch_stack.lambdas", "lambda_function.py") as file_path:
     lambda_script_dir = os.path.dirname(file_path)
 
 logger = logging.getLogger(__name__)
 
@@ -161,14 +161,20 @@
             f"{prefix}-ecr-docker-image-asset",
             directory=docker_base_dir,
             follow_symlinks=core.SymlinkFollowMode.ALWAYS,
             build_args={
                 "AG_BENCH_VERSION": os.getenv("AG_BENCH_VERSION", "latest"),
                 "AG_BENCH_DEV_URL": os.getenv("AG_BENCH_DEV_URL", ""),
                 "CDK_DEPLOY_REGION": os.environ["CDK_DEPLOY_REGION"],
+                "FRAMEWORK_PATH": os.environ["FRAMEWORK_PATH"],
+                "GIT_URI": os.environ["GIT_URI"],
+                "GIT_BRANCH": os.environ["GIT_BRANCH"],
+                "BENCHMARK_DIR": os.environ["BENCHMARK_DIR"],
+                "AMLB_FRAMEWORK": os.getenv("AMLB_FRAMEWORK", ""),
+                "AMLB_USER_DIR": os.getenv("AMLB_USER_DIR", ""),
             },
         )
 
         docker_container_image = ecs.ContainerImage.from_docker_image_asset(docker_image_asset)
 
         container = batch.JobDefinitionContainer(
             image=docker_container_image,
```

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/deploy.sh` & `autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/deploy.sh`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/destroy.sh` & `autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/destroy.sh`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/docker/gpu_utilization.sh` & `autogluon.bench-0.2.1/src/autogluon/bench/utils/gpu_utilization.sh`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/stack_handler.py` & `autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/stack_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,28 +114,28 @@
     Args:
         configs (dict, optional): A dictionary containing custom configuration settings. Defaults to None.
 
     Returns:
         dict: A dictionary containing the CDK context settings used for the deployment.
     """
     cdk_path = _get_temp_cdk_app_path()
-    infra_configs = construct_context(custom_configs=custom_configs)
+    custom_infra_configs = custom_configs.get("cdk_context", {})
+    infra_configs = construct_context(custom_configs=custom_infra_configs)
+    command = [
+        os.path.join(module_base_dir, "deploy.sh"),
+        infra_configs["STACK_NAME_PREFIX"],
+        infra_configs["STACK_NAME_TAG"],
+        infra_configs["STATIC_RESOURCE_STACK_NAME"],
+        infra_configs["BATCH_STACK_NAME"],
+        str(infra_configs["CONTAINER_MEMORY"]),
+        infra_configs["CDK_DEPLOY_REGION"],
+        cdk_path,
+    ]
 
-    subprocess.check_call(
-        [
-            os.path.join(module_base_dir, "deploy.sh"),
-            infra_configs["STACK_NAME_PREFIX"],
-            infra_configs["STACK_NAME_TAG"],
-            infra_configs["STATIC_RESOURCE_STACK_NAME"],
-            infra_configs["BATCH_STACK_NAME"],
-            str(infra_configs["CONTAINER_MEMORY"]),
-            infra_configs["CDK_DEPLOY_REGION"],
-            cdk_path,
-        ]
-    )
+    subprocess.check_call(command)
     shutil.rmtree(os.path.dirname(cdk_path))
 
     return infra_configs
 
 
 @app.command()
 def destroy_stack(
```

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/datasets/multimodal_dataset.py` & `autogluon.bench-0.2.1/src/autogluon/bench/datasets/multimodal_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/datasets/object_detection_dataset.py` & `autogluon.bench-0.2.1/src/autogluon/bench/datasets/object_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/datasets/registry.py` & `autogluon.bench-0.2.1/src/autogluon/bench/datasets/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/eval/aggregate/results.py` & `autogluon.bench-0.2.1/src/autogluon/bench/eval/aggregate/results.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/eval/benchmark_context/output_context.py` & `autogluon.bench-0.2.1/src/autogluon/bench/eval/benchmark_context/output_context.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/eval/benchmark_context/output_suite_context.py` & `autogluon.bench-0.2.1/src/autogluon/bench/eval/benchmark_context/output_suite_context.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/benchmark_evaluator.py` & `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/benchmark_evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/constants.py` & `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/evaluate_results.py` & `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/evaluate_results.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/evaluate_utils.py` & `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/evaluate_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/metadata/metadata_generator.py` & `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/metadata/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/metadata/metadata_loader.py` & `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/preprocess/preprocess_openml.py` & `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/preprocess/preprocess_openml.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/preprocess/preprocess_utils.py` & `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/preprocess/preprocess_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/eval/scripts/aggregate_amlb_results.py` & `autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/aggregate_amlb_results.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/eval/scripts/run_evaluation_openml.py` & `autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/run_evaluation_openml.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/eval/scripts/run_generate_clean_openml.py` & `autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/run_generate_clean_openml.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/frameworks/benchmark.py` & `autogluon.bench-0.2.1/src/autogluon/bench/frameworks/benchmark.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/frameworks/multimodal/exec.py` & `autogluon.bench-0.2.1/src/autogluon/bench/frameworks/multimodal/exec.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py` & `autogluon.bench-0.2.1/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,18 +45,16 @@
         command = [setup_script_path, git_uri, git_branch, self.benchmark_dir]
         if agbench_dev_url is not None:
             command.append(f"--AGBENCH_DEV_URL={agbench_dev_url}")
         else:
             command.append(f"--AG_BENCH_VER={agbench_version}")
         result = subprocess.run(command)
         if result.returncode != 0:
-            logger.error(result.stderr)
             sys.exit(1)
         else:
-            logger.info(result.stdout)
             logger.info("Successfully set up the environment under %s/.venv.", self.benchmark_dir)
 
     def run(
         self,
         dataset_name: str,
         framework: str,
         presets: Optional[str] = None,
@@ -94,12 +92,10 @@
             command += ["--presets", presets]
         if hyperparameters is not None:
             command += ["--hyperparameters", json.dumps(hyperparameters)]
         if time_limit is not None:
             command += ["--time_limit", str(time_limit)]
         result = subprocess.run(command)
         if result.returncode != 0:
-            logger.error(result.stderr)
             sys.exit(1)
         else:
-            logger.info(result.stdout)
             logger.info(f"Benchmark {self.benchmark_name} on dataset {dataset_name} is complete.")
```

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py` & `autogluon.bench-0.2.1/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,78 @@
 import logging
 import os
 import subprocess
 import sys
 from typing import List
 
-import yaml
-
 from autogluon.bench.frameworks.benchmark import Benchmark
 
 logger = logging.getLogger(__name__)
 
 
 class TabularBenchmark(Benchmark):
     def setup(
         self,
+        git_uri: str = "https://github.com/openml/automlbenchmark.git",
+        git_branch: str = "stable",
+        framework: str = "AutoGluon:stable",
+        user_dir: str = None,
     ):
         """Sets up the virtual environment for tabular benchmark."""
         setup_script_path = os.path.abspath(os.path.dirname(__file__)) + "/setup.sh"
-        command = [setup_script_path, self.benchmark_dir]
+        command = [setup_script_path, git_uri, git_branch, self.benchmark_dir, framework]
+        if user_dir is not None:
+            command.append(user_dir)
         result = subprocess.run(command)
         if result.returncode != 0:
             logger.error(result.stderr)
             sys.exit(1)
         else:
             logger.info(result.stdout)
             logger.info("Successfully set up the environment under %s/.venv.", self.benchmark_dir)
 
     def run(
         self,
-        benchmark: str = "test",
-        constraint: str = "test",
-        task: List[str] = None,
-        framework: str = None,
-        custom_branch: str = None,
+        framework: str,
+        benchmark: str,
+        constraint: str,
+        task: str = None,
+        fold: int = None,
+        user_dir: str = None,
     ):
         """Runs the tabular benchmark.
 
         Args:
             benchmark (str): The name of the benchmark to run (default: "test").
             constraint (str): The name of the constraint to use (default: "test").
             task (List[str]): The name of the task to run (default: None).
             framework (str): The name of the framework to use (default: None). Examples: "AutoGluon:latest", "AutoGluon:stable".
-            custom_branch (str): The name of the custom branch to use (default: None).
+            user_dir (str): Path to custom configs to use (default: None).
 
         Returns:
             None
         """
-        if framework is None and custom_branch is None:
-            raise KeyError("Either 'framework' or 'custom_branch' should be provided.")
-
-        custom_branch_dir = None
-        if custom_branch is not None:
-            custom_repo, custom_branch_name = tuple(custom_branch.split("#"))
-            custom_branch_dir = self.benchmark_dir
-
-            framework = "AutoGluon_dev"
-
-            custom_config_contents = {
-                "frameworks": {
-                    "definition_file": ["{root}/resources/frameworks.yaml", "{user}/frameworks.yaml"],
-                    "allow_duplicates": "true",
-                }
-            }
-
-            with open(os.path.join(custom_branch_dir, "amlb_configs.yaml"), "w") as fo:
-                yaml.dump(custom_config_contents, fo)
-
-            custom_framework_contents = {
-                framework: {"extends": "AutoGluon", "repo": custom_repo, "version": custom_branch_name}
-            }
-
-            with open(os.path.join(custom_branch_dir, "frameworks.yaml"), "w") as fo:
-                yaml.dump(custom_framework_contents, fo)
 
         exec_script_path = os.path.abspath(os.path.dirname(__file__)) + "/exec.sh"
         command = [
             exec_script_path,
             framework,
             benchmark,
             constraint,
             self.benchmark_dir,
             self.metrics_dir,
         ]
 
-        if custom_branch_dir is not None:
-            command += ["-c", custom_branch_dir]
-
         if task is not None:
-            command += ["-t", " ".join(task)]
+            command += ["-t", task]
+
+        if fold is not None:
+            command += ["-f", str(fold)]
+
+        if user_dir is not None:
+            command += ["-u", user_dir]
 
         result = subprocess.run(command)
         if result.returncode != 0:
-            logger.error(result.stderr)
             sys.exit(1)
         else:
-            logger.info(result.stdout)
             logger.info(f"Benchmark {self.benchmark_name} is complete.")
```

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/main.py` & `autogluon.bench-0.2.1/src/autogluon/bench/main.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/runbenchmark.py` & `autogluon.bench-0.2.1/src/autogluon/bench/runbenchmark.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import json
 import logging
 import os
 import re
+import subprocess
+import tempfile
 import time
 from typing import List, Optional
 
 import boto3
 import botocore
 import typer
 import yaml
 
 from autogluon.bench import __version__ as agbench_version
 from autogluon.bench.cloud.aws.stack_handler import deploy_stack, destroy_stack
 from autogluon.bench.frameworks.multimodal.multimodal_benchmark import MultiModalBenchmark
 from autogluon.bench.frameworks.tabular.tabular_benchmark import TabularBenchmark
-from autogluon.bench.utils.general_utils import formatted_time
+from autogluon.bench.utils.general_utils import (
+    download_dir_from_s3,
+    download_file_from_s3,
+    formatted_time,
+    upload_to_s3,
+)
 
 app = typer.Typer()
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
@@ -28,17 +35,16 @@
     Args:
         module (str): The name of the module to benchmark (either "multimodal" or "tabular").
         configs (dict): A dictionary of configuration options for the benchmark.
 
     Returns:
         A dictionary containing the keyword arguments to be used for setting up and running the benchmark.
     """
-
+    git_uri, git_branch = _get_git_info(configs["git_uri#branch"])
     if module == "multimodal":
-        git_uri, git_branch = configs["git_uri#branch"].split("#")
         return {
             "setup_kwargs": {
                 "git_uri": git_uri,
                 "git_branch": git_branch,
                 "agbench_dev_url": agbench_dev_url,
             },
             "run_kwargs": {
@@ -47,32 +53,45 @@
                 "presets": configs.get("presets"),
                 "hyperparameters": configs.get("hyperparameters"),
                 "time_limit": configs.get("time_limit"),
             },
         }
     elif module == "tabular":
         return {
-            "setup_kwargs": {},
+            "setup_kwargs": {
+                "git_uri": git_uri,
+                "git_branch": git_branch,
+                "framework": configs["framework"],
+                "user_dir": configs.get("amlb_user_dir"),
+            },
             "run_kwargs": {
-                "benchmark": configs["amlb_benchmark"],
-                "constraint": configs["amlb_constraint"],
-                "task": configs.get("amlb_task") if configs.get("amlb_task") else None,
-                "framework": configs.get("framework"),
-                "custom_branch": configs.get("amlb_custom_branch"),
+                "framework": configs["framework"],
+                "benchmark": configs.get("amlb_benchmark", "test"),
+                "constraint": configs.get("amlb_constraint", "test"),
+                "task": configs.get("amlb_task"),
+                "fold": configs.get("fold_to_run"),
+                "user_dir": configs.get("amlb_user_dir"),
             },
         }
 
 
 def _get_benchmark_name(configs: dict) -> str:
     default_benchmark_name = "ag_bench"
     benchmark_name = configs.get("benchmark_name", default_benchmark_name) or default_benchmark_name
     return benchmark_name
 
 
-def run_benchmark(benchmark_name: str, benchmark_dir: str, configs: dict, agbench_dev_url: str = None):
+def run_benchmark(
+    benchmark_name: str,
+    benchmark_dir: str,
+    configs: dict,
+    benchmark_dir_s3: str = None,
+    agbench_dev_url: str = None,
+    skip_setup: str = False,
+):
     """Runs a benchmark based on the provided configuration options.
 
     Args:
         configs (dict): A dictionary of configuration options for the benchmark.
 
     Returns:
         None
@@ -87,61 +106,23 @@
     benchmark_class = module_to_benchmark.get(module_name, None)
     if benchmark_class is None:
         raise NotImplementedError
 
     benchmark = benchmark_class(benchmark_name=benchmark_name, benchmark_dir=benchmark_dir)
 
     module_kwargs = get_kwargs(module=module_name, configs=configs, agbench_dev_url=agbench_dev_url)
-    benchmark.setup(**module_kwargs.get("setup_kwargs", {}))
-    benchmark.run(**module_kwargs.get("run_kwargs", {}))
+    if not skip_setup:
+        benchmark.setup(**module_kwargs["setup_kwargs"])
+
+    benchmark.run(**module_kwargs["run_kwargs"])
     logger.info(f"Backing up benchmarking configs to {benchmark.metrics_dir}/configs.yaml")
     _dump_configs(benchmark_dir=benchmark.metrics_dir, configs=configs, file_name="configs.yaml")
 
     if configs.get("METRICS_BUCKET", None):
-        s3_dir = f"{module_name}{benchmark_dir.split(module_name, 1)[-1]}"
-        benchmark.upload_metrics(s3_bucket=configs["METRICS_BUCKET"], s3_dir=s3_dir)
-
-
-def upload_config(bucket: str, benchmark_name: str, file: str):
-    """Uploads a configuration file to an S3 bucket.
-
-    Args:
-        bucket (str): The name of the S3 bucket to upload the file to.
-        file (str): The path to the local file to upload.
-
-    Returns:
-        The S3 path of the uploaded file.
-    """
-    s3 = boto3.client("s3")
-    config_file_name = os.path.basename(file)
-    file_name = benchmark_name + "_" + config_file_name
-
-    s3_path = f"configs/{file_name}"
-    s3.upload_file(file, bucket, s3_path)
-    logger.info(f"Config file has been uploaded to S3://{bucket}/{s3_path}")
-    return f"s3://{bucket}/{s3_path}"
-
-
-def download_config(s3_path: str, dir: str = "/tmp"):
-    """Downloads a configuration file from an S3 bucket.
-
-    Args:
-        s3_path (str): The S3 path of the file to download.
-        dir (str): The local directory to download the file to (default: "/tmp").
-
-    Returns:
-        The local path of the downloaded file.
-    """
-
-    s3 = boto3.client("s3")
-    file_path = os.path.join(dir, s3_path.split("/")[-1])
-    bucket = s3_path.strip("s3://").split("/")[0]
-    s3_path = s3_path.split(bucket)[-1].lstrip("/")
-    s3.download_file(bucket, s3_path, file_path)
-    return file_path
+        benchmark.upload_metrics(s3_bucket=configs["METRICS_BUCKET"], s3_dir=benchmark_dir_s3)
 
 
 def invoke_lambda(configs: dict, config_file: str) -> dict:
     """Invokes an AWS Lambda function to run benchmarks based on the provided configuration options.
 
     Args:
         configs (dict): A dictionary of configuration options for the AWS infrastructure.
@@ -254,94 +235,207 @@
     config_path = os.path.join(benchmark_dir, file_name)
     with open(config_path, "w") as file:
         yaml.dump(configs, file)
         logger.info(f"Configs have been saved to {config_path}")
     return config_path
 
 
+def _get_git_info(git_uri_branch: str):
+    git_info = git_uri_branch.split("#")
+    if len(git_info) == 2:
+        git_uri, git_branch = git_info
+    elif len(git_info) == 1:
+        git_uri = git_info[0]
+        git_branch = "stable"
+    return git_uri, git_branch
+
+
+def _validate_single_value(configs: dict, key: str):
+    value = configs[key]
+    if isinstance(value, str):
+        configs[key] = [value]
+    elif isinstance(value, list) and len(value) != 1:
+        raise ValueError(f"Only single value (str, list[str]) is supported for {key}.")
+
+
+def _is_mounted(path: str):
+    with open("/proc/mounts", "r") as mounts:
+        for line in mounts:
+            parts = line.split()
+            if len(parts) > 1 and parts[1] == path:
+                return True
+
+
+def _umount_if_needed(path: str = None):
+    if not path:
+        return
+    if _is_mounted(path):
+        logging.info(f"{path} is a mount point, attempting to umount.")
+        subprocess.run(["sudo", "umount", path])
+        logging.info(f"Successfully umounted {path}.")
+
+
+def _mount_dir(orig_path: str, new_path: str):
+    subprocess.run(["sudo", "mount", "--bind", orig_path, new_path])
+
+
 @app.command()
 def run(
     config_file: str = typer.Argument(..., help="Path to custom config file."),
     remove_resources: bool = typer.Option(False, help="Remove resources after run."),
     wait: bool = typer.Option(False, help="Whether to block and wait for the benchmark to finish."),
     dev_branch: Optional[str] = typer.Option(None, help="Path to a development AutoGluon-Bench branch."),
 ):
     """Main function that runs the benchmark based on the provided configuration options."""
     configs = {}
     if config_file.startswith("s3"):
-        config_file = download_config(s3_path=config_file)
+        config_file = download_file_from_s3(s3_path=config_file)
     with open(config_file, "r") as f:
         configs = yaml.safe_load(f)
 
     benchmark_name = _get_benchmark_name(configs=configs)
     timestamp_pattern = r"\d{8}T\d{6}"  # Timestamp that matches YYYYMMDDTHHMMSS
     if not re.search(timestamp_pattern, benchmark_name):
         benchmark_name += "_" + formatted_time()
 
-    root_dir = configs.get("root_dir", ".ag_bench_runs")
-    benchmark_dir = os.path.join(root_dir, configs["module"], benchmark_name)
+    root_dir = configs.get("root_dir", "ag_bench_runs")
+    module = configs["module"]
+    benchmark_dir = os.path.join(root_dir, module, benchmark_name)
+    tmpdir = None
 
     if configs["mode"] == "aws":
-        configs["benchmark_name"] = benchmark_name
-        cloud_config_path = _dump_configs(
-            benchmark_dir=benchmark_dir, configs=configs, file_name=os.path.basename(config_file)
-        )
-        if dev_branch is not None:
-            os.environ["AG_BENCH_DEV_URL"] = dev_branch  # pull dev branch from GitHub
-        else:
-            os.environ["AG_BENCH_VERSION"] = agbench_version  # set the installed version for Dockerfile to align with
-        infra_configs = deploy_stack(custom_configs=configs.get("cdk_context", {}))
-        config_s3_path = upload_config(
-            bucket=infra_configs["METRICS_BUCKET"], benchmark_name=benchmark_name, file=cloud_config_path
-        )
-        lambda_response = invoke_lambda(configs=infra_configs, config_file=config_s3_path)
-        aws_configs = {**infra_configs, **lambda_response}
-        logger.info(f"Saving infra configs and submitted job configs under {benchmark_dir}.")
-        aws_config_path = _dump_configs(benchmark_dir=benchmark_dir, configs=aws_configs, file_name="aws_configs.yaml")
-
-        if remove_resources:
-            wait = True
-        if wait:
-            logger.info(
-                "Waiting for jobs to complete. You can quit at anytime and the benchmark will continue to run on the cloud"
+        current_path = os.path.dirname(os.path.abspath(__file__))
+        custom_configs_path = os.path.join(current_path, "custom_configs/amlb_configs")
+        lambda_custom_configs_path = os.path.join(current_path, "cloud/aws/batch_stack/lambdas/amlb_configs")
+        paths = [custom_configs_path, lambda_custom_configs_path]
+        try:
+            configs["benchmark_name"] = benchmark_name
+            # setting environment variables for docker build ARG
+            if dev_branch is not None:
+                os.environ["AG_BENCH_DEV_URL"] = dev_branch  # pull dev branch from GitHub
+            else:
+                os.environ[
+                    "AG_BENCH_VERSION"
+                ] = agbench_version  # set the installed version for Dockerfile to align with
+
+            os.environ["FRAMEWORK_PATH"] = f"frameworks/{module}"
+            os.environ["BENCHMARK_DIR"] = benchmark_dir
+
+            _validate_single_value(configs["module_configs"][module], "git_uri#branch")
+            os.environ["GIT_URI"], os.environ["GIT_BRANCH"] = _get_git_info(
+                configs["module_configs"][module]["git_uri#branch"][0]
+            )
+
+            if module == "tabular":
+                _validate_single_value(configs["module_configs"]["tabular"], "framework")
+                os.environ["AMLB_FRAMEWORK"] = configs["module_configs"]["tabular"]["framework"][0]
+
+                if configs["module_configs"]["tabular"].get("amlb_constraint"):
+                    _validate_single_value(configs["module_configs"]["tabular"], "amlb_constraint")
+                else:
+                    configs["module_configs"]["tabular"]["amlb_constraint"] = ["test"]
+
+                amlb_user_dir = configs["module_configs"]["tabular"].get("amlb_user_dir")
+                tmpdir = None
+                if amlb_user_dir is not None:
+                    _validate_single_value(configs["module_configs"]["tabular"], "amlb_user_dir")
+
+                    if amlb_user_dir[0].startswith("s3://"):
+                        tmpdir = tempfile.TemporaryDirectory()
+                        amlb_user_dir_local = download_dir_from_s3(s3_path=amlb_user_dir[0], local_path=tmpdir.name)
+                    else:
+                        amlb_user_dir_local = amlb_user_dir[0]
+
+                    for path in paths:
+                        _umount_if_needed(path)
+                        _mount_dir(orig_path=amlb_user_dir_local, new_path=path)
+
+                    # after mounting to custom_configs_path, custom_configs_path is copied to $WORKDIR in Dockerfile.
+                    # Contents under AMLB_USER_DIR will be seen in $WORKDIR/amlb_configs
+                    os.environ["AMLB_USER_DIR"] = "amlb_configs"
+                    configs["module_configs"]["tabular"]["amlb_user_dir"] = ["amlb_configs"]
+
+            infra_configs = deploy_stack(custom_configs=configs)
+
+            cloud_config_path = _dump_configs(
+                benchmark_dir=benchmark_dir, configs=configs, file_name=os.path.basename(config_file)
             )
+            config_s3_path = upload_to_s3(
+                s3_bucket=infra_configs["METRICS_BUCKET"],
+                s3_dir=f"configs/{benchmark_name}",
+                local_path=cloud_config_path,
+            )
+            lambda_response = invoke_lambda(configs=infra_configs, config_file=config_s3_path)
+            aws_configs = {**infra_configs, **lambda_response}
+            logger.info(f"Saving infra configs and submitted job configs under {benchmark_dir}.")
+            aws_config_path = _dump_configs(
+                benchmark_dir=benchmark_dir, configs=aws_configs, file_name="aws_configs.yaml"
+            )
+
             if remove_resources:
+                wait = True
+            if wait:
                 logger.info(
-                    "Resources will be deleted after the jobs are finished. You can also call \n"
-                    f"`agbench destroy-stack --config-file {aws_config_path}` "
-                    "to delete the stack after jobs have run to completion if you choose to quit now."
+                    "Waiting for jobs to complete. You can quit at anytime and the benchmark will continue to run on the cloud"
                 )
-
-            failed_jobs = wait_for_jobs_to_complete(config_file=aws_config_path)
-            if len(failed_jobs) > 0:
-                logger.warning("Some jobs have failed: %s.", failed_jobs)
-                if remove_resources:
-                    logger.warning("Resources will be kept so error logs can be accessed")
-            elif failed_jobs is None:
-                if remove_resources:
-                    logger.error("Resources are not being removed due to errors.")
-            else:
-                logger.info("All job succeeded.")
                 if remove_resources:
-                    logger.info("Removing resoureces...")
-                    destroy_stack(
-                        static_resource_stack=infra_configs["STATIC_RESOURCE_STACK_NAME"],
-                        batch_stack=infra_configs["BATCH_STACK_NAME"],
-                        cdk_deploy_account=infra_configs["CDK_DEPLOY_ACCOUNT"],
-                        cdk_deploy_region=infra_configs["CDK_DEPLOY_REGION"],
-                        config_file=None,
+                    logger.info(
+                        "Resources will be deleted after the jobs are finished. You can also call \n"
+                        f"`agbench destroy-stack --config-file {aws_config_path}` "
+                        "to delete the stack after jobs have run to completion if you choose to quit now."
                     )
-                    logger.info("Resources removed successfully.")
+
+                failed_jobs = wait_for_jobs_to_complete(config_file=aws_config_path)
+                if len(failed_jobs) > 0:
+                    logger.warning("Some jobs have failed: %s.", failed_jobs)
+                    if remove_resources:
+                        logger.warning("Resources will be kept so error logs can be accessed")
+                elif failed_jobs is None:
+                    if remove_resources:
+                        logger.error("Resources are not being removed due to errors.")
+                else:
+                    logger.info("All job succeeded.")
+                    if remove_resources:
+                        logger.info("Removing resoureces...")
+                        destroy_stack(
+                            static_resource_stack=infra_configs["STATIC_RESOURCE_STACK_NAME"],
+                            batch_stack=infra_configs["BATCH_STACK_NAME"],
+                            cdk_deploy_account=infra_configs["CDK_DEPLOY_ACCOUNT"],
+                            cdk_deploy_region=infra_configs["CDK_DEPLOY_REGION"],
+                            config_file=None,
+                        )
+                        logger.info("Resources removed successfully.")
+        finally:
+            for path in paths:
+                _umount_if_needed(path)
 
     elif configs["mode"] == "local":
         split_id = _get_split_id(config_file)
+        benchmark_dir_s3 = f"{module}/{benchmark_name}"
+        skip_setup = False
         if split_id is not None:
-            benchmark_name += "_" + split_id
-            benchmark_dir = os.path.join(benchmark_dir, benchmark_name)
+            benchmark_dir_s3 += f"/{benchmark_name}_{split_id}"
+            skip_setup = True
+
+        if module == "tabular":
+            amlb_user_dir = configs.get("amlb_user_dir")
+            if amlb_user_dir and amlb_user_dir.startswith("s3://"):
+                tmpdir = tempfile.TemporaryDirectory()
+                configs["amlb_user_dir"] = download_dir_from_s3(s3_path=amlb_user_dir, local_path=tmpdir.name)
+
         logger.info(f"Running benchmark {benchmark_name} at {benchmark_dir}.")
         if dev_branch is not None:
             logger.info(f"Using dev branch at {dev_branch}...")
+
         run_benchmark(
-            benchmark_name=benchmark_name, benchmark_dir=benchmark_dir, configs=configs, agbench_dev_url=dev_branch
+            benchmark_name=benchmark_name,
+            benchmark_dir=benchmark_dir,
+            configs=configs,
+            benchmark_dir_s3=benchmark_dir_s3,
+            agbench_dev_url=dev_branch,
+            skip_setup=skip_setup,
         )
     else:
         raise NotImplementedError
+
+    if tmpdir:
+        tmpdir.cleanup()
```

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/scripts/generate_cloud_configs.py` & `autogluon.bench-0.2.1/src/autogluon/bench/scripts/generate_cloud_configs.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 app = typer.Typer()
 
 
 @app.command()
 def generate_cloud_config(
     module: str = typer.Option(..., help="The module to generate config for: 'multimodal' or 'tabular'"),
-    root_dir: str = typer.Option(".ag_bench_runs", help="Root directory (optional, default = '.ag_bench_runs')"),
+    root_dir: str = typer.Option("ag_bench_runs", help="Root directory (optional, default = 'ag_bench_runs')"),
     benchmark_name: str = typer.Option("ag_bench", help="Benchmark name (optional, default = 'ag_bench')"),
     cdk_deploy_account: str = typer.Option(..., help="CDK deploy account"),
     cdk_deploy_region: str = typer.Option(..., help="CDK deploy region"),
     prefix: str = typer.Option(
         "ag-bench", help="Prefix used to identify infra resources (optional, default = 'ag-bench')"
     ),
     metrics_bucket: str = typer.Option(..., help="Name of the metrics bucket (required)"),
@@ -24,15 +24,15 @@
         None, help="Block device volume for EC2 instances (optional, default = 100)"
     ),
     reserved_memory_size: int = typer.Option(
         None, help="Reserved memory size for Docker container (optional, default = 15000)"
     ),
     instance: str = typer.Option(None, help="EC2 Instance type (optional, default = 'g4dn.2xlarge')"),
     git_uri_branch: str = typer.Option(
-        "", help="AutoGluon MultiModal git_uri#branch (in the format 'git_uri1#branch1,git_uri2#branch2,...')"
+        "", help="AutoGluon MultiModal or AMLB git_uri#branch (in the format 'git_uri1#branch1,git_uri2#branch2,...')"
     ),
     dataset_names: str = typer.Option(
         "",
         help="AutoGluon MultiModal dataset names for '--module multimodal' (comma-separated, to get a list of dataset names, run `from autogluon.bench.datasets.dataset_registry import multimodal_dataset_registry\n multimodal_dataset_registry.list_keys()`)",
     ),
     presets: str = typer.Option(
         None,
@@ -58,17 +58,17 @@
         None,
         help="AMLB Tasks for '--module tabular' (in the format '\"benchmark1:task1,task2;benchmark2:task3,task4,task5;...\"')",
     ),
     amlb_constraint: str = typer.Option(
         "",
         help="AMLB Constraints for '--module tabular', in the format 'test,1h4c,...'. Refer to https://github.com/openml/automlbenchmark/blob/master/resources/constraints.yaml for details.",
     ),
-    amlb_custom_branch: str = typer.Option(
+    amlb_user_dir: str = typer.Option(
         None,
-        help="Custom branch for '--module tabular', in the format 'https://github.com/<ACCOUNT1>/autogluon#<CUSTOM_BRANCH1>,https://github.com/<ACCOUNT2>/autogluon#<CUSTOM_BRANCH2>,...'",
+        help="Custom config directory.",
     ),
 ):
     config = {
         "module": module,
         "mode": "aws",
         "benchmark_name": benchmark_name,
         "root_dir": root_dir,
@@ -89,17 +89,17 @@
         cdk_context["BLOCK_DEVICE_VOLUME"] = block_device_volume
     if reserved_memory_size:
         cdk_context["RESERVED_MEMORY_SIZE"] = reserved_memory_size
     if instance:
         cdk_context["INSTANCE"] = instance
 
     config["cdk_context"] = cdk_context
+    git_uri_branch = git_uri_branch.split(",") if git_uri_branch else None
 
     if module == "multimodal":
-        git_uri_branch = git_uri_branch.split(",") if git_uri_branch else None
         dataset_names = dataset_names.split(",") if dataset_names else None
         presets = presets.split(",") if presets else None
         time_limit = [int(t.strip()) for t in time_limit.split(",")] if time_limit else None
 
         hyperparameters_list = []
         if hyperparameters:
             hyperparameters_items = hyperparameters.split(";")
@@ -133,26 +133,27 @@
             for item in amlb_task.split(";"):
                 if ":" in item:
                     benchmark, tasks = item.split(":")
                     task_list = tasks.split(",")
                     amlb_task_dict[benchmark] = task_list
             amlb_task = amlb_task_dict
         amlb_constraint = amlb_constraint.split(",") if amlb_constraint else None
-        amlb_custom_branch = amlb_custom_branch.split(",") if amlb_custom_branch else None
+        amlb_user_dir = amlb_user_dir.split(",") if amlb_user_dir else None
 
         module_configs = {
+            "git_uri#branch": git_uri_branch,
             "framework": framework,
             "amlb_benchmark": amlb_benchmark,
             "amlb_constraint": amlb_constraint,
         }
 
         if amlb_task:
             module_configs["amlb_task"] = amlb_task
-        if amlb_custom_branch:
-            module_configs["amlb_custom_branch"] = amlb_custom_branch
+        if amlb_user_dir:
+            module_configs["amlb_user_dir"] = amlb_user_dir
 
         config["module_configs"] = {"tabular": module_configs}
     else:
         typer.echo("Invalid module. Please choose 'multimodal' or 'tabular'.")
         return
 
     output_file = f"{module}_cloud_configs.yaml"
```

### Comparing `autogluon.bench-0.2.0/src/autogluon/bench/utils/dataset_utils.py` & `autogluon.bench-0.2.1/src/autogluon/bench/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/src/autogluon.bench.egg-info/PKG-INFO` & `autogluon.bench-0.2.1/src/autogluon.bench.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.bench
-Version: 0.2.0
+Version: 0.2.1
 Summary: A benchmarking tool for AutoML
 Author: AutoGluon Community
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -217,22 +217,21 @@
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Requires-Python: <3.11,>=3.8
+Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 <div align="left">
   <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
 </div>
@@ -267,15 +266,15 @@
 # install from source in editable mode
 pip install -e ".[tests]"
 ```
 
 For development, please be aware that `autogluon.bench` is installed as a dependency in certain places, such as the [Dockerfile](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/Dockerfile) and [Multimodal Setup](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/frameworks/multimodal/setup.sh). We made it possible to reflect the development changes by pushing the changes to a remote GitHub branch, and providing the URI when testing on benchmark runs:
 
 ```
-agbench run sample_configs/multimodal_cloud_configs.yaml --dev-branch https://github.com/suzhoum/autogluon-bench.git\#add_dev_branch
+agbench run sample_configs/multimodal_cloud_configs.yaml --dev-branch https://github.com/<username>/autogluon-bench.git#<dev_branch>
 ```
 
 
 ## Run benchmarks locally
 
 To run the benchmarks on your local machine, use the following command:
 
@@ -286,19 +285,26 @@
 Check out our [sample local configuration files](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs) for local runs.
 
 The results are stored in the following directory: `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}`.
 
 
 ### Tabular Benchmark
 
-To perform tabular benchmarking, set the module to tabular. You must set both Benchmark Configurations and Tabular Specific configurations, and each should have a single value. Refer to the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for more details.
+To perform tabular benchmarking, set the module to tabular. You must set both Benchmark Configurations and Tabular Specific configurations, and each should have a single value. Refer to the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/tabluar_local_configs.yaml) for more details.
 
 The tabular module leverages the [AMLB](https://github.com/openml/automlbenchmark) benchmarking framework. Required and optional AMLB arguments are specified via the configuration file mentioned previously.
 
-To benchmark a custom branch of AutoGluon on `tabular` module, use `amlb_custom_branch: https://github.com/REPO/autogluon#BRANCH` in the configuration file.
+Custom configuration is supported by providing a local directory to `amlb_user_dir` in the config, by which custom frameworks, constraints and datasets can be overriden. We have a minimum working [custom config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/amlb_configs) setup for benchmarking on a custom framework (a `AutoGluon` dev branch). In the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/tabluar_local_configs.yaml), change the following field to:
+
+```
+framework: AutoGluon_dev:example
+amlb_user_dir: path_to/sample_configs/amlb_configs 
+```
+
+For more customizations, please follow the [example custom configuration folder](https://github.com/openml/automlbenchmark/tree/master/examples/custom) provided by AMLB and their [documentation](https://github.com/openml/automlbenchmark/blob/master/docs/HOWTO.md#custom-configuration). 
 
 
 ### Multimodal Benchmark
 
 For multimodal benchmarking, set the module to multimodal. We currently support benchmarking multimodal on a custom branch. Note that multimodal benchmarking directly calls the MultiModalPredictor, bypassing the extra layer of [AMLB](https://github.com/openml/automlbenchmark). Therefore, the required arguments are different from those for tabular.
 
 You can add more datasets to your benchmarking jobs. We provided sample [multimodal datasets](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/multimodal_dataset.py) and [object detection dataset](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/object_detection_dataset.py). Follow these samples to add custom datasets, then specify dataset_name in your local config file. Please follow the section `Install From Source` for more instructions on how to develop with source.
@@ -307,20 +313,21 @@
 
 AutoGluon-Bench uses the AWS CDK to build an AWS Batch compute environment for benchmarking.
 
 To get started, install [Node.js](https://nodejs.org/) and [AWS CDK](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html#getting_started_install) with the following instructions:
 
 1. Install [Node Version Manager](https://github.com/nvm-sh/nvm#installing-and-updating).
 2. Source profile or restart the terminal.
-3. Follow the `Prerequisites` section on the [AWS CDK Guide](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html) and install an appropriate version for your system:
+3. Follow the `Prerequisites` section on the [AWS CDK Guide](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html) and install an appropriate `Node.js` version for your system:
 ```bash
 nvm install $VERSION  # install Node.js
 npm install -g aws-cdk  # install aws-cdk
 cdk --version  # verify the installation, you might need to update the Node.js version depending on the log.
 ```
+4. Follow the [AWS CLI Installation Guide](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) to install `awscliv2`. 
 
 If it is the first time using CDK to deploy to an AWS environment (An AWS environment is a combination of an AWS account and Region), please run the following:
 
 ```bash
 cdk bootstrap aws://CDK_DEPLOY_ACCOUNT/CDK_DEPLOY_REGION
 ```
```

### Comparing `autogluon.bench-0.2.0/src/autogluon.bench.egg-info/SOURCES.txt` & `autogluon.bench-0.2.1/src/autogluon.bench.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,27 @@
 .github/pull_request_template.md
 .github/workflows/continuous_integration.yml
 .github/workflows/pypi_release.yml
 sample_configs/multimodal_cloud_configs.yaml
 sample_configs/multimodal_local_configs.yaml
 sample_configs/tabular_cloud_configs.yaml
 sample_configs/tabular_local_configs.yaml
+sample_configs/amlb_configs/__init__.py
+sample_configs/amlb_configs/config.yaml
+sample_configs/amlb_configs/constraints.yaml
+sample_configs/amlb_configs/frameworks_example.yaml
 src/autogluon.bench.egg-info/PKG-INFO
 src/autogluon.bench.egg-info/SOURCES.txt
 src/autogluon.bench.egg-info/dependency_links.txt
 src/autogluon.bench.egg-info/entry_points.txt
 src/autogluon.bench.egg-info/requires.txt
 src/autogluon.bench.egg-info/top_level.txt
+src/autogluon/bench/Dockerfile
 src/autogluon/bench/__init__.py
+src/autogluon/bench/entrypoint.sh
 src/autogluon/bench/main.py
 src/autogluon/bench/runbenchmark.py
 src/autogluon/bench/version.py
 src/autogluon/bench/cloud/__init__.py
 src/autogluon/bench/cloud/aws/__init__.py
 src/autogluon/bench/cloud/aws/app.py
 src/autogluon/bench/cloud/aws/default_config.yaml
@@ -31,18 +37,16 @@
 src/autogluon/bench/cloud/aws/batch_stack/stack.py
 src/autogluon/bench/cloud/aws/batch_stack/constructs/__init__.py
 src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py
 src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py
 src/autogluon/bench/cloud/aws/batch_stack/lambdas/__init__.py
 src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py
 src/autogluon/bench/cloud/aws/batch_stack/lambdas/requirements.txt
-src/autogluon/bench/cloud/aws/docker/Dockerfile
-src/autogluon/bench/cloud/aws/docker/__init__.py
-src/autogluon/bench/cloud/aws/docker/entrypoint.sh
-src/autogluon/bench/cloud/aws/docker/gpu_utilization.sh
+src/autogluon/bench/cloud/aws/batch_stack/lambdas/amlb_configs/__init__.py
+src/autogluon/bench/custom_configs/amlb_configs/__init__.py
 src/autogluon/bench/datasets/__init__.py
 src/autogluon/bench/datasets/constants.py
 src/autogluon/bench/datasets/dataset_registry.py
 src/autogluon/bench/datasets/multimodal_dataset.py
 src/autogluon/bench/datasets/object_detection_dataset.py
 src/autogluon/bench/datasets/registry.py
 src/autogluon/bench/eval/__init__.py
@@ -78,15 +82,17 @@
 src/autogluon/bench/frameworks/tabular/setup.sh
 src/autogluon/bench/frameworks/tabular/tabular_benchmark.py
 src/autogluon/bench/scripts/__init__.py
 src/autogluon/bench/scripts/generate_cloud_configs.py
 src/autogluon/bench/utils/__init__.py
 src/autogluon/bench/utils/dataset_utils.py
 src/autogluon/bench/utils/general_utils.py
+src/autogluon/bench/utils/gpu_utilization.sh
 tests/unittests/benchmark/conftest.py
 tests/unittests/benchmark/test_benchmark.py
 tests/unittests/benchmark/test_runbenchmarks.py
 tests/unittests/cloud/aws/conftest.py
 tests/unittests/cloud/aws/test_stack.py
 tests/unittests/cloud/aws/test_stack_handler.py
 tests/unittests/datasets/test_registry.py
-tests/unittests/datasets/test_utils.py
+tests/unittests/utils/test_dataset_utils.py
+tests/unittests/utils/test_general_utils.py
```

### Comparing `autogluon.bench-0.2.0/tests/unittests/benchmark/test_benchmark.py` & `autogluon.bench-0.2.1/tests/unittests/benchmark/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/tests/unittests/benchmark/test_runbenchmarks.py` & `autogluon.bench-0.2.1/tests/unittests/benchmark/test_runbenchmarks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,11 @@
 import io
 import os
 
-from autogluon.bench.runbenchmark import (
-    download_config,
-    get_job_status,
-    get_kwargs,
-    invoke_lambda,
-    run,
-    run_benchmark,
-    upload_config,
-)
+from autogluon.bench.runbenchmark import get_job_status, get_kwargs, invoke_lambda, run, run_benchmark
 
 
 def setup_mock(mocker, tmp_path):
     config_file = tmp_path / "config.yaml"
     config_file.touch()
     mock_open = mocker.patch("builtins.open", new_callable=mocker.mock_open)
     mocker.patch("re.search", return_value=False)
@@ -28,45 +20,57 @@
     infra_configs = {
         "STATIC_RESOURCE_STACK_NAME": "test_static_stack",
         "BATCH_STACK_NAME": "test_batch_stack",
         "CDK_DEPLOY_ACCOUNT": "test_account",
         "CDK_DEPLOY_REGION": "test_region",
         "METRICS_BUCKET": "test_bucket",
     }
+
+    module_configs = {
+        "tabular": {
+            "git_uri#branch": "https://github.com/openml/automlbenchmark.git#master",
+            "framework": "AutoGluon:stable",
+            "amlb_benchmark": "small",
+            "amlb_user_dir": "sample_configs/amlb_configs",
+        }
+    }
+
     mock_yaml = mocker.patch("yaml.safe_load")
     yaml_value = {
         "mode": "aws",
-        "module": "test_module",
+        "module": "tabular",
         "cdk_context": cdk_context,
         "job_configs": job_configs,
+        "module_configs": module_configs,
     }
     yaml_value.update(infra_configs)
     mock_yaml.return_value = yaml_value
     mocker.patch("autogluon.bench.runbenchmark._get_benchmark_name", return_value="test_benchmark")
     mocker.patch("autogluon.bench.runbenchmark.formatted_time", return_value="test_time")
     mocker.patch("autogluon.bench.runbenchmark._dump_configs", return_value="test_dump")
     mocker.patch("os.environ.__setitem__")
 
     mock_deploy_stack = mocker.patch("autogluon.bench.runbenchmark.deploy_stack", return_value=infra_configs)
-    mock_upload_config = mocker.patch("autogluon.bench.runbenchmark.upload_config", return_value="test_s3_path")
+    mock_upload_to_s3 = mocker.patch("autogluon.bench.runbenchmark.upload_to_s3", return_value="test_s3_path")
     mock_invoke_lambda = mocker.patch("autogluon.bench.runbenchmark.invoke_lambda", return_value={})
 
     mock_wait_for_jobs = mocker.patch("autogluon.bench.runbenchmark.wait_for_jobs_to_complete", return_value=[])
     mock_destroy_stack = mocker.patch("autogluon.bench.runbenchmark.destroy_stack")
 
     return {
         "config_file": str(config_file),
         "infra_configs": infra_configs,
         "mock_deploy_stack": mock_deploy_stack,
-        "mock_upload_config": mock_upload_config,
+        "mock_upload_to_s3": mock_upload_to_s3,
         "mock_invoke_lambda": mock_invoke_lambda,
         "mock_wait_for_jobs": mock_wait_for_jobs,
         "mock_destroy_stack": mock_destroy_stack,
         "cdk_context": cdk_context,
         "job_configs": job_configs,
+        "custom_configs": yaml_value,
     }
 
 
 def test_get_kwargs_multimodal():
     module = "multimodal"
     configs = {
         "git_uri#branch": "https://github.com/project#master",
@@ -94,115 +98,87 @@
 
     assert get_kwargs(module, configs, agbench_dev_url) == expected_result
 
 
 def test_get_kwargs_tabular():
     module = "tabular"
     configs = {
+        "git_uri#branch": "https://github.com/openml/automlbenchmark.git#stable",
         "framework": "AutoGluon:stable",
         "amlb_benchmark": "test_bench",
         "amlb_task": "iris",
         "amlb_constraint": "test_constraint",
-        "amlb_custom_branch": "https://github.com/test/autogluon",
+        "fold_to_run": 6,
+        "amlb_user_dir": "sample_configs/amlb_configs",
     }
     agbench_dev_url = None
 
     expected_result = {
-        "setup_kwargs": {},
+        "setup_kwargs": {
+            "git_uri": "https://github.com/openml/automlbenchmark.git",
+            "git_branch": "stable",
+            "framework": "AutoGluon:stable",
+            "user_dir": "sample_configs/amlb_configs",
+        },
         "run_kwargs": {
             "framework": "AutoGluon:stable",
             "benchmark": "test_bench",
             "constraint": "test_constraint",
             "task": "iris",
-            "custom_branch": "https://github.com/test/autogluon",
+            "fold": 6,
+            "user_dir": "sample_configs/amlb_configs",
         },
     }
 
     assert get_kwargs(module, configs, agbench_dev_url) == expected_result
 
 
-def test_upload_config(mocker, tmp_path):
-    config_file = tmp_path / "config.yaml"
-    config_file.touch()
-
-    s3_client_mock = mocker.Mock()
-    mocker.patch("boto3.client", return_value=s3_client_mock)
-
-    bucket = "test_bucket"
-    benchmark_name = "test_benchmark"
-    s3_path = upload_config(bucket, benchmark_name, str(config_file))
-
-    s3_client_mock.upload_file.assert_called_once_with(
-        str(config_file),
-        bucket,
-        f"configs/{benchmark_name}_config.yaml",
-    )
-
-    assert s3_path == f"s3://{bucket}/configs/{benchmark_name}_config.yaml"
-
-
-def test_download_config(mocker, tmp_path):
-    s3_client_mock = mocker.Mock()
-    mocker.patch("boto3.client", return_value=s3_client_mock)
-
-    s3_path = "s3://test_bucket/configs/test_benchmark_config.yaml"
-    local_path = download_config(s3_path, str(tmp_path))
-
-    s3_client_mock.download_file.assert_called_once_with(
-        "test_bucket",
-        "configs/test_benchmark_config.yaml",
-        str(tmp_path / "test_benchmark_config.yaml"),
-    )
-
-    assert local_path == str(tmp_path / "test_benchmark_config.yaml")
-
-
 def test_invoke_lambda(mocker):
     configs = {
         "CDK_DEPLOY_REGION": "us-east-1",
         "LAMBDA_FUNCTION_NAME": "test_function",
         "STACK_NAME_PREFIX": "prefix",
     }
     config_file = "test_config_file"
 
     mock_response = {"StatusCode": 200, "Payload": io.BytesIO(b'{"key": "value"}')}
     mock_lambda_client = mocker.MagicMock()
     mock_lambda_client.invoke.return_value = mock_response
 
-    with mocker.patch("boto3.client", return_value=mock_lambda_client):
-        invoke_lambda(configs, config_file)
-        mock_lambda_client.invoke.assert_called_once_with(
-            FunctionName=configs["LAMBDA_FUNCTION_NAME"] + "-" + configs["STACK_NAME_PREFIX"],
-            InvocationType="RequestResponse",
-            Payload='{"config_file": "test_config_file"}',
-        )
+    mocker.patch("boto3.client", return_value=mock_lambda_client)
+    invoke_lambda(configs, config_file)
+    mock_lambda_client.invoke.assert_called_once_with(
+        FunctionName=configs["LAMBDA_FUNCTION_NAME"] + "-" + configs["STACK_NAME_PREFIX"],
+        InvocationType="RequestResponse",
+        Payload='{"config_file": "test_config_file"}',
+    )
 
 
 def test_run_aws_mode(mocker, tmp_path):
     setup = setup_mock(mocker, tmp_path)
 
     run(setup["config_file"], remove_resources=False, wait=False, dev_branch=None)
 
-    setup["mock_deploy_stack"].assert_called_once_with(custom_configs=setup["cdk_context"])
-    setup["mock_upload_config"].assert_called_once_with(
-        bucket="test_bucket", benchmark_name="test_benchmark_test_time", file="test_dump"
+    setup["mock_deploy_stack"].assert_called_once_with(custom_configs=setup["custom_configs"])
+    setup["mock_upload_to_s3"].assert_called_once_with(
+        s3_bucket="test_bucket", s3_dir="configs/test_benchmark_test_time", local_path="test_dump"
     )
     setup["mock_invoke_lambda"].assert_called_once_with(configs=setup["infra_configs"], config_file="test_s3_path")
     setup["mock_wait_for_jobs"].assert_not_called()
     setup["mock_destroy_stack"].assert_not_called()
 
 
 def test_run_aws_mode_remove_resources(mocker, tmp_path):
     setup = setup_mock(mocker, tmp_path)
 
     run(setup["config_file"], remove_resources=True, wait=False, dev_branch=None)
 
-    setup["mock_deploy_stack"].assert_called_once_with(custom_configs=setup["cdk_context"])
-    setup["mock_upload_config"].assert_called_once_with(
-        bucket="test_bucket", benchmark_name="test_benchmark_test_time", file="test_dump"
+    setup["mock_deploy_stack"].assert_called_once_with(custom_configs=setup["custom_configs"])
+    setup["mock_upload_to_s3"].assert_called_once_with(
+        s3_bucket="test_bucket", s3_dir="configs/test_benchmark_test_time", local_path="test_dump"
     )
     setup["mock_invoke_lambda"].assert_called_once_with(configs=setup["infra_configs"], config_file="test_s3_path")
 
     setup["mock_wait_for_jobs"].assert_called_once_with(config_file="test_dump")
     setup["mock_destroy_stack"].assert_called_once_with(
         static_resource_stack=setup["infra_configs"]["STATIC_RESOURCE_STACK_NAME"],
         batch_stack=setup["infra_configs"]["BATCH_STACK_NAME"],
@@ -213,61 +189,84 @@
 
 
 def test_run_aws_mode_wait(mocker, tmp_path):
     setup = setup_mock(mocker, tmp_path)
 
     run(setup["config_file"], remove_resources=False, wait=True, dev_branch=None)
 
-    setup["mock_deploy_stack"].assert_called_once_with(custom_configs=setup["cdk_context"])
-    setup["mock_upload_config"].assert_called_once_with(
-        bucket="test_bucket", benchmark_name="test_benchmark_test_time", file="test_dump"
+    setup["mock_deploy_stack"].assert_called_once_with(custom_configs=setup["custom_configs"])
+    setup["mock_upload_to_s3"].assert_called_once_with(
+        s3_bucket="test_bucket", s3_dir="configs/test_benchmark_test_time", local_path="test_dump"
     )
     setup["mock_invoke_lambda"].assert_called_once_with(configs=setup["infra_configs"], config_file="test_s3_path")
 
     setup["mock_wait_for_jobs"].assert_called_once_with(config_file="test_dump")
 
 
 def test_run_aws_mode_dev_branch(mocker, tmp_path):
     setup = setup_mock(mocker, tmp_path)
     dev_branch = "dev_branch_url"
 
     run(setup["config_file"], remove_resources=False, wait=False, dev_branch=dev_branch)
 
     assert os.environ["AG_BENCH_DEV_URL"] == dev_branch
-    setup["mock_deploy_stack"].assert_called_once_with(custom_configs=setup["cdk_context"])
-    setup["mock_upload_config"].assert_called_once_with(
-        bucket="test_bucket", benchmark_name="test_benchmark_test_time", file="test_dump"
+    setup["mock_deploy_stack"].assert_called_once_with(custom_configs=setup["custom_configs"])
+    setup["mock_upload_to_s3"].assert_called_once_with(
+        s3_bucket="test_bucket", s3_dir="configs/test_benchmark_test_time", local_path="test_dump"
     )
     setup["mock_invoke_lambda"].assert_called_once_with(configs=setup["infra_configs"], config_file="test_s3_path")
 
 
+def test_run_aws_tabular_user_dir(mocker, tmp_path):
+    setup = setup_mock(mocker, tmp_path)
+    temp_dir_mock = mocker.patch("tempfile.TemporaryDirectory")
+    s3_mock = mocker.patch("autogluon.bench.utils.general_utils.download_dir_from_s3")
+    mount_mock = mocker.patch("autogluon.bench.runbenchmark._mount_dir")
+    umount_mock = mocker.patch("autogluon.bench.runbenchmark._umount_if_needed")
+
+    run(setup["config_file"], remove_resources=False, wait=False, dev_branch="https://git_url#git_branch")
+    assert os.environ["AG_BENCH_DEV_URL"] == "https://git_url#git_branch"
+    assert os.environ["FRAMEWORK_PATH"] == "frameworks/tabular"
+    assert os.environ["BENCHMARK_DIR"] == "ag_bench_runs/tabular/test_benchmark_test_time"
+    assert os.environ["GIT_URI"] == "https://github.com/openml/automlbenchmark.git"
+    assert os.environ["GIT_BRANCH"] == "master"
+    assert os.environ["AMLB_FRAMEWORK"] == "AutoGluon:stable"
+    assert os.environ["AMLB_USER_DIR"] == "amlb_configs"
+    temp_dir_mock.assert_not_called()
+    s3_mock.assert_not_called()
+    assert umount_mock.call_count == 4
+    assert mount_mock.call_count == 2
+
+
 def test_run_local_mode(mocker, tmp_path):
     config_file = tmp_path / "config_split_test.yaml"
     config_file.touch()
     mock_open = mocker.patch("builtins.open", new_callable=mocker.mock_open)
 
     configs = {
         "mode": "local",
         "metrics_bucket": "test_bucket",
-        "module": "test_module",
+        "module": "tabular",
     }
     mock_yaml = mocker.patch("yaml.safe_load")
     mock_yaml.return_value = configs
     mocker.patch("autogluon.bench.runbenchmark._get_benchmark_name", return_value="test_benchmark")
     mocker.patch("autogluon.bench.runbenchmark.formatted_time", return_value="test_time")
     mock_run_benchmark = mocker.patch("autogluon.bench.runbenchmark.run_benchmark")
 
     run(str(config_file), remove_resources=False, wait=False, dev_branch=None)
 
     mock_open.assert_called_with(str(config_file), "r")
     mock_run_benchmark.assert_called_with(
         benchmark_name="test_benchmark_test_time",
-        benchmark_dir=".ag_bench_runs/test_module/test_benchmark_test_time",
+        benchmark_dir="ag_bench_runs/tabular/test_benchmark_test_time",
         configs=configs,
+        benchmark_dir_s3="tabular/test_benchmark_test_time",
         agbench_dev_url=None,
+        skip_setup=False,
     )
 
 
 def test_run_benchmark(mocker):
     benchmark_name = "test_benchmark"
     benchmark_dir = "test_dir"
     configs = {
@@ -277,22 +276,49 @@
 
     mocker.patch("autogluon.bench.runbenchmark.get_kwargs", return_value={"setup_kwargs": {}, "run_kwargs": {}})
     setup_mock = mocker.patch("autogluon.bench.runbenchmark.TabularBenchmark.setup")
     run_mock = mocker.patch("autogluon.bench.runbenchmark.TabularBenchmark.run")
     upload_metrics_mock = mocker.patch("autogluon.bench.runbenchmark.TabularBenchmark.upload_metrics")
     mocker.patch("autogluon.bench.runbenchmark._dump_configs")
 
-    run_benchmark(benchmark_name=benchmark_name, benchmark_dir=benchmark_dir, configs=configs)
+    run_benchmark(
+        benchmark_name=benchmark_name, benchmark_dir=benchmark_dir, configs=configs, benchmark_dir_s3="s3_dir"
+    )
 
     setup_mock.assert_called_once_with()
     run_mock.assert_called_once_with()
-    upload_metrics_mock.assert_called_once_with(
-        s3_bucket=configs["METRICS_BUCKET"], s3_dir=f"{configs['module']}{benchmark_dir.split(configs['module'])[-1]}"
+    upload_metrics_mock.assert_called_once_with(s3_bucket=configs["METRICS_BUCKET"], s3_dir="s3_dir")
+
+
+def test_run_benchmark_skip_setup(mocker):
+    benchmark_name = "test_benchmark"
+    benchmark_dir = "test_dir"
+    configs = {
+        "module": "tabular",
+        "METRICS_BUCKET": "test_bucket",
+    }
+
+    mocker.patch("autogluon.bench.runbenchmark.get_kwargs", return_value={"setup_kwargs": {}, "run_kwargs": {}})
+    setup_mock = mocker.patch("autogluon.bench.runbenchmark.TabularBenchmark.setup")
+    run_mock = mocker.patch("autogluon.bench.runbenchmark.TabularBenchmark.run")
+    upload_metrics_mock = mocker.patch("autogluon.bench.runbenchmark.TabularBenchmark.upload_metrics")
+    mocker.patch("autogluon.bench.runbenchmark._dump_configs")
+
+    run_benchmark(
+        benchmark_name=benchmark_name,
+        benchmark_dir=benchmark_dir,
+        configs=configs,
+        benchmark_dir_s3="s3_dir",
+        skip_setup=True,
     )
 
+    setup_mock.assert_not_called()
+    run_mock.assert_called_once_with()
+    upload_metrics_mock.assert_called_once_with(s3_bucket=configs["METRICS_BUCKET"], s3_dir="s3_dir")
+
 
 def test_get_job_status_with_config_file(mocker, tmp_path):
     # Setup mock
     setup = setup_mock(mocker, tmp_path)
 
     # Additional mock for describe_jobs
     mock_boto_client = mocker.patch("boto3.client")
```

### Comparing `autogluon.bench-0.2.0/tests/unittests/cloud/aws/conftest.py` & `autogluon.bench-0.2.1/tests/unittests/cloud/aws/conftest.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/tests/unittests/cloud/aws/test_stack.py` & `autogluon.bench-0.2.1/tests/unittests/cloud/aws/test_stack.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,19 @@
 
 @patch.dict("os.environ", {"CDK_DEPLOY_REGION": "dummy_region", "CDK_DEPLOY_ACCOUNT": "dummy_account"}, clear=True)
 def test_batch_job_stack():
     app = App()
     for key, value in context_values.items():
         app.node.set_context(key, value)
 
+    os.environ["FRAMEWORK_PATH"] = "frameworks/tabular"
+    os.environ["GIT_URI"] = "https://github.com/openml/automlbenchmark.git"
+    os.environ["GIT_BRANCH"] = "master"
+    os.environ["BENCHMARK_DIR"] = "benchmark_name_20230725"
+
     with patch.object(
         StaticResourceStack,
         "create_s3_resources",
         return_value=s3.Bucket(Stack(app, "TestBucketStack"), "DummyBucket"),
     ):
         static_resource_stack = StaticResourceStack(app, "TestStaticResourceStack", env=env)
```

### Comparing `autogluon.bench-0.2.0/tests/unittests/cloud/aws/test_stack_handler.py` & `autogluon.bench-0.2.1/tests/unittests/cloud/aws/test_stack_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,18 @@
         "STACK_NAME_TAG": "benchmark",
         "STATIC_RESOURCE_STACK_NAME": "test-prefix-static-resource-stack",
         "BATCH_STACK_NAME": "test-prefix-batch-stack",
         "CONTAINER_MEMORY": 10000,
         "CDK_DEPLOY_REGION": "us-west-2",
     }
     custom_configs = {
-        "METRICS_BUCKET": "test-metrics-bucket",
-        "DATA_BUCKET": "test-data-bucket",
+        "cdk_context": {
+            "METRICS_BUCKET": "test-metrics-bucket",
+            "DATA_BUCKET": "test-data-bucket",
+        },
     }
 
     mock_subprocess = mocker.patch("subprocess.check_call")
     with importlib.resources.path("autogluon.bench.cloud.aws", "stack_handler.py") as file_path:
         module_base_dir = os.path.dirname(file_path)
 
     with tempfile.TemporaryDirectory() as temp_dir:
@@ -86,15 +88,15 @@
                 "autogluon.bench.cloud.aws.stack_handler.construct_context", return_value=infra_configs_dict
             )
 
             deploy_stack(custom_configs=custom_configs)
 
     assert not os.path.exists(temp_dir)
     mock_cdk_path.assert_called_once()
-    mock_get_context.assert_called_with(custom_configs=custom_configs)
+    mock_get_context.assert_called_with(custom_configs=custom_configs["cdk_context"])
     mock_subprocess.assert_called_once_with(
         [
             os.path.join(module_base_dir, "deploy.sh"),
             infra_configs_dict["STACK_NAME_PREFIX"],
             infra_configs_dict["STACK_NAME_TAG"],
             infra_configs_dict["STATIC_RESOURCE_STACK_NAME"],
             infra_configs_dict["BATCH_STACK_NAME"],
```

### Comparing `autogluon.bench-0.2.0/tests/unittests/datasets/test_registry.py` & `autogluon.bench-0.2.1/tests/unittests/datasets/test_registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.0/tests/unittests/datasets/test_utils.py` & `autogluon.bench-0.2.1/tests/unittests/utils/test_dataset_utils.py`

 * *Files identical despite different names*

