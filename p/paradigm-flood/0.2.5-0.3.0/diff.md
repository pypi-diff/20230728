# Comparing `tmp/paradigm-flood-0.2.5.tar.gz` & `tmp/paradigm_flood-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradigm-flood-0.2.5.tar", last modified: Tue Jun 27 07:15:32 2023, max compression
+gzip compressed data, was "paradigm_flood-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `paradigm-flood-0.2.5.tar` & `paradigm_flood-0.3.0.tar`

### file list

```diff
@@ -1,80 +1,87 @@
--rw-r--r--   0        0        0      513 2023-06-06 19:32:53.475871 paradigm-flood-0.2.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      607 2023-06-06 19:32:53.476113 paradigm-flood-0.2.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      193 2023-06-06 19:32:53.476353 paradigm-flood-0.2.5/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0      781 2023-06-06 19:32:53.476534 paradigm-flood-0.2.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      165 2023-06-06 19:32:53.476751 paradigm-flood-0.2.5/.github/workflows/lint.yml
--rw-r--r--   0        0        0      513 2023-06-22 00:28:24.031464 paradigm-flood-0.2.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0      225 2023-05-06 04:56:40.389625 paradigm-flood-0.2.5/.gitignore
--rw-r--r--   0        0        0    10332 2023-06-04 20:22:19.525565 paradigm-flood-0.2.5/CONTRIBUTING.md
--rw-r--r--   0        0        0      832 2023-06-02 00:45:29.473078 paradigm-flood-0.2.5/Dockerfile
--rw-r--r--   0        0        0    10839 2023-06-04 20:13:59.817606 paradigm-flood-0.2.5/LICENSE-APACHE
--rw-r--r--   0        0        0     1085 2023-06-04 20:13:48.830823 paradigm-flood-0.2.5/LICENSE-MIT
--rw-r--r--   0        0        0     2865 2023-06-06 19:32:53.477627 paradigm-flood-0.2.5/README.md
--rw-r--r--   0        0        0  3038209 2023-06-06 19:32:53.483637 paradigm-flood-0.2.5/assets/cover.png
--rw-r--r--   0        0        0      124 2023-06-06 21:20:36.150174 paradigm-flood-0.2.5/examples/equality_test.sh
--rwxr-xr-x   0        0        0     1905 2023-06-15 16:40:12.596585 paradigm-flood-0.2.5/examples/report.sh
--rw-r--r--   0        0        0      648 2023-06-27 07:14:54.717881 paradigm-flood-0.2.5/flood/__init__.py
--rw-r--r--   0        0        0      117 2023-06-04 23:14:01.291195 paradigm-flood-0.2.5/flood/__main__.py
--rw-r--r--   0        0        0     1556 2023-06-22 00:34:03.891521 paradigm-flood-0.2.5/flood/cli/cli_run.py
--rw-r--r--   0        0        0      877 2023-06-04 23:14:01.298637 paradigm-flood-0.2.5/flood/cli/ls_command.py
--rw-r--r--   0        0        0     1630 2023-06-22 00:34:03.891718 paradigm-flood-0.2.5/flood/cli/print_command.py
--rw-r--r--   0        0        0     1221 2023-06-04 23:14:01.302153 paradigm-flood-0.2.5/flood/cli/report_command.py
--rw-r--r--   0        0        0     6215 2023-06-22 00:34:03.891970 paradigm-flood-0.2.5/flood/cli/root_command.py
--rw-r--r--   0        0        0     1315 2023-06-04 23:14:01.307482 paradigm-flood-0.2.5/flood/cli/samples_collect_command.py
--rw-r--r--   0        0        0     1687 2023-06-06 20:39:09.158213 paradigm-flood-0.2.5/flood/cli/samples_download_command.py
--rw-r--r--   0        0        0     1874 2023-06-06 20:39:23.569867 paradigm-flood-0.2.5/flood/cli/samples_ls_command.py
--rw-r--r--   0        0        0      121 2023-06-03 19:54:58.405209 paradigm-flood-0.2.5/flood/generators/__init__.py
--rw-r--r--   0        0        0      199 2023-06-03 19:54:39.491471 paradigm-flood-0.2.5/flood/generators/object_generators/__init__.py
--rw-r--r--   0        0        0      603 2023-06-04 23:14:01.311234 paradigm-flood-0.2.5/flood/generators/object_generators/address_generators.py
--rw-r--r--   0        0        0     4815 2023-06-04 23:14:01.335388 paradigm-flood-0.2.5/flood/generators/object_generators/block_generators.py
--rw-r--r--   0        0        0    17256 2023-06-06 20:39:37.317485 paradigm-flood-0.2.5/flood/generators/object_generators/call_generators.py
--rw-r--r--   0        0        0      337 2023-06-04 23:14:01.306215 paradigm-flood-0.2.5/flood/generators/object_generators/slot_generators.py
--rw-r--r--   0        0        0     4156 2023-06-06 20:41:05.406418 paradigm-flood-0.2.5/flood/generators/object_generators/timing_generators.py
--rw-r--r--   0        0        0      346 2023-06-04 23:14:01.315806 paradigm-flood-0.2.5/flood/generators/object_generators/transaction_generators.py
--rw-r--r--   0        0        0      129 2023-06-02 06:40:02.759112 paradigm-flood-0.2.5/flood/generators/raw_data_sources/__init__.py
--rw-r--r--   0        0        0      465 2023-06-04 23:14:01.312615 paradigm-flood-0.2.5/flood/generators/raw_data_sources/raw_data_spec.py
--rw-r--r--   0        0        0     1935 2023-06-04 23:14:01.327302 paradigm-flood-0.2.5/flood/generators/raw_data_sources/raw_download_utils.py
--rw-r--r--   0        0        0     5688 2023-06-04 23:14:01.364193 paradigm-flood-0.2.5/flood/generators/raw_data_sources/raw_gather_utils.py
--rw-r--r--   0        0        0     4662 2023-06-04 23:14:01.352117 paradigm-flood-0.2.5/flood/generators/raw_data_sources/raw_sample_loading.py
--rw-r--r--   0        0        0      530 2023-06-04 23:14:01.322799 paradigm-flood-0.2.5/flood/generators/rng_utils.py
--rw-r--r--   0        0        0      307 2023-06-16 00:43:55.812056 paradigm-flood-0.2.5/flood/generators/test_generators/__init__.py
--rw-r--r--   0        0        0     1507 2023-06-04 23:14:01.337667 paradigm-flood-0.2.5/flood/generators/test_generators/address_test_generators.py
--rw-r--r--   0        0        0     1559 2023-06-04 23:14:01.331116 paradigm-flood-0.2.5/flood/generators/test_generators/block_test_generators.py
--rw-r--r--   0        0        0     2150 2023-06-04 23:14:01.346034 paradigm-flood-0.2.5/flood/generators/test_generators/contract_test_generators.py
--rw-r--r--   0        0        0     5333 2023-06-16 00:44:54.451370 paradigm-flood-0.2.5/flood/generators/test_generators/generic_test_generators.py
--rw-r--r--   0        0        0     3870 2023-06-04 23:14:01.341234 paradigm-flood-0.2.5/flood/generators/test_generators/log_test_generators.py
--rw-r--r--   0        0        0      162 2023-06-16 00:43:37.064471 paradigm-flood-0.2.5/flood/generators/test_generators/multi_test_generators.py
--rw-r--r--   0        0        0     5897 2023-06-04 23:14:01.413684 paradigm-flood-0.2.5/flood/generators/test_generators/trace_test_generators.py
--rw-r--r--   0        0        0     1512 2023-06-04 23:14:01.354881 paradigm-flood-0.2.5/flood/generators/test_generators/transaction_test_generators.py
--rw-r--r--   0        0        0       87 2023-06-15 23:24:24.125486 paradigm-flood-0.2.5/flood/runners/__init__.py
--rw-r--r--   0        0        0       40 2023-06-15 23:57:58.076473 paradigm-flood-0.2.5/flood/runners/generic_runner/__init__.py
--rw-r--r--   0        0        0     3437 2023-06-22 00:34:03.892257 paradigm-flood-0.2.5/flood/runners/generic_runner/generic_runner_execution.py
--rw-r--r--   0        0        0       31 2023-06-15 23:25:05.871130 paradigm-flood-0.2.5/flood/runners/multi_runner/__init__.py
--rw-r--r--   0        0        0     1081 2023-06-15 23:25:35.750693 paradigm-flood-0.2.5/flood/runners/multi_runner/multi_runner_io.py
--rw-r--r--   0        0        0       32 2023-06-15 23:24:48.633159 paradigm-flood-0.2.5/flood/runners/single_runner/__init__.py
--rw-r--r--   0        0        0     4845 2023-06-22 00:34:03.892502 paradigm-flood-0.2.5/flood/runners/single_runner/single_runner_execution.py
--rw-r--r--   0        0        0     4751 2023-06-22 00:34:03.892741 paradigm-flood-0.2.5/flood/runners/single_runner/single_runner_io.py
--rw-r--r--   0        0        0     6430 2023-06-15 23:32:29.744850 paradigm-flood-0.2.5/flood/runners/single_runner/single_runner_summary.py
--rw-r--r--   0        0        0     5117 2023-06-20 03:52:27.584215 paradigm-flood-0.2.5/flood/spec.py
--rw-r--r--   0        0        0       56 2023-06-15 23:55:07.358215 paradigm-flood-0.2.5/flood/tests/__init__.py
--rw-r--r--   0        0        0       34 2023-06-04 23:14:01.345292 paradigm-flood-0.2.5/flood/tests/equality_tests/__init__.py
--rw-r--r--   0        0        0     6200 2023-06-22 00:39:58.042086 paradigm-flood-0.2.5/flood/tests/equality_tests/equality_test_runs.py
--rw-r--r--   0        0        0     8699 2023-06-27 07:14:03.167951 paradigm-flood-0.2.5/flood/tests/equality_tests/equality_test_sets.py
--rw-r--r--   0        0        0      154 2023-06-02 00:45:29.480806 paradigm-flood-0.2.5/flood/tests/load_tests/__init__.py
--rw-r--r--   0        0        0     2682 2023-06-04 23:14:01.379714 paradigm-flood-0.2.5/flood/tests/load_tests/load_test_construction.py
--rw-r--r--   0        0        0     5740 2023-06-15 21:26:24.315199 paradigm-flood-0.2.5/flood/tests/load_tests/load_test_plots.py
--rw-r--r--   0        0        0    10242 2023-06-15 23:17:43.297886 paradigm-flood-0.2.5/flood/tests/load_tests/load_test_reports.py
--rw-r--r--   0        0        0    13410 2023-06-22 00:34:03.894287 paradigm-flood-0.2.5/flood/tests/load_tests/load_test_runs.py
--rw-r--r--   0        0        0    10443 2023-06-20 06:29:09.583999 paradigm-flood-0.2.5/flood/tests/load_tests/vegeta.py
--rw-r--r--   0        0        0       45 2023-06-15 23:20:48.386860 paradigm-flood-0.2.5/flood/user_io/__init__.py
--rw-r--r--   0        0        0     5903 2023-06-15 06:32:18.240729 paradigm-flood-0.2.5/flood/user_io/inputs.py
--rw-r--r--   0        0        0     4285 2023-06-04 23:14:01.438468 paradigm-flood-0.2.5/flood/user_io/notebook_io.py
--rw-r--r--   0        0        0     5864 2023-06-06 20:35:25.703304 paradigm-flood-0.2.5/flood/user_io/outputs.py
--rw-r--r--   0        0        0     1919 2023-06-22 00:43:46.791751 paradigm-flood-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      381 2023-06-04 20:35:57.569281 paradigm-flood-0.2.5/tests/README.md
--rw-r--r--   0        0        0      993 2023-06-06 21:03:30.304627 paradigm-flood-0.2.5/tests/conftest.py
--rw-r--r--   0        0        0      593 2023-06-04 20:53:58.379044 paradigm-flood-0.2.5/tests/test_env_vars.py
--rw-r--r--   0        0        0      269 2023-06-06 21:04:00.022725 paradigm-flood-0.2.5/tests/test_equality_tests.py
--rw-r--r--   0        0        0     1128 2023-06-06 21:03:47.012574 paradigm-flood-0.2.5/tests/test_load_tests.py
--rw-r--r--   0        0        0     1736 2023-06-04 16:00:15.996050 paradigm-flood-0.2.5/tests/test_node_parsing.py
--rw-r--r--   0        0        0     4526 1970-01-01 00:00:00.000000 paradigm-flood-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-06 19:32:53.475871 paradigm_flood-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      607 2023-06-06 19:32:53.476113 paradigm_flood-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      193 2023-06-06 19:32:53.476353 paradigm_flood-0.3.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0      781 2023-06-06 19:32:53.476534 paradigm_flood-0.3.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      542 2023-07-25 17:22:45.016960 paradigm_flood-0.3.0/.github/workflows/docker.yml
+-rw-r--r--   0        0        0      165 2023-06-06 19:32:53.476751 paradigm_flood-0.3.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      513 2023-06-22 00:28:24.031464 paradigm_flood-0.3.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      254 2023-07-27 21:19:46.528276 paradigm_flood-0.3.0/.gitignore
+-rw-r--r--   0        0        0    10332 2023-06-04 20:22:19.525565 paradigm_flood-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1186 2023-07-27 16:51:57.722902 paradigm_flood-0.3.0/Dockerfile
+-rw-r--r--   0        0        0    10839 2023-06-04 20:13:59.817606 paradigm_flood-0.3.0/LICENSE-APACHE
+-rw-r--r--   0        0        0     1085 2023-06-04 20:13:48.830823 paradigm_flood-0.3.0/LICENSE-MIT
+-rw-r--r--   0        0        0     7551 2023-07-27 21:38:12.686051 paradigm_flood-0.3.0/README.md
+-rw-r--r--   0        0        0  3038209 2023-06-06 19:32:53.483637 paradigm_flood-0.3.0/assets/cover.png
+-rw-r--r--   0        0        0      124 2023-06-06 21:20:36.150174 paradigm_flood-0.3.0/examples/equality_test.sh
+-rwxr-xr-x   0        0        0     1905 2023-06-15 16:40:12.596585 paradigm_flood-0.3.0/examples/report.sh
+-rw-r--r--   0        0        0     1210 2023-07-28 19:05:42.608410 paradigm_flood-0.3.0/flood/__init__.py
+-rw-r--r--   0        0        0      117 2023-06-04 23:14:01.291195 paradigm_flood-0.3.0/flood/__main__.py
+-rw-r--r--   0        0        0     1569 2023-07-27 20:35:25.899797 paradigm_flood-0.3.0/flood/cli/cli_run.py
+-rw-r--r--   0        0        0      887 2023-07-27 20:35:25.899996 paradigm_flood-0.3.0/flood/cli/ls_command.py
+-rw-r--r--   0        0        0     3369 2023-07-27 20:35:25.900205 paradigm_flood-0.3.0/flood/cli/print_command.py
+-rw-r--r--   0        0        0     1238 2023-07-27 20:35:25.900420 paradigm_flood-0.3.0/flood/cli/report_command.py
+-rw-r--r--   0        0        0     7229 2023-07-27 16:51:57.724485 paradigm_flood-0.3.0/flood/cli/root_command.py
+-rw-r--r--   0        0        0     1337 2023-07-27 20:35:25.900618 paradigm_flood-0.3.0/flood/cli/samples_collect_command.py
+-rw-r--r--   0        0        0     1720 2023-07-27 20:35:25.900812 paradigm_flood-0.3.0/flood/cli/samples_download_command.py
+-rw-r--r--   0        0        0     1918 2023-07-27 20:35:25.901041 paradigm_flood-0.3.0/flood/cli/samples_ls_command.py
+-rw-r--r--   0        0        0     1148 2023-07-27 20:35:25.901250 paradigm_flood-0.3.0/flood/cli/update_command.py
+-rw-r--r--   0        0        0     1089 2023-07-27 18:15:55.094633 paradigm_flood-0.3.0/flood/cli/version_command.py
+-rw-r--r--   0        0        0      121 2023-06-03 19:54:58.405209 paradigm_flood-0.3.0/flood/generators/__init__.py
+-rw-r--r--   0        0        0      199 2023-06-03 19:54:39.491471 paradigm_flood-0.3.0/flood/generators/object_generators/__init__.py
+-rw-r--r--   0        0        0      642 2023-07-27 20:35:25.901507 paradigm_flood-0.3.0/flood/generators/object_generators/address_generators.py
+-rw-r--r--   0        0        0     4829 2023-07-16 18:19:38.519806 paradigm_flood-0.3.0/flood/generators/object_generators/block_generators.py
+-rw-r--r--   0        0        0    18342 2023-07-27 20:35:25.901754 paradigm_flood-0.3.0/flood/generators/object_generators/call_generators.py
+-rw-r--r--   0        0        0      371 2023-07-27 20:35:25.901972 paradigm_flood-0.3.0/flood/generators/object_generators/slot_generators.py
+-rw-r--r--   0        0        0     4156 2023-06-06 20:41:05.406418 paradigm_flood-0.3.0/flood/generators/object_generators/timing_generators.py
+-rw-r--r--   0        0        0      380 2023-07-27 20:35:25.902185 paradigm_flood-0.3.0/flood/generators/object_generators/transaction_generators.py
+-rw-r--r--   0        0        0      129 2023-06-02 06:40:02.759112 paradigm_flood-0.3.0/flood/generators/raw_data_sources/__init__.py
+-rw-r--r--   0        0        0      465 2023-06-04 23:14:01.312615 paradigm_flood-0.3.0/flood/generators/raw_data_sources/raw_data_spec.py
+-rw-r--r--   0        0        0     1935 2023-06-04 23:14:01.327302 paradigm_flood-0.3.0/flood/generators/raw_data_sources/raw_download_utils.py
+-rw-r--r--   0        0        0     5688 2023-06-04 23:14:01.364193 paradigm_flood-0.3.0/flood/generators/raw_data_sources/raw_gather_utils.py
+-rw-r--r--   0        0        0     4701 2023-07-27 20:35:25.902412 paradigm_flood-0.3.0/flood/generators/raw_data_sources/raw_sample_loading.py
+-rw-r--r--   0        0        0      566 2023-07-16 21:04:57.319895 paradigm_flood-0.3.0/flood/generators/rng_utils.py
+-rw-r--r--   0        0        0      307 2023-06-16 00:43:55.812056 paradigm_flood-0.3.0/flood/generators/test_generators/__init__.py
+-rw-r--r--   0        0        0     1657 2023-07-27 20:35:25.902622 paradigm_flood-0.3.0/flood/generators/test_generators/address_test_generators.py
+-rw-r--r--   0        0        0     2491 2023-07-27 20:35:25.902860 paradigm_flood-0.3.0/flood/generators/test_generators/block_test_generators.py
+-rw-r--r--   0        0        0     2386 2023-07-27 20:35:25.903067 paradigm_flood-0.3.0/flood/generators/test_generators/contract_test_generators.py
+-rw-r--r--   0        0        0     6002 2023-07-27 20:35:25.903282 paradigm_flood-0.3.0/flood/generators/test_generators/generic_test_generators.py
+-rw-r--r--   0        0        0     4738 2023-07-27 20:35:25.903500 paradigm_flood-0.3.0/flood/generators/test_generators/log_test_generators.py
+-rw-r--r--   0        0        0      162 2023-06-16 00:43:37.064471 paradigm_flood-0.3.0/flood/generators/test_generators/multi_test_generators.py
+-rw-r--r--   0        0        0     6490 2023-07-27 20:35:25.903718 paradigm_flood-0.3.0/flood/generators/test_generators/trace_test_generators.py
+-rw-r--r--   0        0        0     1681 2023-07-27 20:35:25.903943 paradigm_flood-0.3.0/flood/generators/test_generators/transaction_test_generators.py
+-rw-r--r--   0        0        0       62 2023-07-15 22:45:06.608400 paradigm_flood-0.3.0/flood/ops/__init__.py
+-rw-r--r--   0        0        0     3589 2023-07-17 03:46:04.382619 paradigm_flood-0.3.0/flood/ops/installation_utils.py
+-rw-r--r--   0        0        0     2511 2023-07-16 19:36:40.068297 paradigm_flood-0.3.0/flood/ops/update_utils.py
+-rw-r--r--   0        0        0       87 2023-06-15 23:24:24.125486 paradigm_flood-0.3.0/flood/runners/__init__.py
+-rw-r--r--   0        0        0       40 2023-06-15 23:57:58.076473 paradigm_flood-0.3.0/flood/runners/generic_runner/__init__.py
+-rw-r--r--   0        0        0     3715 2023-07-27 20:35:25.904307 paradigm_flood-0.3.0/flood/runners/generic_runner/generic_runner_execution.py
+-rw-r--r--   0        0        0       31 2023-06-15 23:25:05.871130 paradigm_flood-0.3.0/flood/runners/multi_runner/__init__.py
+-rw-r--r--   0        0        0     1108 2023-07-12 21:44:36.214006 paradigm_flood-0.3.0/flood/runners/multi_runner/multi_runner_io.py
+-rw-r--r--   0        0        0       32 2023-06-15 23:24:48.633159 paradigm_flood-0.3.0/flood/runners/single_runner/__init__.py
+-rw-r--r--   0        0        0     4511 2023-07-27 20:35:25.904502 paradigm_flood-0.3.0/flood/runners/single_runner/single_runner_execution.py
+-rw-r--r--   0        0        0     3896 2023-07-27 20:35:25.904690 paradigm_flood-0.3.0/flood/runners/single_runner/single_runner_io.py
+-rw-r--r--   0        0        0     7377 2023-07-27 20:35:25.904887 paradigm_flood-0.3.0/flood/runners/single_runner/single_runner_summary.py
+-rw-r--r--   0        0        0     9080 2023-07-27 15:00:44.333974 paradigm_flood-0.3.0/flood/spec.py
+-rw-r--r--   0        0        0       56 2023-06-15 23:55:07.358215 paradigm_flood-0.3.0/flood/tests/__init__.py
+-rw-r--r--   0        0        0       34 2023-06-04 23:14:01.345292 paradigm_flood-0.3.0/flood/tests/equality_tests/__init__.py
+-rw-r--r--   0        0        0     6725 2023-07-27 20:35:25.905157 paradigm_flood-0.3.0/flood/tests/equality_tests/equality_test_runs.py
+-rw-r--r--   0        0        0    15296 2023-07-27 20:35:25.905390 paradigm_flood-0.3.0/flood/tests/equality_tests/equality_test_sets.py
+-rw-r--r--   0        0        0      180 2023-07-15 21:32:38.743716 paradigm_flood-0.3.0/flood/tests/load_tests/__init__.py
+-rw-r--r--   0        0        0    10683 2023-07-17 00:18:57.110966 paradigm_flood-0.3.0/flood/tests/load_tests/deep_utils.py
+-rw-r--r--   0        0        0     2831 2023-07-27 17:06:25.738618 paradigm_flood-0.3.0/flood/tests/load_tests/load_test_construction.py
+-rw-r--r--   0        0        0     7756 2023-07-27 20:35:25.905622 paradigm_flood-0.3.0/flood/tests/load_tests/load_test_plots.py
+-rw-r--r--   0        0        0    14133 2023-07-28 18:32:34.652263 paradigm_flood-0.3.0/flood/tests/load_tests/load_test_reports.py
+-rw-r--r--   0        0        0    12696 2023-07-27 20:35:25.906062 paradigm_flood-0.3.0/flood/tests/load_tests/load_test_runs.py
+-rw-r--r--   0        0        0     5822 2023-07-16 17:00:50.279223 paradigm_flood-0.3.0/flood/tests/load_tests/vegeta.py
+-rw-r--r--   0        0        0       45 2023-06-15 23:20:48.386860 paradigm_flood-0.3.0/flood/user_io/__init__.py
+-rw-r--r--   0        0        0     6072 2023-07-27 20:35:25.906311 paradigm_flood-0.3.0/flood/user_io/inputs.py
+-rw-r--r--   0        0        0     4284 2023-07-28 17:10:19.223283 paradigm_flood-0.3.0/flood/user_io/notebook_io.py
+-rw-r--r--   0        0        0     6990 2023-07-28 18:49:39.788730 paradigm_flood-0.3.0/flood/user_io/outputs.py
+-rw-r--r--   0        0        0     2023 2023-07-28 19:00:41.762119 paradigm_flood-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      381 2023-06-04 20:35:57.569281 paradigm_flood-0.3.0/tests/README.md
+-rw-r--r--   0        0        0      993 2023-06-06 21:03:30.304627 paradigm_flood-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0      624 2023-07-27 20:35:25.906746 paradigm_flood-0.3.0/tests/test_env_vars.py
+-rw-r--r--   0        0        0      269 2023-06-06 21:04:00.022725 paradigm_flood-0.3.0/tests/test_equality_tests.py
+-rw-r--r--   0        0        0     1145 2023-07-27 20:35:25.906949 paradigm_flood-0.3.0/tests/test_load_tests.py
+-rw-r--r--   0        0        0     1744 2023-07-27 20:35:25.907146 paradigm_flood-0.3.0/tests/test_node_parsing.py
+-rw-r--r--   0        0        0     9348 1970-01-01 00:00:00.000000 paradigm_flood-0.3.0/PKG-INFO
```

