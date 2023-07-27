# Comparing `tmp/mosaicml-cli-0.5.1.tar.gz` & `tmp/mosaicml-cli-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.5.1.tar", last modified: Wed Jul 26 00:37:20 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.5.2.tar", last modified: Thu Jul 27 22:06:59 2023, max compression
```

## Comparing `mosaicml-cli-0.5.1.tar` & `mosaicml-cli-0.5.2.tar`

### file list

```diff
@@ -1,209 +1,210 @@
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.217841 mosaicml-cli-0.5.1/
--rw-r--r--   0 margaret.qian   (502) staff       (20)      696 2023-07-26 00:37:20.217704 mosaicml-cli-0.5.1/PKG-INFO
--rw-r--r--   0 margaret.qian   (502) staff       (20)     7089 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/README.md
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.190041 mosaicml-cli-0.5.1/mcli/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2122 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/__init__.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.190847 mosaicml-cli-0.5.1/mcli/api/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/__init__.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.191125 mosaicml-cli-0.5.1/mcli/api/cluster/
--rw-r--r--   0 margaret.qian   (502) staff       (20)      134 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/cluster/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4990 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.191482 mosaicml-cli-0.5.1/mcli/api/engine/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/engine/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    26027 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/engine/engine.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    13444 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/exceptions.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.192696 mosaicml-cli-0.5.1/mcli/api/inference_deployments/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1521 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3297 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5045 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3992 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     8413 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2294 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_ping.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2746 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_predict_inference_deployment.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6499 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_update_inference_deployments.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.193084 mosaicml-cli-0.5.1/mcli/api/mint/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/mint/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     7840 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/mint/shell.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2676 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/mint/tty.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.193632 mosaicml-cli-0.5.1/mcli/api/model/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1114 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/model/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     9386 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/api/model/cluster_details.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4583 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/model/inference_deployment.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    14890 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/api/model/run.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.195122 mosaicml-cli-0.5.1/mcli/api/runs/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1269 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3785 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_create_interactive_run.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3034 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_create_run.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4365 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     8796 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    12239 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5366 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_start_run.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5559 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5916 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_update_run.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4091 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    10414 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.195464 mosaicml-cli-0.5.1/mcli/api/schema/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/schema/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      636 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.195942 mosaicml-cli-0.5.1/mcli/api/secrets/
--rw-r--r--   0 margaret.qian   (502) staff       (20)      309 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/secrets/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2386 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2943 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3665 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2354 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/typing_future.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.196210 mosaicml-cli-0.5.1/mcli/api/users/
--rw-r--r--   0 margaret.qian   (502) staff       (20)      139 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/users/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2715 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/users/api_get_users.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      920 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/utils.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.196420 mosaicml-cli-0.5.1/mcli/cli/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/__init__.py
--rwxr-xr-x   0 margaret.qian   (502) staff       (20)     6069 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/cli.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.196761 mosaicml-cli-0.5.1/mcli/cli/common/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/common/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2560 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     7499 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.196993 mosaicml-cli-0.5.1/mcli/cli/m_connect/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6426 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.197339 mosaicml-cli-0.5.1/mcli/cli/m_create/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_create/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2385 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_create/m_create.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    16900 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.197814 mosaicml-cli-0.5.1/mcli/cli/m_delete/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6448 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_delete/delete.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5838 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.198073 mosaicml-cli-0.5.1/mcli/cli/m_deploy/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4253 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.198630 mosaicml-cli-0.5.1/mcli/cli/m_describe/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3929 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    13495 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2259 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.199789 mosaicml-cli-0.5.1/mcli/cli/m_get/
--rw-r--r--   0 margaret.qian   (502) staff       (20)      467 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     7068 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/clusters.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6459 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/display.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5807 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4804 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/m_get.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     8967 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/runs.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2189 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/secrets.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1580 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/users.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.204124 mosaicml-cli-0.5.1/mcli/cli/m_init/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_init/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3908 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_init/m_init.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.204468 mosaicml-cli-0.5.1/mcli/cli/m_interactive/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     9036 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.205155 mosaicml-cli-0.5.1/mcli/cli/m_kube/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_kube/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5523 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_kube/m_get_config.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1398 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_kube/m_kube.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2050 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_kube/m_merge_config.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6946 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_kube/utils.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.205413 mosaicml-cli-0.5.1/mcli/cli/m_log/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_log/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    11756 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.205658 mosaicml-cli-0.5.1/mcli/cli/m_ping/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1411 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.206037 mosaicml-cli-0.5.1/mcli/cli/m_predict/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1905 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.206425 mosaicml-cli-0.5.1/mcli/cli/m_root/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_root/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      536 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.206678 mosaicml-cli-0.5.1/mcli/cli/m_run/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_run/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    11501 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.207840 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2964 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1793 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2267 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1656 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      840 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/organization.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      745 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.208106 mosaicml-cli-0.5.1/mcli/cli/m_stop/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4062 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.208362 mosaicml-cli-0.5.1/mcli/cli/m_update/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_update/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6568 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/cli/m_update/m_update.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.208778 mosaicml-cli-0.5.1/mcli/cli/m_util/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_util/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      797 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_util/m_util.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     9034 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/m_util/util.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.209036 mosaicml-cli-0.5.1/mcli/cli/m_watchdog/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_watchdog/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3544 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/cli/m_watchdog/m_watchdog.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    13108 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/config.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.210159 mosaicml-cli-0.5.1/mcli/models/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1047 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/models/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2103 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/models/gpu_type.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    12287 2023-07-26 00:26:41.000000 mosaicml-cli-0.5.1/mcli/models/inference_deployment_config.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      427 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/models/mcli_cluster.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      456 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/models/mcli_envvar.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6728 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/models/mcli_secret.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    17258 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/models/run_config.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.210283 mosaicml-cli-0.5.1/mcli/objects/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/__init__.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.211336 mosaicml-cli-0.5.1/mcli/objects/secrets/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1090 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.212626 mosaicml-cli-0.5.1/mcli/objects/secrets/create/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1646 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/base.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2244 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2408 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6377 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3858 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3001 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5342 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      783 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1017 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/env_var.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      556 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/gcp.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1267 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/mounted.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      967 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/oci.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      961 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/s3.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1718 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.212903 mosaicml-cli-0.5.1/mcli/proto/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/proto/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1477 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.213067 mosaicml-cli-0.5.1/mcli/sdk/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2006 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/sdk/__init__.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.216058 mosaicml-cli-0.5.1/mcli/utils/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6318 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/utils/utils_cli.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4409 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/utils/utils_completers.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     7047 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_config.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      740 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_date.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    10749 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_docker.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2225 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_epilog.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    10774 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_interactive.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4527 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_logging.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2160 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1087 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/utils/utils_model.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6605 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_pypi.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3115 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_rich.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5358 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/utils/utils_run_status.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4350 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1103 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_spinner.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    10751 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_string_functions.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1677 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_types.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1001 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_yaml.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3876 2023-07-26 00:36:38.000000 mosaicml-cli-0.5.1/mcli/version.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.216784 mosaicml-cli-0.5.1/mosaicml_cli.egg-info/
--rw-r--r--   0 margaret.qian   (502) staff       (20)      696 2023-07-26 00:37:20.000000 mosaicml-cli-0.5.1/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5106 2023-07-26 00:37:20.000000 mosaicml-cli-0.5.1/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 margaret.qian   (502) staff       (20)        1 2023-07-26 00:37:20.000000 mosaicml-cli-0.5.1/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 margaret.qian   (502) staff       (20)       75 2023-07-26 00:37:20.000000 mosaicml-cli-0.5.1/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1654 2023-07-26 00:37:20.000000 mosaicml-cli-0.5.1/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 margaret.qian   (502) staff       (20)        5 2023-07-26 00:37:20.000000 mosaicml-cli-0.5.1/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 margaret.qian   (502) staff       (20)    31087 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/pyproject.toml
--rw-r--r--   0 margaret.qian   (502) staff       (20)       38 2023-07-26 00:37:20.217879 mosaicml-cli-0.5.1/setup.cfg
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3056 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/setup.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.217426 mosaicml-cli-0.5.1/tests/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6449 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/tests/test_config.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)       62 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/tests/test_simple.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6116 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/tests/test_upgrade.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.762686 mosaicml-cli-0.5.2/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      696 2023-07-27 22:06:59.762567 mosaicml-cli-0.5.2/PKG-INFO
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     7089 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/README.md
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.731190 mosaicml-cli-0.5.2/mcli/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2122 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/__init__.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.731972 mosaicml-cli-0.5.2/mcli/api/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/__init__.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.732274 mosaicml-cli-0.5.2/mcli/api/cluster/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      134 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/cluster/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5459 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.732480 mosaicml-cli-0.5.2/mcli/api/engine/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/engine/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    26027 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/engine/engine.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    13444 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/exceptions.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.739746 mosaicml-cli-0.5.2/mcli/api/inference_deployments/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1521 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3297 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5045 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3992 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     8413 2023-07-27 19:50:50.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2294 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_ping.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2746 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_predict_inference_deployment.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6499 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_update_inference_deployments.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.740175 mosaicml-cli-0.5.2/mcli/api/mint/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/mint/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     7840 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/mint/shell.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2676 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/mint/tty.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.740779 mosaicml-cli-0.5.2/mcli/api/model/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1114 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/model/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    10405 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/api/model/cluster_details.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4583 2023-07-27 19:50:50.000000 mosaicml-cli-0.5.2/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    14890 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/api/model/run.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.743071 mosaicml-cli-0.5.2/mcli/api/runs/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1269 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/runs/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3785 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_create_interactive_run.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3034 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4365 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     8796 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    12239 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5367 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5559 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5916 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_update_run.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4091 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    10414 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.743361 mosaicml-cli-0.5.2/mcli/api/schema/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/schema/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      636 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.743900 mosaicml-cli-0.5.2/mcli/api/secrets/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      309 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/secrets/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2386 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2943 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3665 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2354 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/typing_future.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.744186 mosaicml-cli-0.5.2/mcli/api/users/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      139 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/users/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2715 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/users/api_get_users.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      920 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/utils.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.744435 mosaicml-cli-0.5.2/mcli/cli/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/__init__.py
+-rwxr-xr-x   0 margaret.qian   (502) staff       (20)     6069 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/cli/cli.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.745179 mosaicml-cli-0.5.2/mcli/cli/common/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/common/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2560 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     7499 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.745509 mosaicml-cli-0.5.2/mcli/cli/m_connect/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6426 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.746083 mosaicml-cli-0.5.2/mcli/cli/m_create/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2385 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    16900 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.746744 mosaicml-cli-0.5.2/mcli/cli/m_delete/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6448 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5838 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.747137 mosaicml-cli-0.5.2/mcli/cli/m_deploy/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4253 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.748046 mosaicml-cli-0.5.2/mcli/cli/m_describe/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     8364 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/cli/m_describe/describe_clusters.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3929 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    13495 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2719 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.749449 mosaicml-cli-0.5.2/mcli/cli/m_get/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      467 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     7069 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6459 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/display.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5807 2023-07-27 19:50:50.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4804 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     8967 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/runs.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2189 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1580 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/users.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.749743 mosaicml-cli-0.5.2/mcli/cli/m_init/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3908 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_init/m_init.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.750076 mosaicml-cli-0.5.2/mcli/cli/m_interactive/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     9036 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.750948 mosaicml-cli-0.5.2/mcli/cli/m_kube/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_kube/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5523 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_kube/m_get_config.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1398 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_kube/m_kube.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2050 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_kube/m_merge_config.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6946 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_kube/utils.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.751210 mosaicml-cli-0.5.2/mcli/cli/m_log/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    11756 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.751553 mosaicml-cli-0.5.2/mcli/cli/m_ping/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1411 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.751860 mosaicml-cli-0.5.2/mcli/cli/m_predict/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1905 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.752181 mosaicml-cli-0.5.2/mcli/cli/m_root/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      536 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.752415 mosaicml-cli-0.5.2/mcli/cli/m_run/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    11501 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.753593 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2964 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1793 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2267 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1656 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      840 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/organization.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      745 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.753787 mosaicml-cli-0.5.2/mcli/cli/m_stop/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4062 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.754018 mosaicml-cli-0.5.2/mcli/cli/m_update/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_update/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6568 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/cli/m_update/m_update.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.754444 mosaicml-cli-0.5.2/mcli/cli/m_util/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      797 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     9035 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/cli/m_util/util.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.754629 mosaicml-cli-0.5.2/mcli/cli/m_watchdog/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_watchdog/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3544 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/cli/m_watchdog/m_watchdog.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    13108 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/config.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.755578 mosaicml-cli-0.5.2/mcli/models/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1047 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/models/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2103 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/models/gpu_type.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    12287 2023-07-26 00:26:41.000000 mosaicml-cli-0.5.2/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      427 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/models/mcli_cluster.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      456 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/models/mcli_envvar.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6728 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/models/mcli_secret.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    17258 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/models/run_config.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.755850 mosaicml-cli-0.5.2/mcli/objects/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/__init__.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.756774 mosaicml-cli-0.5.2/mcli/objects/secrets/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1090 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.757927 mosaicml-cli-0.5.2/mcli/objects/secrets/create/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1646 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2244 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2408 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6377 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3858 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3001 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5342 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      783 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1017 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      556 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1267 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      967 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/oci.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      961 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/s3.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1718 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.758155 mosaicml-cli-0.5.2/mcli/proto/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/proto/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1477 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.758305 mosaicml-cli-0.5.2/mcli/sdk/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2006 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/sdk/__init__.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.761089 mosaicml-cli-0.5.2/mcli/utils/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6318 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/utils/utils_cli.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4409 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/utils/utils_completers.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     7047 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_config.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      740 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_date.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    10749 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_docker.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2225 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_epilog.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    10774 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_interactive.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4527 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_logging.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2160 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1087 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/utils/utils_model.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6605 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_pypi.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3115 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_rich.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5358 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/utils/utils_run_status.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4350 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1103 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_spinner.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    10751 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1677 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_types.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1001 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_yaml.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3876 2023-07-27 22:06:24.000000 mosaicml-cli-0.5.2/mcli/version.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.761745 mosaicml-cli-0.5.2/mosaicml_cli.egg-info/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      696 2023-07-27 22:06:59.000000 mosaicml-cli-0.5.2/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5147 2023-07-27 22:06:59.000000 mosaicml-cli-0.5.2/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        1 2023-07-27 22:06:59.000000 mosaicml-cli-0.5.2/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 margaret.qian   (502) staff       (20)       75 2023-07-27 22:06:59.000000 mosaicml-cli-0.5.2/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1654 2023-07-27 22:06:59.000000 mosaicml-cli-0.5.2/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        5 2023-07-27 22:06:59.000000 mosaicml-cli-0.5.2/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    31087 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/pyproject.toml
+-rw-r--r--   0 margaret.qian   (502) staff       (20)       38 2023-07-27 22:06:59.762722 mosaicml-cli-0.5.2/setup.cfg
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3056 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/setup.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.762310 mosaicml-cli-0.5.2/tests/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6449 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/tests/test_config.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)       62 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/tests/test_simple.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6116 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.5.1/PKG-INFO` & `mosaicml-cli-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.5.1
+Version: 0.5.2
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.5.1/README.md` & `mosaicml-cli-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/__init__.py` & `mosaicml-cli-0.5.2/mcli/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.5.2/mcli/api/cluster/api_get_clusters.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,43 +19,69 @@
 query GetClusters(${VARIABLE_DATA_NAME}: GetClustersInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
     name
     provider
     allowFractional
     allowMultinode
-    allowedSubmissionType
+    allowedSubmissionTypes
+    isMultiTenant
+    schedulerEnabled
     allowedInstances {{
       name
       gpuType
       gpusPerNode
+      cpus
+      memory
+      storage
       gpuNums
       numNodes
       nodes {{
         name
         isAlive
         isSchedulable
+        upTime {{
+          endDate
+          startDate
+        }}
       }}
     }}
   }}
 }}"""
 QUERY_UTILIZATION = f"""
 query GetClusters(${VARIABLE_DATA_NAME}: GetClustersInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
     name
     provider
-    allowedSubmissionType
+    allowedSubmissionTypes
+    isMultiTenant
+    schedulerEnabled
     utilization {{
-      clusterInstanceUtils {{
+      instanceUtils {{
+        instance {{
+          name
+          gpuType
+          gpuNums      
+          gpusPerNode
+          cpus
+          memory
+          storage
+          numNodes
+          nodes {{
+            name
+            isAlive
+            isSchedulable
+            upTime {{
+              endDate
+              startDate
+            }}
+          }}
+        }}
         clusterId
-        name
-        gpuType
-        gpusPerNode
-        numNodes
         gpusUsed
         gpusAvailable
         gpusTotal
       }}
       activeRunsByUser{{
         id
         createdAt
```

### Comparing `mosaicml-cli-0.5.1/mcli/api/engine/engine.py` & `mosaicml-cli-0.5.2/mcli/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/exceptions.py` & `mosaicml-cli-0.5.2/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.5.2/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_get_inference_deployment_logs.py` & `mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_get_inference_deployment_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_ping.py` & `mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_update_inference_deployments.py` & `mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_update_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/mint/shell.py` & `mosaicml-cli-0.5.2/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/mint/tty.py` & `mosaicml-cli-0.5.2/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/model/__init__.py` & `mosaicml-cli-0.5.2/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.5.2/mcli/api/model/cluster_details.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """ MCLI Abstraction for Clusters and Utilization """
 from __future__ import annotations
 
 import functools
 import logging
 from dataclasses import dataclass, field
 from datetime import datetime
+from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Set
 
 from dateutil import parser
 
-from mcli.api.exceptions import MAPI_DESERIALIZATION_ERROR
+from mcli.api.exceptions import MAPIException
 from mcli.api.schema.generic_model import DeserializableModel
 from mcli.models.run_config import SchedulingConfig, SchedulingTranslation
 from mcli.utils.utils_model import SubmissionType
 from mcli.utils.utils_serializable_dataclass import SerializableDataclass
 
 logger = logging.getLogger(__name__)
 
 
 def check_response(response: Dict[str, Any], expected: Set[str]) -> None:
     missing = expected - set(response)
     if missing:
-        raise MAPI_DESERIALIZATION_ERROR
+        raise MAPIException(HTTPStatus.INTERNAL_SERVER_ERROR, f'Missing fields in response: {", ".join(missing)}')
 
 
 @dataclass
 class ClusterUtilizationByDeployment:
     """Utilization for a specific run on a cluster
     """
 
@@ -86,34 +87,35 @@
                    scheduling=SchedulingTranslation.from_mapi(response.get('scheduling', {})))
 
 
 @dataclass
 class InstanceUtilization:
     """Utilization on a cluster instance
     """
+    instance: Instance
     cluster_id: str
     name: str
-    gpu_type: str
-    gpus_per_node: int
-    num_nodes: int
+    gpu_type: str  # TODO: Deprecate and pull gpu_type from `instance`
+    gpus_per_node: int  # TODO: Deprecate and pull gpus_per_node from `instance`
+    num_nodes: int  # TODO: Deprecate and pull from `instance`
     gpus_used: int
     gpus_available: int
     gpus_total: int
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> InstanceUtilization:
-        check_response(
-            response,
-            {'clusterId', 'name', 'gpuType', 'gpusPerNode', 'numNodes', 'gpusUsed', 'gpusAvailable', 'gpusTotal'})
+        check_response(response, {'clusterId', 'instance', 'gpusUsed', 'gpusAvailable', 'gpusTotal'})
+        instance = Instance.from_mapi_response(response['instance'])
         return cls(
+            instance=instance,
             cluster_id=response['clusterId'],
-            name=response['name'],
-            gpu_type=response['gpuType'],
-            gpus_per_node=response['gpusPerNode'],
-            num_nodes=response['numNodes'],
+            name=instance.name,
+            gpu_type=instance.gpu_type,
+            gpus_per_node=instance.gpus,
+            num_nodes=instance.nodes,
             gpus_used=response['gpusUsed'],
             gpus_available=response['gpusAvailable'],
             gpus_total=response['gpusTotal'],
         )
 
     def __gt__(self, other: InstanceUtilization):
         return self.gpus_available == 0 or self.name > other.name
@@ -138,20 +140,20 @@
         else:
             return self.active_deployments_by_user if is_active else self.queued_deployments_by_user
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> ClusterUtilization:
         check_response(
             response, {
-                'clusterInstanceUtils', 'activeRunsByUser', 'queuedRunsByUser', 'activeDeploymentsByUser',
+                'instanceUtils', 'activeRunsByUser', 'queuedRunsByUser', 'activeDeploymentsByUser',
                 'queuedDeploymentsByUser', 'anonymizeUsers'
             })
         return cls(
             cluster_instance_utils=sorted(
-                [InstanceUtilization.from_mapi_response(i) for i in response['clusterInstanceUtils']]),
+                [InstanceUtilization.from_mapi_response(i) for i in response['instanceUtils']]),
             active_by_user=[ClusterUtilizationByRun.from_mapi_response(i) for i in response['activeRunsByUser']],
             queued_by_user=[ClusterUtilizationByRun.from_mapi_response(i) for i in response['queuedRunsByUser']],
             active_runs_by_user=[ClusterUtilizationByRun.from_mapi_response(i) for i in response['activeRunsByUser']],
             queued_runs_by_user=[ClusterUtilizationByRun.from_mapi_response(i) for i in response['queuedRunsByUser']],
             active_deployments_by_user=[
                 ClusterUtilizationByDeployment.from_mapi_response(i) for i in response['activeDeploymentsByUser']
             ],
@@ -179,27 +181,33 @@
 @functools.total_ordering
 class Instance:
     """Instance of a cluster
     """
     name: str
     gpu_type: str
     gpus: int
+    cpus: Optional[int]
+    memory: str
+    storage: str
     nodes: int
-    gpu_nums: List[int] = field(default_factory=list)
+    gpu_nums: List[int] = field(default_factory=list)  # TODO: Deprecate, no longer used
     node_details: List[Node] = field(default_factory=list)
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> Instance:
-        check_response(response, {'name', 'gpusPerNode', 'numNodes', 'gpuType', 'gpuNums', 'nodes'})
+        check_response(response, {'name', 'gpusPerNode', 'numNodes', 'gpuType', 'nodes'})
         return cls(
             name=response['name'],
             gpu_type=response['gpuType'],
             gpus=response['gpusPerNode'],
+            cpus=response['cpus'] if 'cpus' in response else None,
+            memory=response['memory'] if 'memory' in response else '',
+            storage=response['storage'] if 'storage' in response else '',
             nodes=response['numNodes'],
-            gpu_nums=response['gpuNums'],
+            gpu_nums=response['gpuNums'] if 'gpuNums' in response else [],
             node_details=[Node.from_mapi_response(i) for i in response.get('nodes', [])],
         )
 
     def __lt__(self, other: Instance):
         if self.gpu_type.lower() == 'none':
             return True
         return self.gpu_type < other.gpu_type
@@ -225,31 +233,38 @@
     """
 
     name: str
     provider: str = 'MosaicML'
     allow_fractional: bool = False
     allow_multinode: bool = False
     cluster_instances: List[Instance] = field(default_factory=list)
-    submission_type: SubmissionType = field(default_factory=SubmissionType)
+    submission_type: Optional[SubmissionType] = None
+    submission_types: List[SubmissionType] = field(default_factory=list)
+    is_multitenant: bool = False
+    scheduler_enabled: bool = False
     utilization: Optional[ClusterUtilization] = None
 
     kubernetes_context: str = ''
     namespace: str = ''
 
     id: Optional[str] = None
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> ClusterDetails:
         check_response(response, {'name'})
         utilization = None if 'utilization' not in response else ClusterUtilization.from_mapi_response(
             response['utilization'])
+        submission_types = [SubmissionType.from_mapi(type) for type in response.get('allowedSubmissionTypes', [])]
         return cls(name=response['name'],
                    provider=get_provider_name(response.get('provider', '')),
                    allow_fractional=response.get('allowFractional', False),
                    allow_multinode=response.get('allowMultinode', False),
                    cluster_instances=[Instance.from_mapi_response(i) for i in response.get('allowedInstances', [])],
-                   submission_type=SubmissionType.from_mapi(response.get('allowedSubmissionType', '')),
+                   submission_type=submission_types[0] if submission_types else None,
+                   submission_types=submission_types,
+                   is_multitenant=response.get('isMultiTenant', False),
+                   scheduler_enabled=response.get('schedulerEnabled', False),
                    utilization=utilization,
                    id=response.get('id'))
 
     def __lt__(self, other: ClusterDetails):
         return self.name < other.name
```

### Comparing `mosaicml-cli-0.5.1/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.5.2/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/model/run.py` & `mosaicml-cli-0.5.2/mcli/api/model/run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/runs/__init__.py` & `mosaicml-cli-0.5.2/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/runs/api_create_interactive_run.py` & `mosaicml-cli-0.5.2/mcli/api/runs/api_create_interactive_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.5.2/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.5.2/mcli/api/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.5.2/mcli/api/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.5.2/mcli/api/runs/api_get_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.5.2/mcli/api/runs/api_start_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     completedAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
-   resumptions {{
+    resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
         executionIndex
         startTime
```

### Comparing `mosaicml-cli-0.5.1/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.5.2/mcli/api/runs/api_stop_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/runs/api_update_run.py` & `mosaicml-cli-0.5.2/mcli/api/runs/api_update_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.5.2/mcli/api/runs/api_update_run_metadata.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.5.2/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.5.2/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.5.2/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.5.2/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.5.2/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/typing_future.py` & `mosaicml-cli-0.5.2/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.5.2/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/api/utils.py` & `mosaicml-cli-0.5.2/mcli/api/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/cli.py` & `mosaicml-cli-0.5.2/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.5.2/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.5.2/mcli/cli/common/run_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.5.2/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.5.2/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.5.2/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.5.2/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.5.2/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.5.2/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.5.2/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.5.2/mcli/cli/m_describe/describe_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.5.2/mcli/cli/m_describe/m_describe.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ mcli describe Endpoint """
 from __future__ import annotations
 
 import argparse
 import logging
 
+from mcli.cli.m_describe.describe_clusters import describe_cluster
 from mcli.cli.m_describe.describe_inference_deployments import describe_deploy
 from mcli.cli.m_describe.describe_runs import describe_run
 from mcli.utils import utils_completers
 
 logger = logging.getLogger(__name__)
 
 
@@ -35,14 +36,20 @@
         type=str,
         help='Inference Deployment name',
     )
     deployment_name_parser.completer = utils_completers.DeploymentNameCompleter()  # pyright: ignore
     deploy_parser.set_defaults(func=describe_deploy)
 
 
+def describe_cluster_argparser(subparser: argparse._SubParsersAction) -> None:
+    cluster_parser = subparser.add_parser('cluster', help='List instances and utilization of a specific cluster')
+    cluster_parser.add_argument('cluster_name', type=str, nargs='?', help='Cluster name')
+    cluster_parser.set_defaults(func=describe_cluster)
+
+
 def add_describe_parser(subparser: argparse._SubParsersAction) -> argparse.ArgumentParser:
     describe_parser: argparse.ArgumentParser = subparser.add_parser(
         'describe',
         help='Get detailed information on an object',
     )
     return _configure_argparser(parser=describe_parser)
 
@@ -51,8 +58,9 @@
     subparsers = parser.add_subparsers(title='MCLI Objects',
                                        description='The table below shows the objects that you can describe',
                                        help='DESCRIPTION',
                                        metavar='OBJECT')
     parser.set_defaults(func=describe_entrypoint, parser=parser)
     describe_runs_argparser(subparser=subparsers)
     describe_deployments_argparser(subparser=subparsers)
+    describe_cluster_argparser(subparser=subparsers)
     return parser
```

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.5.2/mcli/cli/m_get/clusters.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
                 # cpu instance sometimes captures non-worker nodes, so we'll just set
                 # the value to 1 (unless it was 0)
                 nodes = get_nodes_description(instance.nodes)
                 if instance.name == 'cpu' and nodes != '-':
                     nodes = '1'
 
-                if self.submission_type is c.submission_type:
+                if self.submission_type in c.submission_types:
                     yield ClusterDisplayItem(
                         id=c.id if self.include_ids else None,
                         name=c.name,
                         provider=c.provider,
                         instance=instance.name,
                         nodes=nodes,
                         gpu_type=instance.gpu_type.lower(),
```

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_get/display.py` & `mosaicml-cli-0.5.2/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.5.2/mcli/cli/m_get/inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.5.2/mcli/cli/m_get/m_get.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.5.2/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.5.2/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_get/users.py` & `mosaicml-cli-0.5.2/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.5.2/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.5.2/mcli/cli/m_interactive/m_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_kube/m_get_config.py` & `mosaicml-cli-0.5.2/mcli/cli/m_kube/m_get_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_kube/m_kube.py` & `mosaicml-cli-0.5.2/mcli/cli/m_kube/m_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_kube/m_merge_config.py` & `mosaicml-cli-0.5.2/mcli/cli/m_kube/m_merge_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_kube/utils.py` & `mosaicml-cli-0.5.2/mcli/cli/m_kube/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.5.2/mcli/cli/m_log/m_log.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.5.2/mcli/cli/m_ping/m_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.5.2/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.5.2/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.5.2/mcli/cli/m_run/m_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.5.2/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.5.2/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.5.2/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.5.2/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_set_unset/organization.py` & `mosaicml-cli-0.5.2/mcli/cli/m_set_unset/organization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.5.2/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.5.2/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_update/m_update.py` & `mosaicml-cli-0.5.2/mcli/cli/m_update/m_update.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.5.2/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_util/util.py` & `mosaicml-cli-0.5.2/mcli/cli/m_util/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
             e.message = MAPIErrorMessages.NOT_FOUND_CLUSTER.value
         raise e
 
     if len(c) == 0:
         raise MAPIException(HTTPStatus.NOT_FOUND, f'No clusters found with name(s): {clusters}')
     # for submission_type in SubmissionType:
     for i, submission_type in enumerate(SubmissionType):
-        submission_cluster = [cluster for cluster in c if cluster.submission_type is submission_type]
+        submission_cluster = [cluster for cluster in c if submission_type in cluster.submission_types]
         if len(submission_cluster) == 0:
             continue
         agg = ''
         if len({cluster.name for cluster in submission_cluster}) > 1:
             agg = ' by Cluster'
 
         print(f'{submission_type.name.capitalize()} Instances{agg}:')
```

### Comparing `mosaicml-cli-0.5.1/mcli/cli/m_watchdog/m_watchdog.py` & `mosaicml-cli-0.5.2/mcli/cli/m_watchdog/m_watchdog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/config.py` & `mosaicml-cli-0.5.2/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/models/__init__.py` & `mosaicml-cli-0.5.2/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/models/gpu_type.py` & `mosaicml-cli-0.5.2/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.5.2/mcli/models/inference_deployment_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/models/mcli_secret.py` & `mosaicml-cli-0.5.2/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/models/run_config.py` & `mosaicml-cli-0.5.2/mcli/models/run_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.5.2/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.5.2/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.5.2/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.5.2/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.5.2/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.5.2/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.5.2/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.5.2/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.5.2/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.5.2/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.5.2/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.5.2/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.5.2/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.5.2/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.5.2/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.5.2/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/sdk/__init__.py` & `mosaicml-cli-0.5.2/mcli/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_cli.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_completers.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_completers.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_config.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_date.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_docker.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_logging.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_model.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,14 @@
             return ["Pending", "Starting", "Ready", "Failed", "Stopped"]
 
     @classmethod
     def from_mapi(cls, value: str) -> SubmissionType:
         try:
             extracted = SubmissionType[value]
         except KeyError:
-            logger.warning('Recieved invalid value for Submission Type. Defaulting to TRAINING')
+            logger.warning('Received invalid value for Submission Type. Defaulting to TRAINING')
             extracted = SubmissionType.TRAINING
         return extracted
 
     def __eq__(self, other: object) -> bool:
         assert isinstance(other, SubmissionType)
         return self.name == other.name
```

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_rich.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_types.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.5.2/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/mcli/version.py` & `mosaicml-cli-0.5.2/mcli/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.5.1/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.5.2/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.5.1
+Version: 0.5.2
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.5.1/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.5.2/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 mcli/cli/m_create/secret.py
 mcli/cli/m_delete/__init__.py
 mcli/cli/m_delete/delete.py
 mcli/cli/m_delete/m_delete.py
 mcli/cli/m_deploy/__init__.py
 mcli/cli/m_deploy/m_deploy.py
 mcli/cli/m_describe/__init__.py
+mcli/cli/m_describe/describe_clusters.py
 mcli/cli/m_describe/describe_inference_deployments.py
 mcli/cli/m_describe/describe_runs.py
 mcli/cli/m_describe/m_describe.py
 mcli/cli/m_get/__init__.py
 mcli/cli/m_get/clusters.py
 mcli/cli/m_get/display.py
 mcli/cli/m_get/inference_deployments.py
```

### Comparing `mosaicml-cli-0.5.1/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.5.2/mosaicml_cli.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -9,47 +9,47 @@
 questionary>=1.10.0
 rich>=12.6.0
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 validators>=0.20.0
 
 [all]
-sphinxcontrib-qthelp>=1.0.3
-sphinxcontrib-htmlhelp>=2.0.0
-toml>=0.10.2
-sphinx-markdown-tables==0.0.17
-myst-parser>=0.16.1
-pylint>=2.12.2
-sphinx==4.4.0
-sphinxcontrib-devhelp>=1.0.2
-sphinx-argparse==0.4.0
-pytest-mock>=3.7.0
-sphinx-panels==0.6.0
-pyright==1.1.256
-sphinx-rtd-theme==1.0.0
-twine>=4.0.2
-radon>=5.1.0
-pytest-cov>=4.0.0
-sphinxcontrib-jsmath>=1.0.1
 sphinxext-opengraph==0.8.2
-yapf>=0.33.0
+sphinxcontrib-jsmath>=1.0.1
+pytest-mock>=3.7.0
+sphinxcontrib-serializinghtml==1.1.5
 sphinx-design
+docutils>=0.17.0
 sphinx-copybutton==0.5.2
+sphinx-markdown-tables==0.0.17
+isort>=5.9.3
+sphinx_external_toc==0.3.0
+sphinxcontrib-applehelp>=1.0.2
+sphinxcontrib-htmlhelp>=2.0.0
 pre-commit>=2.17.0
 sphinxcontrib-katex==0.9.4
-docutils>=0.17.0
+toml>=0.10.2
+pyright==1.1.256
+sphinxemoji==0.2.0
+twine>=4.0.2
+sphinx-rtd-theme==1.0.0
+radon>=5.1.0
 pytest>=6.2.5
-build>=0.10.0
-sphinxcontrib-applehelp>=1.0.2
-isort>=5.9.3
-sphinxcontrib-serializinghtml==1.1.5
-sphinx_external_toc==0.3.0
 sphinxcontrib-images>=0.9.4
+sphinx==4.4.0
+pytest-cov>=4.0.0
+myst-parser>=0.16.1
+sphinx-panels==0.6.0
+build>=0.10.0
+pylint>=2.12.2
+sphinxcontrib-qthelp>=1.0.3
+yapf>=0.33.0
+sphinxcontrib-devhelp>=1.0.2
 furo==2022.9.29
-sphinxemoji==0.2.0
+sphinx-argparse==0.4.0
 
 [dev]
 build>=0.10.0
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright==1.1.256
```

### Comparing `mosaicml-cli-0.5.1/pyproject.toml` & `mosaicml-cli-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/setup.py` & `mosaicml-cli-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/tests/test_config.py` & `mosaicml-cli-0.5.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.1/tests/test_upgrade.py` & `mosaicml-cli-0.5.2/tests/test_upgrade.py`

 * *Files identical despite different names*

