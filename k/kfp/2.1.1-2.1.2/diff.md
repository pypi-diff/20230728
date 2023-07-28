# Comparing `tmp/kfp-2.1.1.tar.gz` & `tmp/kfp-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfp-2.1.1.tar", last modified: Thu Jul 27 17:15:22 2023, max compression
+gzip compressed data, was "/var/folders/s4/q287k45x17x_j2mlv1lc_43r00xv1g/T/tmp.H37Vgq72/kfp-2.1.2.tar", last modified: Fri Jul 28 20:47:19 2023, max compression
```

## Comparing `kfp-2.1.1.tar` & `kfp-2.1.2.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.921663 kfp-2.1.1/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       60 2023-07-08 15:08:27.000000 kfp-2.1.1/MANIFEST.in
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3775 2023-07-27 17:15:22.921509 kfp-2.1.1/PKG-INFO
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1972 2023-07-24 19:29:12.000000 kfp-2.1.1/README.md
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.895246 kfp-2.1.1/kfp/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      909 2023-07-27 01:00:40.000000 kfp-2.1.1/kfp/__init__.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.898441 kfp-2.1.1/kfp/cli/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      878 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/__main__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4024 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7072 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/cli_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5377 2023-07-24 19:29:12.000000 kfp-2.1.1/kfp/cli/compile_.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2304 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/compile_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16208 2023-07-24 19:29:12.000000 kfp-2.1.1/kfp/cli/component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    23333 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/component_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.899704 kfp-2.1.1/kfp/cli/diagnose_me/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2460 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me/dev_env.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2694 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me/dev_env_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6098 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me/gcp.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3786 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me/gcp_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4495 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me/kubernetes_cluster.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3280 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me/kubernetes_cluster_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3040 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/diagnose_me/utility.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2714 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/diagnose_me/utility_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me_cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      744 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/dsl.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5369 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/experiment.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7225 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/output.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8364 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/pipeline.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9395 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/recurring_run.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7291 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/run.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.900739 kfp-2.1.1/kfp/cli/utils/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/utils/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1434 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/utils/aliased_plurals_group.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1684 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/utils/aliased_plurals_group_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2439 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/utils/deprecated_alias_group.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1595 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/utils/deprecated_alias_group_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2568 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/utils/parsing.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4169 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/utils/parsing_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.902476 kfp-2.1.1/kfp/client/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      998 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/client/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20239 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/client/auth.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    66575 2023-07-24 19:29:12.000000 kfp-2.1.1/kfp/client/client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18470 2023-07-24 19:29:12.000000 kfp-2.1.1/kfp/client/client_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3269 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/client/set_volume_credentials.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1926 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/client/set_volume_credentials_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1765 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/client/token_credentials_base.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2390 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/client/token_credentials_base_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.903907 kfp-2.1.1/kfp/compiler/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      749 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/compiler/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3429 2023-07-24 19:29:12.000000 kfp-2.1.1/kfp/compiler/compiler.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)   153764 2023-07-27 17:14:48.000000 kfp-2.1.1/kfp/compiler/compiler_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    33889 2023-07-27 17:14:48.000000 kfp-2.1.1/kfp/compiler/compiler_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1958 2023-07-24 19:29:12.000000 kfp-2.1.1/kfp/compiler/compiler_utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    85340 2023-07-27 17:14:48.000000 kfp-2.1.1/kfp/compiler/pipeline_spec_builder.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16862 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/compiler/pipeline_spec_builder_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8175 2023-07-26 17:38:47.000000 kfp-2.1.1/kfp/compiler/read_write_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.904374 kfp-2.1.1/kfp/components/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1314 2023-07-24 19:29:12.000000 kfp-2.1.1/kfp/components/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6576 2023-07-26 00:11:33.000000 kfp-2.1.1/kfp/components/load_yaml_utilities.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5668 2023-07-26 00:11:33.000000 kfp-2.1.1/kfp/components/load_yaml_utilities_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.905912 kfp-2.1.1/kfp/deprecated/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      811 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      767 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/__main__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9693 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/_auth.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63369 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/deprecated/_client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      799 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/_config.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20892 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/_local_client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3829 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/_runners.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.906304 kfp-2.1.1/kfp/deprecated/auth/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      859 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/auth/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2594 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/auth/_satvolumecredentials.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1551 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/auth/_tokencredentialsbase.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2561 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/aws.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2272 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/azure.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.907810 kfp-2.1.1/kfp/deprecated/cli/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      584 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3038 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15615 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/components.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17870 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/components_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.909141 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2489 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/dev_env.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2734 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/dev_env_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6151 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/gcp.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3826 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/gcp_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4547 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3320 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3169 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/utility.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1529 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/utility_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3729 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me_cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4548 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/experiment.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2156 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/output.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9207 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/pipeline.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7544 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/recurring_run.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7476 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/run.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.910481 kfp-2.1.1/kfp/deprecated/compiler/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      761 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    24589 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/_data_passing_rewriter.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    12032 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/_data_passing_using_volume.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3480 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/_default_transformers.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3168 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/_k8s_helper.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    14459 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/_op_to_template.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    58420 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/compiler.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5028 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/main.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6946 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/v2_compat.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7033 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/v2_compatible_compiler_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.912584 kfp-2.1.1/kfp/deprecated/components/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      740 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6680 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_airflow_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16145 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_component_store.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25925 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_components.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8214 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_data_passing.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3572 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_dynamic.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2552 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_key_value_store.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4189 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_naming.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    52469 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_python_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9535 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_python_to_graph_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    29100 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_structures.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2757 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_yaml_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17572 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/modelbase.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.912718 kfp-2.1.1/kfp/deprecated/components/structures/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       28 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/structures/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1917 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/type_annotation_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2809 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/type_annotation_utils_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.913970 kfp-2.1.1/kfp/deprecated/containers/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      581 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7468 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/_build_image_api.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2527 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/_cache.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17356 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/_component_builder.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10904 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/_container_builder.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3603 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/_gcs_helper.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7344 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/_k8s_job_helper.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8735 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/entrypoint.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7158 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/entrypoint_utils.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.919140 kfp-2.1.1/kfp/deprecated/dsl/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1665 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6364 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    30557 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_component_bridge.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63751 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_container_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1865 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_container_op_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10053 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_for_loop.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3857 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_metadata.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8123 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_ops_group.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    13111 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_pipeline.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9125 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_pipeline_param.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4483 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_pipeline_volume.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8409 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_resource_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6057 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_volume_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4771 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_volume_snapshot_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7871 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/artifact.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3439 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/artifact_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18942 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/component_spec.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25290 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/component_spec_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1210 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/data_passing_methods.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5155 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/dsl_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2119 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/dsl_utils_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.919398 kfp-2.1.1/kfp/deprecated/dsl/extensions/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/extensions/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/extensions/kubernetes.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1311 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/io_types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6121 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/metrics_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2330 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/metrics_utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1367 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/serialization_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1221 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/serialization_utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3750 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/type_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7886 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5984 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/gcp.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.919673 kfp-2.1.1/kfp/deprecated/notebook/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      607 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/notebook/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/notebook/_magic.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4757 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/onprem.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.920106 kfp-2.1.1/kfp/registry/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      837 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/registry/__init__.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.920552 kfp-2.1.1/kfp/registry/context/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/registry/context/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1060 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/registry/context/default_pkg_dev.json
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2381 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/registry/context/kfp_pkg_dev.json
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    21147 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/registry/registry_client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17404 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/registry/registry_client_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.921110 kfp-2.1.1/kfp/v2/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      921 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/v2/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      621 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/v2/compiler.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      623 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/v2/components.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      616 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/v2/dsl.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.896235 kfp-2.1.1/kfp.egg-info/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3775 2023-07-27 17:15:22.000000 kfp-2.1.1/kfp.egg-info/PKG-INFO
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5840 2023-07-27 17:15:22.000000 kfp-2.1.1/kfp.egg-info/SOURCES.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        1 2023-07-27 17:15:22.000000 kfp-2.1.1/kfp.egg-info/dependency_links.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      142 2023-07-27 17:15:22.000000 kfp-2.1.1/kfp.egg-info/entry_points.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      466 2023-07-27 17:15:22.000000 kfp-2.1.1/kfp.egg-info/requires.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        4 2023-07-27 17:15:22.000000 kfp-2.1.1/kfp.egg-info/top_level.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1293 2023-07-27 01:00:40.000000 kfp-2.1.1/requirements.in
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       38 2023-07-27 17:15:22.921710 kfp-2.1.1/setup.cfg
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3769 2023-07-12 22:27:24.000000 kfp-2.1.1/setup.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.921257 kfp-2.1.1/tests/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      158 2023-07-08 15:08:27.000000 kfp-2.1.1/tests/test_kfp.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       60 2023-07-08 15:08:27.000000 kfp-2.1.2/MANIFEST.in
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3775 2023-07-28 20:47:19.000000 kfp-2.1.2/PKG-INFO
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1972 2023-07-24 19:29:12.000000 kfp-2.1.2/README.md
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      909 2023-07-28 18:10:05.000000 kfp-2.1.2/kfp/__init__.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/cli/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      878 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/__main__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4024 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7072 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/cli_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5377 2023-07-24 19:29:12.000000 kfp-2.1.2/kfp/cli/compile_.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2304 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/compile_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16208 2023-07-24 19:29:12.000000 kfp-2.1.2/kfp/cli/component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    23333 2023-07-12 22:27:23.000000 kfp-2.1.2/kfp/cli/component_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/cli/diagnose_me/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/diagnose_me/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2460 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/diagnose_me/dev_env.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2694 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/diagnose_me/dev_env_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6098 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/diagnose_me/gcp.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3786 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/diagnose_me/gcp_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4495 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/diagnose_me/kubernetes_cluster.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3280 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/diagnose_me/kubernetes_cluster_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3040 2023-07-12 22:27:23.000000 kfp-2.1.2/kfp/cli/diagnose_me/utility.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2714 2023-07-12 22:27:23.000000 kfp-2.1.2/kfp/cli/diagnose_me/utility_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/diagnose_me_cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      744 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/dsl.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5369 2023-07-12 22:27:23.000000 kfp-2.1.2/kfp/cli/experiment.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7225 2023-07-12 22:27:23.000000 kfp-2.1.2/kfp/cli/output.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8364 2023-07-12 22:27:23.000000 kfp-2.1.2/kfp/cli/pipeline.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9395 2023-07-12 22:27:23.000000 kfp-2.1.2/kfp/cli/recurring_run.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7291 2023-07-12 22:27:23.000000 kfp-2.1.2/kfp/cli/run.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/cli/utils/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/utils/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1434 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/utils/aliased_plurals_group.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1684 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/utils/aliased_plurals_group_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2439 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/utils/deprecated_alias_group.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1595 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/utils/deprecated_alias_group_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2568 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/utils/parsing.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4169 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/cli/utils/parsing_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/client/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      998 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/client/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20239 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/client/auth.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    66575 2023-07-24 19:29:12.000000 kfp-2.1.2/kfp/client/client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18470 2023-07-24 19:29:12.000000 kfp-2.1.2/kfp/client/client_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3269 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/client/set_volume_credentials.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1926 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/client/set_volume_credentials_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1765 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/client/token_credentials_base.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2390 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/client/token_credentials_base_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/compiler/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      749 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/compiler/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3429 2023-07-24 19:29:12.000000 kfp-2.1.2/kfp/compiler/compiler.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)   153764 2023-07-27 17:14:48.000000 kfp-2.1.2/kfp/compiler/compiler_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    33889 2023-07-27 17:14:48.000000 kfp-2.1.2/kfp/compiler/compiler_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1958 2023-07-24 19:29:12.000000 kfp-2.1.2/kfp/compiler/compiler_utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    85340 2023-07-27 17:14:48.000000 kfp-2.1.2/kfp/compiler/pipeline_spec_builder.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16862 2023-07-12 22:27:23.000000 kfp-2.1.2/kfp/compiler/pipeline_spec_builder_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8175 2023-07-26 17:38:47.000000 kfp-2.1.2/kfp/compiler/read_write_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/components/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1547 2023-07-27 23:59:47.000000 kfp-2.1.2/kfp/components/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6576 2023-07-26 00:11:33.000000 kfp-2.1.2/kfp/components/load_yaml_utilities.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5668 2023-07-26 00:11:33.000000 kfp-2.1.2/kfp/components/load_yaml_utilities_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/deprecated/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      811 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      767 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/__main__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9693 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/_auth.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63369 2023-07-12 22:27:23.000000 kfp-2.1.2/kfp/deprecated/_client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      799 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/_config.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20892 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/_local_client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3829 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/_runners.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/deprecated/auth/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      859 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/auth/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2594 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/auth/_satvolumecredentials.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1551 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/auth/_tokencredentialsbase.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2561 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/aws.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2272 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/azure.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/deprecated/cli/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      584 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3038 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15615 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/components.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17870 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/components_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/deprecated/cli/diagnose_me/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/diagnose_me/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2489 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/diagnose_me/dev_env.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2734 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/diagnose_me/dev_env_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6151 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/diagnose_me/gcp.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3826 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/diagnose_me/gcp_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4547 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3320 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3169 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/diagnose_me/utility.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1529 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/diagnose_me/utility_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3729 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/diagnose_me_cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4548 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/experiment.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2156 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/output.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9207 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/pipeline.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7544 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/recurring_run.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7476 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/cli/run.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/deprecated/compiler/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      761 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/compiler/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    24589 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/compiler/_data_passing_rewriter.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    12032 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/compiler/_data_passing_using_volume.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3480 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/compiler/_default_transformers.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3168 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/compiler/_k8s_helper.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    14459 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/compiler/_op_to_template.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    58420 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/compiler/compiler.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5028 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/compiler/main.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6946 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/compiler/v2_compat.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7033 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/compiler/v2_compatible_compiler_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/deprecated/components/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      740 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6680 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/_airflow_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16145 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/_component_store.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25925 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/_components.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8214 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/_data_passing.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3572 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/_dynamic.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2552 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/_key_value_store.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4189 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/_naming.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    52469 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/_python_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9535 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/_python_to_graph_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    29100 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/_structures.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2757 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/_yaml_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17572 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/modelbase.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/deprecated/components/structures/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       28 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/structures/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1917 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/type_annotation_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2809 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/components/type_annotation_utils_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/deprecated/containers/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      581 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/containers/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7468 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/containers/_build_image_api.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2527 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/containers/_cache.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17356 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/containers/_component_builder.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10904 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/containers/_container_builder.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3603 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/containers/_gcs_helper.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7344 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/containers/_k8s_job_helper.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8735 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/containers/entrypoint.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7158 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/containers/entrypoint_utils.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/deprecated/dsl/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1665 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6364 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    30557 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/_component_bridge.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63751 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/_container_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1865 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/_container_op_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10053 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/_for_loop.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3857 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/_metadata.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8123 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/_ops_group.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    13111 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/_pipeline.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9125 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/_pipeline_param.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4483 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/_pipeline_volume.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8409 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/_resource_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6057 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/_volume_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4771 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/_volume_snapshot_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7871 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/artifact.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3439 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/artifact_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18942 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/component_spec.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25290 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/component_spec_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1210 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/data_passing_methods.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5155 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/dsl_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2119 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/dsl_utils_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/deprecated/dsl/extensions/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/extensions/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/extensions/kubernetes.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1311 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/io_types.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6121 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/metrics_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2330 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/metrics_utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1367 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/serialization_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1221 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/serialization_utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3750 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/type_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7886 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/dsl/types.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5984 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/gcp.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/deprecated/notebook/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      607 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/notebook/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/notebook/_magic.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4757 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/deprecated/onprem.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/registry/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      837 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/registry/__init__.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/registry/context/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/registry/context/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1060 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/registry/context/default_pkg_dev.json
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2381 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/registry/context/kfp_pkg_dev.json
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    21147 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/registry/registry_client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17404 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/registry/registry_client_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp/v2/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1005 2023-07-27 23:59:47.000000 kfp-2.1.2/kfp/v2/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      621 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/v2/compiler.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      623 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/v2/components.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      616 2023-07-08 15:08:27.000000 kfp-2.1.2/kfp/v2/dsl.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp.egg-info/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3775 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp.egg-info/PKG-INFO
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5840 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp.egg-info/SOURCES.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        1 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp.egg-info/dependency_links.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      142 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp.egg-info/entry_points.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      466 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp.egg-info/requires.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        4 2023-07-28 20:47:19.000000 kfp-2.1.2/kfp.egg-info/top_level.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1293 2023-07-28 18:10:05.000000 kfp-2.1.2/requirements.in
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       38 2023-07-28 20:47:19.000000 kfp-2.1.2/setup.cfg
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3769 2023-07-12 22:27:24.000000 kfp-2.1.2/setup.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:47:19.000000 kfp-2.1.2/tests/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      158 2023-07-08 15:08:27.000000 kfp-2.1.2/tests/test_kfp.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `kfp-2.1.1/PKG-INFO` & `kfp-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfp
-Version: 2.1.1
+Version: 2.1.2
 Summary: Kubeflow Pipelines SDK
 Home-page: https://github.com/kubeflow/pipelines
 Author: The Kubeflow Authors
 License: UNKNOWN
 Project-URL: Documentation, https://kubeflow-pipelines.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/kubeflow/pipelines/issues
 Project-URL: Source, https://github.com/kubeflow/pipelines/tree/master/sdk
```

