# Comparing `tmp/mlfoundry-0.9.3.tar.gz` & `tmp/mlfoundry-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfoundry-0.9.3.tar", max compression
+gzip compressed data, was "mlfoundry-0.9.4.tar", max compression
```

## Comparing `mlfoundry-0.9.3.tar` & `mlfoundry-0.9.4.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0     3165 2023-07-25 10:01:39.305001 mlfoundry-0.9.3/README.md
--rw-r--r--   0        0        0      941 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/__init__.py
--rw-r--r--   0        0        0     1211 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/__main__.py
--rw-r--r--   0        0        0     3713 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/amplitude.py
--rw-r--r--   0        0        0        0 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/artifact/__init__.py
--rw-r--r--   0        0        0    29009 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/artifact/truefoundry_artifact_repo.py
--rw-r--r--   0        0        0        0 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/background/__init__.py
--rw-r--r--   0        0        0      287 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/background/events.py
--rw-r--r--   0        0        0     3032 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/background/interface.py
--rw-r--r--   0        0        0     4016 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/background/sender.py
--rw-r--r--   0        0        0     8756 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/background/system_metrics.py
--rw-r--r--   0        0        0     4028 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/background/utils.py
--rw-r--r--   0        0        0        0 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/cli/__init__.py
--rw-r--r--   0        0        0      918 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/cli/cli_interface.py
--rw-r--r--   0        0        0      100 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0     1840 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/cli/commands/download.py
--rw-r--r--   0        0        0      814 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/cli/commands/login.py
--rw-r--r--   0        0        0     2768 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/constants.py
--rw-r--r--   0        0        0     1392 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/enums.py
--rw-r--r--   0        0        0      384 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/env_vars.py
--rw-r--r--   0        0        0      365 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/exceptions.py
--rw-r--r--   0        0        0     2037 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/__init__.py
--rw-r--r--   0        0        0      301 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/base_registry.py
--rw-r--r--   0        0        0      718 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/fastai_registry.py
--rw-r--r--   0        0        0      892 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/gluon_registry.py
--rw-r--r--   0        0        0      700 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/h2o_registry.py
--rw-r--r--   0        0        0      712 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/keras_registry.py
--rw-r--r--   0        0        0      730 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/lightgbm_registry.py
--rw-r--r--   0        0        0      706 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/onnx_registry.py
--rw-r--r--   0        0        0      775 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/paddle_registry.py
--rw-r--r--   0        0        0      744 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/pytorch_registry.py
--rw-r--r--   0        0        0      724 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/sklearn_registry.py
--rw-r--r--   0        0        0      712 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/spacy_registry.py
--rw-r--r--   0        0        0      748 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/statsmodel_registry.py
--rw-r--r--   0        0        0     3077 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/tensorflow_registry.py
--rw-r--r--   0        0        0      774 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/transformers_registry.py
--rw-r--r--   0        0        0      724 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/xgboost_registry.py
--rw-r--r--   0        0        0     2349 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/git_info.py
--rw-r--r--   0        0        0        0 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/integrations/__init__.py
--rw-r--r--   0        0        0    15423 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/integrations/lightning.py
--rw-r--r--   0        0        0    22410 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/integrations/transformers.py
--rw-r--r--   0        0        0     1785 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/internal_namespace.py
--rw-r--r--   0        0        0      153 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/__init__.py
--rw-r--r--   0        0        0    12820 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/artifacts/artifact.py
--rw-r--r--   0        0        0     1019 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/artifacts/constants.py
--rw-r--r--   0        0        0     3072 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/artifacts/general_artifact.py
--rw-r--r--   0        0        0    20095 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/artifacts/model.py
--rw-r--r--   0        0        0     5952 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/artifacts/utils.py
--rw-r--r--   0        0        0       50 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/image/__init__.py
--rw-r--r--   0        0        0      255 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/image/constants.py
--rw-r--r--   0        0        0    11446 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/image/image.py
--rw-r--r--   0        0        0     2767 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/image/image_normalizer.py
--rw-r--r--   0        0        0     1566 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/image/types.py
--rw-r--r--   0        0        0      271 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/model_artifact.py
--rw-r--r--   0        0        0     7125 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/plot.py
--rw-r--r--   0        0        0     2486 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/pydantic_base.py
--rw-r--r--   0        0        0     1332 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/utils.py
--rw-r--r--   0        0        0      453 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/logger.py
--rw-r--r--   0        0        0     9289 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/login.py
--rw-r--r--   0        0        0        0 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/__init__.py
--rw-r--r--   0        0        0     1065 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v1/__init__.py
--rw-r--r--   0        0        0     2080 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v1/base_metrics.py
--rw-r--r--   0        0        0     6852 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v1/binary_classification_metrics.py
--rw-r--r--   0        0        0     6736 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v1/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     4419 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v1/regression_metrics.py
--rw-r--r--   0        0        0     3976 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v1/timeseries_metrics.py
--rw-r--r--   0        0        0     1026 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v2/__init__.py
--rw-r--r--   0        0        0     1898 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v2/base_metrics.py
--rw-r--r--   0        0        0      566 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v2/custom_metric_types.py
--rw-r--r--   0        0        0     6192 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v2/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     2718 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v2/regression_metrics.py
--rw-r--r--   0        0        0     2251 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v2/timeseries_metrics.py
--rw-r--r--   0        0        0      295 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v2/utils.py
--rw-r--r--   0        0        0    50297 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/mlfoundry_api.py
--rw-r--r--   0        0        0    49336 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/mlfoundry_run.py
--rw-r--r--   0        0        0        0 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/__init__.py
--rw-r--r--   0        0        0     1994 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/entities.py
--rw-r--r--   0        0        0       63 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/store/__init__.py
--rw-r--r--   0        0        0     6630 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/store/client.py
--rw-r--r--   0        0        0      169 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/store/constants.py
--rw-r--r--   0        0        0      336 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/store/repositories/__init__.py
--rw-r--r--   0        0        0     1351 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/store/repositories/dto.py
--rw-r--r--   0        0        0     6529 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
--rw-r--r--   0        0        0     2178 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/store/worker.py
--rw-r--r--   0        0        0     4471 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/run_utils.py
--rw-r--r--   0        0        0    10048 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/session.py
--rw-r--r--   0        0        0        0 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/tracking/__init__.py
--rw-r--r--   0        0        0     2766 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/tracking/auth_service.py
--rw-r--r--   0        0        0     2629 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/tracking/entities.py
--rw-r--r--   0        0        0     1175 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/tracking/servicefoundry_service.py
--rw-r--r--   0        0        0     4308 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/tracking/truefoundry_rest_store.py
--rw-r--r--   0        0        0        0 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/vendor/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/vendor/pynvml/__init__.py
--rw-r--r--   0        0        0    56147 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/vendor/pynvml/pynvml.py
--rw-r--r--   0        0        0      253 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/version.py
--rw-r--r--   0        0        0        0 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/webapp/__init__.py
--rw-r--r--   0        0        0       38 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/webapp/inputs.py
--rw-r--r--   0        0        0       39 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/webapp/outputs.py
--rw-r--r--   0        0        0     3329 2023-07-25 10:01:53.607149 mlfoundry-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     4664 1970-01-01 00:00:00.000000 mlfoundry-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     3165 2023-07-28 13:34:19.582888 mlfoundry-0.9.4/README.md
+-rw-r--r--   0        0        0      941 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/__init__.py
+-rw-r--r--   0        0        0     1211 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/__main__.py
+-rw-r--r--   0        0        0     3713 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/amplitude.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/artifact/__init__.py
+-rw-r--r--   0        0        0    29009 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/artifact/truefoundry_artifact_repo.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/background/__init__.py
+-rw-r--r--   0        0        0      287 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/background/events.py
+-rw-r--r--   0        0        0     3032 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/background/interface.py
+-rw-r--r--   0        0        0     4016 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/background/sender.py
+-rw-r--r--   0        0        0     8756 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/background/system_metrics.py
+-rw-r--r--   0        0        0     4028 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/background/utils.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/cli/__init__.py
+-rw-r--r--   0        0        0      918 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/cli/cli_interface.py
+-rw-r--r--   0        0        0      100 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1840 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/cli/commands/download.py
+-rw-r--r--   0        0        0      814 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/cli/commands/login.py
+-rw-r--r--   0        0        0     2768 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/constants.py
+-rw-r--r--   0        0        0     1392 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/enums.py
+-rw-r--r--   0        0        0      384 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/env_vars.py
+-rw-r--r--   0        0        0      365 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/exceptions.py
+-rw-r--r--   0        0        0     2037 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/__init__.py
+-rw-r--r--   0        0        0      301 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/base_registry.py
+-rw-r--r--   0        0        0      718 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/fastai_registry.py
+-rw-r--r--   0        0        0      892 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/gluon_registry.py
+-rw-r--r--   0        0        0      700 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/h2o_registry.py
+-rw-r--r--   0        0        0      712 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/keras_registry.py
+-rw-r--r--   0        0        0      730 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/lightgbm_registry.py
+-rw-r--r--   0        0        0      706 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/onnx_registry.py
+-rw-r--r--   0        0        0      775 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/paddle_registry.py
+-rw-r--r--   0        0        0      744 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/pytorch_registry.py
+-rw-r--r--   0        0        0      724 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/sklearn_registry.py
+-rw-r--r--   0        0        0      712 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/spacy_registry.py
+-rw-r--r--   0        0        0      748 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/statsmodel_registry.py
+-rw-r--r--   0        0        0     3077 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/tensorflow_registry.py
+-rw-r--r--   0        0        0      774 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/transformers_registry.py
+-rw-r--r--   0        0        0      724 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/frameworks/xgboost_registry.py
+-rw-r--r--   0        0        0     2349 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/git_info.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/integrations/__init__.py
+-rw-r--r--   0        0        0    15423 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/integrations/lightning.py
+-rw-r--r--   0        0        0    22410 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/integrations/transformers.py
+-rw-r--r--   0        0        0     1785 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/internal_namespace.py
+-rw-r--r--   0        0        0      153 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/log_types/__init__.py
+-rw-r--r--   0        0        0    12820 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/log_types/artifacts/artifact.py
+-rw-r--r--   0        0        0     1019 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/log_types/artifacts/constants.py
+-rw-r--r--   0        0        0     3072 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/log_types/artifacts/general_artifact.py
+-rw-r--r--   0        0        0    20095 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/log_types/artifacts/model.py
+-rw-r--r--   0        0        0     5952 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/log_types/artifacts/utils.py
+-rw-r--r--   0        0        0       50 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/log_types/image/__init__.py
+-rw-r--r--   0        0        0      255 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/log_types/image/constants.py
+-rw-r--r--   0        0        0    11446 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/log_types/image/image.py
+-rw-r--r--   0        0        0     2767 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/log_types/image/image_normalizer.py
+-rw-r--r--   0        0        0     1566 2023-07-28 13:34:19.602889 mlfoundry-0.9.4/mlfoundry/log_types/image/types.py
+-rw-r--r--   0        0        0      271 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/log_types/model_artifact.py
+-rw-r--r--   0        0        0     7125 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/log_types/plot.py
+-rw-r--r--   0        0        0     2486 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/log_types/pydantic_base.py
+-rw-r--r--   0        0        0     1332 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/log_types/utils.py
+-rw-r--r--   0        0        0      453 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/logger.py
+-rw-r--r--   0        0        0     9289 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/login.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/metrics/__init__.py
+-rw-r--r--   0        0        0     1065 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/metrics/v1/__init__.py
+-rw-r--r--   0        0        0     2080 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/metrics/v1/base_metrics.py
+-rw-r--r--   0        0        0     6852 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/metrics/v1/binary_classification_metrics.py
+-rw-r--r--   0        0        0     6736 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/metrics/v1/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     4419 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/metrics/v1/regression_metrics.py
+-rw-r--r--   0        0        0     3976 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/metrics/v1/timeseries_metrics.py
+-rw-r--r--   0        0        0     1026 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/metrics/v2/__init__.py
+-rw-r--r--   0        0        0     1898 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/metrics/v2/base_metrics.py
+-rw-r--r--   0        0        0      566 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/metrics/v2/custom_metric_types.py
+-rw-r--r--   0        0        0     6192 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/metrics/v2/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     2718 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/metrics/v2/regression_metrics.py
+-rw-r--r--   0        0        0     2251 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/metrics/v2/timeseries_metrics.py
+-rw-r--r--   0        0        0      295 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/metrics/v2/utils.py
+-rw-r--r--   0        0        0    50459 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/mlfoundry_api.py
+-rw-r--r--   0        0        0    49931 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/mlfoundry_run.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/monitoring/__init__.py
+-rw-r--r--   0        0        0     1994 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/monitoring/entities.py
+-rw-r--r--   0        0        0       63 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/monitoring/store/__init__.py
+-rw-r--r--   0        0        0     6630 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/monitoring/store/client.py
+-rw-r--r--   0        0        0      169 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/monitoring/store/constants.py
+-rw-r--r--   0        0        0      336 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/monitoring/store/repositories/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/monitoring/store/repositories/dto.py
+-rw-r--r--   0        0        0     6529 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
+-rw-r--r--   0        0        0     2178 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/monitoring/store/worker.py
+-rw-r--r--   0        0        0     4471 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/run_utils.py
+-rw-r--r--   0        0        0    10048 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/session.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/tracking/__init__.py
+-rw-r--r--   0        0        0     2766 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/tracking/auth_service.py
+-rw-r--r--   0        0        0     2629 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/tracking/entities.py
+-rw-r--r--   0        0        0     1175 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/tracking/servicefoundry_service.py
+-rw-r--r--   0        0        0     4308 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/tracking/truefoundry_rest_store.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/vendor/pynvml/__init__.py
+-rw-r--r--   0        0        0    56147 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/vendor/pynvml/pynvml.py
+-rw-r--r--   0        0        0      253 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/version.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/webapp/__init__.py
+-rw-r--r--   0        0        0       38 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/webapp/inputs.py
+-rw-r--r--   0        0        0       39 2023-07-28 13:34:19.606890 mlfoundry-0.9.4/mlfoundry/webapp/outputs.py
+-rw-r--r--   0        0        0     3329 2023-07-28 13:34:38.004008 mlfoundry-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     4664 1970-01-01 00:00:00.000000 mlfoundry-0.9.4/PKG-INFO
```

### Comparing `mlfoundry-0.9.3/README.md` & `mlfoundry-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/__init__.py` & `mlfoundry-0.9.4/mlfoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/__main__.py` & `mlfoundry-0.9.4/mlfoundry/__main__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/amplitude.py` & `mlfoundry-0.9.4/mlfoundry/amplitude.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/artifact/truefoundry_artifact_repo.py` & `mlfoundry-0.9.4/mlfoundry/artifact/truefoundry_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/background/interface.py` & `mlfoundry-0.9.4/mlfoundry/background/interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/background/sender.py` & `mlfoundry-0.9.4/mlfoundry/background/sender.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/background/system_metrics.py` & `mlfoundry-0.9.4/mlfoundry/background/system_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/background/utils.py` & `mlfoundry-0.9.4/mlfoundry/background/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/cli/cli_interface.py` & `mlfoundry-0.9.4/mlfoundry/cli/cli_interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/cli/commands/download.py` & `mlfoundry-0.9.4/mlfoundry/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/cli/commands/login.py` & `mlfoundry-0.9.4/mlfoundry/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/constants.py` & `mlfoundry-0.9.4/mlfoundry/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/enums.py` & `mlfoundry-0.9.4/mlfoundry/enums.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/frameworks/__init__.py` & `mlfoundry-0.9.4/mlfoundry/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/frameworks/fastai_registry.py` & `mlfoundry-0.9.4/mlfoundry/frameworks/fastai_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/frameworks/gluon_registry.py` & `mlfoundry-0.9.4/mlfoundry/frameworks/gluon_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/frameworks/h2o_registry.py` & `mlfoundry-0.9.4/mlfoundry/frameworks/h2o_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/frameworks/keras_registry.py` & `mlfoundry-0.9.4/mlfoundry/frameworks/keras_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/frameworks/lightgbm_registry.py` & `mlfoundry-0.9.4/mlfoundry/frameworks/lightgbm_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/frameworks/onnx_registry.py` & `mlfoundry-0.9.4/mlfoundry/frameworks/onnx_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/frameworks/paddle_registry.py` & `mlfoundry-0.9.4/mlfoundry/frameworks/paddle_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/frameworks/pytorch_registry.py` & `mlfoundry-0.9.4/mlfoundry/frameworks/pytorch_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/frameworks/sklearn_registry.py` & `mlfoundry-0.9.4/mlfoundry/frameworks/sklearn_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/frameworks/spacy_registry.py` & `mlfoundry-0.9.4/mlfoundry/frameworks/spacy_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/frameworks/statsmodel_registry.py` & `mlfoundry-0.9.4/mlfoundry/frameworks/statsmodel_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/frameworks/tensorflow_registry.py` & `mlfoundry-0.9.4/mlfoundry/frameworks/tensorflow_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/frameworks/transformers_registry.py` & `mlfoundry-0.9.4/mlfoundry/frameworks/transformers_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/frameworks/xgboost_registry.py` & `mlfoundry-0.9.4/mlfoundry/frameworks/xgboost_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/git_info.py` & `mlfoundry-0.9.4/mlfoundry/git_info.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/integrations/lightning.py` & `mlfoundry-0.9.4/mlfoundry/integrations/lightning.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/integrations/transformers.py` & `mlfoundry-0.9.4/mlfoundry/integrations/transformers.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/internal_namespace.py` & `mlfoundry-0.9.4/mlfoundry/internal_namespace.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/log_types/artifacts/artifact.py` & `mlfoundry-0.9.4/mlfoundry/log_types/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/log_types/artifacts/constants.py` & `mlfoundry-0.9.4/mlfoundry/log_types/artifacts/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/log_types/artifacts/general_artifact.py` & `mlfoundry-0.9.4/mlfoundry/log_types/artifacts/general_artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/log_types/artifacts/model.py` & `mlfoundry-0.9.4/mlfoundry/log_types/artifacts/model.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/log_types/artifacts/utils.py` & `mlfoundry-0.9.4/mlfoundry/log_types/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/log_types/image/image.py` & `mlfoundry-0.9.4/mlfoundry/log_types/image/image.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/log_types/image/image_normalizer.py` & `mlfoundry-0.9.4/mlfoundry/log_types/image/image_normalizer.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/log_types/image/types.py` & `mlfoundry-0.9.4/mlfoundry/log_types/image/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/log_types/plot.py` & `mlfoundry-0.9.4/mlfoundry/log_types/plot.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/log_types/pydantic_base.py` & `mlfoundry-0.9.4/mlfoundry/log_types/pydantic_base.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/log_types/utils.py` & `mlfoundry-0.9.4/mlfoundry/log_types/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/login.py` & `mlfoundry-0.9.4/mlfoundry/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/metrics/v1/__init__.py` & `mlfoundry-0.9.4/mlfoundry/metrics/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/metrics/v1/base_metrics.py` & `mlfoundry-0.9.4/mlfoundry/metrics/v1/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/metrics/v1/binary_classification_metrics.py` & `mlfoundry-0.9.4/mlfoundry/metrics/v1/binary_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/metrics/v1/multiclass_classification_metrics.py` & `mlfoundry-0.9.4/mlfoundry/metrics/v1/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/metrics/v1/regression_metrics.py` & `mlfoundry-0.9.4/mlfoundry/metrics/v1/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/metrics/v1/timeseries_metrics.py` & `mlfoundry-0.9.4/mlfoundry/metrics/v1/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/metrics/v2/__init__.py` & `mlfoundry-0.9.4/mlfoundry/metrics/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/metrics/v2/base_metrics.py` & `mlfoundry-0.9.4/mlfoundry/metrics/v2/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/metrics/v2/custom_metric_types.py` & `mlfoundry-0.9.4/mlfoundry/metrics/v2/custom_metric_types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/metrics/v2/multiclass_classification_metrics.py` & `mlfoundry-0.9.4/mlfoundry/metrics/v2/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/metrics/v2/regression_metrics.py` & `mlfoundry-0.9.4/mlfoundry/metrics/v2/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/metrics/v2/timeseries_metrics.py` & `mlfoundry-0.9.4/mlfoundry/metrics/v2/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/mlfoundry_api.py` & `mlfoundry-0.9.4/mlfoundry/mlfoundry_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,14 +339,15 @@
         mlf_run = MlFoundryRun(
             experiment_id=ml_repo_id, run_id=mlf_run_id, auto_end=True, **kwargs
         )
         # TODO(Rizwan): Revisit this once run lifecycle is formalised
         mlf_run._add_git_info()
         mlf_run._add_python_mlf_version()
         logger.info(f"Run {run.info.fqn!r} has started.")