### Comparing `paradigm-flood-0.2.5/.github/ISSUE_TEMPLATE/bug_report.md` & `paradigm_flood-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.5/.github/ISSUE_TEMPLATE/feature_request.md` & `paradigm_flood-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.5/.github/PULL_REQUEST_TEMPLATE.md` & `paradigm_flood-0.3.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.5/.github/workflows/tests.yml` & `paradigm_flood-0.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.5/CONTRIBUTING.md` & `paradigm_flood-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.5/LICENSE-APACHE` & `paradigm_flood-0.3.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.5/LICENSE-MIT` & `paradigm_flood-0.3.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.5/assets/cover.png` & `paradigm_flood-0.3.0/assets/cover.png`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.5/examples/report.sh` & `paradigm_flood-0.3.0/examples/report.sh`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.5/flood/cli/cli_run.py` & `paradigm_flood-0.3.0/flood/cli/cli_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,44 +7,43 @@
 cd_dir_help = {
     'samples': 'FLOOD_SAMPLES_PATH env value',
 }
 
 
 def cd_dir_getter(dirname: str) -> str:
     if dirname == 'samples':
-        return flood.get_flood_samples_dir()
+        return flood.generators.get_flood_samples_dir()
     else:
         raise Exception('unknown path: ' + str(dirname))
 
 
 def run_cli(raw_command: str | None = None) -> None:
     command_index: toolcli.CommandIndex = {
         (): 'flood.cli.root_command',
         ('help',): 'toolcli.command_utils.standard_subcommands.help_command',
         ('ls',): 'flood.cli.ls_command',
         ('print',): 'flood.cli.print_command',
         ('report',): 'flood.cli.report_command',
         ('samples', 'collect'): 'flood.cli.samples_collect_command',
         ('samples', 'download'): 'flood.cli.samples_download_command',
         ('samples', 'ls'): 'flood.cli.samples_ls_command',
-        (
-            'version',
-        ): 'toolcli.command_utils.standard_subcommands.version_command',
+        ('version',): 'flood.cli.version_command',
         ('cd',): 'toolcli.command_utils.standard_subcommands.cd_command',
+        ('update',): 'flood.cli.update_command',
     }
 
     config: toolcli.CLIConfig = {
         'base_command': 'flood',
         'description': flood.__doc__,
         'version': flood.__version__,
         'default_command_sequence': (),
         'root_help_arguments': True,
         # 'root_help_subcommands': False,
         'include_debug_arg': True,
-        'style_theme': flood.styles,
+        'style_theme': flood.user_io.styles,
         'cd_dir_help': cd_dir_help,
         'cd_dir_getter': cd_dir_getter,
     }
 
     toolcli.run_cli(
         command_index=command_index,
         config=config,
```

### Comparing `paradigm-flood-0.2.5/flood/cli/report_command.py` & `paradigm_flood-0.3.0/flood/cli/report_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,12 +42,12 @@
     metrics: typing.Sequence[str] | None,
 ) -> None:
     if output is None:
         import os
 
         output = os.getcwd()
 
-    flood.create_load_test_report(
+    flood.tests.load_tests.create_load_test_report(
         test_paths=test_dirs,
         output_dir=output,
         metrics=metrics,
     )
```

### Comparing `paradigm-flood-0.2.5/flood/cli/root_command.py` & `paradigm_flood-0.3.0/flood/cli/root_command.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,96 +25,109 @@
 
 [bold][title]Remote Usage[/bold][/title]
 - [metavar]flood[/metavar] can be invoked on remote machines
 - Use node syntax [metavar]user@remote:node_url[/metavar] or [metavar]name=user@remote:node_url[/metavar]
 - Can omit the [metavar]user@[/metavar] prefix if ssh config has username specified
 - [metavar]flood[/metavar] must already be installed on each remote machine
 
-[bold][title]Parameter Randomization[/bold][/title]
-- [metavar]flood[/metavar] can call each RPC method multiple times using [metavar]-n <N>[/metavar]
-- For each call, parameters are randomized to minimize caching effects
-- Specify random seed [metavar]-s <seed>[/metavar] for repeatable set of randomized calls"""  # noqa: E501
+For more details, see the [metavar]README.md[/metavar] at [metavar]https://github.com/paradigmxyz/cryo[/metavar]"""  # noqa: E501
 
 
 def get_command_spec() -> toolcli.CommandSpec:
     return {
         'f': root_command,
         'help': help_message,
         'args': [
             {
                 'name': 'test',
-                'help': 'test to run (use [metavar]flood ls[/metavar] for list)',  # noqa: E501
+                'help': 'test to run (see [metavar]flood ls[/metavar] for list)',  # noqa: E501
             },
             {
                 'name': 'nodes',
                 'nargs': '*',
-                'help': 'nodes to test, see syntax above',
+                'help': 'nodes to test (see syntax above)',
             },
             {
                 'name': ['-s', '--seed'],
                 'dest': 'random_seed',
                 'type': int,
-                'help': 'random seed to use, default is current timestamp',
+                'help': 'random seed to use, (default = current timestamp)',
             },
             {
                 'name': ['-q', '--quiet'],
                 'help': 'do not print output to [metavar]STDOUT[/metavar]',
                 'action': 'store_true',
             },
             {
                 'name': ['-e', '--equality'],
                 'help': 'run equality test instead of load test',
                 'action': 'store_true',
             },
             {
                 'name': ['-m', '--mode'],
                 'choices': ['stress', 'spike', 'soak'],
+                'hidden': True,
                 'help': 'load test type: stress, spike, or soak',
             },
             {
                 'name': ['-r', '--rates'],
                 'nargs': '+',
-                'help': 'rates to use in load test (requests per second)',
+                'help': 'rates to use in load test, units = reqs per second\n(default is test-specific, use [metavar]--dry[/metavar] to view)',  # noqa: E501
             },
             {
                 'name': ['-d', '--duration'],
                 'type': int,
-                'help': 'amount of time to test each rate',
+                'help': 'number of seconds to test each rate (default = [metavar]30[/metavar])',  # noqa: E501
             },
             {
                 'name': ['-o', '--output'],
                 'dest': 'output_dir',
-                'help': 'directory to save results, default is tmp dir',
+                'help': 'directory to save results, (default = new tmp dir)',
             },
             {
                 'name': ['--dry'],
                 'help': 'only construct tests, do not run them',
                 'action': 'store_true',
             },
             {
                 'name': ['--metrics'],
                 'nargs': '+',
-                'help': 'space-separated list of performance metrics to show',
+                'help': 'space-separated list of performance metrics to show\n(default = [metavar]success throughput p90[/metavar])',  # noqa: E501
             },
             {
                 'name': ['--no-figures'],
                 'help': 'skip generating summary figures in output_dir',
                 'dest': 'figures',
                 'action': 'store_false',
             },
             {
                 'name': ['--save-raw-output'],
-                'help': 'save raw output from Vegeta',
+                'help': 'save the contents of every RPC response',
                 'action': 'store_true',
             },
             {
                 'name': ['--deep-check'],
                 'help': 'validate the contents of every RPC response',
                 'action': 'store_true',
             },
+            {
+                'name': ['--remote-update'],
+                'help': 'attempt to update nodes to latest flood version',
+                'hidden': True,
+                'action': 'store_true',
+            },
+            {
+                'name': ['--vegeta-args'],
+                'help': 'extra args for vegeta, e.g. [metavar]"-timeout 5s -cpus 1"[/metavar]\nfor single args, use [metavar]--vegeta-args="..."[/metavar] (no space)',  # noqa: E501
+            },
+            {
+                'name': ['-V', '--version'],
+                'help': 'print flood version and exit',
+                'action': 'store_true',
+            },
         ],
         'examples': [
             'eth_getBlockByNumber localhost:8545',
             'eth_getLogs localhost:8545 localhost:8546 localhost:8547',
             'all client1=0.0.0.0:8545 client2=0.0.0.0:8546 --equality',
         ],
     }
@@ -131,15 +144,19 @@
     random_seed: int | None,
     dry: bool,
     quiet: bool,
     figures: bool,
     equality: bool,
     save_raw_output: bool,
     deep_check: bool,
+    remote_update: bool,
+    vegeta_args: str,
+    version: bool,
 ) -> None:
+
     verbose = not quiet
     if nodes is not None and len(nodes) == 0:
         nodes = None
 
     if equality:
         if output_dir is not None:
             raise Exception('output_dir not used in equality test')
@@ -159,25 +176,33 @@
             test_name=test,
             nodes=nodes,
             random_seed=random_seed,
             verbose=verbose,
         )
 
     else:
+
+        include_deep_output: typing.List[flood.DeepOutput] = []
+        if deep_check:
+            include_deep_output.append('metrics')
+        if save_raw_output:
+            include_deep_output.append('raw')
+
         if rates is not None:
             rates = [int(rate) for rate in rates]
         flood.run(
             test_name=test,
             mode=mode,
             nodes=nodes,
             metrics=metrics,
             random_seed=random_seed,
             verbose=verbose,
             rates=rates,
             duration=duration,
             dry=dry,
-            output_dir=output_dir or True,
+            output_dir=output_dir,
             figures=figures,
-            include_raw_output=save_raw_output,
+            include_deep_output=include_deep_output,
             deep_check=deep_check,
+            vegeta_args=vegeta_args,
         )
```

### Comparing `paradigm-flood-0.2.5/flood/cli/samples_collect_command.py` & `paradigm_flood-0.3.0/flood/cli/samples_download_command.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,46 +5,59 @@
 import toolcli
 
 import flood
 
 
 def get_command_spec() -> toolcli.CommandSpec:
     return {
-        'f': samples_collect_command,
-        'help': 'collect raw EVM samples using Paradigm Data Portal datasets',
+        'f': download_samples_command,
+        'help': 'download raw EVM samples for constructing calls',
         'args': [
             {
                 'name': ('-n', '--network'),
                 'help': 'network, default ethereum',
             },
             {
                 'name': ('-s', '--sizes'),
-                'help': 'sample sizes of {XS, S, M, L, XL}, default all',
+                'help': 'sample sizes, one of {XS, S, M, L, XL, all}, default L',  # noqa: E501
+                'nargs': '+',
             },
             {
                 'name': ('-o', '--output-dir'),
                 'help': 'download location, default FLOOD_SAMPLES_DIR or cwd',
             },
             {
                 'name': ('-d', '--datatypes'),
                 'help': 'datatypes to sample, default all',
             },
+            {
+                'name': ('-m', '--missing'),
+                'help': 'only download missing files',
+                'action': 'store_true',
+            },
         ],
     }
 
 