### Comparing `kfp-2.1.1/README.md` & `kfp-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/__init__.py` & `kfp-2.1.2/kfp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # `kfp` is a namespace package.
 # https://packaging.python.org/guides/packaging-namespace-packages/#pkgutil-style-namespace-packages
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
 
-__version__ = '2.1.1'
+__version__ = '2.1.2'
 
 TYPE_CHECK = True
 
 from kfp import components
 from kfp import dsl
 from kfp.client import Client
```

### Comparing `kfp-2.1.1/kfp/cli/__init__.py` & `kfp-2.1.2/kfp/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/__main__.py` & `kfp-2.1.2/kfp/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/cli.py` & `kfp-2.1.2/kfp/cli/cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/cli_test.py` & `kfp-2.1.2/kfp/cli/cli_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/compile_.py` & `kfp-2.1.2/kfp/cli/compile_.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/compile_test.py` & `kfp-2.1.2/kfp/cli/compile_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/component.py` & `kfp-2.1.2/kfp/cli/component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/component_test.py` & `kfp-2.1.2/kfp/cli/component_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/diagnose_me/__init__.py` & `kfp-2.1.2/kfp/cli/diagnose_me/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/diagnose_me/dev_env.py` & `kfp-2.1.2/kfp/cli/diagnose_me/dev_env.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/diagnose_me/dev_env_test.py` & `kfp-2.1.2/kfp/cli/diagnose_me/dev_env_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/diagnose_me/gcp.py` & `kfp-2.1.2/kfp/cli/diagnose_me/gcp.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/diagnose_me/gcp_test.py` & `kfp-2.1.2/kfp/cli/diagnose_me/gcp_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/diagnose_me/kubernetes_cluster.py` & `kfp-2.1.2/kfp/cli/diagnose_me/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/diagnose_me/kubernetes_cluster_test.py` & `kfp-2.1.2/kfp/cli/diagnose_me/kubernetes_cluster_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/diagnose_me/utility.py` & `kfp-2.1.2/kfp/cli/diagnose_me/utility.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/diagnose_me/utility_test.py` & `kfp-2.1.2/kfp/cli/diagnose_me/utility_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/diagnose_me_cli.py` & `kfp-2.1.2/kfp/cli/diagnose_me_cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/dsl.py` & `kfp-2.1.2/kfp/cli/dsl.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/experiment.py` & `kfp-2.1.2/kfp/cli/experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/output.py` & `kfp-2.1.2/kfp/cli/output.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/pipeline.py` & `kfp-2.1.2/kfp/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/recurring_run.py` & `kfp-2.1.2/kfp/cli/recurring_run.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/run.py` & `kfp-2.1.2/kfp/cli/run.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/utils/__init__.py` & `kfp-2.1.2/kfp/cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/utils/aliased_plurals_group.py` & `kfp-2.1.2/kfp/cli/utils/aliased_plurals_group.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/utils/aliased_plurals_group_test.py` & `kfp-2.1.2/kfp/cli/utils/aliased_plurals_group_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/utils/deprecated_alias_group.py` & `kfp-2.1.2/kfp/cli/utils/deprecated_alias_group.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/utils/deprecated_alias_group_test.py` & `kfp-2.1.2/kfp/cli/utils/deprecated_alias_group_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/utils/parsing.py` & `kfp-2.1.2/kfp/cli/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/cli/utils/parsing_test.py` & `kfp-2.1.2/kfp/cli/utils/parsing_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/client/__init__.py` & `kfp-2.1.2/kfp/client/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/client/auth.py` & `kfp-2.1.2/kfp/client/auth.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/client/client.py` & `kfp-2.1.2/kfp/client/client.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/client/client_test.py` & `kfp-2.1.2/kfp/client/client_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/client/set_volume_credentials.py` & `kfp-2.1.2/kfp/client/set_volume_credentials.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/client/set_volume_credentials_test.py` & `kfp-2.1.2/kfp/client/set_volume_credentials_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/client/token_credentials_base.py` & `kfp-2.1.2/kfp/client/token_credentials_base.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/client/token_credentials_base_test.py` & `kfp-2.1.2/kfp/client/token_credentials_base_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/compiler/__init__.py` & `kfp-2.1.2/kfp/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/compiler/compiler.py` & `kfp-2.1.2/kfp/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/compiler/compiler_test.py` & `kfp-2.1.2/kfp/compiler/compiler_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/compiler/compiler_utils.py` & `kfp-2.1.2/kfp/compiler/compiler_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/compiler/compiler_utils_test.py` & `kfp-2.1.2/kfp/compiler/compiler_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/compiler/pipeline_spec_builder.py` & `kfp-2.1.2/kfp/compiler/pipeline_spec_builder.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/compiler/pipeline_spec_builder_test.py` & `kfp-2.1.2/kfp/compiler/pipeline_spec_builder_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/compiler/read_write_test.py` & `kfp-2.1.2/kfp/compiler/read_write_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/components/__init__.py` & `kfp-2.1.2/kfp/components/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,11 +23,15 @@
     'ContainerComponent',
     'YamlComponent',
 ]
 
 from kfp.components.load_yaml_utilities import load_component_from_file
 from kfp.components.load_yaml_utilities import load_component_from_text
 from kfp.components.load_yaml_utilities import load_component_from_url