+        print(f"Link to the dashboard for the run: {mlf_run.dashboard_link}")
         return mlf_run
 
     def get_run_by_id(self, run_id: str) -> MlFoundryRun:
         """Get an existing `run` by the `run_id`.
 
         Args:
             run_id (str): run_id or fqn of an existing `run`.
@@ -372,18 +373,17 @@
                 f"run_id must be string type and not empty. "
                 f"Got {type(run_id)} type with value {run_id}"
             )
         if "/" in run_id:
             return self.get_run_by_fqn(run_id)
 
         run = self.mlflow_client.get_run(run_id)
-        return MlFoundryRun(
-            experiment_id=run.info.experiment_id,
-            run_id=run.info.run_id,
-        )
+        mlfoundry_run = MlFoundryRun._get_run_from_mlflow_run(run)
+        print(f"Link to the dashboard for the run: {mlfoundry_run.dashboard_link}")
+        return mlfoundry_run
 
     def get_run_by_fqn(self, run_fqn: str) -> MlFoundryRun:
         """Get an existing `run` by `fqn`.
 
         `fqn` stands for Fully Qualified Name. A run `fqn` has the following pattern:
         tenant_name/ml_repo/run_name
 
@@ -404,18 +404,17 @@
             client = mlfoundry.get_client()
 
             run = client.get_run_by_fqn(run_fqn='truefoundry/my-repo/svm')
             ```
 
         """
         run = self.mlflow_client.get_run_by_fqn(run_fqn)
-        return MlFoundryRun(
-            experiment_id=run.info.experiment_id,
-            run_id=run.info.run_id,
-        )
+        mlfoundry_run = MlFoundryRun._get_run_from_mlflow_run(run)
+        print(f"Link to the dashboard for the run: {mlfoundry_run.dashboard_link}")
+        return mlfoundry_run
 
     def get_run_by_name(
         self,
         ml_repo: str,
         run_name: str,
     ) -> MlFoundryRun:
         """Get an existing `run` by `run_name`.
@@ -433,25 +432,23 @@
             import mlfoundry
 
             client = mlfoundry.get_client()
 
             run = client.get_run_by_name(run_name='svm', ml_repo='my-repo')
             ```
         """
-        ml_repo = _resolve_ml_repo_name(ml_repo=ml_repo)
-
-        ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
 
         run = self.mlflow_client.get_run_by_name(
-            experiment_id=ml_repo_id, run_name=run_name
-        )
-        return MlFoundryRun(
-            experiment_id=run.info.experiment_id,
-            run_id=run.info.run_id,
+            experiment_id=None,
+            run_name=run_name,
+            experiment_name=ml_repo,
         )
+        mlfoundry_run = MlFoundryRun._get_run_from_mlflow_run(run)
+        print(f"Link to the dashboard for the run: {mlfoundry_run.dashboard_link}")
+        return mlfoundry_run
 
     def get_all_runs(
         self,
         ml_repo: Optional[str] = None,
         project_name: Optional[str] = None,
     ) -> pd.DataFrame:
         """Returns all the run name and id present under a project.