-def samples_collect_command(
+def download_samples_command(
     network: str | None,
     sizes: typing.Sequence[str] | None,
     output_dir: str | None,
     datatypes: typing.Sequence[str] | None,
+    missing: bool,
 ) -> None:
-    if output_dir is None:
-        output_dir = flood.get_flood_samples_dir()
     if network is None:
         network = 'ethereum'
-    flood.create_samples_dataset(
-        output_dir=output_dir,
+    if sizes is None:
+        sizes = ['L']
+    if sizes == 'all':
+        sizes = list(flood.generators.default_sizes.keys())
+    if output_dir is None:
+        output_dir = flood.generators.get_flood_samples_dir()
+
+    flood.generators.download_raw_data(
         network=network,
         sizes=sizes,
         datatypes=datatypes,
+        output_dir=output_dir,
+        only_missing=missing,
     )
```

### Comparing `paradigm-flood-0.2.5/flood/cli/samples_download_command.py` & `paradigm_flood-0.3.0/flood/cli/samples_collect_command.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,59 +5,46 @@
 import toolcli
 
 import flood
 
 
 def get_command_spec() -> toolcli.CommandSpec:
     return {
-        'f': download_samples_command,
-        'help': 'download raw EVM samples for constructing calls',
+        'f': samples_collect_command,
+        'help': 'collect raw EVM samples using Paradigm Data Portal datasets',
         'args': [
             {
                 'name': ('-n', '--network'),
                 'help': 'network, default ethereum',
             },
             {
                 'name': ('-s', '--sizes'),
-                'help': 'sample sizes, one of {XS, S, M, L, XL, all}, default L',  # noqa: E501
-                'nargs': '+',
+                'help': 'sample sizes of {XS, S, M, L, XL}, default all',
             },
             {
                 'name': ('-o', '--output-dir'),
                 'help': 'download location, default FLOOD_SAMPLES_DIR or cwd',
             },
             {
                 'name': ('-d', '--datatypes'),
                 'help': 'datatypes to sample, default all',
             },
-            {
-                'name': ('-m', '--missing'),
-                'help': 'only download missing files',
-                'action': 'store_true',
-            },
         ],
     }
 
 
-def download_samples_command(
+def samples_collect_command(
     network: str | None,
     sizes: typing.Sequence[str] | None,
     output_dir: str | None,
     datatypes: typing.Sequence[str] | None,
-    missing: bool,
 ) -> None:
+    if output_dir is None:
+        output_dir = flood.generators.get_flood_samples_dir()
     if network is None:
         network = 'ethereum'
-    if sizes is None:
-        sizes = ['L']
-    if sizes == 'all':
-        sizes = list(flood.default_sizes.keys())
-    if output_dir is None:
-        output_dir = flood.get_flood_samples_dir()
-
-    flood.download_raw_data(
+    flood.generators.create_samples_dataset(
+        output_dir=output_dir,
         network=network,
         sizes=sizes,
         datatypes=datatypes,
-        output_dir=output_dir,
-        only_missing=missing,
     )
```

### Comparing `paradigm-flood-0.2.5/flood/cli/samples_ls_command.py` & `paradigm_flood-0.3.0/flood/cli/samples_ls_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     }
 
 
 def samples_ls_command() -> None:
     version = 'v1_0_0'
 
     # parse contents of flood samples dir
-    samples_dir = flood.get_flood_samples_dir()
+    samples_dir = flood.generators.get_flood_samples_dir()
     files_by_network: dict[str, list[str]] = {}
     for filename in os.listdir(samples_dir):
         if filename.endswith('parquet'):
             network = filename.split('_')[0]
             files_by_network.setdefault(network, [])
             files_by_network[network].append(filename)
     for network in list(files_by_network.keys()):
@@ -35,17 +35,17 @@
         print(samples_dir)
         print()
         toolstr.print_header('Local Files')
         for filename in files_by_network[network]:
             print('-', filename)
 
         missing = []
-        for size in flood.default_sizes:
-            for datatype in flood.default_datatypes:
-                filename = flood.raw_data_file_template.format(
+        for size in flood.generators.default_sizes:
+            for datatype in flood.generators.default_datatypes:
+                filename = flood.generators.raw_data_file_template.format(
                     network=network,
                     size=size,
                     datatype=datatype,
                     version=version,
                 )
                 if filename not in files_by_network[network]:
                     missing.append(filename)
```

### Comparing `paradigm-flood-0.2.5/flood/generators/object_generators/address_generators.py` & `paradigm_flood-0.3.0/flood/generators/object_generators/address_generators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from __future__ import annotations
 
 import typing
 
 import flood
+from flood import generators
 
 
 def generate_contract_addresses(
     n: int,
     network: str,
     random_seed: flood.RandomSeed | None = None,
 ) -> typing.Sequence[str]:
-    return flood.load_samples(
+    return generators.load_samples(
         network=network,
         datatype='contracts',
         n=n,
         random_seed=random_seed,
     )
 
 
 def generate_eoas(
     n: int,
     network: str,
     random_seed: flood.RandomSeed | None = None,
 ) -> typing.Sequence[str]:
-    return flood.load_samples(
+    return generators.load_samples(
         network=network,
         datatype='eoas',
         n=n,
         random_seed=random_seed,
     )
```

### Comparing `paradigm-flood-0.2.5/flood/generators/object_generators/block_generators.py` & `paradigm_flood-0.3.0/flood/generators/object_generators/block_generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     import numpy as np
 
     # seed a generator
     rng = rng_utils.get_rng(random_seed=random_seed)
 
     # generate blocks
     all_blocks = np.arange(start_block, end_block + 1)
-    chosen_array = rng.choice(all_blocks, size=n, replace=replace)
+    chosen_array = rng.choice(all_blocks, size=n, replace=(n > len(all_blocks)))
     chosen: list[int] = chosen_array.tolist()
 
     # sort
     if sort:
         chosen = sorted(chosen)
 
     return chosen
```

### Comparing `paradigm-flood-0.2.5/flood/generators/object_generators/call_generators.py` & `paradigm_flood-0.3.0/flood/generators/object_generators/call_generators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import typing
 
 import flood
-from flood import spec
+from flood import generators
 from . import address_generators
 from . import block_generators
 from . import slot_generators
 from . import transaction_generators
 
 
 #
@@ -16,21 +16,21 @@
 
 
 def generate_calls_eth_get_block_by_number(
     n_calls: int | None = None,
     *,
     network: str | None = None,
     block_numbers: typing.Sequence[int] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if block_numbers is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         block_numbers = block_generators.generate_block_numbers(
             n=n_calls,
             random_seed=random_seed,
             start_block=0,
             end_block=16_000_000,
             network=network,
         )
@@ -41,60 +41,92 @@
 
 
 def generate_calls_eth_get_block_by_hash(
     n_calls: int | None = None,
     *,
     network: str | None = None,
     block_hashes: typing.Sequence[str] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if block_hashes is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         block_hashes = block_generators.generate_block_hashes(
             n=n_calls,
             network=network,
             random_seed=random_seed,
         )
     return [
         ctc.rpc.construct_eth_get_block_by_hash(block_hash=block_hash)
         for block_hash in block_hashes
     ]
 
 
+def generate_calls_eth_fee_history(
+    n_calls: int | None = None,
+    *,
+    network: str | None = None,
+    random_seed: flood.RandomSeed | None = None,
+    block_numbers: typing.Sequence[int] | None = None,
+    block_count: int | None = None
+) -> typing.Sequence[flood.Call]:
+    import ctc.rpc
+
+    if block_numbers is None:
+        if n_calls is None:
+            raise Exception('must floodify more parameters')
+        block_numbers = block_generators.generate_block_numbers(
+            n=n_calls,
+            random_seed=random_seed,
+            start_block=13_000_000,
+            end_block=17_000_000,
+            network=network,
+        )
+    if block_count is None:
+        block_count = 1024
+
+    return [
+        ctc.rpc.construct_eth_fee_history(
+            block_number,
+            block_count=block_count,
+        )
+        for block_number in block_numbers
+    ]
+
+
 #
 # # addresses
 #
 
 
 def generate_calls_eth_get_eth_balance(
     n_calls: int | None = None,
     *,
     network: str,
     addresses: typing.Sequence[str] | None = None,
     block_numbers: typing.Sequence[int] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if block_numbers is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         block_numbers = block_generators.generate_block_numbers(
             start_block=10_000_000,
             end_block=16_000_000,
             n=n_calls,
             random_seed=random_seed,
             network=network,
         )
     if addresses is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         addresses = address_generators.generate_contract_addresses(
             n_calls,
             network=network,
             random_seed=random_seed,
         )
 
     return [
@@ -107,31 +139,31 @@
 
 def generate_calls_eth_get_transaction_count(
     n_calls: int | None = None,
     *,
     network: str,
     addresses: typing.Sequence[str] | None = None,
     block_numbers: typing.Sequence[int] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if block_numbers is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         block_numbers = block_generators.generate_block_numbers(
             start_block=10_000_000,
             end_block=16_000_000,
             n=n_calls,
             random_seed=random_seed,
             network=network,
         )
     if addresses is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         addresses = address_generators.generate_eoas(
             n_calls,
             network=network,
             random_seed=random_seed,
         )
 
     return [
@@ -148,21 +180,21 @@
 
 
 def generate_calls_eth_get_transaction_by_hash(
     n_calls: int | None = None,
     *,
     network: str,
     transaction_hashes: typing.Sequence[str] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if transaction_hashes is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         transaction_hashes = transaction_generators.generate_transaction_hashes(
             n_calls,
             network=network,
             random_seed=random_seed,
         )
     return [
         ctc.rpc.construct_eth_get_transaction_by_hash(
@@ -173,21 +205,21 @@
 
 
 def generate_calls_eth_get_transaction_receipt(
     n_calls: int | None = None,
     *,
     network: str,
     transaction_hashes: typing.Sequence[str] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if transaction_hashes is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         transaction_hashes = transaction_generators.generate_transaction_hashes(
             n_calls,
             network=network,
             random_seed=random_seed,
         )
     return [
         ctc.rpc.construct_eth_get_transaction_receipt(
@@ -215,29 +247,32 @@
 
 def generate_calls_eth_get_logs(
     n_calls: int | None = None,
     *,
     contract_address: str | None = None,
     topics: typing.Sequence[str | None] | None = None,
     block_ranges: typing.Sequence[tuple[int, int]] | None = None,
+    block_range_size: int | None = None,
     network: str | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if contract_address is None:
         contract_address = _default_contracts['USDC']
     if block_ranges is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
+        if block_range_size is None:
+            block_range_size = 100
         block_ranges = block_generators.generate_block_ranges(
             start_block=10_000_000,
             end_block=16_000_000,
             n=n_calls,
-            range_size=100,
+            range_size=block_range_size,
             random_seed=random_seed,
             network=network,
         )
     if topics is None:
         topics = [_default_event_hashes['Transfer']]
     return [
         ctc.rpc.construct_eth_get_logs(
@@ -258,31 +293,31 @@
 def generate_calls_eth_get_code(
     n_calls: int | None = None,
     *,
     network: str,
     addresses: typing.Sequence[str] | None = None,
     block_numbers: typing.Sequence[int | typing.Literal['latest']]
     | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if block_numbers is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         block_numbers = block_generators.generate_block_numbers(
             start_block=10_000_000,
             end_block=16_000_000,
             n=n_calls,
             random_seed=random_seed,
             network=network,
         )
     if addresses is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         addresses = address_generators.generate_contract_addresses(
             n_calls,
             network=network,
             random_seed=random_seed,
         )
     return [
         ctc.rpc.construct_eth_get_code(
@@ -295,31 +330,31 @@
 def generate_calls_eth_get_storage_at(
     n_calls: int | None = None,
     *,
     network: str,
     slots: typing.Sequence[tuple[str, str]] | None = None,
     block_numbers: typing.Sequence[int | typing.Literal['latest']]
     | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if block_numbers is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         block_numbers = block_generators.generate_block_numbers(
             start_block=10_000_000,
             end_block=16_000_000,
             n=n_calls,
             random_seed=random_seed,
             network=network,
         )
     if slots is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         slots = slot_generators.generate_slots(
             n_calls, network=network, random_seed=random_seed
         )
     return [
         ctc.rpc.construct_eth_get_storage_at(
             address=address, position=slot, block_number=block_number
         )
@@ -333,22 +368,22 @@
     'symbol': '0x95d89b41',
 }
 
 
 def generate_calls_eth_call(
     n_calls: int,
     network: str,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if network != 'ethereum':
         raise Exception('only ethereum supported for eth_call')
 
-    rng = flood.get_rng(random_seed=random_seed)
+    rng = generators.get_rng(random_seed=random_seed)
     contract_addresses = rng.choice(
         list(_default_contracts.values()),
         size=n_calls,
     )
     call_datas = rng.choice(
         list(_default_call_datas.values()),
         size=n_calls,
@@ -379,21 +414,21 @@
 
 
 def generate_calls_trace_block(
     n_calls: int | None = None,
     *,
     block_numbers: typing.Sequence[int] | None = None,
     network: str | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if block_numbers is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         block_numbers = block_generators.generate_block_numbers(
             n=n_calls,
             random_seed=0,
             start_block=0,
             end_block=16_000_000,
             network=network,
         )
@@ -404,23 +439,23 @@
 
 
 def generate_calls_trace_transaction(
     n_calls: int | None = None,
     *,
     transaction_hashes: typing.Sequence[str] | None = None,
     network: str | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if transaction_hashes is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         if network is None:
-            raise Exception('must specify network')
+            raise Exception('must floodify network')
         transaction_hashes = transaction_generators.generate_transaction_hashes(
             n=n_calls,
             network=network,
             random_seed=random_seed,
         )
     return [
         ctc.rpc.construct_trace_transaction(transaction_hash=transaction_hash)
@@ -429,21 +464,21 @@
 
 
 def generate_calls_trace_replay_block_transactions(
     n_calls: int | None = None,
     *,
     block_numbers: typing.Sequence[int] | None = None,
     network: str | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if block_numbers is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         block_numbers = block_generators.generate_block_numbers(
             n=n_calls,
             random_seed=random_seed,
             start_block=0,
             end_block=16_000_000,
             network=network,
         )
@@ -457,21 +492,21 @@
 
 
 def generate_calls_trace_replay_block_transactions_state_diff(
     n_calls: int | None = None,
     *,
     block_numbers: typing.Sequence[int] | None = None,
     network: str | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if block_numbers is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         block_numbers = block_generators.generate_block_numbers(
             n=n_calls,
             random_seed=random_seed,
             start_block=0,
             end_block=16_000_000,
             network=network,
         )
@@ -485,21 +520,21 @@
 
 
 def generate_calls_trace_replay_block_transactions_vm_trace(
     n_calls: int | None = None,
     *,
     block_numbers: typing.Sequence[int] | None = None,
     network: str | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if block_numbers is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         block_numbers = block_generators.generate_block_numbers(
             n=n_calls,
             random_seed=random_seed,
             start_block=0,
             end_block=16_000_000,
             network=network,
         )
@@ -513,23 +548,23 @@
 
 
 def generate_calls_trace_replay_transaction(
     n_calls: int | None = None,
     *,
     transaction_hashes: typing.Sequence[str] | None = None,
     network: str | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if transaction_hashes is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         if network is None:
-            raise Exception('must specify network')
+            raise Exception('must floodify network')
         transaction_hashes = transaction_generators.generate_transaction_hashes(
             n=n_calls,
             random_seed=random_seed,
             network=network,
         )
     return [
         ctc.rpc.construct_trace_replay_transaction(
@@ -541,23 +576,23 @@
 
 
 def generate_calls_trace_replay_transaction_state_diff(
     n_calls: int | None = None,
     *,
     transaction_hashes: typing.Sequence[str] | None = None,
     network: str | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if transaction_hashes is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         if network is None:
-            raise Exception('must specify network')
+            raise Exception('must floodify network')
         transaction_hashes = transaction_generators.generate_transaction_hashes(
             n=n_calls,
             random_seed=random_seed,
             network=network,
         )
     return [
         ctc.rpc.construct_trace_replay_transaction(
@@ -569,23 +604,23 @@
 
 
 def generate_calls_trace_replay_transaction_vm_trace(
     n_calls: int | None = None,
     *,
     transaction_hashes: typing.Sequence[str] | None = None,
     network: str | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> typing.Sequence[spec.Call]:
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.Call]:
     import ctc.rpc
 
     if transaction_hashes is None:
         if n_calls is None:
-            raise Exception('must specify more parameters')
+            raise Exception('must floodify more parameters')
         if network is None:
-            raise Exception('must specify network')
+            raise Exception('must floodify network')
         transaction_hashes = transaction_generators.generate_transaction_hashes(
             n=n_calls,
             random_seed=random_seed,
             network=network,
         )
     return [
         ctc.rpc.construct_trace_replay_transaction(
```

### Comparing `paradigm-flood-0.2.5/flood/generators/object_generators/timing_generators.py` & `paradigm_flood-0.3.0/flood/generators/object_generators/timing_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.5/flood/generators/raw_data_sources/raw_download_utils.py` & `paradigm_flood-0.3.0/flood/generators/raw_data_sources/raw_download_utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.5/flood/generators/raw_data_sources/raw_gather_utils.py` & `paradigm_flood-0.3.0/flood/generators/raw_data_sources/raw_gather_utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.5/flood/generators/raw_data_sources/raw_sample_loading.py` & `paradigm_flood-0.3.0/flood/generators/raw_data_sources/raw_sample_loading.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import typing
 
 import flood
+from flood import generators
 from . import raw_data_spec
 from . import raw_download_utils
 
 if typing.TYPE_CHECKING:
     import polars as pl
 
 
@@ -17,15 +18,15 @@
     size: str | None = None,
     version: str = raw_data_spec.raw_data_version,
     samples_dir: str | None = None,
 ) -> str | None:
     import os
 
     if samples_dir is None:
-        samples_dir = flood.get_flood_samples_dir()
+        samples_dir = generators.get_flood_samples_dir()
 
     # get largest_available file present
     if size is None:
         size = 'largest_available'
     if size == 'largest_available':
         import glob
 
@@ -149,15 +150,15 @@
     df = pl.scan_parquet(path).select(columns).collect()
     if n > len(df):
         import math
 
         n_copies = math.ceil(n / len(df))
         df = pl.concat(n_copies * [df])
     if n < len(df):
-        rng = flood.get_rng(random_seed=random_seed)
+        rng = generators.get_rng(random_seed=random_seed)
         seed = rng.integers(1_000_000_000, size=1)[0]
         df = df.sample(n, shuffle=True, seed=seed)
 
     for column in df.select(pl.col(pl.Binary)).columns:
         df = df.with_columns(
             ('0x' + pl.col(column).bin.encode('hex')).alias(column)
         )
```

### Comparing `paradigm-flood-0.2.5/flood/generators/rng_utils.py` & `paradigm_flood-0.3.0/flood/generators/rng_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     import numpy as np
 
 
 def get_rng(random_seed: spec.RandomSeed | None = None) -> np.random.Generator:
     import numpy as np
 
     if random_seed is None:
-        random_seed = 0
+        import time
+
+        random_seed = int(time.time())
     if isinstance(random_seed, int):
         gen = np.random.Generator(np.random.PCG64(random_seed))
     if isinstance(gen, np.random.Generator):
         return gen
     else:
         raise Exception('invalid seed format: ' + str(type(random_seed)))
```

### Comparing `paradigm-flood-0.2.5/flood/generators/test_generators/address_test_generators.py` & `paradigm_flood-0.3.0/flood/generators/test_generators/transaction_test_generators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 from __future__ import annotations
 
 import typing
 
 import flood
-from flood import spec
+from flood.tests import load_tests
 
 
-def generate_test_eth_get_balance(
+def generate_test_eth_get_transaction_by_hash(
     *,
     rates: typing.Sequence[int],
     duration: int | None = None,
-    durations: typing.Sequence[int] | None = None,
     network: str,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> spec.LoadTest:
-    n_calls = flood.estimate_call_count(
+    durations: typing.Sequence[int] | None = None,
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_eth_get_eth_balance(
+    calls = flood.generators.generate_calls_eth_get_transaction_by_hash(
         n_calls=n_calls,
         network=network,
         random_seed=random_seed,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
 
 
-def generate_test_eth_get_transaction_count(
+def generate_test_eth_get_transaction_receipt(
     *,
     rates: typing.Sequence[int],
     duration: int | None = None,
-    durations: typing.Sequence[int] | None = None,
     network: str,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> spec.LoadTest:
-    n_calls = flood.estimate_call_count(
+    durations: typing.Sequence[int] | None = None,
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_eth_get_transaction_count(
+    calls = flood.generators.generate_calls_eth_get_transaction_receipt(
         n_calls=n_calls,
         network=network,
         random_seed=random_seed,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
```

### Comparing `paradigm-flood-0.2.5/flood/generators/test_generators/block_test_generators.py` & `paradigm_flood-0.3.0/flood/generators/test_generators/address_test_generators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 from __future__ import annotations
 
 import typing
 
-from flood import spec
 import flood
+from flood.tests import load_tests
 
 
-def generate_test_eth_get_block_by_number(
+def generate_test_eth_get_balance(
     *,
     rates: typing.Sequence[int],
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
     network: str,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> flood.LoadTest:
-    n_calls = flood.estimate_call_count(
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_eth_get_block_by_number(
+    calls = flood.generators.generate_calls_eth_get_eth_balance(
         n_calls=n_calls,
         network=network,
         random_seed=random_seed,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
 
 
-# def generate_test_eth_get_block_by_hash(
-#     *,
-#     rates: typing.Sequence[int],
-#     duration: int | None = None,
-#     durations: typing.Sequence[int] | None = None,
-#     network: str,
-#     vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-#     random_seed: spec.RandomSeed | None = None,
-# ) -> flood.LoadTest:
-#     n_calls = flood.estimate_call_count(
-#         rates=rates, duration=duration, durations=durations
-#     )
-#     calls = flood.generate_calls_eth_get_block_by_hash(
-#         n_calls=n_calls,
-#         network=network,
-#         random_seed=random_seed,
-#     )
-#     return flood.create_load_test(
-#         calls=calls,
-#         rates=rates,
-#         duration=duration,
-#         durations=durations,
-#     )
+def generate_test_eth_get_transaction_count(
+    *,
+    rates: typing.Sequence[int],
+    duration: int | None = None,
+    durations: typing.Sequence[int] | None = None,
+    network: str,
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
+        rates=rates, duration=duration, durations=durations
+    )
+    calls = flood.generators.generate_calls_eth_get_transaction_count(
+        n_calls=n_calls,
+        network=network,
+        random_seed=random_seed,
+    )
+    return load_tests.create_load_test(
+        calls=calls,
+        rates=rates,
+        duration=duration,
+        durations=durations,
+        vegeta_args=vegeta_args,
+    )
```

### Comparing `paradigm-flood-0.2.5/flood/generators/test_generators/contract_test_generators.py` & `paradigm_flood-0.3.0/flood/generators/test_generators/block_test_generators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,85 @@
 from __future__ import annotations
 
 import typing
 
+from flood import spec
+from flood.tests import load_tests
 import flood
 
 
-def generate_test_eth_get_code(
+def generate_test_eth_get_block_by_number(
     *,
     rates: typing.Sequence[int],
-    network: str,
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    random_seed: flood.RandomSeed | None = None,
-) -> flood.LoadTest:
-    n_calls = flood.estimate_call_count(
+    network: str,
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
+    random_seed: spec.RandomSeed | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_eth_get_code(
+    calls = flood.generators.generate_calls_eth_get_block_by_number(
         n_calls=n_calls,
         network=network,
         random_seed=random_seed,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
 
 
-def generate_test_eth_get_storage_at(
+def generate_test_eth_fee_history(
     *,
     rates: typing.Sequence[int],
-    network: str,
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    random_seed: flood.RandomSeed | None = None,
-) -> flood.LoadTest:
-    n_calls = flood.estimate_call_count(
+    network: str,
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
+    random_seed: spec.RandomSeed | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_eth_get_storage_at(
+    calls = flood.generators.generate_calls_eth_fee_history(
         n_calls=n_calls,
         network=network,
         random_seed=random_seed,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
 
 
-def generate_test_eth_call(
-    *,
-    rates: typing.Sequence[int],
-    network: str,
-    duration: int | None = None,
-    durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    random_seed: flood.RandomSeed | None = None,
-) -> flood.LoadTest:
-    n_calls = flood.estimate_call_count(
-        rates=rates, duration=duration, durations=durations
-    )
-    calls = flood.generate_calls_eth_call(
-        n_calls=n_calls,
-        network=network,
-        random_seed=random_seed,
-    )
-    return flood.create_load_test(
-        calls=calls,
-        rates=rates,
-        duration=duration,
-        durations=durations,
-    )
+# def generate_test_eth_get_block_by_hash(
+#     *,
+#     rates: typing.Sequence[int],
+#     duration: int | None = None,
+#     durations: typing.Sequence[int] | None = None,
+#     network: str,
+#     vegeta_args: typing.Mapping[str, str | None] | None = None,
+#     random_seed: spec.RandomSeed | None = None,
+# ) -> typing.Sequence[flood.VegetaAttack]:
+#     n_calls = load_tests.estimate_call_count(
+#         rates=rates, duration=duration, durations=durations
+#     )
+#     calls = flood.generate_calls_eth_get_block_by_hash(
+#         n_calls=n_calls,
+#         network=network,
+#         random_seed=random_seed,
+#     )
+#     return load_tests.create_load_test(
+#         calls=calls,
+#         rates=rates,
+#         duration=duration,
+#         durations=durations,
+        # vegeta_args=vegeta_args,
+#     )
```

### Comparing `paradigm-flood-0.2.5/flood/generators/test_generators/generic_test_generators.py` & `paradigm_flood-0.3.0/flood/generators/test_generators/generic_test_generators.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,147 +9,109 @@
 # # bookkeeping
 #
 
 
 def get_single_test_generators() -> (
     typing.Mapping[str, flood.LoadTestGenerator]
 ):
+    """get all single test generators"""
     return {
         get_test_generator_display_name(item): item  # type: ignore
-        for item in dir(flood)
+        for item in dir(flood.generators)
         if item.startswith('generate_test_')
     }
 
 
 def get_multi_test_generators() -> (
     typing.Mapping[str, flood.MultiLoadTestGenerator]
 ):
+    """get all multi test generators"""
     return {
         get_test_generator_display_name(item, multi=True): item  # type: ignore
-        for item in dir(flood)
+        for item in dir(flood.generators)
         if item.startswith('generate_tests_')
     }
 
 
 def get_test_generator(test_name: str) -> flood.LoadTestGenerator:
+    """get particular single test generator"""
     function_name = get_test_generator_function_name(test_name)
-    if hasattr(flood, function_name):
-        return getattr(flood, function_name)  # type: ignore
+    if hasattr(flood.generators, function_name):
+        return getattr(flood.generators, function_name)  # type: ignore
     else:
         raise Exception()
 
 
 def get_tests_generator(test_name: str) -> flood.MultiLoadTestGenerator:
+    """get particular multi test generator"""
     function_name = get_test_generator_function_name(test_name)
-    if hasattr(flood, function_name):
-        return getattr(flood, function_name)  # type: ignore
+    if hasattr(flood.generators, function_name):
+        return getattr(flood.generators, function_name)  # type: ignore
     else:
         raise Exception()
 
 
-def get_test_generator_display_name(
-    test: str | flood.LoadTestGenerator,
-    multi: bool = False,
-) -> str:
-    if multi:
-        prefix = 'generate_tests_'
-    else:
-        prefix = 'generate_test_'
-
-    if not isinstance(test, str):
-        import types
-
-        if not isinstance(test, types.FunctionType):
-            raise Exception('should be str or function')
-        test = test.__name__
-
-    if not test.startswith(prefix):
-        raise Exception()
-    test = test[len(prefix) :]
-    head, tail = test.split('_', 1)
-    test = head + '_' + _snake_case_to_camel_case(tail)
-    return test
-
-
-def get_test_generator_function_name(
-    display_name: str, multi: bool = False
-) -> str:
-    if multi:
-        prefix = 'generate_tests_'
-    else:
-        prefix = 'generate_test_'
-
-    function_name = prefix + _camel_case_to_snake_case(display_name)
-    return function_name
-
-
-def _camel_case_to_snake_case(string: str) -> str:
-    # adapted from https://stackoverflow.com/a/1176023
-    import re
-
-    return re.sub(r'(?<!^)(?=[A-Z])', '_', string).lower()
-
-
-def _snake_case_to_camel_case(string: str) -> str:
-    pieces = string.split('_')
-    return pieces[0] + ''.join(piece.title() for piece in pieces[1:])
-
-
 #
 # # generation
 #
 
 
 def generate_test(
     *,
     test_name: str,
     random_seed: flood.RandomSeed | None = None,
     rates: typing.Sequence[int] | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: flood.VegetaKwargsShorthand | None = None,
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
     network: str,
-    output_dir: str | None = None,
+    # output_dir: str | None = None,
+    flood_version: str,
 ) -> flood.LoadTest:
     if test_name is None:
         raise Exception('must specify test_name')
     test_generator = get_test_generator(test_name)
-    test = test_generator(
+    test_parameters: flood.TestGenerationParameters = {
+        'flood_version': flood.get_flood_version(),
+        'test_name': test_name,
+        'random_seed': random_seed,
+        'rates': rates,
+        'durations': durations,
+        'vegeta_args': vegeta_args,
+        'network': network,
+    }
+    attacks = test_generator(
         rates=rates,
         durations=durations,
-        vegeta_kwargs=vegeta_kwargs,
+        vegeta_args=vegeta_args,
         network=network,
         random_seed=random_seed,
     )
-    if output_dir is not None:
-        flood.runners.single_runner.single_runner_io._save_single_run_test(
-            test_name=test_name, output_dir=output_dir, test=test
-        )
-    return test
+    return {'attacks': attacks, 'test_parameters': test_parameters}
 
 
 def generate_tests(
     *,
     test_name: str,
     random_seed: flood.RandomSeed | None = None,
     rates: typing.Sequence[int] | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: flood.VegetaKwargsShorthand | None = None,
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
     network: str,
     output_dir: str | None = None,
     common_parameters: typing.Mapping[str, typing.Any] | None = None,
     specific_parameters: typing.Mapping[str, typing.Mapping[str, typing.Any]]
     | None = None,
 ) -> typing.Mapping[str, flood.LoadTest]:
     if test_name is None:
         raise Exception('must specify test_name')
     test_generator = get_tests_generator(test_name)
     tests = test_generator(
         rates=rates,
         durations=durations,
-        vegeta_kwargs=vegeta_kwargs,
+        vegeta_args=vegeta_args,
         network=network,
         random_seed=random_seed,
         common_parameters=common_parameters,
         specific_parameters=specific_parameters,
     )
     if output_dir is not None:
         flood.runners.multi_runner.multi_runner_io._save_multi_run_tests(
@@ -187,7 +149,67 @@
 #     tests = []
 #     for test_kwargs in tests_kwargs:
 #         test = test_generator(**test_kwargs)
 #         tests.append(test)
 
 #     return tests
 
+
+#
+# # name formatting
+#
+
+
+def get_test_generator_display_name(
+    test: str | flood.LoadTestGenerator,
+    multi: bool = False,
+) -> str:
+    if multi:
+        prefix = 'generate_tests_'
+    else:
+        prefix = 'generate_test_'
+
+    if not isinstance(test, str):
+        test_id = id(test)
+        for key, value in vars(flood.generators).items():
+            if id(value) == test_id:
+                test = key
+                break
+        else:
+            import types
+
+            if isinstance(test, types.FunctionType):
+                test = test.__name__
+            else:
+                raise Exception('should be str or function')
+
+    if not test.startswith(prefix):
+        raise Exception()
+    test = test[len(prefix) :]
+    head, tail = test.split('_', 1)
+    test = head + '_' + _snake_case_to_camel_case(tail)
+    return test
+
+
+def get_test_generator_function_name(
+    display_name: str, multi: bool = False
+) -> str:
+    if multi:
+        prefix = 'generate_tests_'
+    else:
+        prefix = 'generate_test_'
+
+    function_name = prefix + _camel_case_to_snake_case(display_name)
+    return function_name
+
+
+def _camel_case_to_snake_case(string: str) -> str:
+    # adapted from https://stackoverflow.com/a/1176023
+    import re
+
+    return re.sub(r'(?<!^)(?=[A-Z])', '_', string).lower()
+
+
+def _snake_case_to_camel_case(string: str) -> str:
+    pieces = string.split('_')
+    return pieces[0] + ''.join(piece.title() for piece in pieces[1:])
+
```

### Comparing `paradigm-flood-0.2.5/flood/generators/test_generators/log_test_generators.py` & `paradigm_flood-0.3.0/flood/generators/test_generators/log_test_generators.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,63 @@
 from __future__ import annotations
 
+import functools
 import typing
 
 import flood
+from flood.tests import load_tests
 
 
 def generate_test_eth_get_logs(
     *,
     rates: typing.Sequence[int],
     network: str,
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
     random_seed: flood.RandomSeed | None = None,
-) -> flood.LoadTest:
-    n_calls = flood.estimate_call_count(
+    contract_address: str | None = None,
+    block_range_size: int | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_eth_get_logs(
+    calls = flood.generators.generate_calls_eth_get_logs(
         n_calls,
         network=network,
         random_seed=random_seed,
+        contract_address=contract_address,
+        block_range_size=block_range_size,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
 
 
+generate_test_eth_get_logs_lusd_transfers_s = functools.partial(
+    generate_test_eth_get_logs,
+    contract_address='0x5f98805a4e8be255a32880fdec7f6728c6568ba0',
+    block_range_size=100,
+)
+generate_test_eth_get_logs_lusd_transfers_m = functools.partial(
+    generate_test_eth_get_logs,
+    contract_address='0x5f98805a4e8be255a32880fdec7f6728c6568ba0',
+    block_range_size=1000,
+)
+generate_test_eth_get_logs_lusd_transfers_l = functools.partial(
+    generate_test_eth_get_logs,
+    contract_address='0x5f98805a4e8be255a32880fdec7f6728c6568ba0',
+    block_range_size=10000,
+)
+
+
 # def generate_tests_eth_get_logs_by_contract(
 #     url: str,
 #     rates: typing.Sequence[int],
 #     duration: int,
 #     range_size: int,
 # ) -> typing.Mapping[str, flood.LoadTest]:
 #     """test: Transfers of USDC vs DAI vs LUSD"""
```

### Comparing `paradigm-flood-0.2.5/flood/generators/test_generators/trace_test_generators.py` & `paradigm_flood-0.3.0/flood/generators/test_generators/trace_test_generators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,206 +1,215 @@
 from __future__ import annotations
 
 import typing
 
 import flood
-from flood import spec
+from flood.tests import load_tests
 
 
 def generate_test_trace_block(
     *,
     network: str,
     rates: typing.Sequence[int],
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> spec.LoadTest:
-    n_calls = flood.estimate_call_count(
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_trace_block(
+    calls = flood.generators.generate_calls_trace_block(
         n_calls=n_calls,
         network=network,
         random_seed=random_seed,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
 
 
 def generate_test_trace_transaction(
     *,
     network: str,
     rates: typing.Sequence[int],
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> spec.LoadTest:
-    n_calls = flood.estimate_call_count(
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_trace_transaction(
+    calls = flood.generators.generate_calls_trace_transaction(
         n_calls=n_calls,
         network=network,
         random_seed=random_seed,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
 
 
 def generate_test_trace_replay_block_transactions(
     *,
     network: str,
     rates: typing.Sequence[int],
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> spec.LoadTest:
-    n_calls = flood.estimate_call_count(
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_trace_replay_block_transactions(
+    calls = flood.generators.generate_calls_trace_replay_block_transactions(
         n_calls=n_calls,
         network=network,
         random_seed=random_seed,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
 
 
 def generate_test_trace_replay_block_transactions_state_diff(
     *,
     network: str,
     rates: typing.Sequence[int],
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> spec.LoadTest:
-    n_calls = flood.estimate_call_count(
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_trace_replay_block_transactions_state_diff(
+    calls = flood.generators.generate_calls_trace_replay_block_transactions_state_diff(  # noqa: E501
         n_calls=n_calls,
         network=network,
         random_seed=random_seed,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
 
 
 def generate_test_trace_replay_block_transactions_vm_trace(
     *,
     network: str,
     rates: typing.Sequence[int],
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> spec.LoadTest:
-    n_calls = flood.estimate_call_count(
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_trace_replay_block_transactions_vm_trace(
+    calls = flood.generators.generate_calls_trace_replay_block_transactions_vm_trace(  # noqa: E501
         n_calls=n_calls,
         network=network,
         random_seed=random_seed,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
 
 
 def generate_test_trace_replay_transaction(
     *,
     network: str,
     rates: typing.Sequence[int],
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> spec.LoadTest:
-    n_calls = flood.estimate_call_count(
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_trace_replay_transaction(
+    calls = flood.generators.generate_calls_trace_replay_transaction(
         n_calls=n_calls,
         network=network,
         random_seed=random_seed,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
 
 
 def generate_test_trace_replay_transaction_state_diff(
     *,
     network: str,
     rates: typing.Sequence[int],
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> spec.LoadTest:
-    n_calls = flood.estimate_call_count(
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_trace_replay_transaction_state_diff(
+    calls = flood.generators.generate_calls_trace_replay_transaction_state_diff(
         n_calls=n_calls,
         network=network,
         random_seed=random_seed,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
 
 
 def generate_test_trace_replay_transaction_vm_trace(
     *,
     network: str,
     rates: typing.Sequence[int],
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    random_seed: spec.RandomSeed | None = None,
-) -> spec.LoadTest:
-    n_calls = flood.estimate_call_count(
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_trace_replay_transaction_vm_trace(
+    calls = flood.generators.generate_calls_trace_replay_transaction_vm_trace(
         n_calls=n_calls,
         network=network,
         random_seed=random_seed,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
+
```

### Comparing `paradigm-flood-0.2.5/flood/generators/test_generators/transaction_test_generators.py` & `paradigm_flood-0.3.0/flood/generators/test_generators/contract_test_generators.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,84 @@
 from __future__ import annotations
 
 import typing
 
 import flood
+from flood.tests import load_tests
 
 
-def generate_test_eth_get_transaction_by_hash(
+def generate_test_eth_get_code(
     *,
     rates: typing.Sequence[int],
-    duration: int | None = None,
     network: str,
+    duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
     random_seed: flood.RandomSeed | None = None,
-) -> flood.LoadTest:
-    n_calls = flood.estimate_call_count(
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_eth_get_transaction_by_hash(
+    calls = flood.generators.generate_calls_eth_get_code(
         n_calls=n_calls,
         network=network,
         random_seed=random_seed,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
 
 
-def generate_test_eth_get_transaction_receipt(
+def generate_test_eth_get_storage_at(
     *,
     rates: typing.Sequence[int],
+    network: str,
     duration: int | None = None,
+    durations: typing.Sequence[int] | None = None,
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
+    random_seed: flood.RandomSeed | None = None,
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
+        rates=rates, duration=duration, durations=durations
+    )
+    calls = flood.generators.generate_calls_eth_get_storage_at(
+        n_calls=n_calls,
+        network=network,
+        random_seed=random_seed,
+    )
+    return load_tests.create_load_test(
+        calls=calls,
+        rates=rates,
+        duration=duration,
+        durations=durations,
+        vegeta_args=vegeta_args,
+    )
+
+
+def generate_test_eth_call(
+    *,
+    rates: typing.Sequence[int],
     network: str,
+    duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
     random_seed: flood.RandomSeed | None = None,
-) -> flood.LoadTest:
-    n_calls = flood.estimate_call_count(
+) -> typing.Sequence[flood.VegetaAttack]:
+    n_calls = load_tests.estimate_call_count(
         rates=rates, duration=duration, durations=durations
     )
-    calls = flood.generate_calls_eth_get_transaction_receipt(
+    calls = flood.generators.generate_calls_eth_call(
         n_calls=n_calls,
         network=network,
         random_seed=random_seed,
     )
-    return flood.create_load_test(
+    return load_tests.create_load_test(
         calls=calls,
         rates=rates,
         duration=duration,
         durations=durations,
+        vegeta_args=vegeta_args,
     )
```

### Comparing `paradigm-flood-0.2.5/flood/runners/generic_runner/generic_runner_execution.py` & `paradigm_flood-0.3.0/flood/runners/single_runner/single_runner_io.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,119 +1,154 @@
 from __future__ import annotations
 
 import typing
 
 import flood
-from flood.runners.single_runner import single_runner_execution
-# from flood.runners.multi_runner import multi_runner_execution
 
 
-def run(
+#
+# # path utiltiies
+#
+
+_path_templates = {
+    'single_run_test': '{output_dir}/test.json',
+    'single_run_results': '{output_dir}/results.json',
+    'single_run_figures_dir': '{output_dir}/figures',
+}
+
+
+def get_single_run_test_path(output_dir: str) -> str:
+    return _path_templates['single_run_test'].format(output_dir=output_dir)
+
+
+def get_single_run_results_path(output_dir: str) -> str:
+    return _path_templates['single_run_results'].format(output_dir=output_dir)
+
+
+def get_single_run_figures_path(output_dir: str) -> str:
+    return _path_templates['single_run_figures_dir'].format(
+        output_dir=output_dir
+    )
+
+
+#
+# # save utilities
+#
+
+
+def _save_single_run_test(
     test_name: str,
-    *,
-    nodes: flood.NodesShorthand | None,
-    random_seed: flood.RandomSeed | None = None,
-    verbose: bool | int = True,
-    rates: typing.Sequence[int] | None = None,
-    duration: int | None = None,
-    durations: typing.Sequence[int] | None = None,
-    mode: flood.LoadTestMode | None = None,
-    vegeta_kwargs: flood.VegetaKwargsShorthand | None = None,
-    dry: bool,
-    output_dir: str | bool | None = None,
-    figures: bool = True,
-    metrics: typing.Sequence[str] | None = None,
-    include_raw_output: bool = False,
-    deep_check: bool = False,
+    output_dir: str,
+    test_parameters: flood.TestGenerationParameters,
 ) -> None:
-    """generate and run tests against nodes"""
     import os
+    import orjson
 
-    # get output_dir
-    output_dir = _get_output_dir(output_dir)
+    if not os.path.isdir(output_dir):
+        if os.path.exists(output_dir):
+            raise Exception('output must be a directory path')
+        else:
+            os.makedirs(output_dir, exist_ok=True)
 
-    # run test from path
-    if os.path.exists(test_name) or '/' in test_name:
-        (
-            test_name,
-            path_spec,
-            test,
-            nodes,
-        ) = _load_old_test_data(test_name=test_name, nodes=nodes)
-        return single_runner_execution._run_single(
-            rerun_of=path_spec,
-            test=test,
-            #
-            test_name=test_name,
-            nodes=nodes,
-            random_seed=random_seed,
-            dry=dry,
-            output_dir=output_dir,
-            verbose=verbose,
-            metrics=metrics,
-            figures=figures,
-            include_raw_output=include_raw_output,
-            deep_check=deep_check,
-        )
+    path = _path_templates['single_run_test'].format(output_dir=output_dir)
+    payload: flood.SingleRunTestPayload = {
+        'flood_version': flood.__version__,
+        'type': 'single_test',
+        'name': test_name,
+        'test_parameters': test_parameters,
+    }
+    with open(path, 'wb') as f:
+        f.write(orjson.dumps(payload))
 
-    if nodes is None:
-        raise Exception('must specify nodes')
 
-    if test_name in flood.get_single_test_generators():
-        single_runner_execution._run_single(
-            rates=rates,
-            duration=duration,
-            durations=durations,
-            vegeta_kwargs=vegeta_kwargs,
-            #
+def _save_single_run_results(
+    *,
+    output_dir: str,
+    nodes: flood.Nodes,
+    results: typing.Mapping[str, flood.LoadTestOutput],
+    figures: bool,
+    test_name: str,
+    t_run_start: float,
+    t_run_end: float,
+) -> flood.SingleRunResultsPayload:
+    import os
+    import sys
+
+    import orjson
+
+    if not os.path.isdir(output_dir):
+        if os.path.exists(output_dir):
+            raise Exception('output must be a directory path')
+        else:
+            os.makedirs(output_dir)
+
+    path = _path_templates['single_run_results'].format(output_dir=output_dir)
+    payload: flood.SingleRunResultsPayload = {
+        'flood_version': flood.get_flood_version(),
+        'dependency_versions': flood.get_dependency_versions(),
+        'cli_args': list(sys.argv),
+        'type': 'single_test',
+        't_run_start': t_run_start,
+        't_run_end': t_run_end,
+        'nodes': nodes,
+        'results': results,
+    }
+    with open(path, 'wb') as f:
+        f.write(orjson.dumps(payload))
+
+    if figures:
+        figures_dir = get_single_run_figures_path(output_dir=output_dir)
+        colors = flood.user_io.get_nodes_plot_colors(nodes=nodes)
+        flood.tests.load_tests.plot_load_test_results(
+            outputs=results,
             test_name=test_name,
-            nodes=nodes,
-            random_seed=random_seed,
-            dry=dry,
-            output_dir=output_dir,
-            verbose=verbose,
-            metrics=metrics,
-            figures=figures,
-            include_raw_output=include_raw_output,
-            deep_check=deep_check,
+            output_dir=figures_dir,
+            colors=colors,
         )
-    elif test_name in flood.get_multi_test_generators():
-        raise NotImplementedError()
-    else:
-        raise Exception('invalid test name')
 
+    return payload
 
-def _get_output_dir(output_dir: str | bool | None) -> str | None:
-    import os
 
-    if isinstance(output_dir, bool):
-        if output_dir:
-            import tempfile
+#
+# # load utiltiies
+#
 
-            output_dir = tempfile.mkdtemp()
-        else:
-            output_dir = None
-    if output_dir is not None:
-        output_dir = os.path.abspath(os.path.expanduser(output_dir))
-
-    return output_dir
-
-
-def _load_old_test_data(
-    test_name: str, nodes: flood.NodesShorthand | None
-) -> tuple[str, str, flood.LoadTest, flood.NodesShorthand]:
-    path_spec = test_name
-
-    try:
-        test_payload = flood.load_single_run_test_payload(path_spec)
-        test = test_payload['test']
-        test_name = test_payload['name']
-    except Exception:
-        raise Exception('invalid test path: ' + str(path_spec))
-
-    # use old nodes if none specified
-    if nodes is None:
-        results_payload = flood.load_single_run_results_payload(path_spec)
-        nodes = results_payload['nodes']
 
-    return (test_name, path_spec, test, nodes)
+def load_single_run_test_payload(
+    path_spec: str,
+    allow_other_versions: bool = False,
+) -> flood.SingleRunTestPayload:
+    import os
+    import orjson
+
+    if os.path.isfile(path_spec):
+        path = path_spec
+    else:
+        path = get_single_run_test_path(path_spec)
+    with open(path, 'rb') as f:
+        test: flood.SingleRunTestPayload = orjson.loads(f.read())
+
+    if test['flood_version'] != flood.__version__:
+        if allow_other_versions:
+            pass
+        else:
+            raise Exception(
+                'loaded test version ('
+                + str(test['flood_version'])
+                + ') does not match current flood version ('
+                + flood.__version__
+                + ')'
+            )
+
+    return test
+
+
+def load_single_run_results_payload(
+    output_dir: str,
+) -> flood.SingleRunResultsPayload:
+    import orjson
+
+    path = get_single_run_results_path(output_dir=output_dir)
+    with open(path, 'rb') as f:
+        results: flood.SingleRunResultsPayload = orjson.loads(f.read())
+    return results
```

### Comparing `paradigm-flood-0.2.5/flood/runners/multi_runner/multi_runner_io.py` & `paradigm_flood-0.3.0/flood/runners/multi_runner/multi_runner_io.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from __future__ import annotations
 
 import typing
 
 import flood
-from ..single_runner import single_runner_io
 
 
 _path_templates = {
     'multi_indicator': 'multi_test.fyi',
 }
 
 
 def _save_multi_run_tests(
     output_dir: str,
     tests: typing.Mapping[str, flood.LoadTest],
 ) -> None:
-    import os
+    raise NotImplementedError()
+    # import os
 
-    # make output dir
-    if not os.path.isdir(output_dir):
-        if os.path.exists(output_dir):
-            raise Exception('output must be a directory path')
-        else:
-            os.makedirs(output_dir, exist_ok=True)
-
-    # create individual tests
-    for test_name, test in tests.items():
-        single_runner_io._save_single_run_test(
-            test_name=test_name,
-            output_dir=os.path.join(output_dir, test_name),
-            test=test,
-        )
-
-    # create multitest indicator file
-    indicator_path = os.path.join(
-        output_dir, _path_templates['multi_indicator']
-    )
-    with open(indicator_path, 'a'):
-        pass
+    # # make output dir
+    # if not os.path.isdir(output_dir):
+    #     if os.path.exists(output_dir):
+    #         raise Exception('output must be a directory path')
+    #     else:
+    #         os.makedirs(output_dir, exist_ok=True)
+
+    # # create individual tests
+    # for test_name, test in tests.items():
+    #     single_runner_io._save_single_run_test(
+    #         test_name=test_name,
+    #         output_dir=os.path.join(output_dir, test_name),
+    #         test=test,
+    #     )
+
+    # # create multitest indicator file
+    # indicator_path = os.path.join(
+    #     output_dir, _path_templates['multi_indicator']
+    # )
+    # with open(indicator_path, 'a'):
+    #     pass
 
 
 def _load_multi_run_tests(
     output_dir: str,
 ) -> typing.Mapping[str, flood.LoadTest]:
     raise NotImplementedError()
```

### Comparing `paradigm-flood-0.2.5/flood/runners/single_runner/single_runner_execution.py` & `paradigm_flood-0.3.0/flood/runners/single_runner/single_runner_execution.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,170 +14,146 @@
     test: flood.LoadTest | None = None,
     nodes: flood.NodesShorthand,
     random_seed: flood.RandomSeed | None = None,
     rates: typing.Sequence[int] | None = None,
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
     mode: flood.LoadTestMode | None = None,
-    vegeta_kwargs: flood.VegetaKwargsShorthand | None = None,
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
     dry: bool,
-    output_dir: str | None = None,
+    output_dir: str,
     figures: bool,
     metrics: typing.Sequence[str] | None = None,
     verbose: bool | int,
-    include_raw_output: bool = False,
+    include_deep_output: typing.Sequence[flood.DeepOutput] | None = None,
     deep_check: bool = False,
-) -> None:
-    if deep_check:
-        include_raw_output = True
+) -> flood.SingleRunOutput:
+    import time
+
+    t_start = time.time()
+
+    if include_deep_output is None:
+        include_deep_output = []
+    if deep_check and 'metrics' not in include_deep_output:
+        include_deep_output = list(include_deep_output) + ['metrics']
 
     # get test parameters
-    rates, durations, vegeta_kwargs = _get_single_test_parameters(
+    rates, durations, vegeta_args = _get_single_test_parameters(
         test=test,
         rates=rates,
         duration=duration,
         durations=durations,
         mode=mode,
+        vegeta_args=vegeta_args,
     )
 
     # print preamble
     if verbose:
         single_runner_summary._print_single_run_preamble_copy(
             test_name=test_name,
             rerun_of=rerun_of,
             rates=rates,
             durations=durations,
-            vegeta_kwargs=vegeta_kwargs,
+            vegeta_args=vegeta_args,
             output_dir=output_dir,
         )
 
     # parse nodes
-    nodes = flood.parse_nodes(nodes, verbose=verbose, request_metadata=True)
+    nodes = flood.user_io.parse_nodes(
+        nodes, verbose=verbose, request_metadata=True
+    )
 
     # generate test and save to disk
+    use_test: flood.LoadTest | flood.TestGenerationParameters
+    test_parameters: flood.TestGenerationParameters
     if test is None:
-        test = flood.generate_test(
+        test_parameters = {
+            'flood_version': flood.get_flood_version(),
+            'test_name': test_name,
+            'rates': rates,
+            'durations': durations,
+            'vegeta_args': vegeta_args,
+            'network': flood.user_io.parse_nodes_network(nodes),
+            'random_seed': random_seed,
+        }
+        flood.runners.single_runner.single_runner_io._save_single_run_test(
             test_name=test_name,
-            rates=rates,
-            durations=durations,
-            vegeta_kwargs=vegeta_kwargs,
-            network=flood.parse_nodes_network(nodes),
-            random_seed=random_seed,
             output_dir=output_dir,
+            test_parameters=test_parameters,
         )
+        use_test = test_parameters
+    else:
+        test_parameters = test['test_parameters']
+        use_test = test
 
     # skip dry run
     if dry:
         print()
         print('[dry run, exitting]')
-        return
+        return  # type: ignore
 
     # run tests
     if verbose:
         single_runner_summary._print_run_start()
     results = flood.run_load_tests(
         nodes=nodes,
-        test=test,
+        test=use_test,
         verbose=verbose,
-        include_raw_output=include_raw_output,
+        include_deep_output=include_deep_output,
     )
 
     # output results to file
-    if output_dir is not None:
-        single_runner_io._save_single_run_results(
-            output_dir=output_dir,
-            test=test,
-            nodes=nodes,
-            results=results,
-            figures=figures,
-            test_name=test_name,
-        )
-
-    # perform deep check
-    if deep_check:
-        _perform_deep_check(results, verbose=verbose)
+    payload = single_runner_io._save_single_run_results(
+        output_dir=output_dir,
+        nodes=nodes,
+        results=results,
+        figures=figures,
+        test_name=test_name,
+        t_run_start=t_start,
+        t_run_end=time.time(),
+    )
 
     # print summary
     if verbose:
-        single_runner_summary._print_single_run_conclusion_copy(
+        single_runner_summary._print_single_run_conclusion(
             output_dir=output_dir,
             results=results,
             metrics=metrics,
             verbose=verbose,
             figures=figures,
+            deep_check=deep_check,
         )
 
-
-#
-# # helper functions
-#
-
-
-def _perform_deep_check(
-    results: typing.Mapping[str, flood.LoadTestOutput],
-    verbose: bool | int = False,
-) -> None:
-    """
-    check that responses for each success are
-    1) well-formed json
-    and 2) error = None
-    """
-    import base64
-    import json
-
-    errors = False
-
-    raw_output = flood.load_single_run_raw_output(results=results)
-    for result_name, result in raw_output.items():
-        for status_code, response in zip(
-            result['status_code'], result['response'].to_list()
-        ):
-            if status_code == 200:
-                try:
-                    decoded = json.loads(base64.b64decode(response))
-                    if decoded.get('result') is None:
-                        errors = True
-                except Exception:
-                    errors = True
-
-            if errors:
-                break
-        if errors:
-            break
-
-    if verbose:
-        if errors:
-            print()
-            print('[deep check passed]')
-        else:
-            print('[deep check failed]')
-
-    if errors:
-        raise Exception('some calls that were reported successful had bad data')
+    return {
+        'output_dir': output_dir,
+        'test': test,
+        'test_parameters': test_parameters,
+        'payload': payload,
+    }
 
 
 def _get_single_test_parameters(
     test: flood.LoadTest | None = None,
     rates: typing.Sequence[int] | None = None,
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
     mode: flood.LoadTestMode | None = None,
-    vegeta_kwargs: flood.VegetaKwargsShorthand | None = None,
+    vegeta_args: flood.VegetaArgsShorthand | None = None,
 ) -> tuple[
     typing.Sequence[int],
     typing.Sequence[int],
-    flood.VegetaKwargsShorthand | None,
+    flood.VegetaArgsShorthand | None,
 ]:
     if test is not None:
-        test_data = flood.parse_test_data(test=test)
+        test_data = flood.user_io.parse_test_data(test=test)
         rates = test_data['rates']
         durations = test_data['durations']
-        vegeta_kwargs = test_data['vegeta_kwargs']
+        vegeta_args = test_data['vegeta_args']
     else:
-        rates, durations = flood.generate_timings(
+        rates, durations = flood.generators.generate_timings(
             rates=rates,
             duration=duration,
             durations=durations,
             mode=mode,
         )
-    return rates, durations, vegeta_kwargs
+    return rates, durations, vegeta_args
```

### Comparing `paradigm-flood-0.2.5/flood/runners/single_runner/single_runner_summary.py` & `paradigm_flood-0.3.0/flood/runners/single_runner/single_runner_summary.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,157 +7,142 @@
 
 
 def _print_single_run_preamble(
     *,
     test_name: str,
     rates: typing.Sequence[int],
     durations: typing.Sequence[int],
-    vegeta_kwargs: flood.VegetaKwargsShorthand | None,
+    vegeta_args: flood.VegetaArgsShorthand | None,
     rerun_of: str | None = None,
     output_dir: str | None,
 ) -> None:
     import os
     import toolstr
 
     _print_single_run_preamble_copy(
         test_name=test_name,
         rerun_of=rerun_of,
         rates=rates,
         durations=durations,
-        vegeta_kwargs=vegeta_kwargs,
+        vegeta_args=vegeta_args,
         output_dir=output_dir,
     )
     if output_dir is not None:
         summary_path = os.path.join(output_dir, 'summary.txt')
         with toolstr.write_stdout_to_file(summary_path):
             _print_single_run_preamble_copy(
                 test_name=test_name,
                 rerun_of=rerun_of,
                 rates=rates,
                 durations=durations,
-                vegeta_kwargs=vegeta_kwargs,
+                vegeta_args=vegeta_args,
                 output_dir=output_dir,
             )
 
 
 def _print_single_run_preamble_copy(
     *,
     test_name: str,
     rates: typing.Sequence[int],
     durations: typing.Sequence[int],
-    vegeta_kwargs: flood.VegetaKwargsShorthand | None,
+    vegeta_args: flood.VegetaArgsShorthand | None,
     rerun_of: str | None = None,
     output_dir: str | None,
 ) -> None:
     import toolstr
 
+    styles = flood.user_io.styles
+
     toolstr.print_text_box(
-        toolstr.add_style('Load test: ' + test_name, flood.styles['metavar']),
-        style=flood.styles['content'],
+        toolstr.add_style('Load test: ' + test_name, styles['metavar']),
+        style=flood.user_io.styles['content'],
     )
-    toolstr.print_bullet(key='sample rates', value=rates, styles=flood.styles)
+    toolstr.print_bullet(key='sample rates', value=rates, styles=styles)
     if len(set(durations)) == 1:
         toolstr.print_bullet(
             key='sample duration',
             value=durations[0],
-            styles=flood.styles,
+            styles=styles,
         )
     else:
         toolstr.print_bullet(
-            key='sample durations', value=durations, styles=flood.styles
+            key='sample durations', value=durations, styles=styles
         )
-    if vegeta_kwargs is None or len(vegeta_kwargs) == 0:
-        toolstr.print_bullet(key='extra args', value=None, styles=flood.styles)
+    toolstr.print_bullet(key='extra args', value=vegeta_args, styles=styles)
 
     if rerun_of is not None:
-        toolstr.print_bullet(
-            key='rerun of', value=rerun_of, styles=flood.styles
-        )
+        toolstr.print_bullet(key='rerun of', value=rerun_of, styles=styles)
     toolstr.print_bullet(
-        key='output directory', value=output_dir, styles=flood.styles
+        key='output directory', value=output_dir, styles=styles
     )
     print()
 
 
 def _print_run_start() -> None:
-    import datetime
     import toolstr
 
+    styles = flood.user_io.styles
+
     print()
     print()
     toolstr.print_header(
         'Running load tests...',
-        style=flood.styles['content'],
-        text_style=flood.styles['metavar'],
-    )
-    dt = datetime.datetime.now()
-    if dt.microsecond >= 500_000:
-        dt = dt + datetime.timedelta(microseconds=1_000_000 - dt.microsecond)
-    else:
-        dt = dt - datetime.timedelta(microseconds=dt.microsecond)
-    timestamp = (
-        toolstr.add_style('\[', flood.styles['content'])
-        + toolstr.add_style(str(dt), flood.styles['metavar'])
-        + toolstr.add_style(']', flood.styles['content'])
+        style=styles['content'],
+        text_style=styles['metavar'],
     )
-    toolstr.print(timestamp + ' Starting')
+    flood.user_io.print_timestamped('Starting')
 
 
 def _print_single_run_conclusion(
     *,
     output_dir: str | None,
     results: typing.Mapping[str, flood.LoadTestOutput],
     metrics: typing.Sequence[str] | None,
     verbose: bool | int,
     figures: bool,
+    deep_check: bool,
 ) -> None:
-    _print_single_run_conclusion_copy(
+    _print_single_run_conclusion_text(
         output_dir=output_dir,
         results=results,
         metrics=metrics,
         verbose=verbose,
         figures=figures,
+        deep_check=deep_check,
     )
     if output_dir is not None:
         import os
         import toolstr
 
         summary_path = os.path.join(output_dir, 'summary.txt')
         with toolstr.write_stdout_to_file(summary_path, mode='a'):
-            _print_single_run_conclusion_copy(
+            _print_single_run_conclusion_text(
                 output_dir=output_dir,
                 results=results,
                 metrics=metrics,
                 verbose=verbose,
                 figures=figures,
+                deep_check=deep_check,
             )
 
 
-def _print_single_run_conclusion_copy(
+def _print_single_run_conclusion_text(
     output_dir: str | None,
     results: typing.Mapping[str, flood.LoadTestOutput],
     metrics: typing.Sequence[str] | None,
     verbose: bool | int,
     figures: bool,
+    deep_check: bool,
 ) -> None:
-    import datetime
     import os
     import toolstr
 
-    dt = datetime.datetime.now()
-    if dt.microsecond >= 500_000:
-        dt = dt + datetime.timedelta(microseconds=1_000_000 - dt.microsecond)
-    else:
-        dt = dt - datetime.timedelta(microseconds=dt.microsecond)
-    timestamp = (
-        toolstr.add_style('\[', flood.styles['content'])
-        + toolstr.add_style(str(dt), flood.styles['metavar'])
-        + toolstr.add_style(']', flood.styles['content'])
-    )
-    toolstr.print(timestamp + ' Load tests completed.')
+    styles = flood.user_io.styles
+
+    flood.user_io.print_timestamped('Load tests completed.')
 
     # print message about metrics file
     if output_dir is not None:
         test_path = single_runner_io.get_single_run_test_path(
             output_dir=output_dir
         )
         result_path = single_runner_io.get_single_run_results_path(
@@ -165,60 +150,109 @@
         )
         figures_path = single_runner_io.get_single_run_figures_path(
             output_dir=output_dir
         )
 
         print()
         print()
-        flood.print_header('Saving results...')
+        flood.user_io.print_header('Saving results to output directory...')
         toolstr.print_bullet(
             key=os.path.relpath(test_path, output_dir),
             value='',
             colon_str='',
-            styles=flood.styles,
+            styles=styles,
         )
         toolstr.print_bullet(
             key=os.path.relpath(result_path, output_dir),
             value='',
             colon_str='',
-            styles=flood.styles,
+            styles=styles,
         )
         if figures:
             toolstr.print_bullet(
                 key=os.path.relpath(figures_path, output_dir),
                 value='',
                 colon_str='',
-                styles=flood.styles,
+                styles=styles,
             )
 
     # decide metrics
     if metrics is None:
         metrics = ['success', 'throughput', 'p90']
 
     # print metrics
     print()
     print()
-    flood.print_header('Summarizing performance metrics...')
+    flood.user_io.print_header('Summarizing performance metrics...')
     if verbose > 1:
         toolstr.print_bullet(
             key='metrics shown below',
             value=', '.join(metrics),
-            styles=flood.styles,
+            styles=styles,
         )
         example_result = list(results.values())[0]
         additional = [
             key for key in example_result.keys() if key not in metrics
         ]
         toolstr.print_bullet(
             key='additional metrics available',
             value=', '.join(additional),
-            styles=flood.styles,
+            styles=styles,
         )
 
     # print metric values
     print()
-    flood.print_metric_tables(
-        results=results,
-        metrics=metrics,
-        indent=4,
+    flood.user_io.print_metric_tables(
+        results=results, metrics=metrics, indent=4
     )
 
+    # deep inspection tables
+    if deep_check:
+        print()
+        print()
+        flood.user_io.print_header('Deep inspection of responses...')
+
+        # extract data per category
+        deep_results_by_category: typing.MutableMapping[
+            flood.ResponseCategory,
+            typing.MutableMapping[str, flood.LoadTestDeepOutput],
+        ]
+        deep_results_by_category = {}
+        for result_name, result in results.items():
+            deep_metrics = result['deep_metrics']
+            if deep_metrics is not None:
+                for category, category_results in deep_metrics.items():
+                    deep_results_by_category.setdefault(category, {})
+                    deep_results_by_category[category][
+                        result_name
+                    ] = category_results
+            else:
+                raise Exception('deep metrics not available')
+
+        print()
+        flood.user_io.print_metric_tables(
+            results=deep_results_by_category['failed'],
+            metrics=['n_invalid_json_errors'],
+            indent=4,
+        )
+        print()
+        flood.user_io.print_metric_tables(
+            results=deep_results_by_category['failed'],
+            metrics=['n_rpc_errors'],
+            indent=4,
+        )
+
+        metric_names = [
+            m for m in metrics if m not in ['success', 'throughput']
+        ]
+        for (
+            category,
+            result_category_results,
+        ) in deep_results_by_category.items():
+            print()
+            flood.user_io.print_metric_tables(
+                results=result_category_results,
+                metrics=metric_names,
+                suffix=', ' + category + ' calls',
+                indent=4,
+            )
+
```

### Comparing `paradigm-flood-0.2.5/flood/tests/equality_tests/equality_test_runs.py` & `paradigm_flood-0.3.0/flood/user_io/inputs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,202 +1,216 @@
 from __future__ import annotations
 
 import typing
 
 import flood
-from . import equality_test_sets
+from flood import spec
+from . import outputs
 
 
-def run_equality_test(
-    test_name: str,
-    nodes: flood.NodesShorthand,
+def get_ctc_alias_url(url: str) -> str | None:
+    try:
+        import ctc.config
+
+        ctc_providers = ctc.config.get_providers()
+        if url in ctc_providers:
+            url = ctc_providers[url]['url']
+        return url
+    except ImportError:
+        return None
+
+
+def parse_nodes(
+    nodes: spec.NodesShorthand,
     *,
-    verbose: bool | int = True,
-    random_seed: flood.RandomSeed | None = None,
-    output_dir: str | None = None,
-) -> None:
-    import json
-    import os
-    import requests
-    import toolstr
+    verbose: bool | int = False,
+    request_metadata: bool = False,
+) -> typing.Mapping[str, spec.Node]:
+    """parse given nodes according to input specification"""
+    if verbose:
+        outputs.print_header('Gathering node data...')
+
+    new_nodes: typing.MutableMapping[str, spec.Node] = {}
+    if isinstance(nodes, list):
+        import multiprocessing
+
+        with multiprocessing.Pool() as pool:
+            results = pool.map(parse_node, nodes)
+        new_nodes = {result['name']: result for result in results}
+    elif isinstance(nodes, dict):
+        for key, value in nodes.items():
+            new_nodes[key] = value
+    else:
+        raise Exception('invalid format for nodes')
+
+    if verbose:
+        print_nodes_table(new_nodes)
 
-    nodes = flood.parse_nodes(nodes, request_metadata=True)
+    return new_nodes
+
+
+def print_nodes_table(nodes: typing.Mapping[str, spec.Node]) -> None:
+    rows = []
     for node in nodes.values():
+        url = node['url']
         if node['remote'] is not None:
-            raise Exception('remote not supported for equality test')
-    if len(nodes) != 2:
-        raise Exception('should use two nodes in equality test')
-
-    equality_tests = equality_test_sets.get_all_equality_tests()
-
-    # get tests
-    if test_name != 'all':
-        equality_tests = [t for t in equality_tests if t[0] == test_name]
-        if not equality_tests:
-            raise NotImplementedError(
-                'no matching test found for name "' + test_name + '"'
-            )
+            url = node['remote'] + '\n' + url
+        client_version = node['client_version']
+        if client_version is not None:
+            client_version = client_version.replace('/', '\n')
+        row = [
+            node['name'],
+            url,
+            client_version,
+        ]
+        rows.append(row)
+    labels = ['node', 'url', 'metadata']
+    print()
+    outputs.print_multiline_table(
+        rows=rows,
+        labels=labels,
+        indent=4,
+    )
 
-    if output_dir is None:
-        import tempfile
 
-        output_dir = tempfile.mkdtemp()
+def _get_node_str(node: flood.Node) -> str:
+    node_str = '"' + node['name'] + '", url=' + node['url']
+    remote = node['remote']
+    if remote is not None:
+        node_str += ' remote=' + remote
+    if node['client_version'] is not None:
+        node_str = node_str + ' version=' + node['client_version']
+    return node_str
+
+
+def parse_node(
+    node: str | spec.Node, request_metadata: bool = True
+) -> spec.Node:
+    """parse node according to input specification"""
+    prefixes = ['http', 'https', 'ws', 'wss']
+
+    if isinstance(node, dict):
+        return node
+    elif isinstance(node, str):
+        # parse name
+        if '=' in node:
+            name, url = node.split('=', 1)
+        else:
+            name = node
+            url = node
 
-    # print preamble
-    flood.print_text_box('Equality test: ' + test_name)
-    flood.print_bullet(key='methods', value='')
-    for test in equality_tests:
-        flood.print_bullet(key=test[0], value='', colon_str='', indent=4)
-    flood.print_bullet(key='output_dir', value=output_dir)
-    flood.print_bullet(key='nodes', value='')
-    for n, node in enumerate(nodes.values()):
-        toolstr.print(
-            toolstr.add_style(str(n + 1), flood.styles['metavar'])
-            + '. '
-            + str(node),
-            indent=4,
-            style=flood.styles['description'],
-        )
-
-    # run test
-    successful = []
-    calls = {}
-    call_node_responses: typing.Any = {}
-    headers = {'Content-Type': 'application/json', 'User-Agent': 'flood'}
-    for test in equality_tests:
-        # create call
-        test_name, constructor, args, kwargs = test
-        call = constructor(*args, **kwargs)
-        calls[test_name] = call
-        call_node_responses.setdefault(test_name, {})
-
-        # dispatch call
-        results = []
-        responses = []
-        for node in nodes.values():
-            response = None
-            try:
-                response = requests.post(
-                    url=node['url'], data=json.dumps(call), headers=headers
-                )
-                response_data = response.json()
-                if 'result' in response_data:
-                    result = response_data['result']
+        # check if node is in ctc aliases
+        alias_url = get_ctc_alias_url(url)
+        if alias_url is not None:
+            url = alias_url
+
+        # parse remote and url
+        if ':' in url:
+            head, tail = url.split(':', 1)
+            if head in prefixes:
+                remote = None
+                url = head + ':' + tail
+            else:
+                if tail.split('/')[0].isdecimal():
+                    remote = None
+                    url = url
                 else:
-                    result = None
-            except Exception:
-                result = None
-            responses.append(response)
-            results.append(result)
-            call_node_responses[test_name][node['name']] = result
-
-        # print summary
-        success = _summarize_result(
-            responses=responses,
-            results=results,
-            nodes=nodes,
-            test=test,
-            call=call,
-        )
-        if success:
-            successful.append(test_name)
-    failed = [test[0] for test in equality_tests if test[0] not in successful]
+                    remote = head
+                    url = tail
+        else:
+            remote = None
 
-    # save output file
-    summary = {
-        'calls': calls,
-        'successful': successful,
-        'failed': failed,
-        'responses': call_node_responses,
-    }
-    file_path = os.path.join(output_dir, 'equality_results.json')
-    with open(file_path, 'w') as f:
-        json.dump(summary, f)
+        # add missing prefix
+        if not any(url.startswith(prefix) for prefix in prefixes):
+            # check if is ip
+            pieces = url.split(':')[0].split('.')
+            is_ip = len(pieces) == 4 and all(
+                piece.isdecimal() for piece in pieces
+            )
 
-    # summarize test
-    print()
-    flood.print_text_box('Equality Test Summary')
-    print()
-    flood.print_header(
-        'No differences detected (n = ' + str(len(successful)) + ')'
-    )
-    if len(successful) == 0:
-        print('[none]')
-    else:
-        for name in sorted(successful):
-            flood.print_bullet(key=name, value='', colon_str='')
-    print()
-    flood.print_header('Differences detected (n = ' + str(len(failed)) + ')')
-    if len(failed) == 0:
-        print('[none]')
-    else:
-        for name in sorted(failed):
-            flood.print_bullet(key=name, value='', colon_str='')
-    print()
-    toolstr.print(
-        'summary saved to: ' + file_path, style=flood.styles['comment']
-    )
+            # add prefix
+            if url.startswith('localhost') or is_ip:
+                url = 'http://' + url
+            else:
+                url = 'https://' + url
+
+        if request_metadata:
+            # get client version
+            client_version = get_node_client_version(url=url, remote=remote)
 
+            # get network
+            network = 'ethereum'
 
-def _summarize_result(
-    responses: typing.Sequence[typing.Any],
-    results: typing.Sequence[typing.Any],
-    nodes: flood.Nodes,
-    test: flood.EqualityTest,
-    call: typing.Mapping[str, typing.Any],
-) -> bool:
-    import toolstr
-
-    test_name, constructor, args, kwargs = test
-
-    if results[0] is None or not toolstr.nested_equal(results[0], results[1]):
-        print()
-        flood.print_text_box('Discrepancies in ' + test_name)
-        print()
-        flood.print_header('args')
-        if len(args) > 0:
-            for arg in args:
-                flood.print_bullet(key=arg, value='', colon_str='')
-        if len(kwargs) > 0:
-            for key, value in kwargs.items():
-                flood.print_bullet(key=key, value=value)
-        print()
-        flood.print_header('call')
-        print(call)
-
-        if any(result is None for result in results):
-            print()
-        for node, result, response in zip(nodes.values(), results, responses):
-            if result is None:
-                toolstr.print(
-                    node['name'] + ' failed', style=flood.styles['title']
-                )
-                if response is None:
-                    print('response: no response')
-                elif response.status_code == 200:
-                    print('response:', response.json())
-                else:
-                    print('response: status code ', response.status_code)
+        else:
+            client_version = None
+            network = None
 
-        if results[0] is None or results[1] is None:
-            return False
+        return {
+            'name': name,
+            'url': url,
+            'remote': remote,
+            'client_version': client_version,
+            'network': network,
+        }
 
-        if len(results) == 2:
-            node0, node1 = list(nodes.values())
-            print()
-            flood.print_header('differences in response')
-            toolstr.print_nested_diff(
-                lhs=results[0],
-                rhs=results[1],
-                lhs_name=node0['name'],
-                rhs_name=node1['name'],
-                styles=flood.styles,
-                indent=4,
+    else:
+        raise Exception('invalid node format')
+
+
+def get_node_client_version(url: str, remote: str | None = None) -> str | None:
+    try:
+        if remote is None:
+            import ctc.rpc
+
+            info: str = ctc.rpc.sync_web3_client_version(
+                context={'provider': url}
             )
+            return info
         else:
-            print('omitting details when >2 nodes tested')
+            import json
+            import subprocess
 
-        return False
+            cmd = [
+                """ssh""",
+                remote,
+                """curl -X POST -H 'Content-Type: application/json' -d '{\"jsonrpc\": \"2.0\", \"method\": \"web3_clientVersion\", \"params\": [], \"id\": 1}' """  # noqa: E501
+                + url,
+            ]
+            output = subprocess.check_output(cmd, stderr=subprocess.DEVNULL)
+            response = json.loads(output)
+            info = response['result']
+            return info
+    except Exception:
+        return None
+
+
+def parse_test_data(test: spec.LoadTest) -> spec.LoadTestColumnWise:
+    rates = []
+    durations = []
+    vegeta_args = []
+    calls = []
+    for attack in test['attacks']:
+        rates.append(attack['rate'])
+        durations.append(attack['duration'])
+        vegeta_args.append(attack['vegeta_args'])
+        calls.append(attack['calls'])
+    return {
+        'rates': rates,
+        'durations': durations,
+        'vegeta_args': vegeta_args,
+        'calls': calls,
+    }
 
-    else:
-        return True
 
+def parse_nodes_network(nodes: typing.Mapping[str, spec.Node]) -> str:
+    if len(nodes) == 0:
+        raise Exception('no nodes, cannot get network')
+    networks = [node['network'] for node in nodes.values()]
+    if len(set(networks)) != 1:
+        raise Exception('multiple networks')
+    if networks[0] is None:
+        raise Exception('network could not be determined')
+    network = networks[0]
+    if isinstance(network, str):
+        return network
+    else:
+        raise Exception('need str network')
```

### Comparing `paradigm-flood-0.2.5/flood/tests/load_tests/load_test_construction.py` & `paradigm_flood-0.3.0/flood/tests/load_tests/load_test_construction.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,36 +30,39 @@
 
 
 def create_load_test(
     calls: typing.Sequence[typing.Any],
     rates: typing.Sequence[int],
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
-    vegeta_kwargs: flood.VegetaKwargs
-    | typing.Sequence[flood.VegetaKwargs]
+    vegeta_args: flood.VegetaArgs
+    | typing.Sequence[flood.VegetaArgs]
     | None = None,
     repeat_calls: bool = False,
-) -> flood.LoadTest:
+) -> typing.Sequence[flood.VegetaAttack]:
     # validate inputs
     if len(rates) == 0:
         raise Exception('must specify at least one rate')
 
     # pluralize singular durations
     if durations is None:
         if duration is None:
             raise Exception('must specify duration or durations')
         durations = [duration] * len(rates)
     assert len(durations) == len(rates)
 
     # pluralize singular vegeta kwargs
-    if vegeta_kwargs is None:
-        vegeta_kwargs = {}
-    if isinstance(vegeta_kwargs, dict):
-        vegeta_kwargs = [vegeta_kwargs] * len(rates)
-    if not isinstance(vegeta_kwargs, list):
+    use_vegeta_args: typing.Sequence[str] | typing.Sequence[None]
+    if vegeta_args is None:
+        use_vegeta_args = [vegeta_args] * len(rates)
+    elif isinstance(vegeta_args, str):
+        use_vegeta_args = [vegeta_args] * len(rates)
+    elif isinstance(vegeta_args, list):
+        use_vegeta_args = vegeta_args
+    else:
         raise Exception('invalid input')
 
     # partition calls into individual attacks
     if not repeat_calls:
         attacks_calls: typing.MutableSequence[typing.Sequence[flood.Call]] = []
         calls_iter = iter(calls)
         for rate, duration in zip(rates, durations):
@@ -71,18 +74,19 @@
     else:
         attacks_calls = [calls] * len(rates)
     assert len(attacks_calls) == len(rates)
 
     # create load tests
     load_test: list[flood.VegetaAttack] = []
     for rate, duration, a_calls, attack_kwargs in zip(
-        rates, durations, attacks_calls, vegeta_kwargs
+        rates, durations, attacks_calls, use_vegeta_args
     ):
         attack: flood.VegetaAttack = {
             'rate': rate,
             'duration': duration,
             'calls': a_calls,
-            'vegeta_kwargs': attack_kwargs,
+            'vegeta_args': attack_kwargs,
         }
         load_test.append(attack)
 
     return load_test
+
```

### Comparing `paradigm-flood-0.2.5/flood/tests/load_tests/load_test_plots.py` & `paradigm_flood-0.3.0/flood/tests/load_tests/load_test_plots.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,61 +2,112 @@
 
 import typing
 
 import flood
 
 
 def plot_load_test_results(
-    outputs: typing.Mapping[str, flood.LoadTestOutput],
+    outputs: typing.Mapping[str, flood.LoadTestOutput]
+    | typing.Mapping[str, flood.LoadTestDeepOutput],
     test_name: str,
     output_dir: str | None = None,
     latency_yscale_log: bool = True,
     colors: typing.Mapping[str, str] | None = None,
+    title_suffix: str | None = None,
+    file_suffix: str | None = None,
+    plot_success_rate: bool = True,
+    plot_throughput: bool = True,
+    plot_latency: bool = True,
 ) -> None:
     import os
     import matplotlib.pyplot as plt  # type: ignore
     import toolplot
 
+    if title_suffix is None:
+        title_suffix = ''
+    if file_suffix is None:
+        file_suffix = ''
+
     toolplot.setup_plot_formatting()
 
     if output_dir is not None:
         os.makedirs(output_dir, exist_ok=True)
 
-    plt.figure()
-    plot_load_test_success(outputs, test_name=test_name, colors=colors)
-    if output_dir is not None:
-        path = os.path.join(output_dir, 'success.png')
-        plt.savefig(path)
-    else:
-        plt.show()
+    if plot_success_rate:
+        plt.figure()
+        plot_load_test_success(outputs, test_name=test_name, colors=colors)
+        if output_dir is not None:
+            path = os.path.join(
+                output_dir, 'success_rate' + file_suffix + '.png'
+            )
+            plt.savefig(path)
+        else:
+            plt.show()
 
-    plt.figure()
-    plot_load_test_throughput(outputs, test_name=test_name, colors=colors)
-    if output_dir is not None:
-        path = os.path.join(output_dir, 'throughput.png')
-        plt.savefig(path)
-    else:
-        plt.show()
+    if plot_throughput:
+        plt.figure()
+        plot_load_test_throughput(outputs, test_name=test_name, colors=colors)
+        if output_dir is not None:
+            path = os.path.join(output_dir, 'throughput' + file_suffix + '.png')
+            plt.savefig(path)
+        else:
+            plt.show()
 
-    plt.figure()
-    plot_load_test_latencies(
-        outputs,
-        test_name=test_name,
-        yscale_log=latency_yscale_log,
-        colors=colors,
+    if plot_latency:
+        plt.figure()
+        plot_load_test_latencies(
+            outputs,
+            test_name=test_name,
+            yscale_log=latency_yscale_log,
+            colors=colors,
+        )
+        if output_dir is not None:
+            path = os.path.join(output_dir, 'latencies' + file_suffix + '.png')
+            plt.savefig(path)
+        else:
+            plt.show()
+
+    # deep graphs
+    has_deep_outputs = any(
+        output.get('deep_metrics') is not None for output in outputs.values()
     )
-    if output_dir is not None:
-        path = os.path.join(output_dir, 'latencies.png')
-        plt.savefig(path)
-    else:
-        plt.show()
+    if has_deep_outputs:
+        plot_load_test_results(
+            outputs={
+                name: output['deep_metrics']['successful']  # type: ignore
+                for name, output in outputs.items()
+            },
+            test_name=test_name,
+            title_suffix=', successful calls only',
+            file_suffix='_successful_calls',
+            plot_success_rate=False,
+            plot_throughput=False,
+            output_dir=output_dir,
+            latency_yscale_log=latency_yscale_log,
+            colors=colors,
+        )
+        plot_load_test_results(
+            outputs={
+                name: output['deep_metrics']['failed']  # type: ignore
+                for name, output in outputs.items()
+            },
+            test_name='failed ' + test_name,
+            title_suffix=', failed calls only',
+            file_suffix='_failed_calls',
+            plot_success_rate=False,
+            plot_throughput=False,
+            output_dir=output_dir,
+            latency_yscale_log=latency_yscale_log,
+            colors=colors,
+        )
 
 
 def plot_load_test_success(
-    results: typing.Mapping[str, flood.LoadTestOutput],
+    results: typing.Mapping[str, flood.LoadTestOutput]
+    | typing.Mapping[str, flood.LoadTestDeepOutput],
     colors: typing.Mapping[str, str] | None = None,
     test_name: str | None = None,
 ) -> None:
     import matplotlib.pyplot as plt
 
     plot_load_test_result_metrics(
         results=results,
@@ -67,15 +118,16 @@
         ylabel='success rate',
         ylim=[-0.03, 1.03],
     )
     plt.legend(loc='center right')
 
 
 def plot_load_test_throughput(
-    results: typing.Mapping[str, flood.LoadTestOutput],
+    results: typing.Mapping[str, flood.LoadTestOutput]
+    | typing.Mapping[str, flood.LoadTestDeepOutput],
     colors: typing.Mapping[str, str] | None = None,
     test_name: str | None = None,
 ) -> None:
     import matplotlib.pyplot as plt
 
     plot_load_test_result_metrics(
         results=results,
@@ -86,28 +138,29 @@
         ylabel='throughput\n(responses per second)',
         ymin=0,
     )
     plt.legend(loc='upper left')
 
 
 def plot_load_test_latencies(
-    results: typing.Mapping[str, flood.LoadTestOutput],
+    results: typing.Mapping[str, flood.LoadTestOutput]
+    | typing.Mapping[str, flood.LoadTestDeepOutput],
     colors: typing.Mapping[
         str,
         str | typing.Sequence[str] | typing.Mapping[str, str],
     ]
     | None = None,
     metrics: typing.Sequence[str] = ['p99', 'p90', 'p50'],
     test_name: str | None = None,
     yscale_log: bool = False,
 ) -> None:
     import matplotlib.pyplot as plt
 
     if colors is None:
-        colors = dict(zip(results.keys(), flood.plot_colors.values()))
+        colors = dict(zip(results.keys(), flood.user_io.plot_colors.values()))
 
     if yscale_log:
         ymin = None
     else:
         ymin = 0
 
     plot_load_test_result_metrics(
@@ -120,15 +173,16 @@
         ylabel='latency (seconds)',
         yscale_log=yscale_log,
     )
     plt.legend(loc='upper left')
 
 
 def plot_load_test_result_metrics(
-    results: typing.Mapping[str, flood.LoadTestOutput],
+    results: typing.Mapping[str, flood.LoadTestOutput]
+    | typing.Mapping[str, flood.LoadTestDeepOutput],
     metrics: typing.Sequence[str],
     *,
     colors: typing.Mapping[
         str,
         str | typing.Sequence[str] | typing.Mapping[str, str],
     ]
     | None = None,
@@ -138,28 +192,28 @@
     ylim: typing.Sequence[float] | None = None,
     ymin: float | int | None = None,
     yscale_log: bool = False,
 ) -> None:
     import matplotlib.pyplot as plt
     import toolplot
 
+    plot_colors = flood.user_io.plot_colors
+
     if colors is None:
-        colors = {
-            key: color for key, color in zip(results.keys(), flood.plot_colors)
-        }
+        colors = {key: color for key, color in zip(results.keys(), plot_colors)}
 
     for name, result in results.items():
         # determine colors
         result_colors = colors.get(name)
         if isinstance(result_colors, str):
-            if result_colors in flood.plot_colors:
+            if result_colors in plot_colors:
                 if len(metrics) == 1:
-                    result_colors = [flood.plot_colors[result_colors][1]]
+                    result_colors = [plot_colors[result_colors][1]]
                 else:
-                    result_colors = flood.plot_colors[result_colors]
+                    result_colors = plot_colors[result_colors]
             else:
                 result_colors = [result_colors] * len(metrics)
         elif isinstance(result_colors, list):
             assert len(result_colors) >= len(metrics), 'not enough colors'
         elif isinstance(result_colors, dict):
             for metric in metrics:
                 assert metric in result_colors, 'missing color for ' + metric
@@ -197,7 +251,8 @@
         xlabel += '\n[' + test_name + ']'
     toolplot.set_labels(
         title=title,
         xlabel=xlabel,
         ylabel=ylabel,
     )
     plt.legend(loc='center right')
+
```

### Comparing `paradigm-flood-0.2.5/flood/tests/load_tests/load_test_reports.py` & `paradigm_flood-0.3.0/flood/tests/load_tests/load_test_reports.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,32 +24,33 @@
 
     _create_load_test_report_html(ipynb_path=ipynb_path)
 
 
 def print_load_test_summary(test: flood.LoadTest) -> None:
     import toolstr
 
-    parsed = flood.parse_test_data(test)
+    parsed = flood.user_io.parse_test_data(test)
     rates = parsed['rates']
     durations = parsed['durations']
-    vegeta_kwargs = parsed['vegeta_kwargs']
+    vegeta_args = parsed['vegeta_args']
+    styles = flood.user_io.styles
 
-    toolstr.print_bullet(key='sample rates', value=rates, styles=flood.styles)
+    toolstr.print_bullet(key='sample rates', value=rates, styles=styles)
     if len(set(durations)) == 1:
         toolstr.print_bullet(
             key='sample duration',
             value=durations[0],
-            styles=flood.styles,
+            styles=styles,
         )
     else:
         toolstr.print_bullet(
-            key='sample durations', value=durations, styles=flood.styles
+            key='sample durations', value=durations, styles=styles
         )
-    if vegeta_kwargs is None or len(vegeta_kwargs) == 0:
-        toolstr.print_bullet(key='extra args', value=None, styles=flood.styles)
+    if vegeta_args is None or len(vegeta_args) == 0:
+        toolstr.print_bullet(key='extra args', value=None, styles=styles)
 
 
 def _create_load_test_report_html(
     ipynb_path: str,
 ) -> None:
     import subprocess
 
@@ -151,14 +152,145 @@
 
     return notebook_io.create_cells(
         cell_templates=_test_template_cells,
         inputs={'test_name': test_name},
     )
 
 
+def print_tests_timing(
+    results_payloads: typing.Mapping[str, flood.SingleRunResultsPayload]
+) -> None:
+    import tooltime
+    import toolstr
+
+    time_per_test = {}
+
+    for test_name in results_payloads:
+        results = results_payloads[test_name]["results"]
+        time_per_test[test_name] = 0.0
+        for condition_name in results.keys():
+            time = sum(
+                item
+                for item in results[condition_name]["actual_duration"]
+                if item is not None
+            ) + sum(
+                item
+                for item in results[condition_name]["final_wait_time"]
+                if item is not None
+            )
+            time_per_test[test_name] = float(time_per_test[test_name] + time)
+
+    test_timing_rows = []
+    t_load_total = 0.0
+    for test_name, payload in results_payloads.items():
+        t_load_total += payload["t_run_end"] - payload["t_run_start"]
+        row = [
+            test_name,
+            payload["t_run_end"] - payload["t_run_start"],
+            time_per_test[test_name],
+            tooltime.timestamp_to_iso_pretty(payload["t_run_start"]).replace(
+                " ", "\n"
+            ),
+            tooltime.timestamp_to_iso_pretty(payload["t_run_end"]).replace(
+                " ", "\n"
+            ),
+        ]
+        test_timing_rows.append(row)
+
+    total_row = ['TOTAL', t_load_total, sum(time_per_test.values()), None, None]
+    test_timing_rows.append(total_row)
+
+    toolstr.print_text_box("Test timing")
+    print("(includes setup and cleanup steps)")
+    toolstr.print_multiline_table(
+        test_timing_rows,
+        labels=[
+            "test",
+            "total\nduration",
+            'load test\nduration',
+            "t_start",
+            "t_end",
+        ],
+        column_formats={
+            'load test\nduration': {'postfix': ' s'},
+            'total\nduration': {'postfix': ' s'},
+        },
+    )
+
+
+def print_tests_cli_commands(
+    results_payloads: typing.Mapping[str, flood.SingleRunResultsPayload]
+) -> None:
+    import toolstr
+
+    toolstr.print_text_box('CLI commands used for each test')
+    for test_name, payload in results_payloads.items():
+        toolstr.print_header(test_name)
+        args = payload['cli_args']
+        args = ['"' + arg + '"' if ' ' in arg else arg for arg in args]
+        print(' '.join(args))
+
+
+def print_tests_nodes(
+    results_payloads: typing.Mapping[str, flood.SingleRunResultsPayload]
+) -> None:
+    import json
+    import toolstr
+
+    nodes_per_test = {}
+    for test_name, payload in results_payloads.items():
+        nodes_per_test[test_name] = payload['nodes']
+    n_unique_node_sets = len(
+        set(
+            json.dumps(nodes, sort_keys=True)
+            for nodes in nodes_per_test.values()
+        )
+    )
+    toolstr.print_text_box('Nodes Used')
+    if n_unique_node_sets == 1:
+        flood.user_io.print_nodes_table(nodes_per_test[test_name])
+    else:
+        for test_name, nodes_used in nodes_per_test.items():
+            flood.user_io.print_header(test_name)
+            flood.user_io.print_nodes_table(nodes_used)
+            print()
+
+
+def print_tests_versions(
+    results_payloads: typing.Mapping[str, flood.SingleRunResultsPayload]
+) -> None:
+    import json
+    import toolstr
+
+    deps_per_test = {}
+    for test_name, payload in results_payloads.items():
+        deps_per_test[test_name] = payload['dependency_versions']
+    n_unique_flood_versions = len(
+        set(payload['flood_version'] for payload in results_payloads.values())
+    )
+    n_unique_deps_sets = len(
+        set(json.dumps(deps, sort_keys=True) for deps in deps_per_test.values())
+    )
+    toolstr.print_text_box('Versions Used')
+    if n_unique_flood_versions == 1 and n_unique_deps_sets == 1:
+        print('flood version:', results_payloads[test_name]['flood_version'])
+        print()
+        toolstr.print_table(
+            list(deps_per_test[test_name].items()),
+            labels=['dependency', 'version'],
+        )
+    else:
+        print('flood version:', results_payloads[test_name]['flood_version'])
+        print()
+        for test_name, deps_used in deps_per_test.items():
+            flood.user_io.print_header(test_name)
+            toolstr.print_table(list(deps_used.items()))
+            print()
+
+
 if typing.TYPE_CHECKING:
     from flood.user_io import notebook_io
 
 _report_template_cells: notebook_io.NotebookTemplate = [
     {
         # header
         'type': 'markdown',
@@ -172,15 +304,15 @@
             import IPython
             import polars as pl
             import toolstr
             import tooltime
 
             import flood
 
-            flood.styles = {{}}
+            flood.user_io.disable_text_colors()
         """,
         'inputs': [],
     },
     {
         # parameters
         'type': 'code',
         'f': _create_parameters_cell,
@@ -219,45 +351,43 @@
             toolstr.print_text_box('Tests')
             for t, test_name in enumerate(results_payloads.keys()):
                 print(str(t + 1) + '.', test_name)
         """,
         'inputs': [],
     },
     {
-        # test durations
+        # test list
         'type': 'code',
         'content': """
-            # test durations
-
-            time_per_test = {{}}
-            time_per_condition = {{}}
-
-            for test_name in results_payloads:
-                results = results_payloads[test_name]["results"]
-                time_per_test[test_name] = 0
-                for condition_name in results.keys():
-                    time_per_condition.setdefault(condition_name, 0)
-                    time = sum(results[condition_name]["actual_duration"]) + sum(
-                        results[condition_name]["final_wait_time"]
-                    )
-                    time_per_test[test_name] += time
-                    time_per_condition[condition_name] += time
-
-            toolstr.print_text_box('Total time')
-            toolstr.print(tooltime.timelength_to_phrase(int(sum(time_per_test.values()))))
-            print()
-
-            toolstr.print_text_box('Total time per test')
-            rows = list(time_per_test.items())
-            toolstr.print_table(rows, labels=['test', 'time (s)'])
-
-            toolstr.print_text_box('Total time per condition')
-            rows = list(time_per_condition.items())
-            toolstr.print_table(rows, labels=['condition', 'time (s)'])
-        """,  # noqa: E501
+            flood.tests.print_tests_timing(results_payloads)
+        """,
+        'inputs': [],
+    },
+    {
+        # test list
+        'type': 'code',
+        'content': """
+            flood.tests.print_tests_cli_commands(results_payloads)
+        """,
+        'inputs': [],
+    },
+    {
+        # test list
+        'type': 'code',
+        'content': """
+            flood.tests.print_tests_nodes(results_payloads)
+        """,
+        'inputs': [],
+    },
+    {
+        # test list
+        'type': 'code',
+        'content': """
+            flood.tests.print_tests_versions(results_payloads)
+        """,
         'inputs': [],
     },
     {
         # Tests header
         'type': 'markdown',
         'content': '# Tests',
         'inputs': [],
@@ -281,57 +411,59 @@
     {
         # load test results
         'type': 'code',
         'content': """
             # load test results
 
             test_name = '{test_name}'
+            test_payload = test_payloads[test_name]
             results_payload = results_payloads[test_name]
             results = results_payload['results']
         """,
         'inputs': ['test_name'],
     },
     {
         # show test metadata
         'type': 'code',
         'content': """
             # show test metadata
 
             toolstr.print_text_box(test_name + ' parameters')
-            flood.print_load_test_summary(results_payload['test'])
+            test = flood.generate_test(**test_payload['test_parameters'])
+            flood.tests.load_tests.print_load_test_summary(test)
             toolstr.print('- nodes tested:')
             nodes_df = pl.from_records(list(results_payload['nodes'].values()))
             toolstr.print_dataframe_as_table(nodes_df)
         """,
         'inputs': [],
     },
     {
         # show result tables
         'type': 'code',
         'content': """
             # show result tables
 
-            flood.print_metric_tables(results, metrics=metrics, comparison=True)
-        """,
+            flood.user_io.print_metric_tables(results, metrics=metrics, comparison=len(results) == 2)
+        """,  # noqa: E501
         'inputs': [],
     },
     {
         # show result figures
         'type': 'code',
         'content': """
             # show result figures
 
-            colors = flood.get_nodes_plot_colors(nodes=results_payload['nodes'])
-            flood.plot_load_test_results(
+            colors = flood.user_io.get_nodes_plot_colors(nodes=results_payload['nodes'])
+            flood.tests.load_tests.plot_load_test_results(
                 test_name=test_name,
                 outputs=results,
                 latency_yscale_log=True,
                 colors=colors,
             )
-        """,
+        """,  # noqa: E501
         'inputs': [],
     },
     {
         # show errors
         'type': 'code',
         'content': """
             # show errors
@@ -368,7 +500,8 @@
                     "last_response_timestamp",
                 )
                 IPython.display.display(df)
         """,
         'inputs': [],
     },
 ]
+
```

### Comparing `paradigm-flood-0.2.5/flood/tests/load_tests/vegeta.py` & `paradigm_flood-0.3.0/flood/tests/load_tests/deep_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,231 +1,86 @@
-"""wrapper around the vegeta load testing tool"""
 from __future__ import annotations
 
 import typing
-
 from ... import spec
 
 if typing.TYPE_CHECKING:
     import polars as pl
 
 
-def run_vegeta_attack(
-    *,
-    url: str,
-    rate: int,
-    calls: typing.Sequence[typing.Any],
-    duration: int,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    verbose: bool = False,
-    include_raw_output: bool = False,
-) -> spec.LoadTestOutputDatum:
-    attack = _construct_vegeta_attack(
-        calls=calls,
-        url=url,
-        verbose=verbose,
-    )
-    attack_output = _vegeta_attack(
-        schedule_dir=attack['schedule_dir'],
-        duration=duration,
-        rate=rate,
-        vegeta_kwargs=vegeta_kwargs,
-        verbose=verbose,
-    )
-    report = _create_vegeta_report(
-        attack_output=attack_output,
-        target_rate=rate,
-        target_duration=duration,
-        include_raw_output=include_raw_output,
-    )
-    return report
-
-
-def _construct_vegeta_attack(
-    calls: typing.Sequence[typing.Any],
-    url: str,
-    schedule_dir: str | None = None,
-    verbose: bool = False,
-) -> typing.Mapping[str, str]:
-    import json
-    import os
-    import tempfile
-
-    headers = {'Content-Type': 'application/json'}
-
-    # determine output directory
-    if schedule_dir is None:
-        schedule_dir = tempfile.mkdtemp()
-
-    # create calls file
-    call_paths = []
-    for c, call in enumerate(calls):
-        vegeta_calls_path = os.path.join(
-            schedule_dir, 'vegeta_calls_' + str(c) + '.json'
-        )
-        with open(vegeta_calls_path, 'w') as f:
-            f.write(json.dumps(call))
-        call_paths.append(vegeta_calls_path)
-
-    # create targets specification
-    vegeta_targets_path = os.path.join(schedule_dir, 'vegeta_targets')
-    with open(vegeta_targets_path, 'w') as f:
-        for c, call in enumerate(calls):
-            f.write('POST ' + url + '\n')
-            for key, value in headers.items():
-                f.write(key + ': ' + value + '\n')
-            f.write('@' + call_paths[c] + '\n')
-            f.write('\n')
-
-    # output summary
-    if verbose:
-        print('running vegeta attack...')
-        print('- targets:', vegeta_targets_path)
-        print('- calls:', vegeta_calls_path)
-
-    return {
-        'schedule_dir': schedule_dir,
-        'vegeta_calls_path': vegeta_calls_path,
-        'vegeta_targets_path': vegeta_targets_path,
-    }
-
-
-def _vegeta_attack(
-    schedule_dir: str,
-    *,
-    duration: int | None = None,
-    rate: int | None = None,
-    max_connections: int | None = None,
-    max_workers: int | None = None,
-    n_cpus: int | None = None,
-    report_path: str | None = None,
-    vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
-    verbose: bool = False,
-) -> bytes:
-    import os
-    import subprocess
-
-    # construct command
-    cmd = 'vegeta attack'
-    cmd += ' -targets=' + os.path.join(schedule_dir, 'vegeta_targets')
-    if rate is not None:
-        cmd += ' -rate=' + str(rate)
-    if duration is not None:
-        cmd += ' -duration=' + str(duration) + 's'
-    if max_connections is not None:
-        cmd += ' -max-connections=' + str(max_connections)
-    if max_workers is not None:
-        cmd += ' -max-workers=' + str(max_workers)
-    if vegeta_kwargs is not None:
-        for key, value in vegeta_kwargs.items():
-            cmd += ' -' + key
-            if value is not None:
-                cmd += '=' + str(value)
-
-    if verbose:
-        print('- command:', cmd)
-
-    # run command
-    return subprocess.check_output(cmd.split(' '))
-
-
-def _create_vegeta_report(
-    attack_output: bytes,
+def compute_deep_datum(
+    raw_output: bytes,
     target_rate: int,
     target_duration: int,
-    include_raw_output: bool,
-) -> spec.LoadTestOutputDatum:
-    import json
-    import subprocess
-
-    cmd = 'vegeta report -type json'
-    report_output = (
-        subprocess.check_output(cmd.split(' '), input=attack_output)
-        .decode()
-        .strip()
-    )
-    report: spec.RawLoadTestOutputDatum = json.loads(report_output)
-
-    if 'min' in report['latencies']:
-        latency_min = report['latencies']['min'] / 1e9
-    else:
-        latency_min = None
-
-    if include_raw_output:
-        raw_output = encode_raw_vegeta_output(attack_output)
-    else:
-        raw_output = None
-
-    return {
-        'target_rate': target_rate,
-        'actual_rate': report['rate'],
-        'target_duration': target_duration,
-        'actual_duration': report['duration'] / 1e9,
-        'requests': report['requests'],
-        'throughput': report['throughput'],
-        'success': float(report['success']),
-        'min': latency_min,
-        'mean': report['latencies']['mean'] / 1e9,
-        'p50': report['latencies']['50th'] / 1e9,
-        'p90': report['latencies']['90th'] / 1e9,
-        'p95': report['latencies']['95th'] / 1e9,
-        'p99': report['latencies']['99th'] / 1e9,
-        'max': report['latencies']['max'] / 1e9,
-        #
-        'status_codes': report['status_codes'],
-        'errors': report['errors'],
-        'first_request_timestamp': report['earliest'],
-        'last_request_timestamp': report['latest'],
-        'last_response_timestamp': report['end'],
-        'final_wait_time': report['wait'] / 1e9,
-        'raw_output': raw_output,
-    }
-
-
-#
-# # output processing
-#
-
-
-def encode_raw_vegeta_output(raw_output: bytes) -> str:
-    import base64
-    import io
-    import gzip
-
-    # gzip compress
-    buf = io.BytesIO()
-    f = gzip.GzipFile(fileobj=buf, mode='wb')
-    f.write(raw_output)
-    f.close()
-    compressed = buf.getvalue()
-
-    # encode as base64
-    as_base64 = base64.b64encode(compressed).decode('utf-8')
-
-    return as_base64
-
+    calls: typing.Sequence[typing.Any],
+) -> tuple[
+    typing.Mapping[spec.ResponseCategory, spec.LoadTestDeepOutputDatum],
+    typing.Sequence[spec.ErrorPair],
+]:
+    import polars as pl
 
-def decode_raw_vegeta_output(encoded_output: str) -> bytes:
-    import base64
-    import io
-    import gzip
+    # convert to dataframe
+    all_df = _convert_raw_vegeta_output_to_dataframe(raw_output)
 
-    # decode from base64
-    as_bytes = base64.b64decode(encoded_output.encode())
+    # add error columns
+    rpc_error = []
+    invalid_json_error = []
+    for status_code, response in zip(all_df['status_code'], all_df['response']):
+        if status_code == 200:
+            try:
+                import json
+                import base64
+
+                decoded = json.loads(base64.b64decode(response))
+
+                invalid_json_error.append(False)
+                if decoded.get('result') is None:
+                    rpc_error.append(True)
+                else:
+                    rpc_error.append(False)
+
+            except Exception:
+                invalid_json_error.append(True)
+                rpc_error.append(False)
+        else:
+            invalid_json_error.append(False)
+            rpc_error.append(False)
+    all_df = all_df.with_columns(
+        pl.Series('invalid_json_error', invalid_json_error),
+        pl.Series('rpc_error', rpc_error),
+    )
+    all_df = all_df.with_columns(
+        (
+            (pl.col('status_code') == 200)
+            & ~pl.col('invalid_json_error')
+            & ~pl.col('rpc_error')
+        ).alias('deep_success')
+    )
 
-    # gzip decompress
-    buf = io.BytesIO(as_bytes)
-    f = gzip.GzipFile(fileobj=buf, mode='rb')
-    decompressed = f.read()
-    f.close()
+    # get error pairs
+    rpc_error_pairs: typing.Sequence[spec.ErrorPair] = []
+    rpc_error_pairs = _gather_error_pairs(df=all_df, calls=calls)
+
+    # compute sample metrics
+    category_data = {}
+    dataframes: list[tuple[spec.ResponseCategory, pl.DataFrame]] = [
+        ('all', all_df),
+        ('successful', all_df.filter(pl.col('deep_success'))),
+        ('failed', all_df.filter(~pl.col('deep_success'))),
+    ]
+    for category, df in dataframes:
+        category_data[category] = _compute_raw_output_sample_metrics(
+            df=df, target_rate=target_rate, target_duration=target_duration
+        )
 
-    return decompressed
+    return category_data, rpc_error_pairs
 
 
-def convert_raw_vegeta_output_to_dataframe(raw_output: bytes) -> pl.DataFrame:
+def _convert_raw_vegeta_output_to_dataframe(raw_output: bytes) -> pl.DataFrame:
+    """convert raw vegeta attack output to dataframe, 1 row per response"""
     import io
     import subprocess
     import polars as pl
 
     cmd = 'vegeta encode --to csv'
     report_output = (
         subprocess.check_output(cmd.split(' '), input=raw_output)
@@ -264,44 +119,69 @@
         'status_code': pl.Int64,
         'timestamp': pl.Int64,
         'url': pl.Utf8,
     }
     return pl.read_csv(buf, new_columns=schema, has_header=False, dtypes=dtypes)
 
 
-def compute_raw_output_metrics(
-    raw_output: typing.Mapping[str, pl.DataFrame],
-    results: typing.Mapping[str, spec.LoadTestOutput],
-) -> typing.Mapping[str, spec.LoadTestOutput]:
+def _gather_error_pairs(
+    df: pl.DataFrame, calls: typing.Sequence[typing.Any]
+) -> typing.Sequence[spec.ErrorPair]:
     import polars as pl
 
-    metrics: typing.MutableMapping[str, spec.LoadTestOutput] = {}
-    for node_name, node_results in results.items():
-        node_metrics = []
-        for i, (target_rate, target_duration) in enumerate(
-            zip(node_results['target_rate'], node_results['target_duration'])
-        ):
-            sample_metrics = compute_raw_output_sample_metrics(
-                df=raw_output[node_name].filter(pl.col('sample_index') == i),
-                target_rate=target_rate,
-                target_duration=target_duration,
-            )
-            sample_metrics['raw_output'] = None
-            node_metrics.append(sample_metrics)
-        metrics[node_name] = {
-            metric: [sample_metrics[metric] for sample_metrics in node_metrics]  # type: ignore # noqa: E501
-            for metric in node_results.keys()
-        }
-    return metrics
+    calls_by_id = {}
+    for call in calls:
+        call_id = call.get('id')
+        if call_id is None:
+            raise Exception('id not specified for call')
+        elif call_id in calls_by_id:
+            raise Exception('duplicate call for id')
+        calls_by_id[call_id] = call
+
+    responses = df.filter(pl.col('rpc_error'))['response']
+
+    pairs = []
+    for response in responses:
+        pairs.append((None, response))
+
+    return pairs
 
 
-def compute_raw_output_sample_metrics(
+def _compute_raw_output_sample_metrics(
     df: pl.DataFrame, target_rate: int, target_duration: int
-) -> spec.LoadTestOutputDatum:
+) -> spec.LoadTestDeepOutputDatum:
+    """convert standard test metrics from vegeta raw output dataframe"""
+    if len(df) == 0:
+        return {
+            'target_rate': target_rate,
+            'actual_rate': 0,
+            'target_duration': target_duration,
+            'actual_duration': None,
+            'requests': 0,
+            'throughput': None,
+            'success': None,
+            'min': None,
+            'mean': None,
+            'p50': None,
+            'p90': None,
+            'p95': None,
+            'p99': None,
+            'max': None,
+            'status_codes': {},
+            'errors': [],
+            'first_request_timestamp': None,
+            'last_request_timestamp': None,
+            'last_response_timestamp': None,
+            'final_wait_time': None,
+            'n_invalid_json_errors': 0,
+            'n_rpc_errors': 0,
+        }
+
     import polars as pl
+
     actual_rate = (
         pl.count()
         / (pl.col('timestamp').max() - pl.col('timestamp').min())
         * 1e9
     )
     actual_rate = actual_rate.alias('actual_rate')
     successful = df.filter(pl.col('status_code') == 200)
@@ -348,9 +228,114 @@
         (
             (pl.col('timestamp') + pl.col('latency')).max()
             - pl.max('timestamp')
         ).alias('final_wait_time')
         / 1e9,
     )
 
-    return metrics_df.to_dicts()[0]  # type: ignore
+    output: spec.LoadTestDeepOutputDatum = metrics_df.to_dicts()[0]  # type: ignore # noqa: E501
+    output['n_invalid_json_errors'] = int(df['invalid_json_error'].sum())
+    output['n_rpc_errors'] = int(df['rpc_error'].sum())
+
+    return output
+
+
+# def compute_raw_output_metrics(
+#     raw_output: typing.Mapping[str, pl.DataFrame],
+#     results: typing.Mapping[str, spec.LoadTestOutput],
+# ) -> typing.Mapping[str, spec.LoadTestOutput]:
+#     import polars as pl
+
+#     metrics: typing.MutableMapping[str, spec.LoadTestOutput] = {}
+#     for node_name, node_results in results.items():
+#         node_metrics = []
+#         for i, (target_rate, target_duration) in enumerate(
+#             zip(node_results['target_rate'], node_results['target_duration'])
+#         ):
+#             sample_metrics = compute_raw_output_sample_metrics(
+#                 df=raw_output[node_name].filter(pl.col('sample_index') == i),
+#                 target_rate=target_rate,
+#                 target_duration=target_duration,
+#             )
+#             node_metrics.append(sample_metrics)
+#         metrics[node_name] = {
+#             metric: [sample_metrics[metric] for sample_metrics in node_metrics]  # type: ignore # noqa: E501
+#             for metric in node_results.keys()
+#         }
+#     return metrics
+
+
+# def test_run_to_deep_raw_vegeta_output(
+#     results: typing.Mapping[str, spec.LoadTestOutput],
+#     sample_index: int | typing.Sequence[int] | None = None,
+# ) -> typing.Mapping[str, pl.DataFrame]:
+#     import polars as pl
+
+#     node_dfs = {}
+#     for node_name, node_results in results.items():
+#         raw_output = node_results['deep_raw_output']
+#         if raw_output is None:
+#             raise Exception('raw_outputs were not saved for test')
+#         else:
+#             if sample_index is not None:
+#                 if isinstance(sample_index, int):
+#                     indices = [sample_index]
+#                 elif isinstance(sample_index, list):
+#                     indices = sample_index
+#                 else:
+#                     raise Exception('invalid format for sample_index')
+#             else:
+#                 indices = list(range(len(raw_output)))
+#             dfs = []
+#             for index in indices:
+#                 item = raw_output[index]
+#                 if item is None:
+#                     raise Exception('raw_outputs were not saved for test')
+#                 decoded = decode_raw_vegeta_output(item)
+#                 df = convert_raw_vegeta_output_to_dataframe(decoded)
+#                 df = df.with_columns(pl.lit(index).alias('sample_index'))
+#                 dfs.append(df)
+#             node_dfs[node_name] = pl.concat(dfs)
+#     return node_dfs
+
+
+#
+# # serde
+#
+
+
+def encode_raw_vegeta_output(raw_output: bytes) -> str:
+    """encode raw output to str for use in JSON"""
+    import base64
+    import io
+    import gzip
+
+    # gzip compress
+    buf = io.BytesIO()
+    f = gzip.GzipFile(fileobj=buf, mode='wb')
+    f.write(raw_output)
+    f.close()
+    compressed = buf.getvalue()
+
+    # encode as base64
+    as_base64 = base64.b64encode(compressed).decode('utf-8')
+
+    return as_base64
+
+
+def decode_raw_vegeta_output(encoded_output: str) -> bytes:
+    """decode raw output from str for use in JSON"""
+    import base64
+    import io
+    import gzip
+
+    # decode from base64
+    as_bytes = base64.b64decode(encoded_output.encode())
+
+    # gzip decompress
+    buf = io.BytesIO(as_bytes)
+    f = gzip.GzipFile(fileobj=buf, mode='rb')
+    decompressed = f.read()
+    f.close()
+
+    return decompressed
```

### Comparing `paradigm-flood-0.2.5/flood/user_io/notebook_io.py` & `paradigm_flood-0.3.0/flood/user_io/notebook_io.py`

 * *Files identical despite different names*

```diff
@@ -60,15 +60,15 @@
     lines = content.split('\n')
     if lines[0] == '':
         left_spaces = [
             len(line) - len(line.lstrip(' '))
             for line in lines
             if not set(line).issubset({' '})
         ]
-        cut = min(left_spaces[1:])
+        cut = min(left_spaces[:])
         content = '\n'.join(line[cut:] for line in lines)
 
     content = content.strip()
 
     # create cell object
     cell_obj: nbformat.notebooknode.NotebookNode
     if cell_template['type'] == 'markdown':
```

### Comparing `paradigm-flood-0.2.5/flood/user_io/outputs.py` & `paradigm_flood-0.3.0/flood/user_io/outputs.py`

 * *Files 14% similar despite different names*

```diff
@@ -105,36 +105,41 @@
 
     import tqdm  # type: ignore
 
     return tqdm
 
 
 def print_metric_tables(
-    results: typing.Mapping[str, spec.LoadTestOutput],
+    results: typing.Mapping[str, spec.LoadTestOutput | spec.LoadTestDeepOutput],
     metrics: typing.Sequence[str],
     *,
+    suffix: str = '',
     decimals: int | None = None,
-    comparison: bool = False,
+    comparison: bool | None = None,
     indent: int | str | None = None,
 ) -> None:
     import toolstr
 
     if len(results) == 0:
         toolstr.print('no results', indent=indent)
         print()
+    if comparison is None:
+        comparison = len(results) == 2
 
     names = list(results.keys())
     rates = results[names[0]]['target_rate']
     for metric in metrics:
         # create labels
-        if metric == 'success':
-            suffix = ''
+        if metric in ['success', 'n_invalid_json_errors', 'n_rpc_errors']:
+            metric_suffix = ''
+        elif metric == 'throughput':
+            metric_suffix = ' (rps)'
         else:
-            suffix = ' (s)'
-        unitted_names = [name + suffix for name in names]
+            metric_suffix = ' (s)'
+        unitted_names = [name + metric_suffix for name in names]
         labels = ['rate (rps)'] + unitted_names
         if comparison:
             if len(results) != 2:
                 raise NotImplementedError('comparison of >2 tests')
             comparison_label = names[0] + ' / ' + names[1]
             labels.append(comparison_label)
         else:
@@ -148,15 +153,15 @@
                 row.append(value)
                 values.append(value)
         if comparison:
             for row in rows:
                 row.append(row[-2] / row[-1])
 
         # compute column formats
-        if all(value > 1 for value in values):
+        if all(value > 1 for value in values if value is not None):
             use_decimals = 1
         else:
             if decimals is None:
                 use_decimals = 6
             else:
                 use_decimals = decimals
         column_formats = {
@@ -166,26 +171,34 @@
             column_formats[comparison_label] = {
                 'decimals': 1,
                 'percentage': True,
             }
 
         # print header
         toolstr.print_text_box(
-            toolstr.add_style(metric + ' vs load', flood.styles.get('metavar')),
-            style=flood.styles.get('content'),
+            toolstr.add_style(
+                metric + ' vs load' + suffix, styles.get('metavar')
+            ),
+            style=styles.get('content'),
             indent=indent,
         )
 
+        if metric == 'success':
+            for label in labels[1:]:
+                column_formats.setdefault(label, {})
+                column_formats[label]['percentage'] = True
+                column_formats[label]['decimals'] = 1
+
         # print table
         toolstr.print_table(
             rows,
             labels=labels,
             column_formats=column_formats,  # type: ignore
-            label_style=flood.styles.get('metavar'),
-            border=flood.styles.get('content'),
+            label_style=styles.get('metavar'),
+            border=styles.get('content'),
             indent=indent,
         )
         if metric != metrics[-1]:
             print()
 
 
 #
@@ -194,52 +207,75 @@
 
 
 def print_text_box(text: str) -> None:
     import toolstr
 
     toolstr.print_text_box(
         text,
-        text_style=flood.styles.get('metavar'),
-        style=flood.styles.get('content'),
+        text_style=styles.get('metavar'),
+        style=styles.get('content'),
     )
 
 
 def print_header(text: str) -> None:
     import toolstr
 
     toolstr.print_header(
         text,
-        text_style=flood.styles.get('metavar'),
-        style=flood.styles.get('content'),
+        text_style=styles.get('metavar'),
+        style=styles.get('content'),
     )
 
 
 def print_bullet(*args: typing.Any, **kwargs: typing.Any) -> None:
     import toolstr
 
     toolstr.print_bullet(
         *args,
         **kwargs,
-        styles=flood.styles,
+        styles=styles,
     )
 
 
 def print_table(*args: typing.Any, **kwargs: typing.Any) -> None:
     import toolstr
 
     toolstr.print_table(
         *args,
         **kwargs,
-        label_style=flood.styles.get('metavar'),
-        border=flood.styles.get('content'),
+        label_style=styles.get('metavar'),
+        border=styles.get('content'),
     )
 
 
 def print_multiline_table(*args: typing.Any, **kwargs: typing.Any) -> None:
     import toolstr
 
     toolstr.print_multiline_table(
         *args,
         **kwargs,
-        label_style=flood.styles.get('metavar'),
-        border=flood.styles.get('content'),
+        label_style=styles.get('metavar'),
+        border=styles.get('content'),
     )
+
+
+def print_timestamped(message: str) -> None:
+    import datetime
+    import toolstr
+
+    dt = datetime.datetime.now()
+    if dt.microsecond >= 500_000:
+        dt = dt + datetime.timedelta(microseconds=1_000_000 - dt.microsecond)
+    else:
+        dt = dt - datetime.timedelta(microseconds=dt.microsecond)
+    timestamp = (
+        toolstr.add_style('\[', styles['content'])
+        + toolstr.add_style(str(dt), styles['metavar'])
+        + toolstr.add_style(']', styles['content'])
+    )
+    toolstr.print(timestamp + ' ' + message)
+
+
+def disable_text_colors() -> None:
+    for key in list(styles.keys()):
+        del styles[key]  # type: ignore
+
```

### Comparing `paradigm-flood-0.2.5/pyproject.toml` & `paradigm_flood-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -24,26 +24,30 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 dependencies = [
-    'typing-extensions >=4.2.0, <5',
-    'toolcli >=0.6.14, <0.7',
-    'toolstr >=0.9.7, <0.10',
-    'requests >=2.20.0, <3',
-    'tqdm >=4.65.0, <5',
-    'numpy >=1.19.0, <1.25',
-    'nbformat >= 5.8.0, <6',
-    'toolplot >= 0.3.4, <0.4',
+    'checkthechain >= 0.3.9, <0.4.0',
+    'ipykernel > 6, <7',
+    'ipython_genutils > 0.1, <1',
     'matplotlib >= 3.7.1, <4',
+    'nbconvert > 6, <7',
+    'nbformat >= 5.8.0, <6',
+    'numpy >=1.19.0, <1.25',
+    'orjson >=3.0.0, < 4',
     'paradigm-data-portal >= 0.2.2, <0.3',
-    'checkthechain >= 0.3.6, <0.4.0',
-    'nbconvert > 5.6.0, <6',
+    'polars >= 0.17',
+    'requests >=2.20.0, <3',
+    'toolcli >=0.6.16, <0.7',
+    'toolplot >= 0.3.4, <0.4',
+    'toolstr >=0.9.7, <0.10',
+    'tqdm >=4.65.0, <5',
+    'typing-extensions >=4.2.0, <5',
 ]
 
 [project.optional-dependencies]
 test = [
     'mypy ==1.2.0',
     'mypy_extensions >= 1.0.0, <1.1.0',
     'pytest >=6, <7',
```

### Comparing `paradigm-flood-0.2.5/tests/conftest.py` & `paradigm_flood-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.5/tests/test_env_vars.py` & `paradigm_flood-0.3.0/tests/test_env_vars.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-
 import flood
 
 
 def test_local_node_1(flood_test_local_node_1):
-    result = flood.parse_node(flood_test_local_node_1)
+    result = flood.user_io.parse_node(flood_test_local_node_1)
     assert result['remote'] is None
 
 
 def test_local_node_2(flood_test_local_node_2):
-    result = flood.parse_node(flood_test_local_node_2)
+    result = flood.user_io.parse_node(flood_test_local_node_2)
     assert result['remote'] is None
 
 
 def test_remote_node_1(flood_test_remote_node_1):
-    result = flood.parse_node(flood_test_remote_node_1)
+    result = flood.user_io.parse_node(flood_test_remote_node_1)
     assert result['remote'] is not None
 
 
 def test_remote_node_2(flood_test_remote_node_2):
-    result = flood.parse_node(flood_test_remote_node_2)
+    result = flood.user_io.parse_node(flood_test_remote_node_2)
     assert result['remote'] is not None
```

### Comparing `paradigm-flood-0.2.5/tests/test_load_tests.py` & `paradigm_flood-0.3.0/tests/test_load_tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,17 @@
     'local_bare': 'flood {test_name} {local_node_1} {local_node_2} -d 1 -r 1 2 4',  # noqa: E501
     # 'local_alias': 'flood {test_name} node1={local_node_1} node2={local_node_2} -d 1 -r 1 2 4',  # noqa: E501
     'remote_bare': 'flood {test_name} {remote_node_1} {remote_node_2} -d 1 -r 20 40 60',  # noqa: E501
     # 'remote_alias': 'flood {test_name} node1={remote_node_1} node2={remote_node_2} -d 1 -r 1 2 4',  # noqa: E501
 }
 
 
-@pytest.mark.parametrize('test_name', flood.get_single_test_generators().keys())
+@pytest.mark.parametrize(
+    'test_name', flood.generators.get_single_test_generators().keys()
+)
 @pytest.mark.parametrize('cmd_template', cmd_templates.keys())
 def test_load_test(
     test_name,
     cmd_template,
     flood_test_local_node_1,
     flood_test_local_node_2,
     flood_test_remote_node_1,
```

### Comparing `paradigm-flood-0.2.5/tests/test_node_parsing.py` & `paradigm_flood-0.3.0/tests/test_node_parsing.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     node_str = node_url
     if remote_client is not None:
         node_str = remote_client + ':' + node_str
     unnamed_node_str = node_str
     if name is not None:
         node_str = name + '=' + node_str
 
-    parsed = flood.parse_node(node_str, request_metadata=False)
+    parsed = flood.user_io.parse_node(node_str, request_metadata=False)
 
     if name is not None:
         assert parsed['name'] == name
     else:
         assert parsed['name'] == unnamed_node_str
 
     pieces = node_url.split(':')[0].split('.')
```