+# keep this for backward compatibility with user code "from kfp.components import placholders" and similar
+from kfp.dsl import base_component  # noqa: keep unused import
+from kfp.dsl import placeholders  # noqa: keep unused import
+#
 from kfp.dsl.base_component import BaseComponent
 from kfp.dsl.container_component_class import ContainerComponent
 from kfp.dsl.python_component import PythonComponent
 from kfp.dsl.yaml_component import YamlComponent
```

### Comparing `kfp-2.1.1/kfp/components/load_yaml_utilities.py` & `kfp-2.1.2/kfp/components/load_yaml_utilities.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/components/load_yaml_utilities_test.py` & `kfp-2.1.2/kfp/components/load_yaml_utilities_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/__init__.py` & `kfp-2.1.2/kfp/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/__main__.py` & `kfp-2.1.2/kfp/deprecated/__main__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/_auth.py` & `kfp-2.1.2/kfp/deprecated/_auth.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/_client.py` & `kfp-2.1.2/kfp/deprecated/_client.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/_config.py` & `kfp-2.1.2/kfp/deprecated/_config.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/_local_client.py` & `kfp-2.1.2/kfp/deprecated/_local_client.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/_runners.py` & `kfp-2.1.2/kfp/deprecated/_runners.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/auth/__init__.py` & `kfp-2.1.2/kfp/deprecated/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/auth/_satvolumecredentials.py` & `kfp-2.1.2/kfp/deprecated/auth/_satvolumecredentials.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/auth/_tokencredentialsbase.py` & `kfp-2.1.2/kfp/deprecated/auth/_tokencredentialsbase.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/aws.py` & `kfp-2.1.2/kfp/deprecated/aws.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/azure.py` & `kfp-2.1.2/kfp/deprecated/azure.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/__init__.py` & `kfp-2.1.2/kfp/deprecated/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/cli.py` & `kfp-2.1.2/kfp/deprecated/cli/cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/components.py` & `kfp-2.1.2/kfp/deprecated/cli/components.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/components_test.py` & `kfp-2.1.2/kfp/deprecated/cli/components_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/__init__.py` & `kfp-2.1.2/kfp/deprecated/cli/diagnose_me/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/dev_env.py` & `kfp-2.1.2/kfp/deprecated/cli/diagnose_me/dev_env.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/dev_env_test.py` & `kfp-2.1.2/kfp/deprecated/cli/diagnose_me/dev_env_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/gcp.py` & `kfp-2.1.2/kfp/deprecated/cli/diagnose_me/gcp.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/gcp_test.py` & `kfp-2.1.2/kfp/deprecated/cli/diagnose_me/gcp_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py` & `kfp-2.1.2/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py` & `kfp-2.1.2/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/utility.py` & `kfp-2.1.2/kfp/deprecated/cli/diagnose_me/utility.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/utility_test.py` & `kfp-2.1.2/kfp/deprecated/cli/diagnose_me/utility_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/diagnose_me_cli.py` & `kfp-2.1.2/kfp/deprecated/cli/diagnose_me_cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/experiment.py` & `kfp-2.1.2/kfp/deprecated/cli/experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/output.py` & `kfp-2.1.2/kfp/deprecated/cli/output.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/pipeline.py` & `kfp-2.1.2/kfp/deprecated/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/recurring_run.py` & `kfp-2.1.2/kfp/deprecated/cli/recurring_run.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/cli/run.py` & `kfp-2.1.2/kfp/deprecated/cli/run.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/compiler/__init__.py` & `kfp-2.1.2/kfp/deprecated/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/compiler/_data_passing_rewriter.py` & `kfp-2.1.2/kfp/deprecated/compiler/_data_passing_rewriter.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/compiler/_data_passing_using_volume.py` & `kfp-2.1.2/kfp/deprecated/compiler/_data_passing_using_volume.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/compiler/_default_transformers.py` & `kfp-2.1.2/kfp/deprecated/compiler/_default_transformers.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/compiler/_k8s_helper.py` & `kfp-2.1.2/kfp/deprecated/compiler/_k8s_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/compiler/_op_to_template.py` & `kfp-2.1.2/kfp/deprecated/compiler/_op_to_template.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/compiler/compiler.py` & `kfp-2.1.2/kfp/deprecated/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/compiler/main.py` & `kfp-2.1.2/kfp/deprecated/compiler/main.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/compiler/v2_compat.py` & `kfp-2.1.2/kfp/deprecated/compiler/v2_compat.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/compiler/v2_compatible_compiler_test.py` & `kfp-2.1.2/kfp/deprecated/compiler/v2_compatible_compiler_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/components/__init__.py` & `kfp-2.1.2/kfp/deprecated/components/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/components/_airflow_op.py` & `kfp-2.1.2/kfp/deprecated/components/_airflow_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/components/_component_store.py` & `kfp-2.1.2/kfp/deprecated/components/_component_store.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/components/_components.py` & `kfp-2.1.2/kfp/deprecated/components/_components.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/components/_data_passing.py` & `kfp-2.1.2/kfp/deprecated/components/_data_passing.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/components/_dynamic.py` & `kfp-2.1.2/kfp/deprecated/components/_dynamic.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/components/_key_value_store.py` & `kfp-2.1.2/kfp/deprecated/components/_key_value_store.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/components/_naming.py` & `kfp-2.1.2/kfp/deprecated/components/_naming.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/components/_python_op.py` & `kfp-2.1.2/kfp/deprecated/components/_python_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/components/_python_to_graph_component.py` & `kfp-2.1.2/kfp/deprecated/components/_python_to_graph_component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/components/_structures.py` & `kfp-2.1.2/kfp/deprecated/components/_structures.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/components/_yaml_utils.py` & `kfp-2.1.2/kfp/deprecated/components/_yaml_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/components/modelbase.py` & `kfp-2.1.2/kfp/deprecated/components/modelbase.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/components/type_annotation_utils.py` & `kfp-2.1.2/kfp/deprecated/components/type_annotation_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/components/type_annotation_utils_test.py` & `kfp-2.1.2/kfp/deprecated/components/type_annotation_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/containers/__init__.py` & `kfp-2.1.2/kfp/deprecated/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/containers/_build_image_api.py` & `kfp-2.1.2/kfp/deprecated/containers/_build_image_api.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/containers/_cache.py` & `kfp-2.1.2/kfp/deprecated/containers/_cache.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/containers/_component_builder.py` & `kfp-2.1.2/kfp/deprecated/containers/_component_builder.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/containers/_container_builder.py` & `kfp-2.1.2/kfp/deprecated/containers/_container_builder.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/containers/_gcs_helper.py` & `kfp-2.1.2/kfp/deprecated/containers/_gcs_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/containers/_k8s_job_helper.py` & `kfp-2.1.2/kfp/deprecated/containers/_k8s_job_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/containers/entrypoint.py` & `kfp-2.1.2/kfp/deprecated/containers/entrypoint.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/containers/entrypoint_utils.py` & `kfp-2.1.2/kfp/deprecated/containers/entrypoint_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/__init__.py` & `kfp-2.1.2/kfp/deprecated/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/_component.py` & `kfp-2.1.2/kfp/deprecated/dsl/_component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/_component_bridge.py` & `kfp-2.1.2/kfp/deprecated/dsl/_component_bridge.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/_container_op.py` & `kfp-2.1.2/kfp/deprecated/dsl/_container_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/_container_op_test.py` & `kfp-2.1.2/kfp/deprecated/dsl/_container_op_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/_for_loop.py` & `kfp-2.1.2/kfp/deprecated/dsl/_for_loop.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/_metadata.py` & `kfp-2.1.2/kfp/deprecated/dsl/_metadata.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/_ops_group.py` & `kfp-2.1.2/kfp/deprecated/dsl/_ops_group.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/_pipeline.py` & `kfp-2.1.2/kfp/deprecated/dsl/_pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/_pipeline_param.py` & `kfp-2.1.2/kfp/deprecated/dsl/_pipeline_param.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/_pipeline_volume.py` & `kfp-2.1.2/kfp/deprecated/dsl/_pipeline_volume.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/_resource_op.py` & `kfp-2.1.2/kfp/deprecated/dsl/_resource_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/_volume_op.py` & `kfp-2.1.2/kfp/deprecated/dsl/_volume_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/_volume_snapshot_op.py` & `kfp-2.1.2/kfp/deprecated/dsl/_volume_snapshot_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/artifact.py` & `kfp-2.1.2/kfp/deprecated/dsl/artifact.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/artifact_utils.py` & `kfp-2.1.2/kfp/deprecated/dsl/artifact_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/component_spec.py` & `kfp-2.1.2/kfp/deprecated/dsl/component_spec.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/component_spec_test.py` & `kfp-2.1.2/kfp/deprecated/dsl/component_spec_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/data_passing_methods.py` & `kfp-2.1.2/kfp/deprecated/dsl/data_passing_methods.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/dsl_utils.py` & `kfp-2.1.2/kfp/deprecated/dsl/dsl_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/dsl_utils_test.py` & `kfp-2.1.2/kfp/deprecated/dsl/dsl_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/extensions/kubernetes.py` & `kfp-2.1.2/kfp/deprecated/dsl/extensions/kubernetes.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/io_types.py` & `kfp-2.1.2/kfp/deprecated/dsl/io_types.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/metrics_utils.py` & `kfp-2.1.2/kfp/deprecated/dsl/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/metrics_utils_test.py` & `kfp-2.1.2/kfp/deprecated/dsl/metrics_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/serialization_utils.py` & `kfp-2.1.2/kfp/deprecated/dsl/serialization_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/serialization_utils_test.py` & `kfp-2.1.2/kfp/deprecated/dsl/serialization_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/type_utils.py` & `kfp-2.1.2/kfp/deprecated/dsl/type_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/dsl/types.py` & `kfp-2.1.2/kfp/deprecated/dsl/types.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/gcp.py` & `kfp-2.1.2/kfp/deprecated/gcp.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/notebook/__init__.py` & `kfp-2.1.2/kfp/deprecated/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/notebook/_magic.py` & `kfp-2.1.2/kfp/deprecated/notebook/_magic.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/deprecated/onprem.py` & `kfp-2.1.2/kfp/deprecated/onprem.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/registry/__init__.py` & `kfp-2.1.2/kfp/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/registry/context/__init__.py` & `kfp-2.1.2/kfp/registry/context/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/registry/context/default_pkg_dev.json` & `kfp-2.1.2/kfp/registry/context/default_pkg_dev.json`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/registry/context/kfp_pkg_dev.json` & `kfp-2.1.2/kfp/registry/context/kfp_pkg_dev.json`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/registry/registry_client.py` & `kfp-2.1.2/kfp/registry/registry_client.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/registry/registry_client_test.py` & `kfp-2.1.2/kfp/registry/registry_client_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/v2/__init__.py` & `kfp-2.1.2/kfp/v2/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 warnings.warn(
     (f'The module `{__name__}` is deprecated and will be removed in a future'
      'version. Please import directly from the `kfp` namespace, '
      'instead of `kfp.v2`.'),
     category=DeprecationWarning,
     stacklevel=2)
 