@@ -628,15 +625,15 @@
                 order_by=order_by,
                 page_token=page_token,
             )
             page_token = all_runs.token
             for run in all_runs:
                 if max_results is not None:
                     max_results -= 1
-                yield MlFoundryRun(run.info.experiment_id, run.info.run_id)
+                yield MlFoundryRun._get_run_from_mlflow_run(run)
             done = page_token is None or max_results == 0
 
     @staticmethod
     def get_tracking_uri():
         """
         Get the current tracking URI.
```

### Comparing `mlfoundry-0.9.3/mlfoundry/mlfoundry_run.py` & `mlfoundry-0.9.4/mlfoundry/mlfoundry_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     Artifact,
     ArtifactType,
     ArtifactVersionStatus,
     CustomMetric,
     Metric,
     ModelSchema,
     Param,
+    Run,
+    RunData,
     RunInfo,
     RunStatus,
     RunTag,
 )
 from mlflow.tracking import MlflowClient
 
 from mlfoundry import amplitude, constants, enums, version
@@ -85,19 +87,27 @@
         """
         self._experiment_id = str(experiment_id)
         self._run_id = run_id
         self._auto_end = auto_end
         # TODO (chiragjn): mlflow_client be a protected/private member
         self.mlflow_client = MlflowClient()
         self._run_info: Optional[RunInfo] = None
+        self._run_data: Optional[RunData] = None
         self._deleted = False
         self._terminate_called = False
         if self._auto_end:
             ACTIVE_RUNS.add_run(self)
-        print(f"Link to the dashboard for the run: {self.dashboard_link}")
+
+    @classmethod
+    def _get_run_from_mlflow_run(cls, mlflow_run: Run):
+        """classmethod to get MLfoundry run from mlfow_run instance"""
+        run = cls(mlflow_run.info.experiment_id, mlflow_run.info.run_id)
+        run._run_info = mlflow_run.info
+        run._run_data = mlflow_run.data
+        return run
 
     def _get_run_info(self) -> RunInfo:
         if self._run_info is not None:
             return self._run_info
 
         self._run_info = self.mlflow_client.get_run(self.run_id).info
         return self._run_info
@@ -795,15 +805,15 @@
                 run_id=self.run_id, metrics=[], params=[], tags=tags_arr
             )
         except MlflowException as e:
             raise MlFoundryException(e.message) from e
         logger.info("Tags set successfully")
 
     @_ensure_not_deleted
-    def get_tags(self) -> Dict[str, str]:
+    def get_tags(self, no_cache=False) -> Dict[str, str]:
         """Returns all the tags set for the current `run`.
 
         Returns:
             Dict[str, str]: A dictionary containing tags. The keys in the dictionary
                 are tag names and the values are corresponding tag values.
 
         Examples:
@@ -818,16 +828,20 @@
         print(run.get_tags())
 
         run.end()
         ```
         """
         amplitude.track(amplitude.Event.GET_TAGS)
 