-from kfp import compiler
-from kfp import components
-from kfp import dsl
+from kfp import compiler  # noqa: keep unused import
+from kfp import components  # noqa: keep unused import
+from kfp import dsl  # noqa: keep unused import
```

### Comparing `kfp-2.1.1/kfp/v2/compiler.py` & `kfp-2.1.2/kfp/v2/compiler.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/v2/components.py` & `kfp-2.1.2/kfp/v2/components.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp/v2/dsl.py` & `kfp-2.1.2/kfp/v2/dsl.py`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/kfp.egg-info/PKG-INFO` & `kfp-2.1.2/kfp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfp
-Version: 2.1.1
+Version: 2.1.2
 Summary: Kubeflow Pipelines SDK
 Home-page: https://github.com/kubeflow/pipelines
 Author: The Kubeflow Authors
 License: UNKNOWN
 Project-URL: Documentation, https://kubeflow-pipelines.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/kubeflow/pipelines/issues
 Project-URL: Source, https://github.com/kubeflow/pipelines/tree/master/sdk
```

### Comparing `kfp-2.1.1/kfp.egg-info/SOURCES.txt` & `kfp-2.1.2/kfp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kfp-2.1.1/requirements.in` & `kfp-2.1.2/requirements.in`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 docstring-parser>=0.7.3,<1
 # Pin google-api-core version for the bug fixing in 1.31.5
 # https://github.com/googleapis/python-api-core/releases/tag/v1.31.5
 google-api-core>=1.31.5,<3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.0
 google-auth>=1.6.1,<3
 # https://github.com/googleapis/python-storage/blob/main/CHANGELOG.md#221-2022-03-15
 google-cloud-storage>=2.2.1,<3
-kfp-dsl==2.1.1
+kfp-dsl==2.1.2
 # pin kfp-pipeline-spec to an exact version, since this is the contract between a given KFP SDK version and the BE. we don't want old version of the SDK to write new fields and to have the BE reject the new unsupported field (even if the new field backward compatible from a proto perspective)
 kfp-pipeline-spec==0.2.2
 # Update the upper version whenever a new major version of the
 # kfp-server-api package is released.
 # Update the lower version when kfp sdk depends on new apis/fields in
 # kfp-server-api.
 kfp-server-api>=2.0.0,<2.1.0
```

### Comparing `kfp-2.1.1/setup.py` & `kfp-2.1.2/setup.py`

 * *Files identical despite different names*