+        if not no_cache and self._run_data:
+            return self._run_data.tags
+
         run = self.mlflow_client.get_run(self.run_id)
-        return run.data.tags
+        self._run_data = run.data
+        return self._run_data.tags
 
     @_ensure_not_deleted
     def auto_log_metrics(
         self,
         model_type: enums.ModelType,
         data_slice: enums.DataSlice,
         predictions: Collection[Any],
@@ -919,15 +933,15 @@
         for metric_name in valid_metrics:
             metrics_dict[metric_name] = self.mlflow_client.get_metric_history(
                 self.run_id, metric_name
             )
         return metrics_dict
 
     @_ensure_not_deleted
-    def get_params(self) -> Dict[str, str]:
+    def get_params(self, no_cache=False) -> Dict[str, str]:
         """Get all the params logged for the current `run`.
 
         Returns:
             Dict[str, str]: A dictionary containing the parameters. The keys in the dictionary
                 are parameter names and the values are corresponding parameter values.
 
         Examples:
@@ -941,16 +955,20 @@
         run.log_params({"learning_rate": 0.01, "epochs": 10})
         print(run.get_params())
 
         run.end()
         ```
         """
         amplitude.track(amplitude.Event.GET_PARAMS)
+        if not no_cache and self._run_data:
+            return self._run_data.params
+
         run = self.mlflow_client.get_run(self.run_id)
-        return run.data.params
+        self._run_data = run.data
+        return self._run_data.params
 
     @_ensure_not_deleted
     def log_model(
         self,
         *,
         name: str,
         model: Any,
```

### Comparing `mlfoundry-0.9.3/mlfoundry/monitoring/entities.py` & `mlfoundry-0.9.4/mlfoundry/monitoring/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/monitoring/store/client.py` & `mlfoundry-0.9.4/mlfoundry/monitoring/store/client.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/monitoring/store/repositories/dto.py` & `mlfoundry-0.9.4/mlfoundry/monitoring/store/repositories/dto.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py` & `mlfoundry-0.9.4/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/monitoring/store/worker.py` & `mlfoundry-0.9.4/mlfoundry/monitoring/store/worker.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/run_utils.py` & `mlfoundry-0.9.4/mlfoundry/run_utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/session.py` & `mlfoundry-0.9.4/mlfoundry/session.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/tracking/auth_service.py` & `mlfoundry-0.9.4/mlfoundry/tracking/auth_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/tracking/entities.py` & `mlfoundry-0.9.4/mlfoundry/tracking/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/tracking/servicefoundry_service.py` & `mlfoundry-0.9.4/mlfoundry/tracking/servicefoundry_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/tracking/truefoundry_rest_store.py` & `mlfoundry-0.9.4/mlfoundry/tracking/truefoundry_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/mlfoundry/vendor/pynvml/pynvml.py` & `mlfoundry-0.9.4/mlfoundry/vendor/pynvml/pynvml.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.3/pyproject.toml` & `mlfoundry-0.9.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlfoundry"
-version = "0.9.3" # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.9.4" # do not change, auto-generated by poetry-dynamic-versioning
 description = "Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/truefoundry/mlfoundry"
 repository = "https://github.com/truefoundry/mlfoundry"
 readme = "README.md"
 packages = [
     { include = "mlfoundry" },
@@ -30,15 +30,15 @@
 pydantic = ">=1.8.2,<2.0.0"
 scikit-learn = ">=0.24.2,<2.0.0"
 scipy = [
     # This is split into two because poetry will select a version which has no wheel on python >= 3.10 :/
     { version = ">=1.5.4,<2.0.0", python = "<3.10" },
     { version = ">=1.8.0,<2.0.0", python = ">=3.10" },
 ]
-tfy-mlflow-client = "0.0.37"
+tfy-mlflow-client = "0.0.38"
 tqdm = ">=4.62.3,<5.0.0"
 # Check and try to eliminate libs below this comment
 importlib-metadata = ">=4.11.3,<5.0.0"
 packaging = ">=20.0,<24.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "2.21.0"
```

### Comparing `mlfoundry-0.9.3/PKG-INFO` & `mlfoundry-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfoundry
-Version: 0.9.3
+Version: 0.9.4
 Summary: Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library
 Home-page: https://github.com/truefoundry/mlfoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -23,15 +23,15 @@
 Requires-Dist: pandas (>=1.0.0,<2.0.0) ; python_version < "3.10"
 Requires-Dist: pandas (>=1.4.0,<2.0.0) ; python_version >= "3.10"
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: scikit-learn (>=0.24.2,<2.0.0)
 Requires-Dist: scipy (>=1.5.4,<2.0.0) ; python_version < "3.10"
 Requires-Dist: scipy (>=1.8.0,<2.0.0) ; python_version >= "3.10"
-Requires-Dist: tfy-mlflow-client (==0.0.37)
+Requires-Dist: tfy-mlflow-client (==0.0.38)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Project-URL: Repository, https://github.com/truefoundry/mlfoundry
 Description-Content-Type: text/markdown
 
 # MlFoundry
 
 ![](https://github.com/MyName/my-project/workflows/Project%20Tests/badge.svg)
```

