# Comparing `tmp/jdaviz-3.5.0.tar.gz` & `tmp/jdaviz-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdaviz-3.5.0.tar", last modified: Thu May 25 17:33:01 2023, max compression
+gzip compressed data, was "jdaviz-3.6.0.tar", last modified: Fri Jul 28 18:47:40 2023, max compression
```

## Comparing `jdaviz-3.5.0.tar` & `jdaviz-3.6.0.tar`

### file list

```diff
@@ -1,483 +1,522 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.116366 jdaviz-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.bandit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.064365 jdaviz-3.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.064365 jdaviz-3.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.064365 jdaviz-3.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/workflows/changelog_check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/workflows/ci_cron_weekly.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/workflows/open_actions.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/workflows/predeps_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    43042 2023-05-25 17:32:41.000000 jdaviz-3.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-25 17:32:41.000000 jdaviz-3.5.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-25 17:32:41.000000 jdaviz-3.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-25 17:32:41.000000 jdaviz-3.5.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 17:32:41.000000 jdaviz-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-25 17:33:01.116366 jdaviz-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-25 17:32:41.000000 jdaviz-3.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-25 17:32:41.000000 jdaviz-3.5.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.064365 jdaviz-3.5.0/jdaviz/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    91295 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/app.vue
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.068365 jdaviz-3.5.0/jdaviz/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/docs_link.vue
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/external_link.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/glue_state_sync_wrapper.vue
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/layer_viewer_icon.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/number_uncertainty.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/play_pause_widget.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_add_results.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_auto_label.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_dataset_select.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_layer_select.vue
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_popout.vue
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_section_header.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_subset_select.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_table.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_viewer_select.vue
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/toolbar_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/toolbar_nested.vue
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/tooltip.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/tray_plugin.vue
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/viewer_data_select.vue
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/viewer_data_select_item.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.068365 jdaviz-3.5.0/jdaviz/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.068365 jdaviz-3.5.0/jdaviz/configs/cubeviz/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/cubeviz.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)    18788 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/slice.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/default/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/default/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/collapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/collapse.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/data_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/data_tools.vue
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/file_chooser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/export_plot/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/export_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/export_plot/export_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/export_plot/export_plot.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    36035 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/line_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/line_lists.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/markers.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    40907 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32160 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/plot_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    25473 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/plot_options.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18521 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/default/plugins/viewer_creator/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/viewer_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/imviz/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/imviz.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/aper_phot_simple/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/aper_phot_simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28436 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/compass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/compass.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/tests/test_compass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/coords_info/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/coords_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/image_viewer_creator/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/image_viewer_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/line_profile_xy/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/line_profile_xy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/links_control/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/links_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/links_control/links_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/links_control/links_control.vue
--rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/imviz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/imviz/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf
--rw-r--r--   0 runner    (1001) docker     (123)    41043 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/data/roman_wfi_image_model.asdf
--rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_astrowidgets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_line_profile_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_linking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_links_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    25880 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_parser_roman.py
--rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16331 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_simple_aper_phot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_subset_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_viewer_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_wcs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/wcs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/mosviz/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43652 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/mosviz.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40162 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/row_lock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/row_lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/mosviz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_data_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/specviz/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27550 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17378 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue
--rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/specviz.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20565 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/tests/test_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz2d/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42877 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/specviz2d.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz2d/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/container.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.100365 jdaviz-3.5.0/jdaviz/core/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21374 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/astrowidgets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/custom_traitlets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/data_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/freezable_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    37472 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/linelists.py
--rw-r--r--   0 runner    (1001) docker     (123)    21700 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/marks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14489 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/region_translators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/registries.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/style_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    99210 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/template_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.100365 jdaviz-3.5.0/jdaviz/core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tests/test_custom_traitlets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tests/test_data_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tests/test_region_translators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tests/test_template_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/validunits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.060365 jdaviz-3.5.0/jdaviz/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.104365 jdaviz-3.5.0/jdaviz/data/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/blink.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/checktoradial.svg
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/compass.svg
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/contrast.svg
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/left-east.svg
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/line_select.svg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/line_select_disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/pan.svg
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/pan2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/pan_x.svg
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/pan_y.svg
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/panzoom_match.svg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/pixelspectra.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/radialtocheck.svg
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/right-east.svg
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/select_circle.svg
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/select_ellipse.svg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/select_lasso.svg
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/select_single_pixel.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/select_x.svg
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/select_xy.svg
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/select_y.svg
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/slice.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/spectral_range.svg
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/tune.svg
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/zoom_back.svg
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/zoom_box.svg
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/zoom_box_match.svg
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/zoom_xrange.svg
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/zoom_yrange.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.108365 jdaviz-3.5.0/jdaviz/data/linelists/
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/Atomic-ISO.csv
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/Atomic-Ionic.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/CO-band-heads.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/CO.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/Common_nebular.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/Common_stellar.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/DEV_NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/H-He.csv
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/H-Paschen-Brackett.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20639 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/H2-ISO.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/H2-alt.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/H2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/HeI-HeII.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/JWST_line_list_original.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/PAH.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/SDSS-IV.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/SDSS.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/UV_linelist_vacuum.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/linelist_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/jdaviz_cli.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.108365 jdaviz-3.5.0/jdaviz/models/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/models/physical_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.108365 jdaviz-3.5.0/jdaviz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/test_data_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    27097 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/test_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/test_viewer_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-25 17:33:00.000000 jdaviz-3.5.0/jdaviz/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.068365 jdaviz-3.5.0/jdaviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-25 17:33:00.000000 jdaviz-3.5.0/jdaviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-05-25 17:33:01.000000 jdaviz-3.5.0/jdaviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:33:00.000000 jdaviz-3.5.0/jdaviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-25 17:33:00.000000 jdaviz-3.5.0/jdaviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:33:00.000000 jdaviz-3.5.0/jdaviz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-25 17:33:00.000000 jdaviz-3.5.0/jdaviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 17:33:00.000000 jdaviz-3.5.0/jdaviz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.108365 jdaviz-3.5.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-25 17:32:41.000000 jdaviz-3.5.0/licenses/GINGA_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-25 17:32:41.000000 jdaviz-3.5.0/licenses/IMEXAM_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-25 17:32:41.000000 jdaviz-3.5.0/licenses/IPYFILECHOOSER_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-25 17:32:41.000000 jdaviz-3.5.0/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-25 17:32:41.000000 jdaviz-3.5.0/licenses/TEMPLATE_LICENCE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.112365 jdaviz-3.5.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/CubevizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/ImvizDitheredExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19956 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/ImvizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/MosvizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/MosvizNIRISSExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/Specviz2dExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/SpecvizExample.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.116366 jdaviz-3.5.0/notebooks/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/cubeviz_contour_overlay.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/cubeviz_data_interactions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/cubeviz_fitting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/cubeviz_ndarray_gif.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/cubeviz_spectral_fitting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_color_display.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_compass_mpl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_custom_colormap.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_dithered_gwcs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_edit_subset_programmatic.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_line_profiles.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_load_3d_slices.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_load_fits_hdu.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_roman_asdf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_simple_aper_phot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20943 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/mosviz_concept.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/mosviz_generate_photometry.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/mosviz_niriss_parser.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/mosviz_overplot_slit.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/pypi_metrics.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/specviz_from_list.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    82825 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/specviz_from_splot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/specviz_line_lists.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/specviz_minimal.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/specviz_spectrum_list.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/specviz_unit_conversion.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-25 17:32:41.000000 jdaviz-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:33:01.116366 jdaviz-3.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5534 2023-05-25 17:32:41.000000 jdaviz-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.060365 jdaviz-3.5.0/share/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.060365 jdaviz-3.5.0/share/jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.060365 jdaviz-3.5.0/share/jupyter/nbconvert/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.060365 jdaviz-3.5.0/share/jupyter/nbconvert/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.116366 jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-25 17:32:41.000000 jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-05-25 17:32:41.000000 jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/app.html
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 17:32:41.000000 jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/conf.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     3265 2023-05-25 17:32:41.000000 jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2
--rwxr-xr-x   0 runner    (1001) docker     (123)     5993 2023-05-25 17:32:41.000000 jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/util.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.060365 jdaviz-3.5.0/share/jupyter/voila/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.060365 jdaviz-3.5.0/share/jupyter/voila/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.116366 jdaviz-3.5.0/share/jupyter/voila/templates/jdaviz-default/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-25 17:32:41.000000 jdaviz-3.5.0/share/jupyter/voila/templates/jdaviz-default/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-25 17:32:41.000000 jdaviz-3.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.301016 jdaviz-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.bandit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.241016 jdaviz-3.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.241016 jdaviz-3.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.245016 jdaviz-3.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/changelog_check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/ci_cron_weekly.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/open_actions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/predeps_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/standalone.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    47182 2023-07-28 18:47:24.000000 jdaviz-3.6.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-28 18:47:24.000000 jdaviz-3.6.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-28 18:47:24.000000 jdaviz-3.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-28 18:47:24.000000 jdaviz-3.6.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-28 18:47:24.000000 jdaviz-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-07-28 18:47:40.301016 jdaviz-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-28 18:47:24.000000 jdaviz-3.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-28 18:47:24.000000 jdaviz-3.6.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.245016 jdaviz-3.6.0/jdaviz/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/_astropy_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100517 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/app.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/docs_link.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/external_link.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/glue_state_sync_wrapper.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/layer_viewer_icon.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/number_uncertainty.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/play_pause_widget.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_add_results.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_auto_label.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_dataset_select.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_layer_select.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_plot.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_popout.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_section_header.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_subset_select.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_table.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_viewer_select.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/toolbar_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/toolbar_nested.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/tooltip.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/tray_plugin.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/viewer_data_select.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/viewer_data_select_item.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/configs/cubeviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/cubeviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/cubeviz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18788 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/slice.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_export_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/default.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/collapse.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/data_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/data_tools.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/file_chooser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/plugins/export_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/export_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/export_plot/export_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/export_plot/export_plot.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35599 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/line_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/line_lists.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/markers.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12863 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44507 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16097 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15676 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35709 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/plot_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/plot_options.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/default/plugins/viewer_creator/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/viewer_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/imviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/imviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/imviz.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/aper_phot_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/aper_phot_simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25491 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/compass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/compass.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/tests/test_compass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/coords_info/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/coords_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23107 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.265016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/image_viewer_creator/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/image_viewer_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.265016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/line_profile_xy/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/line_profile_xy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.265016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/links_control/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/links_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/links_control/links_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/links_control/links_control.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    14277 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.265016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.265016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.269016 jdaviz-3.6.0/jdaviz/configs/imviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.269016 jdaviz-3.6.0/jdaviz/configs/imviz/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/data/ds9_annulus_01.reg
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf
+-rw-r--r--   0 runner    (1001) docker     (123)  8425199 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/data/roman_wfi_image_model.asdf
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_astrowidgets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_line_profile_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_linking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_links_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25880 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_parser_roman.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_simple_aper_phot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_subset_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_viewer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_wcs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/wcs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.277016 jdaviz-3.6.0/jdaviz/configs/mosviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38346 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/mosviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/mosviz.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.277016 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40180 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.277016 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/row_lock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/row_lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.277016 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.277016 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18704 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.277016 jdaviz-3.6.0/jdaviz/configs/mosviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_data_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14962 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29328 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/specviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/specviz.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19884 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/tests/test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz2d/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42246 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/specviz2d.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.285016 jdaviz-3.6.0/jdaviz/configs/specviz2d/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/container.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.285016 jdaviz-3.6.0/jdaviz/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21374 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/astrowidgets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/custom_traitlets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/data_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/freezable_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40896 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/linelists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25077 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/marks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/region_translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/registries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/style_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108581 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/template_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.285016 jdaviz-3.6.0/jdaviz/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/test_autoconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/test_custom_traitlets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/test_data_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/test_region_translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/test_template_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/validunits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.237016 jdaviz-3.6.0/jdaviz/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.293016 jdaviz-3.6.0/jdaviz/data/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/blink.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/checktoradial.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/compass.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/contrast.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/home_match.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/left-east.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/line_select.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/line_select_disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/pan.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/pan2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/pan_x.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/pan_x_match.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/pan_y.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/pan_y_match.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/panzoom_match.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/pixelspectra.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/radialtocheck.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/right-east.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_annulus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_circle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_ellipse.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_lasso.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_single_pixel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_x.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_xy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_y.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/slice.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/spectral_range.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/tune.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/zoom_back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/zoom_box.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/zoom_box_match.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/zoom_xrange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/zoom_xrange_match.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/zoom_yrange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/zoom_yrange_match.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.293016 jdaviz-3.6.0/jdaviz/data/linelists/
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/Atomic-ISO.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/Atomic-Ionic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/CO-band-heads.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/CO.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/Common_nebular.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/Common_stellar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/DEV_NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/H-He.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/H-Paschen-Brackett.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20639 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/H2-ISO.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/H2-alt.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/H2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/HeI-HeII.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/JWST_line_list_original.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/PAH.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/SDSS-IV.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/SDSS.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/UV_linelist_vacuum.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/linelist_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/jdaviz_cli.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/jdaviz_cli_launcher.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.293016 jdaviz-3.6.0/jdaviz/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/models/physical_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.293016 jdaviz-3.6.0/jdaviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/test_data_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34729 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/test_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/test_viewer_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-28 18:47:39.000000 jdaviz-3.6.0/jdaviz/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.245016 jdaviz-3.6.0/jdaviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-07-28 18:47:40.000000 jdaviz-3.6.0/jdaviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18571 2023-07-28 18:47:40.000000 jdaviz-3.6.0/jdaviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:47:40.000000 jdaviz-3.6.0/jdaviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-28 18:47:40.000000 jdaviz-3.6.0/jdaviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:47:40.000000 jdaviz-3.6.0/jdaviz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-28 18:47:40.000000 jdaviz-3.6.0/jdaviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 18:47:40.000000 jdaviz-3.6.0/jdaviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.297016 jdaviz-3.6.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-28 18:47:24.000000 jdaviz-3.6.0/licenses/GINGA_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-28 18:47:24.000000 jdaviz-3.6.0/licenses/IMEXAM_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-28 18:47:24.000000 jdaviz-3.6.0/licenses/IPYFILECHOOSER_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-28 18:47:24.000000 jdaviz-3.6.0/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-28 18:47:24.000000 jdaviz-3.6.0/licenses/TEMPLATE_LICENCE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.297016 jdaviz-3.6.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/CubevizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17801 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/ImvizDitheredExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20170 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/ImvizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/MosvizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/MosvizNIRISSExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/Specviz2dExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/SpecvizExample.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.301016 jdaviz-3.6.0/notebooks/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/cubeviz_contour_overlay.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/cubeviz_data_interactions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/cubeviz_fitting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/cubeviz_ndarray_gif.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/cubeviz_spectral_fitting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_color_display.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_compass_mpl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_custom_colormap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_dithered_gwcs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_edit_subset_programmatic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_line_profiles.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_load_3d_slices.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_load_fits_hdu.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_roman_asdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_simple_aper_phot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/mosviz_concept.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/mosviz_generate_photometry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/mosviz_niriss_parser.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/mosviz_overplot_slit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/pypi_metrics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/specviz_from_list.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    82825 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/specviz_from_splot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/specviz_glue_unit_conversion.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/specviz_line_lists.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/specviz_minimal.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/specviz_spectrum_list.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-28 18:47:24.000000 jdaviz-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-28 18:47:40.305017 jdaviz-3.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5534 2023-07-28 18:47:24.000000 jdaviz-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.237016 jdaviz-3.6.0/share/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.237016 jdaviz-3.6.0/share/jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.237016 jdaviz-3.6.0/share/jupyter/nbconvert/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.237016 jdaviz-3.6.0/share/jupyter/nbconvert/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.301016 jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-28 18:47:24.000000 jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-07-28 18:47:24.000000 jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 18:47:24.000000 jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/conf.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3265 2023-07-28 18:47:24.000000 jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5993 2023-07-28 18:47:24.000000 jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/util.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.241016 jdaviz-3.6.0/share/jupyter/voila/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.241016 jdaviz-3.6.0/share/jupyter/voila/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.301016 jdaviz-3.6.0/share/jupyter/voila/templates/jdaviz-default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-28 18:47:24.000000 jdaviz-3.6.0/share/jupyter/voila/templates/jdaviz-default/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.301016 jdaviz-3.6.0/standalone/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/entitlements.plist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.301016 jdaviz-3.6.0/standalone/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-bqplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-debugpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-glue_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-ipypopout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-jdaviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-jupyter_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-mistune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-photutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-skimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/jdaviz-cli-entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/jdaviz.spec
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-28 18:47:24.000000 jdaviz-3.6.0/tox.ini
```

### Comparing `jdaviz-3.5.0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `jdaviz-3.6.0/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/.github/ISSUE_TEMPLATE/feature_request.yaml` & `jdaviz-3.6.0/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/.github/PULL_REQUEST_TEMPLATE.md` & `jdaviz-3.6.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/.github/workflows/ci_cron_weekly.yml` & `jdaviz-3.6.0/.github/workflows/ci_cron_weekly.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/.github/workflows/ci_workflows.yml` & `jdaviz-3.6.0/.github/workflows/ci_workflows.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/.github/workflows/codeql-analysis.yml` & `jdaviz-3.6.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/.github/workflows/open_actions.yml` & `jdaviz-3.6.0/.github/workflows/open_actions.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/.github/workflows/predeps_workflows.yml` & `jdaviz-3.6.0/.github/workflows/predeps_workflows.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/.github/workflows/publish.yml` & `jdaviz-3.6.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/.gitignore` & `jdaviz-3.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/.readthedocs.yaml` & `jdaviz-3.6.0/.readthedocs.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 version: 2
 
 build:
-  os: ubuntu-20.04
+  os: ubuntu-22.04
   apt_packages:
     - graphviz
   tools:
-    python: "3.9"
+    python: "3.11"
   jobs:
     post_checkout:
       # Use `git log` to check if the latest commit contains "skip rtd" or "rtd skip",
       # in that case exit the command with 183 to skip the build
       - MSG=`git --no-pager log --pretty="tformat:%s -- %b" -1`; case $MSG in *"skip rtd"*|*"rtd skip"*) exit 183;; *);; esac
 
 sphinx:
```

### Comparing `jdaviz-3.5.0/CHANGES.rst` & `jdaviz-3.6.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,153 @@
+3.6 (2023-07-28)
+================
+
+New Features
+------------
+
+- Introduce jdaviz.open to automatically detect the appropriate config and load data [#2221]
+
+- Add Simplify button to subset plugin to make composite spectral subsets more user
+  friendly. [#2237]
+
+- Plots within plugins can now be popped-out into their own windows. [#2254]
+
+- The ``specviz.load_spectrum`` method is deprecated; use ``specviz.load_data`` instead. [#2273]
+
+- Add launcher to select and identify compatible configurations,
+  and require --layout argument when launching standalone. [#2257, #2267]
+
+- Viewer toolbar items hide themselves when they are not applicable. [#2284]
+
+- Data menu single select will default to the first element. [#2298]
+
+- Line Analysis "Redshift from Centroid" only visible when lines are loaded. [#2294]
+
+- Add lines representing the stretch vmin and vmax to the plot options histogram. [#2301]
+
+- Add option to set bin size in plot options plugin and API call to change histogram
+  viewer limits. [#2309]
+
+
+Cubeviz
+^^^^^^^
+
+- Added the ability to export cube slices to video. User will need to install
+  ``opencv-python`` separately or use ``[all]`` specifier when installing Jdaviz. [#2264]
+
+Imviz
+^^^^^
+
+- Added the ability to load DS9 region files (``.reg``) using the ``IMPORT DATA``
+  button. However, this only works after loading at least one image into Imviz. [#2201]
+
+- Added support for new ``CircularAnnulusROI`` subset from glue, including
+  a new draw tool. [#2201, #2240]
+
+Mosviz
+^^^^^^
+
+- Improved x-axis limit-matching between 2d and 1d spectrum viewers. [#2219]
+
+Specviz
+^^^^^^^
+
+Specviz2d
+^^^^^^^^^
+
+- Re-enable support for displaying the 1d spectrum in wavelength/frequency space, with improved
+  x-axis limit-matching. [#2219]
+
+API Changes
+-----------
+
+- ``viz.app.get_data_from_viewer()`` is deprecated; use ``viz.get_data()``. [#2242]
+
+- ``viz.app.get_subsets_from_viewer()`` is deprecated; use ``viz.app.get_subsets()``. [#2242]
+
+- ``viz.get_data()`` now takes optional ``**kwargs``; e.g., you could pass in
+  ``function="sum"`` to collapse a cube in Cubeviz. [#2242]
+
+- Live-previews and keypress events that depend on the plugin being opened now work for inline
+  and popout windows. [#2295]
+
+Cubeviz
+^^^^^^^
+
+Imviz
+^^^^^
+
+- Simple Aperture Photometry plugin: Custom annulus background options are removed.
+  Please draw/load annulus as you would with other region shapes, then select it
+  in the plugin from Subset dropdown for the background. Using annulus region as
+  aperture is not supported. [#2276, #2287]
+
+Mosviz
+^^^^^^
+
+- Added new ``statistic`` keyword to ``mosviz.get_viewer("spectrum-2d-viewer").data()``
+  to allow user to collapse 2D spectrum to 1D. [#2242]
+
+Specviz
+^^^^^^^
+
+- Re-enabled unit conversion support. [#2127]
+
+Specviz2d
+^^^^^^^^^
+
+Bug Fixes
+---------
+
+- Fixed wrong elliptical region translation in ``app.get_subsets()``. [#2244]
+
+- Fixed ``cls`` input being ignored in ``viz.get_data()``. [#2242]
+
+- Line analysis plugin's ``show_continuum_marks`` is deprecated, use ``plugin.as_active()`` 
+  instead. [#2295]
+
+Cubeviz
+^^^^^^^
+
+- Moment Map plugin now writes FITS file to working directory if no path provided
+  in standalone mode. [#2264]
+
+- Fixes detection of spatial vs spectral subsets for composite subsets.
+  Also fixes the shadow mark that shows the intersection between spatial and spectral
+  subsets. [#2207, #2266, #2291]
+
+- Prevent Plot Options plugin from hanging when selecting a spectrum viewer in Cubeviz. [#2305]
+
+Imviz
+^^^^^
+
+Mosviz
+^^^^^^
+
+Specviz
+^^^^^^^
+
+- Uncertainties in spectra given to Specviz will now work correctly when non-standard deviation type [#2283]
+
+Specviz2d
+^^^^^^^^^
+
+Other Changes and Additions
+---------------------------
+
+- Gaussian smooth plugin excludes results from the gaussian smooth plugin from the input
+  dataset dropdown. [#2239]
+
+- CLI launchers no longer require data to be specified [#1960]
+
+- Added direct launchers for each config (e.g. ``specviz``) [#1960]
+
+- Replacing existing data from a plugin (e.g., refitting a model with the same label)
+  now preserves the plot options of the data as previously displayed. [#2288]
+
 3.5 (2023-05-25)
 ================
 
 New Features
 ------------
 
 - Model fitting results are logged in a table within the plugin. [#2093]
@@ -26,14 +172,15 @@
 ^^^^^^^
 
 - ``get_data`` now supports ``function=True`` to adopt the collapse-function from the spectrum viewer.
   [#2117]
 
 - ``get_data`` now supports applying a spectral mask to a collapse spatial subset. [#2199, #2214]
 
+
 Imviz
 ^^^^^
 
 - Table exposing past results in the aperture photometry plugin. [#1985, #2015]
 
 - New canvas rotation plugin to rotate displayed image without affecting actual data. [#1983]
```

### Comparing `jdaviz-3.5.0/CITATION.cff` & `jdaviz-3.6.0/CITATION.cff`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 - family-names: "Geda"
   given-names: "Robel"
   orcid: "https://orcid.org/0000-0003-1509-9966"
 - family-names: "Jones"
   given-names: "Craig"
 - family-names: "Karatay"
   given-names: "Hatice"
+  orcid: "https://orcid.org/0009-0003-9872-9384"
 - family-names: "Kotler"
   given-names: "Jenn"
   orcid: "https://orcid.org/0000-0002-1294-7862"
 - family-names: "Lim"
   given-names: "Pey Lian"
   orcid: "https://orcid.org/0000-0003-0079-4114"
 - family-names: "Morris"
@@ -65,13 +66,13 @@
   orcid: "https://orcid.org/0009-0008-4112-7418"
 - family-names: "Tollerud"
   given-names: "Erik"
   orcid: "https://orcid.org/0000-0002-9599-310X"
 - family-names: "Volfman"
   given-names: "Sabrina"
 title: "Jdaviz"
-version: 3.5.0
+version: 3.6.0
 doi: https://doi.org/10.5281/zenodo.5513927
-date-released: 2023-05-25
+date-released: 2023-07-28
 url: "https://github.com/spacetelescope/jdaviz"
 
 # see a full list of contributors here: https://github.com/spacetelescope/jdaviz/graphs/contributors
```

### Comparing `jdaviz-3.5.0/CODE_OF_CONDUCT.md` & `jdaviz-3.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/LICENSE.rst` & `jdaviz-3.6.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/PKG-INFO` & `jdaviz-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: jdaviz
-Version: 3.5.0
+Version: 3.6.0
 Summary: Astronomical data analysis development leveraging the Jupyter platform
-Author-email: JDADF Developers <rosteen@stsci.edu>
+Home-page: https://jdaviz.readthedocs.io/en/latest/
+Author: JDADF Developers
+Author-email: JDADF Developers <help@stsci.edu>
 Project-URL: Homepage, https://jdaviz.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: all
 Provides-Extra: roman
 License-File: LICENSE.rst
 
 .. image:: docs/logos/jdaviz.svg
     :width: 400
     :alt: Jdaviz logo
     :align: center
@@ -89,15 +92,15 @@
 
 ``jdaviz`` provides a command-line tool to start the web application. To see the syntax and usage,
 from a terminal, type:
 
 .. code-block:: bash
 
     jdaviz --help
-    jdaviz specviz /path/to/data/spectral_file
+    jdaviz --layout=specviz /path/to/data/spectral_file
 
 For more information on the command line interfaces for each tool, see the
 `Jdaviz docs <https://jdaviz.readthedocs.io/en/latest/index.html>`_.
 
 
 In a Jupyter Notebook
 +++++++++++++++++++++
```

### Comparing `jdaviz-3.5.0/README.rst` & `jdaviz-3.6.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 ``jdaviz`` provides a command-line tool to start the web application. To see the syntax and usage,
 from a terminal, type:
 
 .. code-block:: bash
 
     jdaviz --help
-    jdaviz specviz /path/to/data/spectral_file
+    jdaviz --layout=specviz /path/to/data/spectral_file
 
 For more information on the command line interfaces for each tool, see the
 `Jdaviz docs <https://jdaviz.readthedocs.io/en/latest/index.html>`_.
 
 
 In a Jupyter Notebook
 +++++++++++++++++++++
```

### Comparing `jdaviz-3.5.0/conftest.py` & `jdaviz-3.6.0/conftest.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/__init__.py` & `jdaviz-3.6.0/jdaviz/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 from jdaviz.app import *  # noqa: F401, F403
 from jdaviz.configs.specviz import Specviz  # noqa: F401
 from jdaviz.configs.specviz2d import Specviz2d  # noqa: F401
 from jdaviz.configs.mosviz import Mosviz  # noqa: F401
 from jdaviz.configs.cubeviz import Cubeviz  # noqa: F401
 from jdaviz.configs.imviz import Imviz  # noqa: F401
 from jdaviz.utils import enable_hot_reloading  # noqa: F401
+from jdaviz.core.launcher import open  # noqa: F401
 
 # Clean up namespace.
 del os
 del TestRunner
```

### Comparing `jdaviz-3.5.0/jdaviz/app.py` & `jdaviz-3.6.0/jdaviz/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,45 +5,44 @@
 import warnings
 from inspect import isclass
 import operator
 
 from ipywidgets import widget_serialization
 import ipyvue
 
+from astropy import units as u
 from astropy.nddata import CCDData, NDData
 from astropy.io import fits
-from astropy import units as u
-from astropy.coordinates import Angle
 from astropy.time import Time
-from regions import PixCoord, CirclePixelRegion, RectanglePixelRegion, EllipsePixelRegion
-
+from astropy.utils.decorators import deprecated
 from echo import CallbackProperty, DictCallbackProperty, ListCallbackProperty
 from ipygoldenlayout import GoldenLayout
 from ipysplitpanes import SplitPanes
 from traitlets import Dict, Bool, Unicode, Any
 from specutils import Spectrum1D, SpectralRegion
 import matplotlib.cm as cm
 import numpy as np
 
 from glue.core.exceptions import IncompatibleAttribute
 from glue.config import colormaps, data_translator
 from glue.config import settings as glue_settings
 from glue.core import BaseData, HubListener, Data, DataCollection
-from glue.core.link_helpers import LinkSame
+from glue.core.link_helpers import LinkSame, LinkSameWithUnits
 from glue.plugins.wcs_autolinking.wcs_autolinking import WCSLink, IncompatibleWCS
 from glue.core.message import (DataCollectionAddMessage,
                                DataCollectionDeleteMessage,
                                SubsetCreateMessage,
                                SubsetUpdateMessage,
                                SubsetDeleteMessage)
 from glue.core.state_objects import State
 from glue.core.subset import (Subset, RangeSubsetState, RoiSubsetState,
                               CompositeSubsetState, InvertState)
-from glue.core.roi import CircularROI, EllipticalROI, RectangularROI
+from glue.core.units import unit_converter
 from glue_astronomy.spectral_coordinates import SpectralCoordinates
+from glue_astronomy.translators.regions import roi_subset_state_to_region
 from glue_jupyter.app import JupyterApplication
 from glue_jupyter.common.toolbar_vuetify import read_icon
 from glue_jupyter.state_traitlets_helpers import GlueState
 from glue_jupyter.bqplot.profile import BqplotProfileView
 from ipyvuetify import VuetifyTemplate
 
 from jdaviz import __version__
@@ -66,18 +65,65 @@
 
 CONTAINER_TYPES = dict(row='gl-row', col='gl-col', stack='gl-stack')
 EXT_TYPES = dict(flux=['flux', 'sci'],
                  uncert=['ivar', 'err', 'var', 'uncert'],
                  mask=['mask', 'dq'])
 
 
+@unit_converter('custom-jdaviz')
+class UnitConverterWithSpectral:
+
+    def equivalent_units(self, data, cid, units):
+        if cid.label == "flux":
+            eqv = u.spectral_density(1 * u.m)  # Value does not matter here.
+            list_of_units = set(list(map(str, u.Unit(units).find_equivalent_units(
+                include_prefix_units=True, equivalencies=eqv))) + [
+                    'Jy', 'mJy', 'uJy',
+                    'W / (m2 Hz)', 'W / (Hz m2)',  # Order is different in astropy v5.3
+                    'eV / (s m2 Hz)', 'eV / (Hz s m2)',
+                    'erg / (s cm2)',
+                    'erg / (s cm2 Angstrom)', 'erg / (Angstrom s cm2)',
+                    'erg / (s cm2 Hz)', 'erg / (Hz s cm2)',
+                    'ph / (s cm2 Angstrom)', 'ph / (Angstrom s cm2)',
+                    'ph / (s cm2 Hz)', 'ph / (Hz s cm2)'
+                ])
+        else:  # spectral axis
+            # prefer Hz over Bq and um over micron
+            exclude = {'Bq', 'micron'}
+            list_of_units = set(list(map(str, u.Unit(units).find_equivalent_units(
+                include_prefix_units=True, equivalencies=u.spectral())))) - exclude
+        return list_of_units
+
+    def to_unit(self, data, cid, values, original_units, target_units):
+        # Given a glue data object (data), a component ID (cid), the values
+        # to convert, and the original and target units of the values, this method
+        # should return the converted values. Note that original_units
+        # gives the units of the values array, which might not be the same
+        # as the original native units of the component in the data.
+        if cid.label == "flux":
+            spec = data.get_object(cls=Spectrum1D)
+            if len(values) == 2:
+                # Need this for setting the y-limits
+                spec_limits = [spec.spectral_axis[0].value, spec.spectral_axis[-1].value]
+                eqv = u.spectral_density(spec_limits*spec.spectral_axis.unit)
+            else:
+                eqv = u.spectral_density(spec.spectral_axis)
+        else:  # spectral axis
+            eqv = u.spectral()
+
+        return (values * u.Unit(original_units)).to_value(u.Unit(target_units), equivalencies=eqv)
+
+
 # Set default opacity for data layers to 1 instead of 0.8 in
 # some glue-core versions
 glue_settings.DATA_ALPHA = 1
 
+# Enable spectrum unit conversion.
+glue_settings.UNIT_CONVERTER = 'custom-jdaviz'
+
 custom_components = {'j-tooltip': 'components/tooltip.vue',
                      'j-external-link': 'components/external_link.vue',
                      'j-docs-link': 'components/docs_link.vue',
                      'j-viewer-data-select': 'components/viewer_data_select.vue',
                      'j-viewer-data-select-item': 'components/viewer_data_select_item.vue',
                      'j-layer-viewer-icon': 'components/layer_viewer_icon.vue',
                      'j-tray-plugin': 'components/tray_plugin.vue',
@@ -447,30 +493,31 @@
         linked_data = dc[data_to_be_linked] if data_to_be_linked else dc[-1]
 
         if 'Trace' in linked_data.meta:
             links = [LinkSame(linked_data.components[1], ref_data.components[0]),
                      LinkSame(linked_data.components[0], ref_data.components[1])]
             dc.add_link(links)
             return
-        elif (linked_data.meta.get('Plugin', None) == 'SpectralExtraction' or
-                (linked_data.meta.get('Plugin', None) == ('GaussianSmooth') and
-                 linked_data.ndim < 3 and  # Cube linking requires special logic. See below
-                 ref_data.ndim < 3)
+        elif ((self.config in ('specviz2d', 'mosviz') and
+               linked_data.meta.get('Plugin', None) is not None) or
+              (linked_data.meta.get('Plugin', None) == 'GaussianSmooth' and
+               linked_data.ndim < 3 and  # Cube linking requires special logic. See below
+               ref_data.ndim < 3)
               ):
             links = [LinkSame(linked_data.components[0], ref_data.components[0]),
                      LinkSame(linked_data.components[1], ref_data.components[1])]
             dc.add_link(links)
             return
 
         # The glue-astronomy SpectralCoordinates currently seems incompatible with glue
         # WCSLink. This gets around it until there's an upstream fix.
         if isinstance(linked_data.coords, SpectralCoordinates):
             wc_old = ref_data.world_component_ids[-1]
             wc_new = linked_data.world_component_ids[0]
-            self.data_collection.add_link(LinkSame(wc_old, wc_new))
+            self.data_collection.add_link(LinkSameWithUnits(wc_old, wc_new))
             return
 
         try:
             if linked_data.meta.get("Plugin", None) == 'GaussianSmooth':
                 raise AttributeError
             dc.add_link(WCSLink(ref_data, linked_data))
         except (AttributeError, IncompatibleWCS):
@@ -508,16 +555,16 @@
                     else:
                         continue
                 elif pixel_coord in pc_linked:
                     linked_index = pc_linked.index(pixel_coord)
                 else:
                     continue
 
-                links.append(LinkSame(ref_data.pixel_component_ids[ref_index],
-                                      linked_data.pixel_component_ids[linked_index]))
+                links.append(LinkSameWithUnits(ref_data.pixel_component_ids[ref_index],
+                                               linked_data.pixel_component_ids[linked_index]))
 
             dc.add_link(links)
 
     def load_data(self, file_obj, parser_reference=None, **kwargs):
         """
         Provided a path to a data file, open and parse the data into the
         `~glue.core.data_collection.DataCollection` for this session.
@@ -609,14 +656,15 @@
 
     def get_viewer_by_id(self, vid):
         """Like :meth:`get_viewer` but use ID directly instead of reference name.
         This is useful when reference name is `None`.
         """
         return self._viewer_store.get(vid)
 
+    @deprecated(since="3.6", alternative="viz_helper.get_data")
     def get_data_from_viewer(self, viewer_reference, data_label=None,
                              cls='default', include_subsets=True):
         """
         Returns each data component currently rendered within a viewer
         instance. Viewers themselves store a default data type to which the
         Glue data components are transformed upon retrieval. This can be
         optionally overridden with the ``cls`` keyword.
@@ -716,14 +764,15 @@
                                 continue
 
                         data[label] = layer_data
 
         # If a data label was provided, return only the corresponding data, otherwise return all:
         return data.get(data_label, data)
 
+    @deprecated(since="3.6", alternative="get_subsets")
     def get_subsets_from_viewer(self, viewer_reference, data_label=None, subset_type=None):
         """
         Returns the subsets of a specified viewer converted to astropy regions
         objects.
 
         It should be noted that the subset translation machinery lives in the
         glue-astronomy repository. Currently, the machinery only works on 2D
@@ -750,17 +799,19 @@
         -------
         data : dict
             A dict of the transformed Glue subset objects, with keys
             representing the subset name and values as astropy regions
             objects.
         """
         viewer = self.get_viewer(viewer_reference)
-        data = self.get_data_from_viewer(viewer_reference,
-                                         data_label,
-                                         cls=None)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            data = self.get_data_from_viewer(viewer_reference,
+                                             data_label,
+                                             cls=None)
         regions = {}
 
         if data_label is not None:
             data = {data_label: data}
 
         for key, value in data.items():
             if isinstance(value, Subset):
@@ -792,15 +843,17 @@
                 #  supported currently). We now eschew the use of the
                 #  translation machinery entirely and construct the astropy
                 #  region ourselves.
                 elif value.data.ndim == 1:
                     regions[key] = self.get_subsets(key)
                     continue
 
-                temp_data = self.get_data_from_viewer(viewer_reference, value.label)
+                with warnings.catch_warnings():
+                    warnings.simplefilter("ignore")
+                    temp_data = self.get_data_from_viewer(viewer_reference, value.label)
                 if isinstance(temp_data, Spectrum1D):
                     regions[key] = self.get_subsets(key)
                     continue
 
                 # Get the pixel coordinate [z] of the 3D data, repeating the
                 #  wavelength axis. This doesn't seem strictly necessary as it
                 #  returns the same data if the pixel axis is [y] or [x]
@@ -848,15 +901,16 @@
                 region = subset_group.subsets[0].data.get_selection_definition(
                     format='astropy-regions')
                 regions[key] = region
 
         return regions
 
     def get_subsets(self, subset_name=None, spectral_only=False,
-                    spatial_only=False, object_only=False, simplify_spectral=True):
+                    spatial_only=False, object_only=False, simplify_spectral=True,
+                    use_display_units=False):
         """
         Returns all branches of glue subset tree in the form that subset plugin can recognize.
 
         Parameters
         ----------
         subset_name : str
             The subset name.
@@ -865,14 +919,17 @@
         spatial_only : bool
             Return only spatial subsets, except masked subsets (uncommon).
         object_only : bool
             Return only object relevant information and
             leave out the region class name and glue_state.
         simplify_spectral : bool
             Return a composite spectral subset collapsed to a simplified SpectralRegion.
+        use_display_units: bool, optional
+            Whether to convert to the display units defined in the
+            :ref:`Unit Conversion <unit-conversion>` plugin.
 
         Returns
         -------
         data : dict
             A dict with keys representing the subset name and values as astropy regions
             objects.
         """
@@ -883,23 +940,25 @@
         all_subsets = {}
 
         for subset in subsets:
             label = subset.label
             if isinstance(subset.subset_state, CompositeSubsetState):
                 # Region composed of multiple ROI or Range subset
                 # objects that must be traversed
-                subset_region = self.get_sub_regions(subset.subset_state, simplify_spectral)
+                subset_region = self.get_sub_regions(subset.subset_state,
+                                                     simplify_spectral, use_display_units)
             elif isinstance(subset.subset_state, RoiSubsetState):
                 # 3D regions represented as a dict including an
                 # AstropyRegion object if possible
                 subset_region = self._get_roi_subset_definition(subset.subset_state)
             elif isinstance(subset.subset_state, RangeSubsetState):
                 # 2D regions represented as SpectralRegion objects
                 subset_region = self._get_range_subset_bounds(subset.subset_state,
-                                                              simplify_spectral)
+                                                              simplify_spectral,
+                                                              use_display_units)
             else:
                 # subset.subset_state can be an instance of MaskSubsetState
                 # or something else we do not know how to handle
                 all_subsets[label] = None
                 continue
 
             # Is the subset spectral, spatial, temporal?
@@ -962,67 +1021,56 @@
         for region in spec_regions:
             if not regions_no_dups:
                 regions_no_dups = region
             elif region.bounds not in regions_no_dups.subregions:
                 regions_no_dups += region
         return regions_no_dups
 
-    def _get_range_subset_bounds(self, subset_state, simplify_spectral=True):
+    def _get_range_subset_bounds(self, subset_state,
+                                 simplify_spectral=True, use_display_units=False):
         # TODO: Use global display units
         # units = dc[0].data.coords.spectral_axis.unit
         viewer = self.get_viewer(self._jdaviz_helper. _default_spectrum_viewer_reference_name)
         data = viewer.data()
-        if viewer:
-            units = u.Unit(viewer.state.x_display_unit)
-        elif data and len(data) > 0 and isinstance(data[0], Spectrum1D):
+        if data and len(data) > 0 and isinstance(data[0], Spectrum1D):
             units = data[0].spectral_axis.unit
         else:
             raise ValueError("Unable to find spectral axis units")
+        if use_display_units:
+            # converting may result in flipping order (wavelength <-> frequency)
+            ret_units = self._get_display_unit('spectral')
+            subset_bounds = [(subset_state.lo * units).to(ret_units, u.spectral()),
+                             (subset_state.hi * units).to(ret_units, u.spectral())]
+            spec_region = SpectralRegion(min(subset_bounds), max(subset_bounds))
+        else:
+            spec_region = SpectralRegion(subset_state.lo * units, subset_state.hi * units)
 
-        spec_region = SpectralRegion(subset_state.lo * units, subset_state.hi * units)
         if not simplify_spectral:
             return [{"name": subset_state.__class__.__name__,
                      "glue_state": subset_state.__class__.__name__,
                      "region": spec_region,
                      "subset_state": subset_state}]
         return spec_region
 
     def _get_roi_subset_definition(self, subset_state):
-        _around_decimals = 6
-        roi = subset_state.roi
-        roi_as_region = None
-        if isinstance(roi, CircularROI):
-            x, y = roi.get_center()
-            r = roi.radius
-            roi_as_region = CirclePixelRegion(PixCoord(x, y), r)
-
-        elif isinstance(roi, RectangularROI):
-            theta = np.around(np.degrees(roi.theta), decimals=_around_decimals)
-            roi_as_region = RectanglePixelRegion(PixCoord(roi.center()[0], roi.center()[1]),
-                                                 roi.width(), roi.height(), Angle(theta, "deg"))
-
-        elif isinstance(roi, EllipticalROI):
-            xc = roi.xc
-            yc = roi.yc
-            rx = roi.radius_x
-            ry = roi.radius_y
-            theta = np.around(np.degrees(roi.theta), decimals=_around_decimals)
-            roi_as_region = EllipsePixelRegion(PixCoord(xc, yc), rx, ry, Angle(theta, "deg"))
-
+        # TODO: Imviz: Return sky region if link type is WCS.
+        roi_as_region = roi_subset_state_to_region(subset_state)
         return [{"name": subset_state.roi.__class__.__name__,
                  "glue_state": subset_state.__class__.__name__,
                  "region": roi_as_region,
                  "subset_state": subset_state}]
 
-    def get_sub_regions(self, subset_state, simplify_spectral=True):
+    def get_sub_regions(self, subset_state, simplify_spectral=True, use_display_units=False):
 
         if isinstance(subset_state, CompositeSubsetState):
             if subset_state and hasattr(subset_state, "state2") and subset_state.state2:
-                one = self.get_sub_regions(subset_state.state1, simplify_spectral)
-                two = self.get_sub_regions(subset_state.state2, simplify_spectral)
+                one = self.get_sub_regions(subset_state.state1,
+                                           simplify_spectral, use_display_units)
+                two = self.get_sub_regions(subset_state.state2,
+                                           simplify_spectral, use_display_units)
 
                 if isinstance(one, list) and "glue_state" in one[0]:
                     one[0]["glue_state"] = subset_state.__class__.__name__
 
                 if isinstance(subset_state.state2, InvertState):
                     # This covers the REMOVE subset mode
 
@@ -1102,34 +1150,168 @@
                     #   (4.0 um, 4.5 um)
 
                     # two.invert(one.lower, one.upper) + one.invert(two.lower, two.upper)
                     # Spectral Region, 3 sub-regions:
                     #   (4.0 um, 4.5 um)    (5.0 um, 6.0 um)    (9.0 um, 12.0 um)
 
                     if isinstance(two, SpectralRegion):
-                        if one.lower > two.lower:
-                            # If one.lower is less than two.lower, it will be included
-                            # in the two.invert() call. Otherwise, we can add it like this.
-                            return (two.invert(one.lower, one.upper) +
-                                    one.invert(two.lower, two.upper))
-                        return two.invert(one.lower, one.upper)
+                        new_region = None
+                        temp_region = None
+                        for subregion in two:
+                            # Add all subregions that do not intersect with XOR region
+                            # to a new SpectralRegion object
+                            if subregion.lower > one.upper or subregion.upper < one.lower:
+                                if not new_region:
+                                    new_region = subregion
+                                else:
+                                    new_region += subregion
+                            # All other subregions are added to temp_region
+                            else:
+                                if not temp_region:
+                                    temp_region = subregion
+                                else:
+                                    temp_region += subregion
+                        # This is the main application of XOR to other regions
+                        if not new_region:
+                            new_region = temp_region.invert(one.lower, one.upper)
+                        else:
+                            new_region = new_region + temp_region.invert(one.lower, one.upper)
+                        # This adds the edge regions that are otherwise not included
+                        if not (one.lower == temp_region.lower and one.upper == temp_region.upper):
+                            new_region = new_region + one.invert(temp_region.lower,
+                                                                 temp_region.upper)
+                        return new_region
                     else:
                         return two + one
             else:
                 # This gets triggered in the InvertState case where state1
                 # is an object and state2 is None
-                return self.get_sub_regions(subset_state.state1, simplify_spectral)
+                return self.get_sub_regions(subset_state.state1,
+                                            simplify_spectral, use_display_units)
         elif subset_state is not None:
             # This is the leaf node of the glue subset state tree where
             # a subset_state is either ROI or Range.
             if isinstance(subset_state, RoiSubsetState):
                 return self._get_roi_subset_definition(subset_state)
 
             elif isinstance(subset_state, RangeSubsetState):
-                return self._get_range_subset_bounds(subset_state, simplify_spectral)
+                return self._get_range_subset_bounds(subset_state,
+                                                     simplify_spectral, use_display_units)
+
+    def _get_display_unit(self, axis):
+        if self._jdaviz_helper is None or self._jdaviz_helper.plugins.get('Unit Conversion') is None:  # noqa
+            # fallback on native units (unit conversion is not enabled)
+            if axis == 'spectral':
+                sv = self.get_viewer(self._jdaviz_helper._default_spectrum_viewer_reference_name)
+                return sv.data()[0].spectral_axis.unit
+            elif axis == 'flux':
+                sv = self.get_viewer(self._jdaviz_helper._default_spectrum_viewer_reference_name)
+                return sv.data()[0].flux.unit
+            else:
+                raise ValueError(f"could not find units for axis='{axis}'")
+        try:
+            return getattr(self._jdaviz_helper.plugins.get('Unit Conversion')._obj,
+                           f'{axis}_unit_selected')
+        except AttributeError:
+            raise ValueError(f"could not find display unit for axis='{axis}'")
+
+    def simplify_spectral_subset(self, subset_name, att, overwrite=False):
+        """
+        Convert a composite spectral subset consisting of And, AndNot, Or, Replace, and Xor
+        into one consisting of just Range and Or state objects.
+
+        Parameters
+        ----------
+        subset_name : str
+            Name of subset to simplify.
+        att : str
+            Attribute that the subset uses to apply to data.
+        overwrite : bool
+            Whether to update the current subset with the simplified state or apply it
+            to a new subset.
+        """
+        if self.is_there_overlap_spectral_subset(subset_name):
+            new_state = self.merge_overlapping_spectral_regions(subset_name, att)
+        else:
+            new_state = None
+            spectral_region = self.get_subsets(subset_name, spectral_only=True)
+            # Reverse through sub regions so that they are added back
+            # in the order of lowest values to highest
+            for index in range(len(spectral_region) - 1, -1, -1):
+                convert_to_range = RangeSubsetState(spectral_region[index].lower.value,
+                                                    spectral_region[index].upper.value,
+                                                    att)
+                if new_state is None:
+                    new_state = convert_to_range
+                else:
+                    new_state = new_state | convert_to_range
+
+        dc = self.data_collection
+        if not overwrite:
+            dc.new_subset_group(subset_state=new_state)
+        else:
+            old_subset = [subsets for subsets in dc.subset_groups
+                          if subsets.label == subset_name][0]
+            old_subset.subset_state = new_state
+
+    def is_there_overlap_spectral_subset(self, subset_name):
+        """
+        Returns True if the spectral subset with subset_name has overlapping
+        subregions.
+        """
+        spectral_region = self.get_subsets(subset_name, spectral_only=True)
+        if not spectral_region or len(spectral_region) < 2:
+            return False
+        for index in range(0, len(spectral_region) - 1):
+            if spectral_region[index].upper.value >= spectral_region[index + 1].lower.value:
+                return True
+        return False
+
+    def merge_overlapping_spectral_regions(self, subset_name, att):
+        """
+        Takes a spectral subset with subset_name and returns an ``OrState`` object
+        that merges all overlapping subregions.
+
+        Parameters
+        ----------
+        subset_name : str
+            Name of subset to simplify.
+        att : str
+            Attribute that the subset uses to apply to data.
+        """
+        spectral_region = self.get_subsets(subset_name, spectral_only=True)
+        merged_regions = None
+        # Convert SpectralRegion object into a list with tuples representing
+        # the lower and upper values of each region.
+        reg_as_tup = [(sr.lower.value, sr.upper.value) for sr in spectral_region]
+        for index in range(0, len(spectral_region)):
+            # Instantiate merged regions
+            if not merged_regions:
+                merged_regions = [reg_as_tup[index]]
+            else:
+                last_merged = merged_regions[-1]
+                # If the lower value of the current subregion is less than or equal to the upper
+                # value of the last subregion added to merged_regions, update last_merged
+                # with the max upper value between the two regions.
+                if reg_as_tup[index][0] <= last_merged[1]:
+                    last_merged = (last_merged[0], max(last_merged[1], reg_as_tup[index][1]))
+                    merged_regions = merged_regions[:-1]
+                    merged_regions.append(last_merged)
+                else:
+                    merged_regions.append(reg_as_tup[index])
+
+        new_state = None
+        for region in reversed(merged_regions):
+            convert_to_range = RangeSubsetState(region[0], region[1], att)
+            if new_state is None:
+                new_state = convert_to_range
+            else:
+                new_state = new_state | convert_to_range
+
+        return new_state
 
     def add_data(self, data, data_label=None, notify_done=True):
         """
         Add data to the Glue ``DataCollection``.
 
         Parameters
         ----------
@@ -1303,27 +1485,14 @@
 
         viewer_item = self._get_viewer_item(viewer_reference)
         if viewer_item is None:
             raise ValueError(f"Could not identify viewer with reference {viewer_reference}")
 
         self.set_data_visibility(viewer_item, data_label, visible=visible, replace=clear_other_data)
 
-    def _set_plot_axes_labels(self, viewer_id):
-        """
-        Sets the plot axes labels to be the units of the data to be loaded.
-
-        Parameters
-        ----------
-        viewer_id : str
-            The UUID associated with the desired viewer item.
-        """
-        viewer = self._viewer_by_id(viewer_id)
-
-        viewer.set_plot_axes()
-
     def remove_data_from_viewer(self, viewer_reference, data_label):
         """
         Removes a data set from the specified viewer.
 
         Parameters
         ----------
         viewer_reference : str
@@ -1656,14 +1825,15 @@
                 raise ValueError(
                     f"No data item found with label '{data_label}'. Label must be one "
                     "of:\n\t" + "\n\t".join(dc_labels))
 
             [data] = [x for x in self.data_collection if x.label == data_label]
 
             viewer.add_data(data, percentile=95, color=viewer.color_cycler())
+            viewer.set_plot_axes()
 
             add_data_message = AddDataMessage(data, viewer,
                                               viewer_id=viewer_id,
                                               sender=self)
             self.hub.broadcast(add_data_message)
 
         # set visibility state of all applicable layers
@@ -1691,19 +1861,16 @@
                 if id != data_id:
                     selected_items[id] = 'hidden'
 
         # Sets the plot axes labels to be the units of the most recently
         # active data.
         viewer_data_labels = [layer.layer.label for layer in viewer.layers]
         if len(viewer_data_labels) > 0 and getattr(self._jdaviz_helper, '_in_batch_load', 0) == 0:
-            active_data = self.data_collection[viewer_data_labels[0]]
-            if (hasattr(active_data, "_preferred_translation")
-                    and active_data._preferred_translation is not None):
-                self._set_plot_axes_labels(viewer_id)
-
+            # This "if" is nested on purpose to make parent "if" available
+            # for other configs in the future, as needed.
             if self.config == 'imviz':
                 viewer.on_limits_change()  # Trigger compass redraw
 
     def vue_data_item_remove(self, event):
         self.data_collection.remove(self.data_collection[event['item_name']])
 
     def vue_close_snackbar_message(self, event):
@@ -1760,14 +1927,21 @@
             The Glue data collection add message containing information about
             the new data.
         """
         for data_item in self.state.data_items:
             if data_item['name'] == msg.data.label:
                 self.state.data_items.remove(data_item)
 
+        # TODO: Fix bug with DataCollectionDeleteMessage not working with
+        #  a handler in cubeviz/plugins/viewers.py. This code is a temporary
+        #  workaround for that.
+        if self.config == 'cubeviz':
+            viewer = self.get_viewer(self._jdaviz_helper._default_spectrum_viewer_reference_name)
+            viewer._check_if_data_removed(msg=msg)
+
         self._clear_object_cache(msg.data.label)
 
     @staticmethod
     def _create_data_item(data):
         ndims = len(data.shape)
         wcsaxes = data.meta.get('WCSAXES', None)
         if wcsaxes is None:
```

### Comparing `jdaviz-3.5.0/jdaviz/app.vue` & `jdaviz-3.6.0/jdaviz/app.vue`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                   <div v-if="trayItemVisible(trayItem, state.tray_items_filter)">
                     <v-expansion-panel-header >
                       <j-tooltip :tipid="trayItem.name">
                         {{ trayItem.label }}
                       </j-tooltip>
                     </v-expansion-panel-header>
                     <v-expansion-panel-content style="margin-left: -12px; margin-right: -12px;">
-                      <jupyter-widget :widget="trayItem.widget"></jupyter-widget>
+                      <jupyter-widget :widget="trayItem.widget" v-if="state.tray_items_open.includes(index)"></jupyter-widget>
                     </v-expansion-panel-content>
                   </div>
                 </v-expansion-panel>
               </v-expansion-panels>
               <v-divider></v-divider>
             </v-card>
           </pane>
```

### Comparing `jdaviz-3.5.0/jdaviz/cli.py` & `jdaviz-3.6.0/jdaviz/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 # Command-line interface for jdaviz
 
+import inspect
 import os
 import pathlib
 import sys
 import tempfile
 
 from voila.app import Voila
 from voila.configuration import VoilaConfiguration
 
 from jdaviz import __version__
 from jdaviz.app import _verbosity_levels
+from jdaviz import configs
 
 __all__ = ['main']
 
+CONFIGS_DIR = str(pathlib.Path(inspect.getfile(configs)).parent)
 JDAVIZ_DIR = pathlib.Path(__file__).parent.resolve()
+DEFAULT_VERBOSITY = 'warning'
+DEFAULT_HISTORY_VERBOSITY = 'info'
+ALL_JDAVIZ_CONFIGS = ['cubeviz', 'specviz', 'specviz2d', 'mosviz', 'imviz']
 
 
 def main(filepaths=None, layout='default', instrument=None, browser='default',
-         theme='light', verbosity='warning', history_verbosity='info',
+         theme='light', verbosity=DEFAULT_VERBOSITY, history_verbosity=DEFAULT_HISTORY_VERBOSITY,
          hotreload=False):
     """
     Start a Jdaviz application instance with data loaded from FILENAME.
 
     Parameters
     ----------
     filepaths : list of str, optional
@@ -54,15 +60,20 @@
         if layout == "imviz":
             # Imviz multiloading should be done all at once for batch processing.
             # Imviz convention is a single string of consecutive, comma-separated file paths
             file_list = [','.join(file_list)]
     else:
         file_list = []
 
-    with open(JDAVIZ_DIR / "jdaviz_cli.ipynb") as f:
+    if len(file_list) == 0 and layout == '':
+        notebook = "jdaviz_cli_launcher.ipynb"
+    else:
+        notebook = "jdaviz_cli.ipynb"
+
+    with open(JDAVIZ_DIR / notebook) as f:
         notebook_template = f.read()
 
     start_dir = os.path.abspath('.')
 
     # Keep track of start directory in environment variable so that it can be
     # easily accessed e.g. in the file load dialog.
     os.environ['JDAVIZ_START_DIR'] = start_dir
@@ -105,16 +116,15 @@
     import argparse
     import sys
 
     parser = argparse.ArgumentParser(description='Start a Jdaviz application instance with data '
                                      'loaded from FILENAME.')
     filepaths_nargs = '*'
     if config is None:
-        parser.add_argument('layout', choices=['cubeviz', 'specviz', 'specviz2d',
-                                               'mosviz', 'imviz'],
+        parser.add_argument('--layout', default='', choices=ALL_JDAVIZ_CONFIGS,
                             help='Configuration to use.')
     if (config == "mosviz") or ("mosviz" in sys.argv):
         filepaths_nargs = 1
     parser.add_argument('filepaths', type=str, nargs=filepaths_nargs, default=None,
                         help='The paths to the files to be loaded into the Jdaviz application.')
     parser.add_argument('--instrument', type=str, default='nirspec',
                         help='Manually specifies which instrument parser to use, for Mosviz')
@@ -140,7 +150,31 @@
         layout = args.layout
     else:
         layout = config
 
     main(filepaths=args.filepaths, layout=layout, instrument=args.instrument, browser=args.browser,
          theme=args.theme, verbosity=args.verbosity, history_verbosity=args.history_verbosity,
          hotreload=args.hotreload)
+
+
+def _specviz():
+    _main(config='specviz')
+
+
+def _specviz2d():
+    _main(config='specviz2d')
+
+
+def _imviz():
+    _main(config='imviz')
+
+
+def _cubeviz():
+    _main(config='cubeviz')
+
+
+def _mosviz():
+    _main(config='mosviz')
+
+
+if __name__ == "__main__":
+    _main()
```

### Comparing `jdaviz-3.5.0/jdaviz/components/docs_link.vue` & `jdaviz-3.6.0/jdaviz/components/docs_link.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/components/glue_state_sync_wrapper.vue` & `jdaviz-3.6.0/jdaviz/components/glue_state_sync_wrapper.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/components/layer_viewer_icon.vue` & `jdaviz-3.6.0/jdaviz/components/layer_viewer_icon.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/components/number_uncertainty.vue` & `jdaviz-3.6.0/jdaviz/components/number_uncertainty.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/components/play_pause_widget.vue` & `jdaviz-3.6.0/jdaviz/components/play_pause_widget.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/components/plugin_add_results.vue` & `jdaviz-3.6.0/jdaviz/components/plugin_add_results.vue`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,32 @@
       :auto="label_auto"
       @update:auto="$emit('update:label_auto', $event)"
       :invalid_msg="label_invalid_msg"
       :label="label_label ? label_label : 'Output Data Label'"
       :hint="label_hint ? label_hint : 'Label for the resulting data item.'"
     ></plugin-auto-label>   
 
-    <plugin-viewer-select v-if="add_to_viewer_items.length > 2"
-      :items="add_to_viewer_items"
-      :selected="add_to_viewer_selected"
-      @update:selected="$emit('update:add_to_viewer_selected', $event)"
-      show_if_single_entry="true"
-      label='Plot in Viewer'
-      :hint="add_to_viewer_hint ? add_to_viewer_hint : 'Plot results in the specified viewer.  Data entry will be available in the data dropdown for all applicable viewers.'"
-    ></plugin-viewer-select>
+    <div v-if="add_to_viewer_items.length > 2">
+      <v-switch v-if="label_overwrite"
+        class="hide-input"
+        label="Show in viewers"
+        :disabled="true"
+        :hint="'Visibility of the modified entry will be adopted from the current \''+label+'\' data entry.'"
+        persistent-hint
+      >
+      </v-switch>
+      <plugin-viewer-select v-else
+        :items="add_to_viewer_items"
+        :selected="add_to_viewer_selected"
+        @update:selected="$emit('update:add_to_viewer_selected', $event)"
+        show_if_single_entry="true"
+        label='Plot in Viewer'
+        :hint="add_to_viewer_hint ? add_to_viewer_hint : 'Plot results in the specified viewer.  Data entry will be available in the data dropdown for all applicable viewers.'"
+      ></plugin-viewer-select>
+    </div>
 
     <v-row v-else>
       <v-switch v-if="label_overwrite"
         class="hide-input"
         :label="'Show in '+add_to_viewer_items[1].label"
         :disabled="true"
         :hint="'Visibility of the modified entry will be adopted from the current \''+label+'\' data entry.'"
@@ -41,15 +51,16 @@
     </v-row>
 
     <slot></slot>
 
     <v-row justify="end">
       <j-tooltip :tooltipcontent="label_overwrite ? action_tooltip+' and replace existing entry' : action_tooltip">
         <v-btn :disabled="label_invalid_msg.length > 0 || action_disabled"
-          color="accent" text
+          text
+          color="accent"
           @click="$emit('click:action')"
         >{{action_label}}{{label_overwrite ? ' (Overwrite)' : ''}}
         </v-btn>
       </j-tooltip>
     </v-row>
   </div>
 </template>
```

### Comparing `jdaviz-3.5.0/jdaviz/components/plugin_auto_label.vue` & `jdaviz-3.6.0/jdaviz/components/plugin_auto_label.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/components/plugin_dataset_select.vue` & `jdaviz-3.6.0/jdaviz/components/plugin_dataset_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/components/plugin_layer_select.vue` & `jdaviz-3.6.0/jdaviz/components/plugin_layer_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/components/plugin_section_header.vue` & `jdaviz-3.6.0/jdaviz/components/plugin_section_header.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/components/plugin_subset_select.vue` & `jdaviz-3.6.0/jdaviz/components/plugin_subset_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/components/plugin_table.vue` & `jdaviz-3.6.0/jdaviz/components/plugin_table.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/components/plugin_viewer_select.vue` & `jdaviz-3.6.0/jdaviz/components/plugin_viewer_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/components/toolbar_nested.vue` & `jdaviz-3.6.0/jdaviz/components/toolbar_nested.vue`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <template>
   <div style="overflow: hidden">
     <v-btn-toggle v-model="active_tool_id" class="transparent">
-        <v-tooltip v-for="[id, {tooltip, img, menu_ind, has_suboptions, primary}] of Object.entries(tools_data)" v-if="primary" bottom>
+        <v-tooltip v-for="[id, {tooltip, img, menu_ind, has_suboptions, primary, visible}] of Object.entries(tools_data)" v-if="primary && visible" bottom>
             <template v-slot:activator="{ on }">
                 <v-btn v-on="on" icon :value="id" style="min-width: 40px !important" @contextmenu="(e) => show_submenu(e, has_suboptions, menu_ind)">
                     <img :src="img" width="20px" @click.ctrl.stop=""/>
                     <v-icon small v-if="has_suboptions" class="suboptions-carrot" @click.ctrl.stop="">mdi-menu-down</v-icon>
                 </v-btn>
             </template>
             <span>{{ tooltip }}{{has_suboptions ? " [right-click for alt. tools]" : ""}}</span>
@@ -18,16 +18,16 @@
       absolute
       offset-y
       dense
       :close-on-click="close_on_click"
     >
       <v-list>
         <v-tooltip
-          v-for="[id, {tooltip, img, menu_ind, has_suboptions, primary}] of Object.entries(tools_data)"
-          v-if="menu_ind==suboptions_ind"
+          v-for="[id, {tooltip, img, menu_ind, has_suboptions, primary, visible}] of Object.entries(tools_data)"
+          v-if="menu_ind==suboptions_ind && visible"
           :key="id"
           left
         >
           <template v-slot:activator="{ on, attrs }">
             <v-list-item v-bind="attrs" v-on="on" :input-value="primary" @click="() => select_primary([menu_ind, id])">
               <v-list-item-title><img class='invert-if-dark' :src="img" width="20"/></v-list-item-title>
             </v-list-item>
```

### Comparing `jdaviz-3.5.0/jdaviz/components/tooltip.vue` & `jdaviz-3.6.0/jdaviz/components/tooltip.vue`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
   'table-next': 'Select next row in table',
   'table-play-pause-toggle': 'Toggle cycling through rows of table',
   'table-play-pause-delay': 'Set delay before cycling to next entry',
   'plugin-plot-options-multiselect-toggle': 'Toggle between simple (single-select) and advanced (multiselect)',
   'plugin-plot-options-mixed-state': 'Current values are mixed, click to sync at shown value',
   'plugin-model-fitting-add-model': 'Create model component',
   'plugin-model-fitting-param-fixed': 'Check the box to freeze parameter value',
-  'plugin-model-fitting-reestimate-all': 'Re-estimate initial values based on the current data/subset selection for all free parameters',
+  'plugin-model-fitting-reestimate-all': 'Re-estimate initial values based on the current data/subset selection for all free parameters based on current display units',
   'plugin-model-fitting-reestimate': 'Re-estimate initial values based on the current data/subset selection for all free parameters in this component',
   'plugin-unit-conversion-apply': 'Apply unit conversion',
   'plugin-line-lists-load': 'Load list into "Loaded Lines" section of plugin',
   'plugin-line-lists-plot-all-in-list': 'Plot all lines in this list',
   'plugin-line-lists-erase-all-in-list': 'Hide all lines in this list',
   'plugin-line-lists-plot-all': 'Plot all lines from every loaded list',
   'plugin-line-lists-erase-all': 'Hide all lines from every loaded list',
```

### Comparing `jdaviz-3.5.0/jdaviz/components/viewer_data_select.vue` & `jdaviz-3.6.0/jdaviz/components/viewer_data_select.vue`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
               {{viewerTitleCase}}
             </span>
 
             <span style="position: absolute; right: 5px">
               <j-tooltip :tipid="multi_select ? 'viewer-data-select-enabled' : 'viewer-data-radio-enabled'">
                 <v-btn
                   icon
-                  @click="() => {multi_select = !multi_select}"
+                  @click="toggleMultiSelect"
                   style="opacity: 0.7"
                   >
                     <img :src="multi_select ? icons.checktoradial : icons.radialtocheck" width="24"/>
                 </v-btn>
               </j-tooltip>
             </span>
         </v-row>
@@ -172,14 +172,32 @@
       // for any situation not covered above, default to showing the entry
       return this.dataItemInViewer(item, returnExtraItems)
     },
     toggleShowExtraItems() {
       // toggle the visibility of the extra items in the menu
       this.showExtraItems = !this.showExtraItems
     },
+    toggleMultiSelect() {
+      this.multi_select = !this.multi_select
+      if (this.multi_select === false){
+        // If we're toggling to single select, set the first item visibility to replace the rest
+        // Find the "first" item
+        for (item_index in this.filteredDataItems){
+          if (this.$props.viewer.selected_data_items[this.filteredDataItems[item_index].id] === 'visible') {
+            this.$emit('data-item-visibility', {
+              id: this.$props.viewer.id,
+              item_id: this.filteredDataItems[item_index].id,
+              visible: true,
+              replace: true})
+            break;
+          }
+        }
+      }
+      
+    },
   },
   computed: {
     viewerTitleCase() {
       var title = this.$props.viewer.reference || this.$props.viewer.id
       // this translates from kebab-case to human readable (individual words, in title case)
       // each word that should NOT be capitalized needs to explicitly be set here
       return title.toLowerCase().replaceAll('-', ' ').split(' ').map((word) => {if (['vs'].indexOf(word) !== -1) {return word} else {return word.charAt(0).toUpperCase() + word.slice(1)}}).join(' ');
```

### Comparing `jdaviz-3.5.0/jdaviz/components/viewer_data_select_item.vue` & `jdaviz-3.6.0/jdaviz/components/viewer_data_select_item.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/cubeviz.yaml` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/cubeviz.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,14 @@
   - g-plot-options
   - g-subset-plugin
   - g-markers
   - cubeviz-slice
   - g-gaussian-smooth
   - g-collapse
   - g-model-fitting
-  - g-unit-conversion
   - g-line-list
   - specviz-line-analysis
   - cubeviz-moment-maps
   - g-export-plot
 viewer_area:
   - container: col
     children:
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/helper.py` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,18 +117,18 @@
         application that is wrapped by Cubeviz.
         """
         if not hasattr(self, '_specviz'):
             self._specviz = Specviz(app=self.app)
         return self._specviz
 
     def get_data(self, data_label=None, spatial_subset=None, spectral_subset=None, function=None,
-                 cls=None):
+                 cls=None, use_display_units=False):
         """
-        Returns data with name equal to data_label of type cls with subsets applied from
-        subset_to_apply.
+        Returns data with name equal to ``data_label`` of type ``cls`` with subsets applied from
+        ``spatial_subset`` and/or ``spectral_subset`` using ``function`` if applicable.
 
         Parameters
         ----------
         data_label : str, optional
             Provide a label to retrieve a specific data set from data_collection.
         spatial_subset : str, optional
             Spatial subset applied to data.
@@ -158,15 +158,16 @@
                                          cls=cls, spatial_subset=spatial_subset, function=function)
         elif function is False and spectral_subset:
             raise ValueError("function cannot be False if spectral_subset"
                              " is set")
         elif function is False:
             function = None
         return self._get_data(data_label=data_label, spatial_subset=spatial_subset,
-                              spectral_subset=spectral_subset, function=function, cls=cls)
+                              spectral_subset=spectral_subset, function=function,
+                              cls=cls, use_display_units=use_display_units)
 
 
 def layer_is_cube_image_data(layer):
     return isinstance(layer, BaseData) and layer.ndim in (2, 3)
 
 
 # TODO: We can remove this when specutils supports it, i.e.,
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py`

 * *Files 10% similar despite different names*

```diff
@@ -133,24 +133,33 @@
         self.overwrite_warn = False
         self._write_moment_to_fits(overwrite=True)
 
     def _write_moment_to_fits(self, overwrite=False, *args):
         if self.moment is None or not self.filename:  # pragma: no cover
             return
 
-        path = Path(self.filename).resolve()
-        if path.exists():
+        # Make sure file does not end up in weird places in standalone mode.
+        path = os.path.dirname(self.filename)
+        if path and not os.path.exists(path):
+            raise ValueError(f"Invalid path={path}")
+        elif (not path or path.startswith("..")) and os.environ.get("JDAVIZ_START_DIR", ""):  # noqa: E501 # pragma: no cover
+            filename = Path(os.environ["JDAVIZ_START_DIR"]) / self.filename
+        else:
+            filename = Path(self.filename).resolve()
+
+        if filename.exists():
             if overwrite:
                 # Try to delete the file
-                path.unlink()
-                if path.exists():
+                filename.unlink()
+                if filename.exists():
                     # Warn the user if the file still exists
-                    raise FileExistsError(f"Unable to delete {path}. Check user permissions.")
+                    raise FileExistsError(f"Unable to delete {filename}. Check user permissions.")
             else:
                 self.overwrite_warn = True
                 return
 
-        self.moment.write(str(path))
+        filename = str(filename)
+        self.moment.write(filename)
 
         # Let the user know where we saved the file.
         self.hub.broadcast(SnackbarMessage(
-            f"Moment map saved to {os.path.abspath(self.filename)}", sender=self, color="success"))
+            f"Moment map saved to {os.path.abspath(filename)}", sender=self, color="success"))
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,7 +127,11 @@
     # Read back in the file and check that it is equal to the one we calculated
     with fits.open(test_file_str) as pf:
         assert_allclose(pf[0].data, moment.data)
         w = WCS(pf[0].header)
         sky = w.pixel_to_world(0, 0)
         assert_allclose(sky.ra.deg, 204.9998877673)
         assert_allclose(sky.dec.deg, 27.0001)
+
+    plugin._obj.filename = "fake_path/test_file.fits"
+    with pytest.raises(ValueError, match="Invalid path"):
+        plugin._obj.vue_save_as_fits()
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/parsers.py` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/slice.py` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/slice.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import threading
 import time
 import warnings
 
 import numpy as np
+import astropy.units as u
 from astropy.units import UnitsWarning
 from glue_jupyter.bqplot.image import BqplotImageView
 from glue_jupyter.bqplot.profile import BqplotProfileView
 from traitlets import Bool, Float, observe, Any, Int
 from specutils.spectra.spectrum1d import Spectrum1D
 
-from jdaviz.core.events import AddDataMessage, SliceToolStateMessage, SliceSelectSliceMessage
+from jdaviz.core.events import (AddDataMessage, SliceToolStateMessage,
+                                SliceSelectSliceMessage, GlobalDisplayUnitChanged)
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import PluginTemplateMixin
 from jdaviz.core.user_api import PluginUserApi
 
 __all__ = ['Slice']
 
 
@@ -79,19 +81,27 @@
         # Listen for add data events. **Note** this should only be used in
         #  cases where there is a specific type of data expected and arbitrary
         #  viewers are not expected to be created. That is, the expected data
         #  in _all_ viewers should be uniform.
         self.session.hub.subscribe(self, AddDataMessage,
                                    handler=self._on_data_added)
 
+        # update internal wavelength when x display unit is changed (preserving slice)
+        self.session.hub.subscribe(self, GlobalDisplayUnitChanged,
+                                   handler=self._on_global_display_unit_changed)
+
     @property
     def user_api(self):
         return PluginUserApi(self, expose=('slice', 'wavelength',
                                            'show_indicator', 'show_wavelength'))
 
+    @property
+    def slice_indicator(self):
+        return self.spectrum_viewer.slice_indicator
+
     def _watch_viewer(self, viewer, watch=True):
         if isinstance(viewer, BqplotImageView):
             if watch and viewer not in self._watched_viewers:
                 self._watched_viewers.append(viewer)
                 viewer.state.add_callback('slices',
                                           self._viewer_slices_changed)
             elif not watch and viewer in self._watched_viewers:
@@ -108,44 +118,46 @@
                 # if the units (or data) change, we need to update internally
                 viewer.state.add_callback("reference_data",
                                           self._update_reference_data)
 
     def _on_data_added(self, msg):
         if isinstance(msg.viewer, BqplotImageView):
             if len(msg.data.shape) == 3:
-                self.max_value = msg.data.shape[-1] - 1
+                self.max_value = msg.data.shape[-1] - 1  # Same as i_end in Export Plot plugin
                 self._watch_viewer(msg.viewer, True)
                 msg.viewer.state.slices = (0, 0, int(self.slice))
 
         elif isinstance(msg.viewer, BqplotProfileView):
             self._watch_viewer(msg.viewer, True)
 
     def _update_reference_data(self, reference_data):
         if reference_data is None:
             return  # pragma: no cover
         self._update_data(reference_data.get_object(cls=Spectrum1D).spectral_axis)
 
     def _update_data(self, x_all):
-        if hasattr(x_all, 'unit'):
-            self.wavelength_unit = str(x_all.unit)
-            x_all = x_all.value
-
-        self._x_all = x_all
+        self._x_all = x_all.value
 
         if self.wavelength == -1:
             if len(x_all):
                 # initialize at middle of cube
                 self.slice = int(len(x_all)/2)
             else:
                 # leave in the pre-init state and don't update the wavelength/slice
                 return
 
+        # Also update unit when data is updated
+        self.wavelength_unit = x_all.unit.to_string()
+
         # force wavelength to update from the current slider value
         self._on_slider_updated({'new': self.slice})
 
+        # update data held inside slice indicator and force reverting to original active status
+        self.slice_indicator._update_data(x_all)
+
     def _viewer_slices_changed(self, value):
         # the slices attribute on the viewer state was changed,
         # so we'll update the slider to match which will trigger
         # the slider observer (_on_slider_updated) and sync across
         # any other applicable viewers
         if len(value) == 3:
             self.slice = float(value[-1])
@@ -153,14 +165,23 @@
     def _on_select_slice_message(self, msg):
         # NOTE: by setting the slice index, the observer (_on_slider_updated)
         # will sync across all viewers and update the wavelength
         with warnings.catch_warnings():
             warnings.simplefilter('ignore', category=UnitsWarning)
             self.slice = msg.slice
 
+    def _on_global_display_unit_changed(self, msg):
+        if msg.axis != 'spectral':
+            return
+        prev_unit = self.wavelength_unit
+        # original unit during init can be blank or deg (before axis is set correctly)
+        if self._x_all is None or prev_unit in ('deg', ''):
+            return
+        self._update_data((self._x_all * u.Unit(prev_unit)).to(msg.unit, u.spectral()))
+
     @observe('wavelength')
     def _on_wavelength_updated(self, event):
         # convert to float (JS handles stripping any invalid characters)
         try:
             value = float(event.get('new'))
         except ValueError:
             # do not accept changes, we'll revert via the slider
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/slice.vue` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/slice.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,36 @@
+import warnings
+
 import pytest
 import numpy as np
 
 from astropy.utils.data import download_file
 
 
-@pytest.mark.filterwarnings('ignore')
 @pytest.mark.remote_data
 def test_data_retrieval(cubeviz_helper):
     """The purpose of this test is to check that both methods:
 
     - app.get_viewer('spectrum-viewer').data()
-    - app.get_data_from_viewer("spectrum-viewer")
+    - cubeviz_helper.get_data()
 
     return the same spectrum values.
     """
     # This file is originally from
     # https://data.sdss.org/sas/dr14/manga/spectro/redux/v2_1_2/7495/stack/manga-7495-12704-LOGCUBE.fits.gz
     URL = 'https://stsci.box.com/shared/static/28a88k1qfipo4yxc4p4d40v4axtlal8y.fits'
 
     spectrum_viewer_reference_name = "spectrum-viewer"
     fn = download_file(URL, cache=True)
-    cubeviz_helper.load_data(fn)
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore")
+        cubeviz_helper.load_data(fn)
 
     # two ways of retrieving data from the viewer.
     # They should return the same spectral values
     a1 = cubeviz_helper.app.get_viewer(spectrum_viewer_reference_name).data()
-    a2 = cubeviz_helper.app.get_data_from_viewer(spectrum_viewer_reference_name)
+    a2 = cubeviz_helper.get_data("contents[FLUX]", function="sum")
 
     test_value_1 = a1[0].data
-    test_value_2 = list(a2.values())[0].data
+    test_value_2 = a2.flux.value
 
     assert np.allclose(test_value_1, test_value_2, atol=1e-5)
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
     dc = cubeviz_helper.app.data_collection
     dc[0].meta["_orig_spec"] = spectrum1d
 
     cubeviz_helper.app.add_data_to_viewer('spectrum-viewer', 'test')
     cubeviz_helper.app.get_viewer('spectrum-viewer').apply_roi(XRangeROI(6600, 7400))
 
-    subsets = cubeviz_helper.app.get_subsets_from_viewer("spectrum-viewer")
+    subsets = cubeviz_helper.app.get_subsets()
     reg = subsets.get('Subset 1')
 
     assert len(subsets) == 1
     assert_allclose(reg.lower.value, 6600.)
     assert_allclose(reg.upper.value, 7400.)
     assert reg.lower.unit == 'Angstrom'
     assert reg.upper.unit == 'Angstrom'
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_regions.py` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_regions.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_tools.py` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,78 +11,78 @@
     flux_viewer = cubeviz_helper.app.get_viewer("flux-viewer")
     spectrum_viewer = cubeviz_helper.app.get_viewer("spectrum-viewer")
 
     # Set the active tool to spectrumperspaxel
     flux_viewer.toolbar.active_tool = flux_viewer.toolbar.tools['jdaviz:spectrumperspaxel']
     x = 1
     y = 1
-    assert len(flux_viewer.figure.marks) == 2
+    assert len(flux_viewer.native_marks) == 2
     assert len(spectrum_viewer.data()) == 1
 
     # Click on spaxel location
     flux_viewer.toolbar.active_tool.on_mouse_event(
         {'event': 'click', 'domain': {'x': x, 'y': y}, 'altKey': False})
-    assert len(flux_viewer.figure.marks) == 3
+    assert len(flux_viewer.native_marks) == 3
     assert len(spectrum_viewer.data()) == 2
 
     # Check that a new subset was created
-    subsets = cubeviz_helper.app.get_subsets_from_viewer('flux-viewer')
-    reg = subsets.get('Subset 1')
+    subsets = cubeviz_helper.app.get_subsets()
+    reg = subsets.get('Subset 1')[0]['region']
     assert len(subsets) == 1
     assert isinstance(reg, RectanglePixelRegion)
 
     # Deselect tool
     flux_viewer.toolbar.active_tool = None
-    assert len(flux_viewer.figure.marks) == 3
+    assert len(flux_viewer.native_marks) == 3
 
 
 def test_spectrum_at_spaxel_altkey_true(cubeviz_helper, spectrum1d_cube):
     cubeviz_helper.load_data(spectrum1d_cube, data_label='test')
 
     flux_viewer = cubeviz_helper.app.get_viewer("flux-viewer")
     uncert_viewer = cubeviz_helper.app.get_viewer("uncert-viewer")
     spectrum_viewer = cubeviz_helper.app.get_viewer("spectrum-viewer")
 
     # Set the active tool to spectrumperspaxel
     flux_viewer.toolbar.active_tool = flux_viewer.toolbar.tools['jdaviz:spectrumperspaxel']
     x = 1
     y = 1
-    assert len(flux_viewer.figure.marks) == 2
+    assert len(flux_viewer.native_marks) == 2
     assert len(spectrum_viewer.data()) == 1
 
     # Check coordinate info panel
     label_mouseover = cubeviz_helper.app.session.application._tools['g-coords-info']
     label_mouseover._viewer_mouse_event(flux_viewer,
                                         {'event': 'mousemove', 'domain': {'x': 1, 'y': 1}})
     assert label_mouseover.as_text() == ('Pixel x=01.0 y=01.0 Value +1.30000e+01 Jy',
                                          'World 13h39m59.9461s +27d00m00.7200s (ICRS)',
                                          '204.9997755344 27.0001999998 (deg)')
 
     # Click on spaxel location
     flux_viewer.toolbar.active_tool.on_mouse_event(
         {'event': 'click', 'domain': {'x': x, 'y': y}, 'altKey': False})
-    assert len(flux_viewer.figure.marks) == 3
+    assert len(flux_viewer.native_marks) == 3
     assert len(spectrum_viewer.data()) == 2
 
     # Check that subset was created
-    subsets = cubeviz_helper.app.get_subsets_from_viewer('flux-viewer')
-    reg = subsets.get('Subset 1')
+    subsets = cubeviz_helper.app.get_subsets()
+    reg = subsets.get('Subset 1')[0]['region']
     assert len(subsets) == 1
     assert isinstance(reg, RectanglePixelRegion)
 
     # Using altKey should create a new subset
     x = 2
     y = 2
     flux_viewer.toolbar.active_tool.on_mouse_event(
         {'event': 'click', 'domain': {'x': x, 'y': y}, 'altKey': True})
-    assert len(flux_viewer.figure.marks) == 4
+    assert len(flux_viewer.native_marks) == 4
     assert len(spectrum_viewer.data()) == 3
 
-    subsets = cubeviz_helper.app.get_subsets_from_viewer('flux-viewer')
-    reg2 = subsets.get('Subset 2')
+    subsets = cubeviz_helper.app.get_subsets()
+    reg2 = subsets.get('Subset 2')[0]['region']
     assert len(subsets) == 2
     assert isinstance(reg2, RectanglePixelRegion)
 
     # Make sure coordinate info panel did not change
     label_mouseover._viewer_mouse_event(flux_viewer,
                                         {'event': 'mousemove', 'domain': {'x': 1, 'y': 1}})
     assert label_mouseover.as_text() == ('Pixel x=01.0 y=01.0 Value +1.30000e+01 Jy',
@@ -114,19 +114,19 @@
     flux_viewer = cubeviz_helper.app.get_viewer("flux-viewer")
     spectrum_viewer = cubeviz_helper.app.get_viewer("spectrum-viewer")
 
     # Set the active tool to spectrumperspaxel
     flux_viewer.toolbar.active_tool = flux_viewer.toolbar.tools['jdaviz:spectrumperspaxel']
     x = 1
     y = 1
-    assert len(flux_viewer.figure.marks) == 2
+    assert len(flux_viewer.native_marks) == 2
     assert len(spectrum_viewer.data()) == 0
 
     # Click on spaxel location
     flux_viewer.toolbar.active_tool.on_mouse_event(
         {'event': 'click', 'domain': {'x': x, 'y': y}, 'altKey': False})
-    assert len(flux_viewer.figure.marks) == 3
+    assert len(flux_viewer.native_marks) == 3
     assert len(spectrum_viewer.data()) == 0
 
     # Deselect tool
     flux_viewer.toolbar.active_tool = None
-    assert len(flux_viewer.figure.marks) == 3
+    assert len(flux_viewer.native_marks) == 3
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tools.py` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/viewers.py` & `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/viewers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from glue.core import BaseData
-from glue.core.subset import RoiSubsetState, RangeSubsetState
+
+from glue.core.subset_group import GroupedSubset
 from glue_jupyter.bqplot.image import BqplotImageView
 
 from jdaviz.core.registries import viewer_registry
 from jdaviz.core.marks import SliceIndicatorMarks, ShadowSpatialSpectral
 from jdaviz.configs.cubeviz.helper import layer_is_cube_image_data
 from jdaviz.configs.default.plugins.viewers import JdavizViewerMixin
 from jdaviz.configs.specviz.plugins.viewers import SpecvizProfileView
+from jdaviz.utils import get_subset_type
+from jdaviz.core.events import AddDataMessage, RemoveDataMessage
 
 __all__ = ['CubevizImageView', 'CubevizProfileView']
 
 
 @viewer_registry("cubeviz-image-viewer", label="Image 2D (Cubeviz)")
 class CubevizImageView(JdavizViewerMixin, BqplotImageView):
     # categories: zoom resets, (zoom, pan), subset, select tools, shortcuts
@@ -94,37 +97,65 @@
                     ['jdaviz:panzoom', 'jdaviz:panzoom_x', 'jdaviz:panzoom_y'],
                     ['bqplot:xrange'],
                     ['jdaviz:selectslice', 'jdaviz:selectline'],
                     ['jdaviz:sidebar_plot', 'jdaviz:sidebar_export']
                 ]
 
     def __init__(self, *args, **kwargs):
-        # NOTE: super will initialize nested toolbar with
-        # default_tool_priority=['jdaviz:selectslice']
+        kwargs.setdefault('default_tool_priority', ['jdaviz:selectslice'])
         super().__init__(*args, **kwargs)
 
         self._default_flux_viewer_reference_name = kwargs.get(
             "flux_viewer_reference_name", "flux-viewer"
         )
+        self.hub.subscribe(self, RemoveDataMessage,
+                           handler=self._check_if_data_removed)
+
+        # TODO: Find out why this is not working
+        # self.hub.subscribe(self, DataCollectionDeleteMessage,
+        #                    handler=self._check_if_data_removed)
+
+        self.hub.subscribe(self, AddDataMessage,
+                           handler=self._check_if_data_added)
+
+    def _check_if_data_removed(self, msg):
+        # isinstance and the data uuid check will be true for the data
+        # that is being removed
+        self.figure.marks = [m for m in self.figure.marks
+                             if not (isinstance(m, ShadowSpatialSpectral)
+                                     and m.data_uuid == msg.data.uuid)]
+
+    def _check_if_data_added(self, msg=None):
+        # When data is added, make sure that all spatial subset layers
+        # that correspond with that data are checked for intersections
+        # with spectral subset layers
+        for layer in self.state.layers:
+            if layer.layer.data.label == msg.data.label:
+                if (isinstance(layer.layer, GroupedSubset) and
+                        get_subset_type(layer.layer.subset_state) == 'spatial'):
+                    self._expected_subset_layer_default(layer)
 
     def _is_spatial_subset(self, layer):
-        # spatial subset layers will have the same data-label as the collapsed flux cube
-        ref_data_label = self.state.reference_data.label
-        return (isinstance(getattr(layer.layer, 'subset_state', None), RoiSubsetState)
-                and layer.layer.data.label == ref_data_label)
+        subset_state = getattr(layer.layer, 'subset_state', None)
+        return get_subset_type(subset_state) == 'spatial'
 
-    def _get_spatial_subset_layers(self):
+    def _get_spatial_subset_layers(self, data_label=None):
+        if data_label:
+            return [ls for ls in self.state.layers if (ls.layer.data.label == data_label and
+                                                       self._is_spatial_subset(ls))]
         return [ls for ls in self.state.layers if self._is_spatial_subset(ls)]
 
     def _is_spectral_subset(self, layer):
-        ref_data_label = self.layers[0].layer.data.label
-        return (isinstance(getattr(layer.layer, 'subset_state', None), RangeSubsetState)
-                and layer.layer.data.label == ref_data_label)
+        subset_state = getattr(layer.layer, 'subset_state', None)
+        return get_subset_type(subset_state) == 'spectral'
 
-    def _get_spectral_subset_layers(self):
+    def _get_spectral_subset_layers(self, data_label=None):
+        if data_label:
+            return [ls for ls in self.state.layers if (ls.layer.data.label == data_label and
+                                                       self._is_spectral_subset(ls))]
         return [ls for ls in self.state.layers if self._is_spectral_subset(ls)]
 
     def _get_marks_for_layers(self, layers):
         layers_list = list(self.state.layers)
         # here we'll assume that all custom marks are subclasses of Lines/GL but don't directly
         # use Lines/LinesGL (so an isinstance check won't be sufficient here)
         layer_marks = self.native_marks
@@ -133,53 +164,89 @@
         # is added but the mark has not yet been created, this will ignore that entry rather than
         # raising an IndexError.
         inds = [layers_list.index(layer) for layer in layers]
         return [layer_marks[ind] for ind in inds if ind < len(layer_marks)]
 
     def _on_subset_delete(self, msg):
         # delete any ShadowSpatialSpectral mark for which either of the spectral or spatial marks
-        # no longer exists
-        spectral_marks = self._get_marks_for_layers(self._get_spectral_subset_layers())
-        spatial_marks = self._get_marks_for_layers(self._get_spatial_subset_layers())
+        # no longer exists by matching the uuid of the msg subset to the uuid of the subsets
+        # in ShadowSpatialSpectral
         self.figure.marks = [m for m in self.figure.marks
-                             if not (isinstance(m, ShadowSpatialSpectral) and
-                                     (m.spatial_spectrum_mark in spatial_marks or
-                                      m.spectral_subset_mark in spectral_marks))]
+                             if not (isinstance(m, ShadowSpatialSpectral)
+                                     and msg.subset.uuid in [m.spatial_uuid, m.spectral_uuid])]
 
     def _expected_subset_layer_default(self, layer_state):
         """
         This gets called whenever the layer of an expected new subset is added, we want to set the
         default for the linewidth depending on whether it is spatial or spectral, and handle
         creating any necessary marks for spatial-spectral subset intersections.
         """
-        super()._expected_subset_layer_default(layer_state)
+        def _marks_are_same(m, other):
+            # Check if ShadowSpatialSpectral mark already exists for particular
+            # data, spatial subset, and spectral subset combo
+            if (m.data_uuid == other.data_uuid
+                and m.spatial_uuid == other.spatial_uuid
+                    and m.spectral_uuid == other.spectral_uuid):
+                return True
+            return False
+
+        def _is_unique(m):
+            unique = True
+            for m in existing_shadows_for_data:
+                if _marks_are_same(m, new_shadow):
+                    unique = False
+                    break
+            return unique
 
-        if not (self._is_spatial_subset(layer_state) or self._is_spectral_subset(layer_state)):
+        super()._expected_subset_layer_default(layer_state)
+        subset_type = get_subset_type(layer_state.layer)
+        if subset_type is None:
             return
 
         this_mark = self._get_marks_for_layers([layer_state])[0]
-
+        # new ShadowSpatialSpectral marks to be added
         new_marks = []
-
-        if isinstance(layer_state.layer.subset_state, RoiSubsetState):
+        # ShadowSpatialSpectral marks that already exists in the viewer
+        existing_shadows_for_data = [m for m in self.figure.marks
+                                     if isinstance(m, ShadowSpatialSpectral)]
+        if subset_type == 'spatial':
             layer_state.linewidth = 1
 
             # need to add marks for every intersection between THIS spatial subset and ALL spectral
-            spectral_marks = self._get_marks_for_layers(self._get_spectral_subset_layers())
-            for spectral_mark in spectral_marks:
-                new_marks += [ShadowSpatialSpectral(this_mark, spectral_mark)]
-
-        else:
-            layer_state.linewidth = 3
+            # subset marks corresponding to this data
+            spectral_layers = [sub_layer for sub_layer in
+                               self._get_spectral_subset_layers(layer_state.layer.data.label)]
+            spectral_marks = self._get_marks_for_layers(spectral_layers)
+
+            for index, spectral_mark in enumerate(spectral_marks):
+                new_shadow = ShadowSpatialSpectral(spatial_spectrum_mark=this_mark,
+                                                   spectral_subset_mark=spectral_mark,
+                                                   spatial_uuid=layer_state.layer.uuid,
+                                                   spectral_uuid=spectral_layers[index].layer.uuid,
+                                                   data_uuid=layer_state.layer.data.uuid)
+                if _is_unique(new_shadow):
+                    new_marks.append(new_shadow)
 
+        elif subset_type == 'spectral':
             # need to add marks for every intersection between THIS spectral subset and ALL spatial
-            spatial_marks = self._get_marks_for_layers(self._get_spatial_subset_layers())
-            for spatial_mark in spatial_marks:
-                new_marks += [ShadowSpatialSpectral(spatial_mark, this_mark)]
+            # subset marks corresponding to this data
+            spatial_layers = [sub_layer for sub_layer in
+                              self._get_spatial_subset_layers(layer_state.layer.data.label)]
+            spatial_marks = self._get_marks_for_layers(spatial_layers)
+            for index, spatial_mark in enumerate(spatial_marks):
+                new_shadow = ShadowSpatialSpectral(spatial_spectrum_mark=spatial_mark,
+                                                   spectral_subset_mark=this_mark,
+                                                   spatial_uuid=spatial_layers[index].layer.uuid,
+                                                   spectral_uuid=layer_state.layer.uuid,
+                                                   data_uuid=layer_state.layer.data.uuid)
+                if _is_unique(new_shadow):
+                    new_marks.append(new_shadow)
 
+        else:
+            return
         # NOTE: += or append won't pick up on change
         self.figure.marks = self.figure.marks + new_marks
 
     @property
     def slice_indicator(self):
         for mark in self.figure.marks:
             if isinstance(mark, SliceIndicatorMarks):
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/__init__.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/collapse.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/collapse.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/collapse.vue` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/collapse.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/data_tools.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/data_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/data_tools.vue` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/data_tools.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/file_chooser.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/file_chooser.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,19 +62,21 @@
             # retrieve the data from the cube, not the collapsed 1d spectrum
             self.dataset._viewers = [
                 self._default_flux_viewer_reference_name,
                 self._default_spectrum_viewer_reference_name
             ]
             # clear the cache in case the spectrum-viewer selection was already cached
             self.dataset._clear_cache()
-        elif self.config == "mosviz":
+        elif self.config in ("mosviz", "specviz2d"):
             # only allow smoothing 1d spectra
             self.dataset._viewers = [self._default_spectrum_viewer_reference_name]
             self.dataset._clear_cache()
 
+        self.dataset.add_filter('not_from_this_plugin')
+
         self.mode = SelectPluginComponent(self,
                                           items='mode_items',
                                           selected='mode_selected',
                                           manual_options=['Spectral', 'Spatial'])
 
         # set the filter on the viewer options
         self._update_viewer_filters()
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     gs.add_to_viewer_selected = 'spectrum-viewer'
     gs.vue_apply()
 
     # FOR HISTORICAL CONTEXT:
     # The data label used to be prepended to the results_label ONLY if there were multiple
     # smoothed spectra. As of PR#1973, POs requested the data label to always be present.
     # As a result, label will overwrite here
-    assert len(gs.dataset_items) == 2
+    assert len(gs.dataset_items) == 1
     assert gs.dataset_selected == f'{data_label}[FLUX]'
     assert gs.results_label == f'{data_label}[FLUX] spectral-smooth stddev-3.2'
     assert gs.results_label_overwrite is True
 
     assert len(dc) == 2
     assert dc[1].label == f'{data_label}[FLUX] spectral-smooth stddev-3.2'
     assert len(dc.external_links) == 3
@@ -116,15 +116,15 @@
     assert dc[1].label == f'{data_label}[FLUX] spatial-smooth stddev-3.0'
     assert dc[1].shape == (2, 4, 2)  # specutils moved spectral axis to last
     assert (dc[f'{data_label}[FLUX] spatial-smooth stddev-3.0'].get_object(cls=Spectrum1D,
                                                                            statistic=None).shape
             == (2, 4, 2))
 
 
-def test_spectrum1d_smooth(specviz_helper, spectrum1d):
+def test_specviz_smooth(specviz_helper, spectrum1d):
     data_label = 'test'
     dc = specviz_helper.app.data_collection
     specviz_helper.load_data(spectrum1d, data_label=data_label)
     spec_viewer = specviz_helper.app.get_viewer('spectrum-viewer')
 
     gs = specviz_helper.plugins['Gaussian Smooth']._obj
     gs.dataset_selected = data_label
@@ -156,32 +156,34 @@
     # Out-of-bounds shows only cursor info.
     label_mouseover._viewer_mouse_event(spec_viewer,
                                         {'event': 'mousemove', 'domain': {'x': 5500, 'y': 120}})
     assert label_mouseover.as_text() == ('Cursor 5.50000e+03, 1.20000e+02', '', '')
     assert label_mouseover.icon == 'mdi-cursor-default'
 
 
-def test_spectrum2d_smooth(specviz2d_helper, spectrum2d):
+def test_specviz2d_smooth(specviz2d_helper, spectrum2d):
     data_label = 'test'
     dc = specviz2d_helper.app.data_collection
     specviz2d_helper.load_data(spectrum_2d=spectrum2d, spectrum_2d_label=data_label)
 
     gs_plugin = specviz2d_helper.plugins['Gaussian Smooth']
 
     # The Autocollapsed spectrum is given the label of "Spectrum 1D by default"
     smooth_source_dataset = "Spectrum 1D"
     gs_plugin.dataset = smooth_source_dataset
-    test_stddev_level = 100.0
+    test_stddev_level = 10.0
     gs_plugin.stddev = test_stddev_level
-    gs_plugin.smooth()
+    smoothed_spectrum = gs_plugin.smooth(add_data=True)
 
     assert len(dc) == 3
     assert dc[2].label == f'{smooth_source_dataset} smooth stddev-{test_stddev_level}'
+    np.testing.assert_allclose(smoothed_spectrum.spectral_axis.value,
+                               spectrum2d.spectral_axis.value)
 
     # Ensure all marks were created properly (i.e. not in their initialized state)
     # [0,1] is the default (initialization) value for the marks
     marks = specviz2d_helper.app.get_viewer('spectrum-viewer').native_marks
-
     assert len(marks) == 2
-    for mark in marks:
-        np.testing.assert_allclose(mark.x, spectrum2d.spectral_axis.value)
-        assert not np.array_equal(mark.y, [0, 1])
+
+    gp_mark = marks[-1]
+    np.testing.assert_allclose(gp_mark.x, smoothed_spectrum.spectral_axis.value)
+    np.testing.assert_allclose(gp_mark.y, smoothed_spectrum.flux.value)
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/line_lists.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/line_lists.py`

 * *Files 5% similar despite different names*

```diff
@@ -195,15 +195,16 @@
         if viewer_data.meta.get('plugin', None) is not None:
             self.rs_redshift = (viewer_data.redshift.value
                                 if hasattr(viewer_data.redshift, 'value')
                                 else viewer_data.redshift)
         self._on_spectrum_viewer_limits_changed()  # will also trigger _auto_slider_step
 
         # set the choices (and default) for the units for new custom lines
-        self.custom_unit_choices = create_spectral_equivalencies_list(viewer_data)
+        self.custom_unit_choices = create_spectral_equivalencies_list(
+            viewer_data.spectral_axis.unit)
         self.custom_unit = str(viewer_data.spectral_axis.unit)
 
     def _parse_redshift_msg(self, msg):
         '''
         Handle incoming redshift messages from the app hub. Generally these
         will be created by Specviz helper methods.
         '''
@@ -317,35 +318,29 @@
             self._update_line_list_obs()
 
             # Send the redshift back to the Specviz helper (and also trigger
             # self._update_global_redshift)
             msg = RedshiftMessage("redshift", value, sender=self)
             self.app.hub.broadcast(msg)
 
-    @observe('plugin_opened')
     def _update_line_list_obs(self, *args):
-        if not self.plugin_opened:
-            return
-
-        new_list_contents = {}
         for list_name, line_list in self.list_contents.items():
             for i, line in enumerate(line_list['lines']):
                 if self._rs_line_obs_change[0] == list_name and self._rs_line_obs_change[1] == i:  # noqa
                     # this trigger is coming from a manual change to the observed
                     # wavelength and would result in a small change to the value before the
                     # user can finish typing.  So we'll just keep the old value until the
                     # widget is blurred (loses focus)
                     line_list['lines'][i]['obs'] = self._rs_line_obs_change[2]
                 else:
                     line_list['lines'][i]['obs'] = self._rest_to_obs(float(line['rest']))
 
-            new_list_contents[list_name] = line_list
+            self.list_contents[list_name] = line_list
 
-        self.list_contents = {}
-        self.list_contents = new_list_contents
+        self.send_state('list_contents')
 
     def vue_change_line_obs(self, kwargs):
         # NOTE: we can only pass one argument from vue (it seems), so we'll pass as
         # a dictionary (kwargs) instead of positional or keyword arguments (**kwargs)
         line_obs = kwargs.get('obs_new')
         if isinstance(line_obs, str) and not len(line_obs):
             # empty string, we don't want to revert yet because then
@@ -406,14 +401,16 @@
         self._rs_pause_tables = False
         # the redshift value in the MOS table and observed wavelengths weren't
         # updating during slide, so update them now
         self.vue_unpause_tables()
 
     def _on_spectrum_viewer_limits_changed(self, event=None):
         sv = self.app.get_viewer(self._default_spectrum_viewer_reference_name)
+        if sv.state.x_min is None or sv.state.x_max is None:
+            return
         self.spectrum_viewer_min = float(sv.state.x_min)
         self.spectrum_viewer_max = float(sv.state.x_max)
 
         # Also update the slider range
         self._auto_slider_range()
 
     def _auto_slider_range(self, event=None):
@@ -506,18 +503,16 @@
                          "unit": str(row["rest"].unit),
                          "colors": row["colors"] if "colors" in row else "#FF0000FF",
                          "show": row["show"],
                          "name_rest": row["name_rest"]}
             list_contents[row["listname"]]["lines"].append(temp_dict)
             tmp_names_rest.append(row["name_rest"])
 
-        self.loaded_lists = []
-        self.loaded_lists = loaded_lists
-        self.list_contents = {}
-        self.list_contents = list_contents
+        self.send_state('loaded_lists')
+        self.send_state('list_contents')
 
         self._viewer.plot_spectral_lines(tmp_names_rest)
         self.update_line_mark_dict()
 
         msg_text = ("Spectral lines loaded from notebook. Lines can be hidden"
                     "/shown in the Line Lists plugin")
         lines_loaded_message = SnackbarMessage(msg_text, sender=self,
@@ -647,74 +642,68 @@
         """
         Toggle all lines in list to be visible
         """
         lc = self.list_contents
         for line in lc[listname]["lines"]:
             line["show"] = True
             self._viewer.spectral_lines.loc[line["name_rest"]]["show"] = True
-        # Trick traitlets into updating
-        self.list_contents = {}
+
         self.list_contents = lc
+        self.send_state('list_contents')
 
         self._viewer.plot_spectral_lines()
         self.update_line_mark_dict()
 
     def vue_hide_all_in_list(self, listname):
         """
         Toggle all lines in list to be hidden
         """
-        lc = self.list_contents
         name_rests = []
-        for line in lc[listname]["lines"]:
+        for line in self.list_contents[listname]["lines"]:
             line["show"] = False
             name_rests.append(line["name_rest"])
-        # Trick traitlets into updating
-        self.list_contents = {}
-        self.list_contents = lc
+
+        self.send_state('list_contents')
 
         self._viewer.erase_spectral_lines(name_rest=name_rests)
         self.update_line_mark_dict()
 
     def vue_plot_all_lines(self, event):
         """
         Plot all the currently loaded lines in the viewer
         """
         if self._viewer.spectral_lines is None:
             warn_message = SnackbarMessage("No spectral lines loaded to plot",
                                            sender=self, color="error")
             self.hub.broadcast(warn_message)
             return
-        lc = self.list_contents
-        for listname in lc:
-            for line in lc[listname]["lines"]:
+        for listname in self.list_contents:
+            for line in self.list_contents[listname]["lines"]:
                 line["show"] = True
         self._viewer.spectral_lines["show"] = True
-        # Trick traitlets into updating
-        self.list_contents = {}
-        self.list_contents = lc
+
+        self.send_state('list_contents')
 
         self._viewer.plot_spectral_lines()
         self.update_line_mark_dict()
 
     def vue_erase_all_lines(self, event):
         """
         Erase all lines from the viewer
         """
         if self._viewer.spectral_lines is None:
             warn_message = SnackbarMessage("No spectral lines to erase",
                                            sender=self, color="error")
             self.hub.broadcast(warn_message)
             return
-        lc = self.list_contents
-        for listname in lc:
-            for line in lc[listname]["lines"]:
+        for listname in self.list_contents:
+            for line in self.list_contents[listname]["lines"]:
                 line["show"] = False
-        # Trick traitlets into updating
-        self.list_contents = {}
-        self.list_contents = lc
+
+        self.send_state('list_contents')
 
         self._viewer.erase_spectral_lines()
         self.update_line_mark_dict()
 
     def vue_change_visible(self, data):
         """
         Plot or erase a single line as needed when "Visible" checkbox is changed
@@ -791,28 +780,27 @@
         """
         Change the color either of all members of a line list, or of an
         individual line.
         """
         color = data['color']
         if "listname" in data:
             listname = data["listname"]
-            # force a copy so that the change is picked up by traitlets
-            lc = self.list_contents[listname].copy()
-            lc["color"] = color
 
-            for line in lc["lines"]:
+            self.list_contents[listname]["color"] = color
+
+            for line in self.list_contents[listname]["lines"]:
                 line["colors"] = color
                 # Update the astropy table entry
                 name_rest = line["name_rest"]
                 self._viewer.spectral_lines.loc[name_rest]["colors"] = color
                 # Update the color on the plot
                 if name_rest in self.line_mark_dict:
                     self.line_mark_dict[name_rest].colors = [color]
 
-            self.list_contents = {**self.list_contents, listname: lc}
+            self.send_state('list_contents')
 
         elif "linename" in data:
             pass
 
     def vue_remove_list(self, listname):
         """
         Method to remove line list from available expansion panels when the x
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/line_lists.vue` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/line_lists.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from jdaviz.core.linelists import get_available_linelists
 
 
 def test_line_lists(specviz_helper):
     spec = Spectrum1D(flux=np.random.rand(100)*u.Jy,
                       spectral_axis=np.arange(6000, 7000, 10)*u.AA)
-    specviz_helper.load_spectrum(spec)
+    specviz_helper.load_data(spec)
 
     lt = QTable()
     lt['linename'] = ['O III', 'Halpha']
     lt['rest'] = [0, 6563]*u.AA
     with pytest.raises(ValueError, match='all rest values must be positive'):
         specviz_helper.load_line_list(lt)
 
@@ -43,32 +43,31 @@
         specviz_helper.plugins["Line Lists"]._obj.list_contents["Custom"]["medium"]
         == "Unknown (Custom)"
     )
 
 
 def test_redshift(specviz_helper, spectrum1d):
     # Also test that plugin is disabled before data is loaded.
-    plg = specviz_helper.plugins['Line Lists']
-    assert plg._obj.disabled_msg
+    ll_plugin = specviz_helper.plugins['Line Lists']._obj
+    assert ll_plugin.disabled_msg
 
     label = "Test 1D Spectrum"
-    specviz_helper.load_spectrum(spectrum1d, data_label=label)
+    specviz_helper.load_data(spectrum1d, data_label=label)
 
-    assert not plg._obj.disabled_msg
+    assert not ll_plugin.disabled_msg
 
     lt = QTable()
     lt['linename'] = ['O III', 'Halpha']
     lt['rest'] = [5007, 6563]*u.AA
     lt['redshift'] = u.Quantity(0.046)
     lt['listname'] = 'Test List'
     with pytest.warns(UserWarning, match='per line/list redshifts not supported, use viz.set_redshift'):  # noqa
         specviz_helper.load_line_list(lt)
 
-    ll_plugin = specviz_helper.app.get_tray_item_from_name('g-line-list')
-    # fake the plugin to be opened so that all updates run
+    # open the plugin so that all updates run
     ll_plugin.plugin_opened = True
     line = ll_plugin.list_contents['Test List']['lines'][0]
     assert_allclose(line['obs'], line['rest'])
     # test API access
     specviz_helper.set_redshift(0.01)
     specviz_helper.set_redshift_slider_bounds(range=0.5, step=0.01)
     specviz_helper.set_redshift_slider_bounds(range='auto', step='auto')
@@ -98,15 +97,15 @@
     assert ll_plugin._viewer.spectral_lines is None
     assert ll_plugin.identify_label == ''
 
 
 def test_load_available_preset_lists(specviz_helper, spectrum1d):
     """ Loads all available line lists and checks the medium requirement """
     label = "Test 1D Spectrum"
-    specviz_helper.load_spectrum(spectrum1d, data_label=label)
+    specviz_helper.load_data(spectrum1d, data_label=label)
 
     # Check to make sure we got our line lists
     available_linelists = get_available_linelists()
     assert len(available_linelists) > 0
 
     for linelist in available_linelists:
         specviz_helper.plugins['Line Lists']._obj.vue_list_selected(linelist)
@@ -121,15 +120,15 @@
     # Line list must have "medium" info to be available
     for list in specviz_helper.plugins['Line Lists']._obj.list_contents.values():  # noqa
         assert 'medium' in list
 
 
 def test_line_identify(specviz_helper, spectrum1d):
     label = "Test 1D Spectrum"
-    specviz_helper.load_spectrum(spectrum1d, data_label=label)
+    specviz_helper.load_data(spectrum1d, data_label=label)
 
     lt = QTable()
     lt['linename'] = ['O III', 'Halpha']
     lt['rest'] = [5007, 6563]*u.AA
     lt['listname'] = 'Test List'
     specviz_helper.load_line_list(lt)
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/markers.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/markers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from traitlets import observe
+from traitlets import Bool, observe
 
 from jdaviz.core.events import ViewerAddedMessage
 from jdaviz.core.marks import MarkersMark
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import PluginTemplateMixin, ViewerSelectMixin, TableMixin
 from jdaviz.core.user_api import PluginUserApi
 
@@ -20,14 +20,15 @@
 
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.show`
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.open_in_tray`
     * :meth:`clear_table`
     * :meth:`~jdaviz.core.template_mixin.TableMixin.export_table`
     """
     template_file = __file__, "markers.vue"
+    uses_active_status = Bool(True).tag(sync=True)
 
     _default_table_values = {'spectral_axis': np.nan,
                              'spectral_axis:unit': '',
                              'slice': np.nan,
                              'pixel': (np.nan, np.nan),
                              'pixel:unreliable': None,
                              'world': (np.nan, np.nan),
@@ -75,15 +76,15 @@
         self.table.headers_visible = headers
         self.table._default_values_by_colname = self._default_table_values
 
         # subscribe to mouse events on any new viewers
         self.hub.subscribe(self, ViewerAddedMessage, handler=self._on_viewer_added)
 
     def _create_viewer_callbacks(self, viewer):
-        if not self.plugin_opened:
+        if not self.is_active:
             return
 
         callback = self._viewer_callback(viewer, self._on_viewer_key_event)
         viewer.add_event_callback(callback, events=['keydown'])
 
     def _on_viewer_added(self, msg):
         self._create_viewer_callbacks(self.app.get_viewer_by_id(msg.viewer_id))
@@ -102,31 +103,31 @@
                 for viewer_id, viewer in self.app._viewer_store.items()
                 if hasattr(viewer, 'figure')}
 
     @property
     def coords_info(self):
         return self.app.session.application._tools['g-coords-info']
 
-    @observe('plugin_opened')
-    def _on_plugin_opened_changed(self, *args):
+    @observe('is_active')
+    def _on_is_active_changed(self, *args):
         if self.disabled_msg:
             return
 
         # toggle visibility of markers
         for mark in self.marks.values():
-            mark.visible = self.plugin_opened
+            mark.visible = self.is_active
 
         # subscribe/unsubscribe to keypress events across all viewers
         for viewer in self.app._viewer_store.values():
             if not hasattr(viewer, 'figure'):
                 # table viewer, etc
                 continue
             callback = self._viewer_callback(viewer, self._on_viewer_key_event)
 
-            if self.plugin_opened:
+            if self.is_active:
                 viewer.add_event_callback(callback, events=['keydown'])
             else:
                 viewer.remove_event_callback(callback)
 
     def _on_viewer_key_event(self, viewer, data):
         if data['event'] == 'keydown' and data['key'] == 'm':
             row_info = self.coords_info.as_dict()
@@ -140,15 +141,14 @@
             try:
                 self.table.add_item({k: v for k, v in row_info.items()
                                      if k in self.table.headers_avail})
             except ValueError as err:
                 raise ValueError(f'failed to add {row_info} to table: {repr(err)}')
 
             x, y = row_info['axes_x'], row_info['axes_y']
-            # TODO: will need to test/update when adding support for display units
             self._get_mark(viewer).append_xy(getattr(x, 'value', x), getattr(y, 'value', y))
 
     def clear_table(self):
         """
         Clear all entries/markers from the current table.
         """
         super().clear_table()
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     cubeviz_helper.load_data(spectrum1d_cube, "test")
     fv = cubeviz_helper.app.get_viewer('flux-viewer')
     sv = cubeviz_helper.app.get_viewer('spectrum-viewer')
 
     label_mouseover = cubeviz_helper.app.session.application._tools['g-coords-info']
 
     mp = cubeviz_helper.plugins['Markers']
-    mp.open_in_tray()
+    mp.keep_active = True
 
     # test event in flux viewer
     label_mouseover._viewer_mouse_event(fv,
                                         {'event': 'mousemove',
                                          'domain': {'x': 0, 'y': 0}})
 
     assert label_mouseover.as_text() == ('Pixel x=00.0 y=00.0 Value +8.00000e+00 Jy',
@@ -108,21 +108,21 @@
 
     mp._obj._on_viewer_key_event(sv, {'event': 'keydown',
                                       'key': 'm'})
     assert len(mp.export_table()) == 3
     assert len(_get_markers_from_viewer(fv).x) == 1
     assert len(_get_markers_from_viewer(sv).x) == 2
 
-    # markers hide when plugin closed
-    cubeviz_helper.app.state.drawer = False
+    # markers hide when plugin closed and keep_active = False
+    mp.keep_active = False
     assert _get_markers_from_viewer(fv).visible is False
     assert _get_markers_from_viewer(sv).visible is False
 
     # markers re-appear when plugin re-opened
-    mp.open_in_tray()
+    mp._obj.plugin_opened = True
     assert _get_markers_from_viewer(fv).visible is True
     assert _get_markers_from_viewer(sv).visible is True
     assert len(_get_markers_from_viewer(fv).x) == 1
     assert len(_get_markers_from_viewer(sv).x) == 2
 
     # clearing table clears markers
     mp.clear_table()
@@ -132,15 +132,15 @@
 
 
 class TestImvizMultiLayer(BaseImviz_WCS_NoWCS):
     def test_markers_layer_cycle(self):
         label_mouseover = self.imviz.app.session.application._tools['g-coords-info']
 
         mp = self.imviz.plugins['Markers']
-        mp.open_in_tray()
+        mp.plugin_opened = True
 
         # cycle through dataset options (used for both coords info and markers)
         assert label_mouseover.dataset.choices == ['auto', 'none',
                                                    'has_wcs[SCI,1]',
                                                    'no_wcs[SCI,1]']
         assert label_mouseover.dataset.selected == 'auto'
 
@@ -213,15 +213,15 @@
                                                    'key': 'm'})
         assert len(_get_markers_from_viewer(self.viewer).x) == 3
 
     def test_markers_custom_viewer(self):
         label_mouseover = self.imviz.app.session.application._tools['g-coords-info']
 
         mp = self.imviz.plugins['Markers']
-        mp.open_in_tray()
+        mp.plugin_opened = True
 
         nv = self.imviz.create_image_viewer()
         self.imviz.app.add_data_to_viewer('imviz-1', 'has_wcs[SCI,1]')
 
         assert label_mouseover.dataset.choices == ['auto', 'none',
                                                    'has_wcs[SCI,1]',
                                                    'no_wcs[SCI,1]']
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/initializers.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/initializers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import astropy.units as u
 from specutils import Spectrum1D
 from specutils.utils import QuantityModel
 from traitlets import Bool, List, Unicode, observe
 from glue.core.data import Data
 
-from jdaviz.core.events import SnackbarMessage
+from jdaviz.core.events import SnackbarMessage, GlobalDisplayUnitChanged
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import (PluginTemplateMixin,
                                         SelectPluginComponent,
                                         SpectralSubsetSelectMixin,
                                         SubsetSelect,
                                         DatasetSelectMixin,
                                         DatasetSpectralSubsetValidMixin,
@@ -56,14 +56,15 @@
     * ``spectral_subset`` (:class:`~jdaviz.core.template_mixin.SubsetSelect`)
     * ``model_component`` (:class:`~jdaviz.core.template_mixin.SelectPluginComponent`)
     * ``poly_order``
     * ``model_component_label`` (:class:`~jdaviz.core.template_mixin.AutoTextField`)
     * :meth:`create_model_component`
     * :meth:`remove_model_component`
     * :meth:`model_components`
+    * :meth:`valid_model_components`
     * :meth:`get_model_component`
     * :meth:`set_model_component`
     * :meth:`reestimate_model_parameters`
     * ``equation`` (:class:`~jdaviz.core.template_mixin.AutoTextField`)
     * :meth:`equation_components`
     * ``cube_fit``
       Only exposed for Cubeviz.  Whether to fit the model to the cube instead of to the
@@ -127,15 +128,15 @@
         self._initialized_models = {}
         self._display_order = False
         if self.config == "cubeviz":
             self.spatial_subset = SubsetSelect(self,
                                                'spatial_subset_items',
                                                'spatial_subset_selected',
                                                default_text='Entire Cube',
-                                               allowed_type='spatial')
+                                               filters=['is_spatial'])
         else:
             self.spatial_subset = None
 
         # create the label first so that when model_component defaults to the first selection,
         # the label automatically defaults as well
         self.model_component_label = AutoTextField(self, 'comp_label', 'comp_label_default',
                                                    'comp_label_auto', 'comp_label_invalid_msg')
@@ -165,21 +166,25 @@
         # when model parameters are added as columns, only show the value columns by default
         # (other columns can be show in the dropdown by the user)
         self.table._new_col_visible = lambda colname: colname.split(':')[-1] not in ('unit', 'fixed', 'uncert', 'std')  # noqa
 
         # set the filter on the viewer options
         self._update_viewer_filters()
 
+        self.hub.subscribe(self, GlobalDisplayUnitChanged,
+                           handler=self._on_global_display_unit_changed)
+
     @property
     def user_api(self):
         expose = ['dataset']
         if self.config == "cubeviz":
             expose += ['spatial_subset']
         expose += ['spectral_subset', 'model_component', 'poly_order', 'model_component_label',
-                   'model_components', 'create_model_component', 'remove_model_component',
+                   'model_components', 'valid_model_components',
+                   'create_model_component', 'remove_model_component',
                    'get_model_component', 'set_model_component', 'reestimate_model_parameters',
                    'equation', 'equation_components',
                    'add_results', 'residuals_calculate', 'residuals']
         if self.config == "cubeviz":
             expose += ['cube_fit']
         expose += ['calculate_fit', 'clear_table', 'export_table']
         return PluginUserApi(self, expose=expose)
@@ -232,18 +237,15 @@
                     if std_name in self._fitted_model.stds.param_names:
                         temp_param[0]["std"] = self._fitted_model.stds[std_name]
 
                 temp_params += temp_param
 
             m["parameters"] = temp_params
 
-        # Trick traitlets into updating the displayed values
-        component_models = self.component_models
-        self.component_models = []
-        self.component_models = component_models
+        self.send_state('component_models')
 
     def _update_parameters_from_QM(self):
         """
         Parse out result parameters from a QuantityModel, which isn't
         subscriptable with model name
         """
         if hasattr(self._fitted_model, "submodel_names"):
@@ -274,18 +276,15 @@
                 else:
                     temp_param = [x for x in m["parameters"] if x["name"] ==
                                   param_names[idx]]
                 temp_param[0]["value"] = fit_params[idx]
                 temp_params += temp_param
             m["parameters"] = temp_params
 
-        # Trick traitlets into updating the displayed values
-        component_models = self.component_models
-        self.component_models = []
-        self.component_models = component_models
+        self.send_state('component_models')
 
     def _update_initialized_parameters(self):
         # If the user changes a parameter value, we need to change it in the
         # initialized model
         for m in self.component_models:
             name = m["id"]
             for param in m["parameters"]:
@@ -332,14 +331,15 @@
         if selected_spec is None:
             return
 
         # Replace NaNs from collapsed Spectrum1D in Cubeviz
         # (won't affect calculations because these locations are masked)
         selected_spec.flux[np.isnan(selected_spec.flux)] = 0.0
 
+        # TODO: can we simplify this logic?
         self._units["x"] = str(
             selected_spec.spectral_axis.unit)
         self._units["y"] = str(
             selected_spec.flux.unit)
 
     def _default_comp_label(self, model, poly_order=None):
         abbrevs = {'BlackBody': 'BB', 'PowerLaw': 'PL', 'Lorentz1D': 'Lo'}
@@ -499,16 +499,46 @@
                                             "value": param_quant.value,
                                             "unit": str(param_quant.unit),
                                             "fixed": False})
 
         self._initialized_models[comp_label] = initialized_model
 
         new_model["Initialized"] = True
+        new_model["initialized_display_units"] = self._units.copy()
+
+        new_model["compat_display_units"] = True  # always compatible at time of creation
         return new_model
 
+    def _check_model_component_compat(self, axes=['x', 'y'], display_units=None):
+        if display_units is None:
+            display_units = [u.Unit(self._units[ax]) for ax in axes]
+
+        disp_physical_types = [unit.physical_type for unit in display_units]
+
+        for model_index, comp_model in enumerate(self.component_models):
+            compat = True
+            for ax, ax_physical_type in zip(axes, disp_physical_types):
+                comp_unit = u.Unit(comp_model["initialized_display_units"][ax])
+                compat = comp_unit.physical_type == ax_physical_type
+                if not compat:
+                    break
+            self.component_models[model_index]["compat_display_units"] = compat
+
+        # length hasn't changed, so we need to force the traitlet to update
+        self.send_state("component_models")
+        self._check_model_equation_invalid()
+
+    def _on_global_display_unit_changed(self, msg):
+        axis = {'spectral': 'x', 'flux': 'y'}.get(msg.axis)
+
+        # update internal tracking of current units
+        self._units[axis] = str(msg.unit)
+
+        self._check_model_component_compat([axis], [msg.unit])
+
     def remove_model_component(self, model_component_label):
         """
         Remove an existing model component.
 
         Parameters
         ----------
         model_component_label : str
@@ -630,42 +660,83 @@
         # revert fixed parameters to user-value
         new_model['parameters'] = [fixed_params.get(p['name'], p) for p in new_model['parameters']]
 
         self.component_models[model_index] = new_model
         # length hasn't changed, so we need to force the traitlet to update
         self.send_state("component_models")
 
+        # model units may have changed, need to re-check their compatibility with display units
+        self._check_model_component_compat()
+
         # return user-friendly info on revised model
         return self.get_model_component(model_component_label)
 
     @property
     def model_components(self):
         """
         List of the labels of existing model components
         """
         return [x["id"] for x in self.component_models]
 
     @property
+    def valid_model_components(self):
+        """
+        List of the labels of existing valid (due to display units) model components
+        """
+        return [x["id"] for x in self.component_models if x["compat_display_units"]]
+
+    @property
     def equation_components(self):
         """
         List of the labels of model components in the current equation
         """
-        return re.split('[+*/-]', self.equation.value)
+        return re.split(r'[+*/-]', self.equation.value.replace(' ', ''))
 
     def vue_add_model(self, event):
         self.create_model_component()
 
     def vue_remove_model(self, event):
         self.remove_model_component(event)
 
     @observe('model_equation')
-    def _model_equation_changed(self, event):
+    def _check_model_equation_invalid(self, event=None):
         # Length is a dummy check to test the infrastructure
         if len(self.model_equation) == 0:
-            self.model_equation_invalid_msg = 'model equation is required'
+            self.model_equation_invalid_msg = 'model equation is required.'
+            return
+        if '' in self.equation_components:
+            # includes an operator without a variable (ex: 'C+')
+            self.model_equation_invalid_msg = 'incomplete equation.'
+            return
+
+        components_not_existing = [comp for comp in self.equation_components
+                                   if comp not in self.model_components]
+        if len(components_not_existing):
+            if len(components_not_existing) == 1:
+                msg = "is not an existing model component."
+            else:
+                msg = "are not existing model components."
+            self.model_equation_invalid_msg = f'{", ".join(components_not_existing)} {msg}'
+            return
+        components_not_valid = [comp for comp in self.equation_components
+                                if comp not in self.valid_model_components]
+        if len(components_not_valid):
+            if len(components_not_valid) == 1:
+                msg = ("is currently disabled because it has"
+                       " incompatible units with the current display units."
+                       " Remove the component from the equation,"
+                       " re-estimate its free parameters to use the new units"
+                       " or revert the display units.")
+            else:
+                msg = ("are currently disabled because they have"
+                       " incompatible units with the current display units."
+                       " Remove the components from the equation,"
+                       " re-estimate their free parameters to use the new units"
+                       " or revert the display units.")
+            self.model_equation_invalid_msg = f'{", ".join(components_not_valid)} {msg}'
             return
         self.model_equation_invalid_msg = ''
 
     @observe("dataset_selected", "dataset_items", "cube_fit")
     def _set_default_results_label(self, event={}):
         label_comps = []
         if hasattr(self, 'dataset') and (len(self.dataset.labels) > 1 or self.app.config == 'mosviz'):  # noqa
@@ -703,14 +774,16 @@
         fitted model
         fitted spectrum/cube
         residuals (if ``residuals_calculate`` is set to ``True``)
         """
         if not self.spectral_subset_valid:
             valid, spec_range, subset_range = self._check_dataset_spectral_subset_valid(return_ranges=True)  # noqa
             raise ValueError(f"spectral subset '{self.spectral_subset.selected}' {subset_range} is outside data range of '{self.dataset.selected}' {spec_range}")  # noqa
+        if len(self.model_equation_invalid_msg):
+            raise ValueError(f"model equation is invalid: {self.model_equation_invalid_msg}")
 
         if self.cube_fit:
             ret = self._fit_model_to_cube(add_data=add_data)
         else:
             ret = self._fit_model_to_spectrum(add_data=add_data)
 
         if ret is None:  # pragma: no cover
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue`

 * *Files 3% similar despite different names*

```diff
@@ -124,22 +124,46 @@
                       {{ param.name }} = {{ param.value }}                      
                     </span>
                   </v-row>
                 </v-col>
               </v-row>
             </v-expansion-panel-header>
             <v-expansion-panel-content>
-              <v-row 
-                v-if="!componentInEquation(item.id)"
-                class="v-messages v-messages__message text--secondary"
-                style="padding-top: 12px"
-              >
-                <span><b>{{ item.id }}</b> model component not in equation</span>
+              <v-row v-if="!item.compat_display_units">
+                <v-alert :type="componentInEquation(item.id) ? 'error' : 'warning'">
+                  <b>{{ item.id }}</b> is inconsistent with the current display units so cannot be used in the model equation.
+                  Create a new model component or re-estimate the free parameters based on the current display units.
+                  <v-row
+                    justify="end"
+                    style="padding-top: 12px; padding-right: 2px"
+                  >
+                    <j-tooltip tipid='plugin-model-fitting-reestimate'>
+                      <v-btn
+                        tile
+                        :elevation=0
+                        x-small
+                        dense 
+                        color="turquoise"
+                        dark
+                        style="padding-left: 8px; padding-right: 6px;"
+                        @click="reestimate_model_parameters(item.id)">
+                        <v-icon left small dense style="margin-right: 2px">mdi-restart</v-icon>
+                        Re-estimate free parameters
+                      </v-btn>
+                    </j-tooltip>
+                  </v-row>
+                </v-alert>
+              </v-row>
+              <v-row v-if="item.compat_display_units && !componentInEquation(item.id)">
+                <v-alert type="info">
+                  <b>{{ item.id }}</b> model component not in equation
+                </v-alert>
               </v-row>
-              <v-row justify="end"
+              <v-row v-if="item.compat_display_units"
+                justify="end"
                 style="padding-top: 12px; padding-right: 2px"
               >
                 <j-tooltip tipid='plugin-model-fitting-reestimate'>
                   <v-btn
                     tile
                     :elevation=0
                     x-small
@@ -286,15 +310,15 @@
       this.sanitizeCompLabel = (v) => {
         // strip non-word character entries
         this.comp_label = v.replace(/[\W]+/g, '');
       }
     },
     methods: {
       componentInEquation(componentId) {
-        return this.model_equation.split(/[+*\/-]/).indexOf(componentId) !== -1
+        return this.model_equation.replace(/\s/g, '').split(/[+*\/-]/).indexOf(componentId) !== -1
       },
       roundUncertainty(uncertainty) {
         return uncertainty.toPrecision(2)
       }
     }
   }
 </script>
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py`

 * *Files 12% similar despite different names*

```diff
@@ -323,7 +323,60 @@
                                  'L:intercept_0:fixed', 'L:intercept_0:std',
                                  'G:amplitude_1', 'G:amplitude_1:unit',
                                  'G:amplitude_1:fixed', 'G:amplitude_1:std',
                                  'G:mean_1', 'G:mean_1:unit',
                                  'G:mean_1:fixed', 'G:mean_1:std',
                                  'G:stddev_1', 'G:stddev_1:unit',
                                  'G:stddev_1:fixed', 'G:stddev_1:std']
+
+
+def test_equation_validation(specviz_helper, spectrum1d):
+    data_label = 'test'
+    specviz_helper.load_data(spectrum1d, data_label=data_label)
+
+    mf = specviz_helper.plugins['Model Fitting']
+    mf.create_model_component('Const1D')
+    mf.create_model_component('Linear1D')
+
+    assert mf.equation == 'C+L'
+    assert mf._obj.model_equation_invalid_msg == ''
+
+    mf.equation = 'L+'
+    assert mf._obj.model_equation_invalid_msg == 'incomplete equation.'
+
+    mf.equation = 'L+C'
+    assert mf._obj.model_equation_invalid_msg == ''
+
+    mf.equation = 'L+CC'
+    assert mf._obj.model_equation_invalid_msg == 'CC is not an existing model component.'
+
+    mf.equation = 'L+CC+DD'
+    assert mf._obj.model_equation_invalid_msg == 'CC, DD are not existing model components.'
+
+    mf.equation = ''
+    assert mf._obj.model_equation_invalid_msg == 'model equation is required.'
+
+
+@pytest.mark.filterwarnings(r"ignore:Model is linear in parameters.*")
+@pytest.mark.filterwarnings(r"ignore:The fit may be unsuccessful.*")
+def test_incompatible_units(specviz_helper, spectrum1d):
+    data_label = 'test'
+    specviz_helper.load_data(spectrum1d, data_label=data_label)
+
+    mf = specviz_helper.plugins['Model Fitting']
+    mf.create_model_component('Linear1D')
+
+    mf.add_results.label = 'model native units'
+    mf.calculate_fit(add_data=True)
+
+    uc = specviz_helper.plugins['Unit Conversion']
+    assert uc.spectral_unit.selected == "Angstrom"
+    uc.spectral_unit = u.Hz
+
+    assert 'L is currently disabled' in mf._obj.model_equation_invalid_msg
+    mf.add_results.label = 'frequency units'
+    with pytest.raises(ValueError, match=r"model equation is invalid.*"):
+        mf.calculate_fit(add_data=True)
+
+    mf.reestimate_model_parameters()
+    assert mf._obj.model_equation_invalid_msg == ''
+    mf.calculate_fit(add_data=True)
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from specutils import Spectrum1D
 
 from jdaviz.configs.cubeviz.plugins.tests.test_parsers import ASTROPY_LT_5_3
 from jdaviz.configs.default.plugins.model_fitting.initializers import MODELS
 
 
 def test_default_model_labels(specviz_helper, spectrum1d):
-    specviz_helper.load_spectrum(spectrum1d)
+    specviz_helper.load_data(spectrum1d)
     modelfit_plugin = specviz_helper.plugins['Model Fitting']
     # By default, the spectral region should be the entire spectrum
     assert modelfit_plugin._obj.spectral_subset_selected == "Entire Spectrum"
 
     for model in MODELS:
         # Check that the auto label is set correctly (or at least the first character matches)
         # BlackBody and Polynomial labels behave differently, so check only the first character
@@ -42,15 +42,15 @@
     assert (
         modelfit_plugin._obj.model_equation
         == "+".join(param["id"] for param in modelfit_plugin._obj.component_models)
     )
 
 
 def test_custom_model_labels(specviz_helper, spectrum1d):
-    specviz_helper.load_spectrum(spectrum1d)
+    specviz_helper.load_data(spectrum1d)
     modelfit_plugin = specviz_helper.plugins['Model Fitting']
 
     for i, model in enumerate(MODELS):
         # Add one of each model with a unique name
         modelfit_plugin.model_comp_selected = model
         modelfit_plugin._obj.comp_label = f"test_model_{i}"
         modelfit_plugin._obj.vue_add_model({})
@@ -64,15 +64,15 @@
     )
 
 
 def test_register_model_with_uncertainty_weighting(specviz_helper, spectrum1d):
     spectrum1d.uncertainty = StdDevUncertainty(spectrum1d.flux * 0.1)
     with warnings.catch_warnings():
         warnings.simplefilter('ignore')
-        specviz_helper.load_spectrum(spectrum1d)
+        specviz_helper.load_data(spectrum1d)
     modelfit_plugin = specviz_helper.plugins['Model Fitting']
 
     # Test registering a simple linear fit
     modelfit_plugin._obj.model_comp_selected = 'Linear1D'
     modelfit_plugin._obj.vue_add_model({})
     with pytest.warns(AstropyUserWarning, match='Model is linear in parameters'):
         modelfit_plugin.calculate_fit()
@@ -101,15 +101,15 @@
 
 
 def test_register_model_uncertainty_is_none(specviz_helper, spectrum1d):
     # Set uncertainty to None
     spectrum1d.uncertainty = None
     with warnings.catch_warnings():
         warnings.simplefilter('ignore')
-        specviz_helper.load_spectrum(spectrum1d)
+        specviz_helper.load_data(spectrum1d)
     modelfit_plugin = specviz_helper.plugins['Model Fitting']
 
     # Test registering a simple linear fit
     modelfit_plugin._obj.model_comp_selected = 'Linear1D'
     modelfit_plugin._obj.vue_add_model({})
     with pytest.warns(AstropyUserWarning, match='Model is linear in parameters'):
         modelfit_plugin.calculate_fit()
@@ -150,18 +150,47 @@
     assert modelfit_plugin._obj.results_label_default == 'cube-fit model'
     assert modelfit_plugin._obj.results_label == test_label
     with pytest.warns(AstropyUserWarning):
         modelfit_plugin.calculate_fit()
     assert test_label in cubeviz_helper.app.data_collection
 
 
+def test_refit_plot_options(specviz_helper, spectrum1d):
+    specviz_helper.load_data(spectrum1d)
+    modelfit_plugin = specviz_helper.plugins['Model Fitting']
+
+    modelfit_plugin.model_comp_selected = 'Const1D'
+    modelfit_plugin._obj.comp_label = "C"
+    modelfit_plugin._obj.vue_add_model({})
+
+    with pytest.warns(AstropyUserWarning):
+        modelfit_plugin.calculate_fit(add_data=True)
+
+    sv = specviz_helper.app.get_viewer('spectrum-viewer')
+    atts = {"color": "red", "linewidth": 2, "alpha": 0.8}
+    layer_state = [layer.state for layer in sv.layers if layer.layer.label == "model"][0]
+    for att in atts:
+        setattr(layer_state, att, atts[att])
+
+    # Refit using the same name, which will replace the data by default.
+    modelfit_plugin.create_model_component('Linear1D', 'L')
+
+    with pytest.warns(AstropyUserWarning):
+        modelfit_plugin.calculate_fit(add_data=True)
+
+    layer_state = [layer.state for layer in sv.layers if layer.layer.label == "model"][0]
+
+    for att in atts:
+        assert atts[att] == getattr(layer_state, att)
+
+
 def test_user_api(specviz_helper, spectrum1d):
     with warnings.catch_warnings():
         warnings.simplefilter('ignore')
-        specviz_helper.load_spectrum(spectrum1d)
+        specviz_helper.load_data(spectrum1d)
     p = specviz_helper.plugins['Model Fitting']
 
     # even though the default label is set to C, adding Linear1D should default to its automatic
     # default label of 'L'
     assert p.model_component == 'Const1D'  # tests SelectPluginComponent's __eq__
     assert p.model_component_label.value == 'C'
     assert p.model_component_label == 'C'  # tests AutoTextField's __eq__
@@ -191,15 +220,15 @@
     assert p.get_model_component('P2', 'c0')['value'] == 0.2
     assert p.get_model_component('P2', 'c0')['fixed'] is True
 
 
 def test_fit_gaussian_with_fixed_mean(specviz_helper, spectrum1d):
     with warnings.catch_warnings():
         warnings.simplefilter('ignore')
-        specviz_helper.load_spectrum(spectrum1d)
+        specviz_helper.load_data(spectrum1d)
     modelfit_plugin = specviz_helper.plugins['Model Fitting']
 
     modelfit_plugin.create_model_component('Gaussian1D', 'G')
     params = modelfit_plugin._obj.component_models[0]['parameters']
     params[1]['fixed'] = True  # Fix mean
 
     old_amp = params[0]['value']
@@ -213,15 +242,15 @@
     assert_allclose(result.mean.value, old_mean)
     assert not np.allclose((result.amplitude.value, result.stddev.value), (old_amp, old_std))
 
 
 def test_reestimate_parameters(specviz_helper, spectrum1d):
     with warnings.catch_warnings():
         warnings.simplefilter('ignore')
-        specviz_helper.load_spectrum(spectrum1d)
+        specviz_helper.load_data(spectrum1d)
     mf = specviz_helper.plugins['Model Fitting']
 
     mf.create_model_component('Gaussian1D', 'G')
     mf.set_model_component('G', 'stddev', value=1, fixed=True)
     mc = mf.get_model_component('G')
 
     assert_allclose(mc['parameters']['mean']['value'], 7055.519926198364)
@@ -323,20 +352,20 @@
 
     # Check that both masks are applied correctly
     assert np.all(masked_data.mask == (expected_spectral_mask | expected_spatial_mask))
 
 
 def test_invalid_subset(specviz_helper, spectrum1d):
     # 6000-8000
-    specviz_helper.load_spectrum(spectrum1d, data_label="right_spectrum")
+    specviz_helper.load_data(spectrum1d, data_label="right_spectrum")
 
     # 5000-7000
     sp2 = Spectrum1D(spectral_axis=spectrum1d.spectral_axis - 1000*spectrum1d.spectral_axis.unit,
                      flux=spectrum1d.flux * 1.25)
-    specviz_helper.load_spectrum(sp2, data_label="left_spectrum")
+    specviz_helper.load_data(sp2, data_label="left_spectrum")
 
     # apply subset that overlaps on left_spectrum, but not right_spectrum
     # NOTE: using a subset that overlaps the right_spectrum (reference) results in errors when
     # retrieving the subset (https://github.com/spacetelescope/jdaviz/issues/1868)
     specviz_helper.app.get_viewer('spectrum-viewer').apply_roi(XRangeROI(5000, 6000))
 
     plugin = specviz_helper.plugins['Model Fitting']
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/plot_options.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/plot_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 from glue_jupyter.common.toolbar_vuetify import read_icon
 
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import (PluginTemplateMixin, ViewerSelect, LayerSelect,
                                         PlotOptionsSyncState)
 from jdaviz.core.user_api import PluginUserApi
 from jdaviz.core.tools import ICON_DIR
+from jdaviz.core.custom_traitlets import IntHandleEmpty
 from jdaviz.utils import bqplot_clear_figure
+from jdaviz.core.marks import HistogramMark
 
 __all__ = ['PlotOptions']
 
 
 @tray_registry('g-plot-options', label="Plot Options")
 class PlotOptions(PluginTemplateMixin):
     """
@@ -91,16 +93,18 @@
       not exposed for Specviz. This only applies when ``contour_mode`` is "Linear".
     * ``contour_max`` (:class:`~jdaviz.core.template_mixin.PlotOptionsSyncState`):
       not exposed for Specviz. This only applies when ``contour_mode`` is "Linear".
     * ``contour_nlevels`` (:class:`~jdaviz.core.template_mixin.PlotOptionsSyncState`):
       not exposed for Specviz. This only applies when ``contour_mode`` is "Linear".
     * ``contour_custom_levels`` (:class:`~jdaviz.core.template_mixin.PlotOptionsSyncState`):
       not exposed for Specviz. This only applies when ``contour_mode`` is "Custom".
+    * :meth: `set_histogram_nbins`
     """
     template_file = __file__, "plot_options.vue"
+    uses_active_status = Bool(True).tag(sync=True)
 
     # multiselect is shared between viewer and layer
     multiselect = Bool(False).tag(sync=True)
 
     viewer_items = List().tag(sync=True)
     viewer_selected = Any().tag(sync=True)  # Any needed for multiselect
     layer_items = List().tag(sync=True)
@@ -184,14 +188,15 @@
     stretch_vmin_value = Float().tag(sync=True)
     stretch_vmin_sync = Dict().tag(sync=True)
 
     stretch_vmax_value = Float().tag(sync=True)
     stretch_vmax_sync = Dict().tag(sync=True)
 
     stretch_hist_zoom_limits = Bool().tag(sync=True)
+    stretch_hist_nbins = IntHandleEmpty().tag(sync=True)
     stretch_histogram = Any().tag(sync=True, **widget_serialization)
 
     subset_visible_value = Bool().tag(sync=True)
     subset_visible_sync = Dict().tag(sync=True)
 
     subset_color_value = Unicode().tag(sync=True)
     subset_color_sync = Dict().tag(sync=True)
@@ -423,15 +428,16 @@
         # display_units
 
         self.show_viewer_labels = self.app.state.settings['viewer_labels']
         self.app.state.add_callback('settings', self._on_app_settings_changed)
 
     @property
     def user_api(self):
-        expose = ['multiselect', 'viewer', 'layer', 'select_all', 'subset_visible']
+        expose = ['multiselect', 'viewer', 'layer', 'select_all', 'subset_visible',
+                  'set_histogram_nbins']
         if self.config == "cubeviz":
             expose += ['collapse_function']
         if self.config != "imviz":
             expose += ['axes_visible', 'line_visible', 'line_color', 'line_width', 'line_opacity',
                        'line_as_steps', 'uncertainty_visible']
         if self.config != "specviz":
             expose += ['subset_color',
@@ -475,24 +481,28 @@
         sync_state.unmix_state()
 
     def vue_set_value(self, data):
         attr_name = data.get('name')
         value = data.get('value')
         setattr(self, attr_name, value)
 
-    @observe('plugin_opened', 'layer_selected', 'viewer_selected',
+    @observe('is_active', 'layer_selected', 'viewer_selected',
              'stretch_hist_zoom_limits')
     def _update_stretch_histogram(self, msg={}):
+        # Import here to prevent circular import.
+        from jdaviz.configs.imviz.plugins.viewers import ImvizImageView
+        from jdaviz.configs.cubeviz.plugins.viewers import CubevizImageView
+
         if not self.stretch_function_sync.get('in_subscribed_states'):  # pragma: no cover
             # no (image) viewer with stretch function options
             return
         if not hasattr(self, 'viewer'):  # pragma: no cover
             # plugin hasn't been fully initialized yet
             return
-        if (not self.plugin_opened
+        if (not self.is_active
                 or not self.viewer.selected
                 or not self.layer.selected):  # pragma: no cover
             # no need to make updates, updates will be redrawn when plugin is opened
             # NOTE: this won't update when the plugin is shown but not open in the tray
             return
         if not isinstance(msg, dict) and not self.stretch_hist_zoom_limits:  # pragma: no cover
             # then this is from the limits callbacks and we don't want to waste resources
@@ -503,14 +513,18 @@
         if self.multiselect and (len(self.viewer.selected) > 1
                                  or len(self.layer.selected) > 1):  # pragma: no cover
             # currently only support single-layer/viewer.  For now we'll just clear and return.
             # TODO: add support for multi-layer/viewer
             bqplot_clear_figure(self.stretch_histogram)
             return
 
+        if not isinstance(self.viewer.selected_obj, (ImvizImageView, CubevizImageView)):
+            # don't update histogram if selected viewer is not an image viewer:
+            return
+
         viewer = self.viewer.selected_obj[0] if self.multiselect else self.viewer.selected_obj
 
         # manage viewer zoom limit callbacks
         if ((isinstance(msg, dict) and msg.get('name') == 'viewer_selected')
                 or not self.stretch_hist_zoom_limits):
             vs = viewer.state
             for attr in ('x_min', 'x_max', 'y_min', 'y_max'):
@@ -518,15 +532,22 @@
         if isinstance(msg, dict) and msg.get('name') == 'viewer_selected':
             viewer_label_old = msg.get('old')[0] if self.multiselect else msg.get('old')
             if len(viewer_label_old):
                 vs_old = self.app.get_viewer(viewer_label_old).state
                 for attr in ('x_min', 'x_max', 'y_min', 'y_max'):
                     vs_old.remove_callback(attr, self._update_stretch_histogram)
 
-        data = self.layer.selected_obj[0][0].layer if self.multiselect else self.layer.selected_obj[0].layer  # noqa
+        if self.multiselect:
+            data = self.layer.selected_obj[0][0].layer
+        elif len(self.layer.selected_obj):
+            data = self.layer.selected_obj[0].layer
+        else:
+            # skip further updates if no data are available:
+            return
+
         comp = data.get_component(data.main_components[0])
 
         if self.stretch_hist_zoom_limits:
             if hasattr(viewer, '_get_zoom_limits'):
                 # Viewer limits. This takes account of Imviz linking.
                 xy_limits = viewer._get_zoom_limits(data).astype(int)
                 x_limits = xy_limits[:, 0]
@@ -579,18 +600,76 @@
                                                        label='pixel value'),
                                            bqplot.Axis(scale=hist_y_sc,
                                                        num_ticks=2,
                                                        orientation='vertical',
                                                        label='density')]
 
             self.bqplot_figs_resize = [self.stretch_histogram]
+            self.stretch_hist_nbins = 25
 
         else:
             hist_mark = self.stretch_histogram.marks[0]
             hist_mark.sample = sub_data
             # TODO: Let user change the number of bins?
             # TODO: Let user set y-scale to log
 
         interval = PercentileInterval(95)
         if len(sub_data) > 0:
             hist_lims = interval.get_limits(sub_data)
             hist_mark.min, hist_mark.max = hist_lims
+
+        self._check_if_v_stretch_changed()
+
+    @observe('stretch_vmin_value', 'stretch_vmax_value')
+    def _check_if_v_stretch_changed(self, msg=None):
+        self._remove_histogram_marks()
+        self._add_histogram_marks()
+
+    def _add_histogram_marks(self):
+        if self.stretch_histogram is None:
+            return
+        scales = {'x': self.stretch_histogram.axes[0].scale, 'y': bqplot.LinearScale()}
+        v_stretch_lines = []
+        # Set the viewer limits if they are None
+        if self.stretch_histogram.axes[0].scale.min is None:
+            self.stretch_histogram.axes[0].scale.min = self.stretch_histogram.marks[0].min
+        if self.stretch_histogram.axes[0].scale.max is None:
+            self.stretch_histogram.axes[0].scale.max = self.stretch_histogram.marks[0].max
+
+        # If the stretch limits are within the viewer limits, draw the HistogramMark
+        if self.stretch_vmin.value >= self.stretch_histogram.axes[0].scale.min:
+            vmin_lines = HistogramMark(min_max_value=[self.stretch_vmin.value, self.stretch_vmin.value], # noqa
+                                       scales=scales)
+            v_stretch_lines.append(vmin_lines)
+        if self.stretch_vmax.value <= self.stretch_histogram.axes[0].scale.max:
+            vmax_lines = HistogramMark(min_max_value=[self.stretch_vmax.value, self.stretch_vmax.value], # noqa
+                                       scales=scales)
+            v_stretch_lines.append(vmax_lines)
+        self.stretch_histogram.marks = self.stretch_histogram.marks + v_stretch_lines
+
+    def _remove_histogram_marks(self):
+        if self.stretch_histogram is None:
+            return
+        self.stretch_histogram.marks = [mark for mark in self.stretch_histogram.marks
+                                        if not isinstance(mark, HistogramMark)]
+
+    @observe("stretch_hist_nbins")
+    def histogram_nbins_changed(self, msg):
+        if self.stretch_histogram is None or msg['new'] == '' or msg['new'] < 1:
+            return
+        self.set_histogram_nbins(msg['new'])
+
+    def set_histogram_nbins(self, nbins):
+        self.stretch_histogram.marks[0].bins = nbins
+        self.stretch_hist_nbins = nbins
+
+    def set_histogram_x_limits(self, x_min, x_max):
+        if x_min:
+            self.stretch_histogram.axes[0].scale.min = x_min
+        if x_max:
+            self.stretch_histogram.axes[0].scale.max = x_max
+
+    def set_histogram_y_limits(self, y_min, y_max):
+        if y_min:
+            self.stretch_histogram.axes[1].scale.min = y_min
+        if y_max:
+            self.stretch_histogram.axes[1].scale.max = y_max
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/plot_options.vue` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/plot_options.vue`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 <template>
   <j-tray-plugin
     description='Viewer and data/layer options.'
     :link="'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#plot-options'"
+    :uses_active_status="uses_active_status"
+    @plugin-ping="plugin_ping($event)"
     :popout_button="popout_button">
 
     <v-row>
       <v-expansion-panels popout>
         <v-expansion-panel>
           <v-expansion-panel-header v-slot="{ open }">
             <span style="padding: 6px">Settings</span>
@@ -344,14 +346,24 @@
 
     <glue-state-sync-wrapper :sync="stretch_vmax_sync" :multiselect="multiselect" @unmix-state="unmix_state('stretch_vmax')">
       <glue-float-field label="Stretch VMax" :value.sync="stretch_vmax_value" />
     </glue-state-sync-wrapper>
 
     <v-row v-if="stretch_function_sync.in_subscribed_states">
       <!-- z-index to ensure on top of the jupyter widget with negative margin-top -->
+      <v-text-field
+          ref="stretch_hist_nbins"
+          type="number"
+          label="Number of Bins"
+          v-model.number="stretch_hist_nbins"
+          hint="The amount of bins used in the histogram."
+          persistent-hint
+          :rules="[() => stretch_hist_nbins !== '' || 'This field is required',
+                   () => stretch_hist_nbins > 0 || 'Number of Bins must be greater than zero']"
+      ></v-text-field>
       <v-switch
         v-model="stretch_hist_zoom_limits"
         class="hide-input"
         label="Limit histogram to current zoom limits"
         style="z-index: 1"
       ></v-switch>
       <!-- NOTE: height defined here should match that in the custom CSS rules
@@ -490,15 +502,14 @@
                 :value="contour_custom_levels_txt"
                 @focus="contour_custom_levels_focus"
                 @blur="contour_custom_levels_blur"
                 @input="contour_custom_levels_set_value"/>
             </glue-state-sync-wrapper>
           </div>
         </div>
-
       </div>
       <div v-if="contour_spinner"
            class="text-center"
            style="grid-area: 1/1; 
                   z-index:2;
                   margin-left: -24px;
                   margin-right: -24px;
@@ -507,15 +518,15 @@
         <v-progress-circular
           indeterminate
           color="spinner"
           size="50"
           width="6"
         ></v-progress-circular>
       </div>
-
+    </div>
     <!-- GENERAL:AXES -->
     <j-plugin-section-header v-if="axes_visible_sync.in_subscribed_states && config !== 'imviz'">Axes</j-plugin-section-header>
     <glue-state-sync-wrapper v-if="config !== 'imviz'":sync="axes_visible_sync" :multiselect="multiselect" @unmix-state="unmix_state('axes_visible')">
       <v-switch
         v-model="axes_visible_value"
         label="Show Axes"
         />
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,24 @@
+import os
+
 import numpy as np
+
+from astropy.time import Time
+import astropy.units as u
 from glue.core.message import EditSubsetMessage, SubsetUpdateMessage
 from glue.core.edit_subset_mode import (AndMode, AndNotMode, OrMode,
                                         ReplaceMode, XorMode)
-from glue.core.roi import CircularROI, EllipticalROI, RectangularROI
-from glue.core.subset import RoiSubsetState, RangeSubsetState, CompositeSubsetState
+from glue.core.roi import CircularROI, CircularAnnulusROI, EllipticalROI, RectangularROI
+from glue.core.subset import RoiSubsetState, RangeSubsetState
+from glue.icons import icon_path
 from glue_jupyter.widgets.subset_mode_vuetify import SelectionModeMenu
+from glue_jupyter.common.toolbar_vuetify import read_icon
 from traitlets import Any, List, Unicode, Bool, observe
 
-from jdaviz.core.events import SnackbarMessage
+from jdaviz.core.events import SnackbarMessage, GlobalDisplayUnitChanged
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import PluginTemplateMixin, DatasetSelectMixin, SubsetSelect
 
 __all__ = ['SubsetPlugin']
 
 SUBSET_MODES = {
     'replace': ReplaceMode,
@@ -36,32 +43,42 @@
     subset_definitions = List([]).tag(sync=True)
     glue_state_types = List([]).tag(sync=True)
     has_subset_details = Bool(False).tag(sync=True)
 
     subplugins_opened = Any().tag(sync=True)
 
     is_centerable = Bool(False).tag(sync=True)
+    can_simplify = Bool(False).tag(sync=True)
+
+    icon_replace = Unicode(read_icon(os.path.join(icon_path("glue_replace", icon_format="svg")), 'svg+xml')).tag(sync=True)  # noqa
+    icon_or = Unicode(read_icon(os.path.join(icon_path("glue_or", icon_format="svg")), 'svg+xml')).tag(sync=True)  # noqa
+    icon_and = Unicode(read_icon(os.path.join(icon_path("glue_and", icon_format="svg")), 'svg+xml')).tag(sync=True)  # noqa
+    icon_xor = Unicode(read_icon(os.path.join(icon_path("glue_xor", icon_format="svg")), 'svg+xml')).tag(sync=True)  # noqa
+    icon_andnot = Unicode(read_icon(os.path.join(icon_path("glue_andnot", icon_format="svg")), 'svg+xml')).tag(sync=True)  # noqa
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.components = {
             'g-subset-mode': SelectionModeMenu(session=self.session)
         }
 
         self.session.hub.subscribe(self, EditSubsetMessage,
                                    handler=self._sync_selected_from_state)
         self.session.hub.subscribe(self, SubsetUpdateMessage,
                                    handler=self._on_subset_update)
+        self.session.hub.subscribe(self, GlobalDisplayUnitChanged,
+                                   handler=self._on_display_unit_changed)
 
         self.subset_select = SubsetSelect(self,
                                           'subset_items',
                                           'subset_selected',
                                           default_text="Create New")
         self.subset_states = []
+        self.spectral_display_unit = None
 
     def _sync_selected_from_state(self, *args):
         if not hasattr(self, 'subset_select'):
             # during initial init, this can trigger before the component is initialized
             return
         if self.session.edit_subset_mode.edit_subset == []:
             if self.subset_selected != self.subset_select.default_text:
@@ -123,31 +140,36 @@
         Convert what app.get_subsets returns into something the UI of this plugin
         can display.
 
         Returns
         -------
 
         """
-        subset_information = self.app.get_subsets(self.subset_selected, simplify_spectral=False)
+        subset_information = self.app.get_subsets(self.subset_selected, simplify_spectral=False,
+                                                  use_display_units=True)
         _around_decimals = 6  # Avoid 30 degrees from coming back as 29.999999999999996
         if not subset_information:
             return
-        if len(subset_information) == 1:
+        if ((len(subset_information) == 1) and
+                (isinstance(subset_information[0]["subset_state"], RangeSubsetState) or
+                 (isinstance(subset_information[0]["subset_state"], RoiSubsetState) and
+                  isinstance(subset_information[0]["subset_state"].roi,
+                             (CircularROI, RectangularROI, EllipticalROI))))):
             self.is_centerable = True
         else:
             self.is_centerable = False
 
         for spec in subset_information:
             subset_definition = []
             subset_type = ''
             subset_state = spec["subset_state"]
             glue_state = spec["glue_state"]
             if isinstance(subset_state, RoiSubsetState):
                 if isinstance(subset_state.roi, CircularROI):
-                    x, y = subset_state.roi.get_center()
+                    x, y = subset_state.roi.center()
                     r = subset_state.roi.radius
                     subset_definition = [{"name": "X Center", "att": "xc", "value": x, "orig": x},
                                          {"name": "Y Center", "att": "yc", "value": y, "orig": y},
                                          {"name": "Radius", "att": "radius", "value": r, "orig": r}]
 
                 elif isinstance(subset_state.roi, RectangularROI):
                     for att in ("Xmin", "Xmax", "Ymin", "Ymax"):
@@ -156,53 +178,103 @@
                         subset_definition.append(
                             {"name": att, "att": real_att, "value": val, "orig": val})
                     theta = np.around(np.degrees(subset_state.roi.theta), decimals=_around_decimals)
                     subset_definition.append(
                         {"name": "Angle", "att": "theta", "value": theta, "orig": theta})
 
                 elif isinstance(subset_state.roi, EllipticalROI):
-                    xc = subset_state.roi.xc
-                    yc = subset_state.roi.yc
+                    xc, yc = subset_state.roi.center()
                     rx = subset_state.roi.radius_x
                     ry = subset_state.roi.radius_y
                     theta = np.around(np.degrees(subset_state.roi.theta), decimals=_around_decimals)
                     subset_definition = [
                         {"name": "X Center", "att": "xc", "value": xc, "orig": xc},
                         {"name": "Y Center", "att": "yc", "value": yc, "orig": yc},
                         {"name": "X Radius", "att": "radius_x", "value": rx, "orig": rx},
                         {"name": "Y Radius", "att": "radius_y", "value": ry, "orig": ry},
                         {"name": "Angle", "att": "theta", "value": theta, "orig": theta}]
 
+                elif isinstance(subset_state.roi, CircularAnnulusROI):
+                    x, y = subset_state.roi.center()
+                    inner_r = subset_state.roi.inner_radius
+                    outer_r = subset_state.roi.outer_radius
+                    subset_definition = [{"name": "X Center", "att": "xc", "value": x, "orig": x},
+                                         {"name": "Y Center", "att": "yc", "value": y, "orig": y},
+                                         {"name": "Inner radius", "att": "inner_radius",
+                                          "value": inner_r, "orig": inner_r},
+                                         {"name": "Outer radius", "att": "outer_radius",
+                                          "value": outer_r, "orig": outer_r}]
+
                 subset_type = subset_state.roi.__class__.__name__
 
             elif isinstance(subset_state, RangeSubsetState):
-                lo = subset_state.lo
-                hi = subset_state.hi
-                subset_definition = [{"name": "Lower bound", "att": "lo", "value": lo, "orig": lo},
-                                     {"name": "Upper bound", "att": "hi", "value": hi, "orig": hi}]
+                region = spec['region']
+                if isinstance(region, Time):
+                    lo = region.min()
+                    hi = region.max()
+                    subset_definition = [{"name": "Lower bound", "att": "lo", "value": lo.value,
+                                          "orig": lo.value},
+                                         {"name": "Upper bound", "att": "hi", "value": hi.value,
+                                          "orig": hi.value}]
+                else:
+                    lo = region.lower
+                    hi = region.upper
+                    subset_definition = [{"name": "Lower bound", "att": "lo", "value": lo.value,
+                                          "orig": lo.value, "unit": str(lo.unit)},
+                                         {"name": "Upper bound", "att": "hi", "value": hi.value,
+                                          "orig": hi.value, "unit": str(hi.unit)}]
                 subset_type = "Range"
             if len(subset_definition) > 0:
                 # Note: .append() does not work for List traitlet.
                 self.subset_definitions = self.subset_definitions + [subset_definition]
                 self.subset_types = self.subset_types + [subset_type]
                 self.glue_state_types = self.glue_state_types + [glue_state]
                 self.subset_states = self.subset_states + [subset_state]
 
+        simplifiable_states = set(['AndState', 'XorState', 'AndNotState'])
+        # Check if the subset has more than one subregion, is a range subset type, and
+        # uses one of the states that can be simplified.
+        if (len(self.subset_states) > 1 and isinstance(self.subset_states[0], RangeSubsetState)
+                and len(simplifiable_states - set(self.glue_state_types)) < 3):
+            self.can_simplify = True
+        elif (len(self.subset_states) > 1 and isinstance(self.subset_states[0], RangeSubsetState)
+              and self.app.is_there_overlap_spectral_subset(self.subset_selected)):
+            self.can_simplify = True
+        else:
+            self.can_simplify = False
+
     def _get_subset_definition(self, *args):
         """
         Retrieve the parameters defining the selected subset, for example the
         upper and lower bounds for a simple spectral subset.
         """
         self.subset_definitions = []
         self.subset_types = []
         self.glue_state_types = []
         self.subset_states = []
 
         self._unpack_get_subsets_for_ui()
 
+    def vue_simplify_subset(self, *args):
+        if len(self.subset_states) < 2:
+            self.hub.broadcast(SnackbarMessage("Cannot simplify spectral subset "
+                                               "of length less than 2", color='warning',
+                                               sender=self))
+            return
+        att = self.subset_states[0].att
+        self.app.simplify_spectral_subset(subset_name=self.subset_selected, att=att,
+                                          overwrite=True)
+
+    def _on_display_unit_changed(self, msg):
+        # We only care about the spectral units, since flux units don't affect spectral subsets
+        if msg.axis == "spectral":
+            self.spectral_display_unit = msg.unit
+            if self.subset_selected != self.subset_select.default_text:
+                self._get_subset_definition(self.subset_selected)
+
     def vue_update_subset(self, *args):
         status, reason = self._check_input()
         if not status:
             self.hub.broadcast(SnackbarMessage(reason, color='error', sender=self))
             return
 
         for index, sub in enumerate(self.subset_definitions):
@@ -211,14 +283,24 @@
             sub_states = self.subset_states[index]
             for d_att in sub:
                 if d_att["att"] == 'theta':  # Humans use degrees but glue uses radians
                     d_val = np.radians(d_att["value"])
                 else:
                     d_val = float(d_att["value"])
 
+                # Convert from display unit to original unit if necessary
+                if self.subset_types[index] == "Range":
+                    if self.spectral_display_unit is not None:
+                        x_att = sub_states.att
+                        base_units = self.app.data_collection[0].get_component(x_att).units
+                        if self.spectral_display_unit != base_units:
+                            d_val = d_val*u.Unit(self.spectral_display_unit)
+                            d_val = d_val.to(u.Unit(base_units))
+                            d_val = d_val.value
+
                 if float(d_att["orig"]) != d_val:
                     if self.subset_types[index] == "Range":
                         setattr(sub_states, d_att["att"], d_val)
                     else:
                         setattr(sub_states.roi, d_att["att"], d_val)
         try:
             dc = self.data_collection
@@ -231,14 +313,15 @@
                 f"Failed to update Subset: {repr(err)}", color='error', sender=self))
 
     def _check_input(self):
         status = True
         reason = ""
         for index, sub in enumerate(self.subset_definitions):
             lo = hi = xmin = xmax = ymin = ymax = None
+            inner_radius = outer_radius = None
             for d_att in sub:
                 if d_att["att"] == "lo":
                     lo = d_att["value"]
                 elif d_att["att"] == "hi":
                     hi = d_att["value"]
                 elif d_att["att"] == "radius" and d_att["value"] <= 0:
                     status = False
@@ -248,23 +331,31 @@
                     xmin = d_att["value"]
                 elif d_att["att"] == "xmax":
                     xmax = d_att["value"]
                 elif d_att["att"] == "ymin":
                     ymin = d_att["value"]
                 elif d_att["att"] == "ymax":
                     ymax = d_att["value"]
+                elif d_att["att"] == "outer_radius":
+                    outer_radius = d_att["value"]
+                elif d_att["att"] == "inner_radius":
+                    inner_radius = d_att["value"]
 
                 if lo and hi and hi <= lo:
                     status = False
                     reason = "Failed to update Subset: lower bound must be less than upper bound"
                     break
                 elif xmin and xmax and ymin and ymax and (xmax - xmin <= 0 or ymax - ymin <= 0):
                     status = False
                     reason = "Failed to update Subset: width and length must be positive scalars"
                     break
+                elif inner_radius and outer_radius and inner_radius >= outer_radius:
+                    status = False
+                    reason = "Failed to update Subset: inner radius must be less than outer radius"
+                    break
 
         return status, reason
 
     def vue_recenter_subset(self, *args):
         # Composite region cannot be centered. This only works for Imviz.
         if not self.is_centerable or self.config != 'imviz':  # no-op
             raise NotImplementedError(
@@ -303,47 +394,21 @@
         Returns
         -------
         cen : number, tuple of numbers, or `None`
             The center of the Subset in ``x`` or ``(x, y)``,
             depending on the Subset type, if applicable.
             If Subset is not centerable, this returns `None`.
 
-        Raises
-        ------
-        NotImplementedError
-            Subset type is not supported.
-
         """
         # Composite region cannot be centered.
         if not self.is_centerable:  # no-op
             return
 
         subset_state = self.subset_select.selected_subset_state
-
-        if isinstance(subset_state, RoiSubsetState):
-            sbst_obj = subset_state.roi
-            if isinstance(sbst_obj, (CircularROI, EllipticalROI)):
-                cen = sbst_obj.get_center()
-            elif isinstance(sbst_obj, RectangularROI):
-                cen = sbst_obj.center()
-            else:  # pragma: no cover
-                raise NotImplementedError(
-                    f'Getting center of {sbst_obj.__class__} is not supported')
-
-        elif isinstance(subset_state, RangeSubsetState):
-            cen = (subset_state.hi - subset_state.lo) * 0.5 + subset_state.lo
-
-        elif isinstance(subset_state, CompositeSubsetState):
-            cen = None
-
-        else:  # pragma: no cover
-            raise NotImplementedError(
-                f'Getting center of {subset_state.__class__} is not supported')
-
-        return cen
+        return subset_state.center()
 
     def set_center(self, new_cen, update=False):
         """Set the desired center for the selected Subset, if applicable.
         If Subset is not centerable, nothing is done.
 
         Parameters
         ----------
@@ -367,30 +432,30 @@
             return
 
         subset_state = self.subset_select.selected_subset_state
 
         if isinstance(subset_state, RoiSubsetState):
             x, y = new_cen
             sbst_obj = subset_state.roi
-            if isinstance(sbst_obj, (CircularROI, EllipticalROI)):
+            if isinstance(sbst_obj, (CircularROI, CircularAnnulusROI, EllipticalROI)):
                 self._set_value_in_subset_definition(0, "X Center", "value", x)
                 self._set_value_in_subset_definition(0, "Y Center", "value", y)
             elif isinstance(sbst_obj, RectangularROI):
                 cx, cy = sbst_obj.center()
                 dx = x - cx
                 dy = y - cy
                 self._set_value_in_subset_definition(0, "Xmin", "value", sbst_obj.xmin + dx)
                 self._set_value_in_subset_definition(0, "Xmax", "value", sbst_obj.xmax + dx)
                 self._set_value_in_subset_definition(0, "Ymin", "value", sbst_obj.ymin + dy)
                 self._set_value_in_subset_definition(0, "Ymax", "value", sbst_obj.ymax + dy)
             else:  # pragma: no cover
                 raise NotImplementedError(f'Recentering of {sbst_obj.__class__} is not supported')
 
         elif isinstance(subset_state, RangeSubsetState):
-            dx = new_cen - ((subset_state.hi - subset_state.lo) * 0.5 + subset_state.lo)
+            dx = new_cen - subset_state.center()
             self._set_value_in_subset_definition(0, "Lower bound", "value", subset_state.lo + dx)
             self._set_value_in_subset_definition(0, "Upper bound", "value", subset_state.hi + dx)
 
         else:  # pragma: no cover
             raise NotImplementedError(
                 f'Getting center of {subset_state.__class__} is not supported')
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pytest
 
 from glue.core.roi import XRangeROI
 
 
 @pytest.mark.filterwarnings('ignore')
 def test_plugin(specviz_helper, spectrum1d):
-    specviz_helper.load_spectrum(spectrum1d)
+    specviz_helper.load_data(spectrum1d)
     p = specviz_helper.plugins['Subset Tools']
 
     # regression test for https://github.com/spacetelescope/jdaviz/issues/1693
     sv = specviz_helper.app.get_viewer('spectrum-viewer')
     sv.apply_roi(XRangeROI(6500, 7400))
 
     p._obj.subset_select.selected = 'Create New'
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/default/plugins/viewers.py` & `jdaviz-3.6.0/jdaviz/configs/default/plugins/viewers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 import numpy as np
 
-from glue.core.subset import RoiSubsetState
 from glue_jupyter.bqplot.profile import BqplotProfileView
 from glue_jupyter.bqplot.image import BqplotImageView
 from glue_jupyter.bqplot.scatter.layer_artist import BqplotScatterLayerState
 from glue_jupyter.table import TableViewer
 
 from jdaviz.configs.imviz.helper import layer_is_image_data
 from jdaviz.components.toolbar_nested import NestedJupyterToolbar
 from jdaviz.core.registries import viewer_registry
-from jdaviz.utils import ColorCycler
+from jdaviz.utils import ColorCycler, get_subset_type
 
 __all__ = ['JdavizViewerMixin']
 
 viewer_registry.add("g-profile-viewer", label="Profile 1D", cls=BqplotProfileView)
 viewer_registry.add("g-image-viewer", label="Image 2D", cls=BqplotImageView)
 viewer_registry.add("g-table-viewer", label="Table", cls=TableViewer)
 
 
 class JdavizViewerMixin:
     toolbar = None
     tools_nested = []
     _prev_limits = None
+    _native_mark_classnames = ('Lines', 'LinesGL', 'FRBImage', 'Contour')
 
     def __init__(self, *args, **kwargs):
         # NOTE: anything here most likely won't be called by viewers because of inheritance order
         super().__init__(*args, **kwargs)
 
         # Allow each viewer to cycle through colors for each new addition to the viewer:
         self.color_cycler = ColorCycler()
 
     @property
     def native_marks(self):
         """
         Return all marks that are Lines/LinesGL objects (and not subclasses)
         """
-        return [m for m in self.figure.marks if m.__class__.__name__ in ['Lines', 'LinesGL']]
+        return [m for m in self.figure.marks
+                if m.__class__.__name__ in self._native_mark_classnames]
 
     @property
     def custom_marks(self):
         """
         Return all marks that are not Lines/LinesGL objects (but can be subclasses)
         """
-        return [m for m in self.figure.marks if m.__class__.__name__ not in ['Lines', 'LinesGL']]
+        return [m for m in self.figure.marks
+                if m.__class__.__name__ not in self._native_mark_classnames]
 
     def _subscribe_to_layers_update(self):
         # subscribe to new layers
         self._expected_subset_layers = []
         self._layers_with_defaults_applied = []
         self.state.add_callback('layers', self._on_layers_update)
 
@@ -105,22 +107,21 @@
             if 'Trace' in layer.layer.data.meta:
                 return "mdi-chart-line-stacked", ""
 
             # then the underlying data is cube-like and we're in the profile viewer, so we
             # want to include the collapse function *unless* the layer is a spectral subset
             for subset in self.jdaviz_app.data_collection.subset_groups:
                 if subset.label == layer.layer.label:
-                    if isinstance(subset.subset_state, RoiSubsetState):
+                    subset_type = get_subset_type(subset)
+                    if subset_type == 'spatial':
                         return "mdi-chart-scatter-plot", suffix
                     else:
                         return "mdi-chart-bell-curve", ""
             return "", suffix
 
-            return '', ''
-
         visible_layers = {}
         for layer in self.state.layers[::-1]:
             if layer.visible:
                 prefix_icon, suffix = _get_layer_info(layer)
                 visible_layers[layer.layer.label] = {'color': _get_layer_color(layer),
                                                      'linewidth': _get_layer_linewidth(layer),
                                                      'prefix_icon': prefix_icon,
@@ -215,13 +216,21 @@
 
     @property
     def jdaviz_helper(self):
         """The Jdaviz configuration helper tied to the viewer."""
         return self.jdaviz_app._jdaviz_helper
 
     @property
+    def hub(self):
+        return self.session.hub
+
+    @property
     def reference_id(self):
         return self._reference_id
 
     @property
     def reference(self):
         return self.jdaviz_app._viewer_item_by_id(self.reference_id).get('reference')
+
+    def set_plot_axes(self):
+        # individual viewers can override to set custom axes labels/ticks/styling
+        return
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/helper.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/imviz.yaml` & `jdaviz-3.6.0/jdaviz/configs/imviz/imviz.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,44 @@
 import os
 import warnings
 from datetime import datetime
 
 import astropy
-import bqplot
 import numpy as np
 from astropy import units as u
 from astropy.modeling.fitting import LevMarLSQFitter
 from astropy.modeling import Parameter
 from astropy.modeling.models import Gaussian1D
 from astropy.time import Time
 from glue.core.message import SubsetUpdateMessage
 from ipywidgets import widget_serialization
 from packaging.version import Version
 from photutils.aperture import (ApertureStats, CircularAperture, EllipticalAperture,
                                 RectangularAperture)
-from regions import (CircleAnnulusPixelRegion, CirclePixelRegion, EllipsePixelRegion,
-                     RectanglePixelRegion)
 from traitlets import Any, Bool, Integer, List, Unicode, observe
 
-from jdaviz.core.custom_traitlets import FloatHandleEmpty
 from jdaviz.core.events import SnackbarMessage, LinkUpdatedMessage
 from jdaviz.core.region_translators import regions2aperture, _get_region_from_spatial_subset
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import (PluginTemplateMixin, DatasetSelectMixin,
-                                        SubsetSelect, TableMixin)
-from jdaviz.utils import bqplot_clear_figure, PRIHDR_KEY
+                                        SubsetSelect, TableMixin, PlotMixin)
+from jdaviz.utils import PRIHDR_KEY
 
 __all__ = ['SimpleAperturePhotometry']
 
 
 @tray_registry('imviz-aper-phot-simple', label="Imviz Simple Aperture Photometry")
-class SimpleAperturePhotometry(PluginTemplateMixin, DatasetSelectMixin, TableMixin):
+class SimpleAperturePhotometry(PluginTemplateMixin, DatasetSelectMixin, TableMixin, PlotMixin):
     template_file = __file__, "aper_phot_simple.vue"
     subset_items = List([]).tag(sync=True)
     subset_selected = Unicode("").tag(sync=True)
     subset_area = Integer().tag(sync=True)
     bg_subset_items = List().tag(sync=True)
     bg_subset_selected = Unicode("").tag(sync=True)
     background_value = Any(0).tag(sync=True)
-    bg_annulus_inner_r = FloatHandleEmpty(0).tag(sync=True)
-    bg_annulus_width = FloatHandleEmpty(10).tag(sync=True)
     pixel_area = Any(0).tag(sync=True)
     counts_factor = Any(0).tag(sync=True)
     flux_scaling = Any(0).tag(sync=True)
     result_available = Bool(False).tag(sync=True)
     result_failed_msg = Unicode("").tag(sync=True)
     results = List().tag(sync=True)
     plot_types = List([]).tag(sync=True)
@@ -57,41 +51,44 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.subset = SubsetSelect(self,
                                    'subset_items',
                                    'subset_selected',
                                    default_text=None,
-                                   allowed_type='spatial')
+                                   filters=['is_spatial', 'is_not_composite', 'is_not_annulus'])
 
         self.bg_subset = SubsetSelect(self,
                                       'bg_subset_items',
                                       'bg_subset_selected',
                                       default_text='Manual',
-                                      manual_options=['Manual', 'Annulus'],
-                                      allowed_type='spatial')
+                                      manual_options=['Manual'],
+                                      filters=['is_spatial', 'is_not_composite'])
 
         headers = ['xcenter', 'ycenter', 'sky_center',
                    'sum', 'sum_aper_area',
                    'aperture_sum_counts', 'aperture_sum_counts_err',
                    'aperture_sum_mag',
                    'min', 'max', 'mean', 'median', 'mode', 'std', 'mad_std', 'var',
                    'biweight_location', 'biweight_midvariance', 'fwhm',
                    'semimajor_sigma', 'semiminor_sigma', 'orientation', 'eccentricity',
                    'data_label', 'subset_label']
         self.table.headers_avail = headers
         self.table.headers_visible = headers
 
         self._selected_data = None
         self._selected_subset = None
-        self._fig = bqplot.Figure()
         self.plot_types = ["Curve of Growth", "Radial Profile", "Radial Profile (Raw)"]
         self.current_plot_type = self.plot_types[0]
         self._fitted_model_name = 'phot_radial_profile'
 
+        self.plot.add_line('line', color='gray', marker_size=32)
+        self.plot.add_scatter('scatter', color='gray', default_size=1)
+        self.plot.add_line('fit_line', color='magenta', line_style='dashed')
+
         self.session.hub.subscribe(self, SubsetUpdateMessage, handler=self._on_subset_update)
         self.session.hub.subscribe(self, LinkUpdatedMessage, handler=self._on_link_update)
 
     @observe('dataset_selected')
     def _dataset_selected_changed(self, event={}):
         try:
             self._selected_data = self.dataset.selected_dc_item
@@ -155,38 +152,26 @@
         elif sbst.label == self.bg_subset_selected and sbst.data.label == self.dataset_selected:
             self._bg_subset_selected_changed()
 
     def _on_link_update(self, msg):
         if self.dataset_selected == '' or self.subset_selected == '':
             return
 
-        # Force background auto-calculation (including annulus) to update when linking has changed.
+        # Force background auto-calculation to update when linking has changed.
         self._subset_selected_changed()
 
     @observe('subset_selected')
     def _subset_selected_changed(self, event={}):
         subset_selected = event.get('new', self.subset_selected)
         if self._selected_data is None or subset_selected == '':
             return
 
         try:
             self._selected_subset = _get_region_from_spatial_subset(self, subset_selected)
             self._selected_subset.meta['label'] = subset_selected
-
-            if isinstance(self._selected_subset, CirclePixelRegion):
-                self.bg_annulus_inner_r = self._selected_subset.radius
-            elif isinstance(self._selected_subset, EllipsePixelRegion):
-                self.bg_annulus_inner_r = max(self._selected_subset.width,
-                                              self._selected_subset.height) * 0.5
-            elif isinstance(self._selected_subset, RectanglePixelRegion):
-                self.bg_annulus_inner_r = np.sqrt(self._selected_subset.width ** 2 +
-                                                  self._selected_subset.height ** 2) * 0.5
-            else:  # pragma: no cover
-                raise TypeError(f'Unsupported region shape: {self._selected_subset.__class__}')
-
             self.subset_area = int(np.ceil(self._selected_subset.area))
 
         except Exception as e:
             self._selected_subset = None
             self.hub.broadcast(SnackbarMessage(
                 f"Failed to extract {subset_selected}: {repr(e)}", color='error', sender=self))
 
@@ -200,38 +185,20 @@
         comp = data.get_component(data.main_components[0])
         aper_mask_stat = reg.to_mask(mode='center')
         img_stat = aper_mask_stat.get_values(comp.data, mask=None)
 
         # photutils/background/_utils.py --> nanmedian()
         return np.nanmedian(img_stat)  # Naturally in data unit
 
-    @observe('bg_annulus_inner_r', 'bg_annulus_width')
-    def _bg_annulus_updated(self, *args):
-        if self.bg_subset_selected != 'Annulus':
-            return
-
-        try:
-            inner_r = float(self.bg_annulus_inner_r)
-            reg = CircleAnnulusPixelRegion(
-                self._selected_subset.center, inner_radius=inner_r,
-                outer_radius=inner_r + float(self.bg_annulus_width))
-            self.background_value = self._calc_bg_subset_median(reg)
-
-        except Exception:  # Error snackbar suppressed to prevent excessive queue.
-            self.background_value = 0
-
     @observe('bg_subset_selected')
     def _bg_subset_selected_changed(self, event={}):
         bg_subset_selected = event.get('new', self.bg_subset_selected)
         if bg_subset_selected == 'Manual':
             # we'll later access the user's self.background_value directly
             return
-        if bg_subset_selected == 'Annulus':
-            self._bg_annulus_updated()
-            return
 
         try:
             reg = _get_region_from_spatial_subset(self, bg_subset_selected)
             self.background_value = self._calc_bg_subset_median(reg)
         except Exception as e:
             self.background_value = 0
             self.hub.broadcast(SnackbarMessage(
@@ -341,56 +308,48 @@
                 self.table.add_item(phot_table)
             except Exception:  # Discard incompatible QTable
                 self.table.clear_table()
                 phot_table['id'][0] = 1
                 self.table.add_item(phot_table)
 
             # Plots.
-            # TODO: Jenn wants title at bottom.
-            bqplot_clear_figure(self._fig)
-            self._fig.title_style = {'font-size': '12px'}
-            # NOTE: default margin in bqplot is 60 in all directions
-            self._fig.fig_margin = {'top': 60, 'bottom': 60, 'left': 40, 'right': 10}
-            line_x_sc = bqplot.LinearScale()
-            line_y_sc = bqplot.LinearScale()
+            line = self.plot.marks['line']
+            sc = self.plot.marks['scatter']
+            fit_line = self.plot.marks['fit_line']
 
             if self.current_plot_type == "Curve of Growth":
-                self._fig.title = 'Curve of growth from aperture center'
+                self.plot.figure.title = 'Curve of growth from aperture center'
                 x_arr, sum_arr, x_label, y_label = _curve_of_growth(
                     comp_data, (xcenter, ycenter), aperture, phot_table['sum'][0],
                     wcs=data.coords, background=bg, pixarea_fac=pixarea_fac)
-                self._fig.axes = [bqplot.Axis(scale=line_x_sc, label=x_label),
-                                  bqplot.Axis(scale=line_y_sc, orientation='vertical',
-                                              label=y_label)]
-                bqplot_line = bqplot.Lines(x=x_arr, y=sum_arr, marker='circle',
-                                           scales={'x': line_x_sc, 'y': line_y_sc},
-                                           marker_size=32, colors='gray')
-                bqplot_marks = [bqplot_line]
+                line.x, line.y = x_arr, sum_arr
+                self.plot.clear_marks('scatter', 'fit_line')
+                self.plot.figure.axes[0].label = x_label
+                self.plot.figure.axes[1].label = y_label
 
             else:  # Radial profile
-                self._fig.axes = [bqplot.Axis(scale=line_x_sc, label='pix'),
-                                  bqplot.Axis(scale=line_y_sc, orientation='vertical',
-                                              label=comp.units or 'Value')]
+                self.plot.figure.axes[0].label = 'pix'
+                self.plot.figure.axes[1].label = comp.units or 'Value'
 
                 if self.current_plot_type == "Radial Profile":
-                    self._fig.title = 'Radial profile from aperture center'
+                    self.plot.figure.title = 'Radial profile from aperture center'
                     x_data, y_data = _radial_profile(
                         phot_aperstats.data_cutout, phot_aperstats.bbox, (xcenter, ycenter),
                         raw=False)
-                    bqplot_line = bqplot.Lines(x=x_data, y=y_data, marker='circle',
-                                               scales={'x': line_x_sc, 'y': line_y_sc},
-                                               marker_size=32, colors='gray')
+                    line.x, line.y = x_data, y_data
+                    self.plot.clear_marks('scatter')
+
                 else:  # Radial Profile (Raw)
-                    self._fig.title = 'Raw radial profile from aperture center'
+                    self.plot.figure.title = 'Raw radial profile from aperture center'
                     x_data, y_data = _radial_profile(
                         phot_aperstats.data_cutout, phot_aperstats.bbox, (xcenter, ycenter),
                         raw=True)
-                    bqplot_line = bqplot.Scatter(x=x_data, y=y_data, marker='circle',
-                                                 scales={'x': line_x_sc, 'y': line_y_sc},
-                                                 default_size=1, colors='gray')
+
+                    sc.x, sc.y = x_data, y_data
+                    self.plot.clear_marks('line')
 
                 # Fit Gaussian1D to radial profile data.
                 if self.fit_radial_profile:
                     fitter = LevMarLSQFitter()
                     y_max = y_data.max()
                     x_mean = x_data[np.where(y_data == y_max)].mean()
                     std = 0.5 * (phot_table['semimajor_sigma'][0] +
@@ -408,29 +367,25 @@
                         fit_model = fitter(gs, x_data, y_data, **fitter_kw)
                     if len(warns) > 0:
                         msg = os.linesep.join([str(w.message) for w in warns])
                         self.hub.broadcast(SnackbarMessage(
                             f"Radial profile fitting: {msg}", color='warning', sender=self))
                     y_fit = fit_model(x_data)
                     self.app.fitted_models[self._fitted_model_name] = fit_model
-                    bqplot_fit = bqplot.Lines(x=x_data, y=y_fit, marker=None,
-                                              scales={'x': line_x_sc, 'y': line_y_sc},
-                                              colors='magenta', line_style='dashed')
-                    bqplot_marks = [bqplot_line, bqplot_fit]
+                    fit_line.x, fit_line.y = x_data, y_fit
                 else:
-                    bqplot_marks = [bqplot_line]
+                    self.plot.clear_marks('fit_line')
 
         except Exception as e:  # pragma: no cover
-            bqplot_clear_figure(self._fig)
+            self.plot.clear_all_marks()
             msg = f"Aperture photometry failed: {repr(e)}"
             self.hub.broadcast(SnackbarMessage(msg, color='error', sender=self))
             self.result_failed_msg = msg
         else:
             self.result_failed_msg = ''
-            self._fig.marks = bqplot_marks
 
             # Parse results for GUI.
             tmp = []
             for key in phot_table.colnames:
                 if key in ('id', 'data_label', 'subset_label', 'background', 'pixarea_tot',
                            'counts_fac', 'aperture_sum_counts_err', 'flux_scaling', 'timestamp'):
                     continue
@@ -460,16 +415,14 @@
                     if isinstance(p_val, Parameter):
                         p_val = p_val.value
                     fit_tmp.append({'function': param, 'result': f'{p_val:.4e}'})
 
             self.results = tmp
             self.fit_results = fit_tmp
             self.result_available = True
-            self.radial_plot = self._fig
-            self.bqplot_figs_resize = [self._fig]
             self.plot_available = True
 
 
 # NOTE: These are hidden because the APIs are for internal use only
 # but we need them as a separate functions for unit testing.
 
 def _radial_profile(radial_cutout, reg_bb, centroid, raw=False):
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue`

 * *Files 12% similar despite different names*

```diff
@@ -14,56 +14,32 @@
 
     <div v-if='dataset_selected'>
       <plugin-subset-select
         :items="subset_items"
         :selected.sync="subset_selected"
         :show_if_single_entry="true"
         label="Aperture"
-        hint="Select aperture region for photometry."
+        hint="Select aperture region for photometry (cannot be an annulus or composite subset)."
       />
 
       <div v-if="subset_selected">
         <plugin-subset-select
           :items="bg_subset_items"
           :selected.sync="bg_subset_selected"
           :show_if_single_entry="true"
           label="Background"
-          hint="Select subset region for background calculation."
+          hint="Select subset region for background calculation (cannot be a composite subset)."
         />
 
         <v-row v-if="subset_selected === bg_subset_selected">
           <span class="v-messages v-messages__message text--secondary" style="color: red !important">
               Background and aperture cannot be set to the same subset
           </span>
         </v-row>
 
-        <v-row v-if="bg_subset_selected=='Annulus'">
-          <v-text-field
-            label="Annulus inner radius"
-            v-model.number="bg_annulus_inner_r"
-            type="number"
-            :rules="[() => bg_annulus_inner_r>0 || 'Must be positive.']"
-            hint="Background annulus inner radius in pixels"
-            persistent-hint
-          >
-          </v-text-field>
-        </v-row>
-
-        <v-row v-if="bg_subset_selected=='Annulus'">
-          <v-text-field
-            label="Annulus width"
-            v-model.number="bg_annulus_width"
-            type="number"
-            :rules="[() => bg_annulus_width>0 || 'Must be positive.']"
-            hint="Background annulus width in pixels (inner radius + width = outer radius)"
-            persistent-hint
-          >
-          </v-text-field>
-        </v-row>
-
         <v-row>
           <v-text-field
             label="Background value"
             v-model.number="background_value"
             type="number"
             hint="Background to subtract, same unit as data"
             :disabled="bg_subset_selected!='Manual'"
@@ -142,18 +118,15 @@
     <v-row v-if="result_failed_msg.length > 0">
       <span class="v-messages v-messages__message text--secondary" style="color: red !important">
           <b>WARNING</b>: {{result_failed_msg}}
       </span>
     </v-row>
 
     <v-row v-if="plot_available">
-      <!-- NOTE: the internal bqplot widget defaults to 480 pixels, so if choosing something else,
-           we will likely need to override that with custom CSS rules in order to avoid the initial
-           rendering of the plot from overlapping with content below -->
-      <jupyter-widget :widget="radial_plot" style="width: 100%; height: 480px" />
+      <jupyter-widget :widget="plot_widget"/> 
     </v-row>
 
     <div v-if="plot_available && fit_radial_profile && current_plot_type != 'Curve of Growth'">
       <j-plugin-section-header>Gaussian Fit Results</j-plugin-section-header>
       <v-row no-gutters>
         <v-col cols=6><U>Result</U></v-col>
         <v-col cols=6><U>Value</U></v-col>
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/compass.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/compass.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.show`
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.open_in_tray`
     * ``viewer`` (:class:`~jdaviz.core.template_mixin.ViewerSelect`):
       Viewer to show orientation/compass information.
     * ``data_label``: label of the top-layer shown in the compass (read-only)
     """
     template_file = __file__, "compass.vue"
+    uses_active_status = Bool(True).tag(sync=True)
+
     icon = Unicode("").tag(sync=True)
     data_label = Unicode("").tag(sync=True)
     img_data = Unicode("").tag(sync=True)
     canvas_angle = Float(0).tag(sync=True)  # set by canvas rotation plugin
     canvas_flip_horizontal = Bool(False).tag(sync=True)  # set by canvas rotation plugin
 
     def __init__(self, *args, **kwargs):
@@ -36,18 +38,14 @@
         self.hub.subscribe(self, RemoveDataMessage, handler=self._on_viewer_data_changed)
         self.hub.subscribe(self, CanvasRotationChangedMessage, handler=self._on_canvas_rotation_changed)  # noqa
 
     @property
     def user_api(self):
         return PluginUserApi(self, expose=('viewer',), readonly=('data_label',))
 
-    def show(self, *args, **kwargs):
-        super().show(*args, **kwargs)
-        self._compass_with_new_viewer(from_show=True)
-
     def _on_viewer_data_changed(self, msg=None):
         if self.viewer_selected:
             viewer = self.viewer.selected_obj
             viewer.on_limits_change()  # Force redraw
 
     def _on_canvas_rotation_changed(self, msg=None):
         viewer_id = msg.viewer_id
@@ -57,23 +55,23 @@
         self._set_compass_rotation()
 
     def _set_compass_rotation(self):
         viewer_item = self.app._viewer_item_by_id(self.viewer.selected_id)
         self.canvas_angle = viewer_item.get('canvas_angle', 0)  # noqa
         self.canvas_flip_horizontal = viewer_item.get('canvas_flip_horizontal', False)
 
-    @observe("viewer_selected", "plugin_opened")
+    @observe("viewer_selected", "is_active")
     def _compass_with_new_viewer(self, *args, **kwargs):
         if not hasattr(self, 'viewer'):
             # mixin object not yet initialized
             return
 
         # There can be only one!
         for vid, viewer in self.app._viewer_store.items():
-            if vid == self.viewer.selected_id and (self.plugin_opened or kwargs.get('from_show')):
+            if vid == self.viewer.selected_id and self.plugin_opened:
                 viewer.compass = self
                 viewer.on_limits_change()  # Force redraw
 
                 self._set_compass_rotation()
             else:
                 viewer.compass = None
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/compass.vue` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/compass.vue`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 <template>
   <j-tray-plugin
     description='Show active data label, compass, and zoom box.'
     :link="'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#compass'"
+    :uses_active_status="uses_active_status"
+    @plugin-ping="plugin_ping($event)"
     :popout_button="popout_button">
 
     <plugin-viewer-select
       :items="viewer_items"
       :selected.sync="viewer_selected"
       label="Viewer"
       hint="Select a viewer to show."
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import math
 import numpy as np
 from traitlets import Bool, Unicode, observe
 
 from astropy import units as u
 from glue.core import BaseData
-from glue.core.subset import RoiSubsetState
 from glue.core.subset_group import GroupedSubset
 from glue_jupyter.bqplot.image.layer_artist import BqplotImageSubsetLayerArtist
 
 from jdaviz.configs.cubeviz.plugins.viewers import CubevizImageView
 from jdaviz.configs.imviz.plugins.viewers import ImvizImageView
 from jdaviz.configs.mosviz.plugins.viewers import MosvizImageView, MosvizProfile2DView
 from jdaviz.configs.specviz.plugins.viewers import SpecvizProfileView
 from jdaviz.core.events import ViewerAddedMessage
 from jdaviz.core.helpers import data_has_valid_wcs
 from jdaviz.core.marks import PluginScatter
 from jdaviz.core.registries import tool_registry
 from jdaviz.core.template_mixin import TemplateMixin, DatasetSelectMixin
+from jdaviz.utils import get_subset_type
 
 __all__ = ['CoordsInfo']
 
 
 @tool_registry('g-coords-info')
 class CoordsInfo(TemplateMixin, DatasetSelectMixin):
     template_file = __file__, "coords_info.vue"
@@ -395,21 +395,18 @@
             self._dict['value:unreliable'] = unreliable_pixel
         else:
             self.row1b_title = ''
             self.row1b_text = ''
 
     def _spectrum_viewer_update(self, viewer, x, y):
         def _cursor_fallback():
-            statistic = getattr(viewer.state, 'function', None)
-            cache_key = (viewer.state.layers[0].layer.label, statistic)
-            sp = self.app._get_object_cache.get(cache_key, viewer.data()[0])
             self._dict['axes_x'] = x
-            self._dict['axes_x:unit'] = sp.spectral_axis.unit.to_string()
+            self._dict['axes_x:unit'] = viewer.state.x_display_unit
             self._dict['axes_y'] = y
-            self._dict['axes_y:unit'] = sp.flux.unit.to_string()
+            self._dict['axes_y:unit'] = viewer.state.y_display_unit
             self._dict['data_label'] = ''
 
         def _copy_axes_to_spectral():
             self._dict['spectral_axis'] = self._dict['axes_x']
             self._dict['spectral_axis:unit'] = self._dict['axes_x:unit']
             self._dict['value'] = self._dict['axes_y']
             self._dict['value:unit'] = self._dict['axes_y:unit']
@@ -424,16 +421,14 @@
         if self.dataset.selected == 'none':
             self.row2_title = '\u00A0'
             self.row2_text = ''
             self.row3_title = '\u00A0'
             self.row3_text = ''
             self.icon = 'mdi-cursor-default'
             self.marks[viewer._reference_id].visible = False
-            # get the units from the first layer
-            # TODO: replace with display units once implemented
             _cursor_fallback()
             _copy_axes_to_spectral()
             return
 
         # Snap to the closest data point, not the actual mouse location.
         sp = None
         closest_i = None
@@ -444,15 +439,19 @@
         for lyr in viewer.state.layers:
             if self.dataset.selected == 'auto' and not lyr.visible:
                 continue
             if self.dataset.selected != 'auto' and self.dataset.selected != lyr.layer.label:
                 continue
 
             if isinstance(lyr.layer, GroupedSubset):
-                if not isinstance(lyr.layer.subset_state, RoiSubsetState):
+                subset_state = getattr(lyr.layer, 'subset_state', None)
+                if subset_state is None:
+                    continue
+                subset_type = get_subset_type(subset_state)
+                if subset_type == 'spectral':
                     # then this is a SPECTRAL subset
                     continue
                 # For use later in data retrieval
                 subset_label = lyr.layer.label
                 data_label = lyr.layer.data.label
             elif ((not isinstance(lyr.layer, BaseData)) or (lyr.layer.ndim not in (1, 3))):
                 continue
@@ -465,28 +464,33 @@
                 # But if not (maybe user changed statistic), we cache it here too.
                 statistic = getattr(viewer.state, 'function', None)
                 cache_key = (lyr.layer.label, statistic)
                 if cache_key in self.app._get_object_cache:
                     sp = self.app._get_object_cache[cache_key]
                 else:
                     sp = self._specviz_helper.get_data(data_label=data_label,
-                                                       subset_to_apply=subset_label)
+                                                       spatial_subset=subset_label)
                     self.app._get_object_cache[cache_key] = sp
 
+                # Calculations have to happen in the frame of viewer display units.
+                disp_wave = sp.spectral_axis.to_value(viewer.state.x_display_unit, u.spectral())
+                disp_flux = sp.flux.to_value(viewer.state.y_display_unit,
+                                             u.spectral_density(sp.spectral_axis))
+
                 # Out of range in spectral axis.
                 if (self.dataset.selected != lyr.layer.label and
-                        (x < sp.spectral_axis.value.min() or x > sp.spectral_axis.value.max())):
+                        (x < disp_wave.min() or x > disp_wave.max())):
                     continue
 
-                cur_i = np.argmin(abs(sp.spectral_axis.value - x))
-                cur_wave = sp.spectral_axis[cur_i]
-                cur_flux = sp.flux[cur_i]
+                cur_i = np.argmin(abs(disp_wave - x))
+                cur_wave = disp_wave[cur_i]
+                cur_flux = disp_flux[cur_i]
 
-                dx = cur_wave.value - x
-                dy = cur_flux.value - y
+                dx = cur_wave - x
+                dy = cur_flux - y
                 cur_distance = math.sqrt(dx * dx + dy * dy)
                 if (closest_distance is None) or (cur_distance < closest_distance):
                     closest_distance = cur_distance
                     closest_i = cur_i
                     closest_wave = cur_wave
                     closest_flux = cur_flux
                     closest_icon = self.app.state.layer_icons.get(lyr.layer.label, '')
@@ -503,31 +507,38 @@
             self.icon = 'mdi-cursor-default'
             self.marks[viewer._reference_id].visible = False
             _cursor_fallback()
             _copy_axes_to_spectral()
             return
 
         self.row2_title = 'Wave'
-        self.row2_text = f'{closest_wave.value:10.5e} {closest_wave.unit.to_string()}'
-        self._dict['axes_x'] = closest_wave.value
-        self._dict['axes_x:unit'] = closest_wave.unit.to_string()
-        if closest_wave.unit != u.pix:
+        self.row2_text = f'{closest_wave:10.5e} {viewer.state.x_display_unit}'
+        self._dict['axes_x'] = closest_wave
+        self._dict['axes_x:unit'] = viewer.state.x_display_unit
+        if viewer.state.x_display_unit != u.pix:
             self.row2_text += f' ({int(closest_i)} pix)'
             if self.app.config == 'cubeviz':
                 # float to be compatible with nan
                 self._dict['slice'] = float(closest_i)
-                self._dict['spectral_axis'] = closest_wave.value
-                self._dict['spectral_axis:unit'] = closest_wave.unit.to_string()
+                self._dict['spectral_axis'] = closest_wave
+                self._dict['spectral_axis:unit'] = viewer.state.x_display_unit
             else:
                 # float to be compatible with nan
                 self._dict['index'] = float(closest_i)
 
+        if viewer.state.y_display_unit is None:
+            flux_unit = ""
+        else:
+            flux_unit = viewer.state.y_display_unit
         self.row3_title = 'Flux'
-        self.row3_text = f'{closest_flux.value:10.5e} {closest_flux.unit.to_string()}'
-        self._dict['axes_y'] = closest_flux.value
-        self._dict['axes_y:unit'] = closest_flux.unit.to_string()
+        self.row3_text = f'{closest_flux:10.5e} {flux_unit}'
+        self._dict['axes_y'] = closest_flux
+        self._dict['axes_y:unit'] = viewer.state.y_display_unit
 
-        self.icon = closest_icon
+        if closest_icon is not None:
+            self.icon = closest_icon
+        else:
+            self.icon = ""
 
-        self.marks[viewer._reference_id].update_xy([closest_wave.value], [closest_flux.value])  # noqa
+        self.marks[viewer._reference_id].update_xy([closest_wave], [closest_flux])
         self.marks[viewer._reference_id].visible = True
         _copy_axes_to_spectral()
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,98 @@
-import bqplot
-from ipywidgets import widget_serialization
-from traitlets import Any, Bool, List, Unicode, observe
+from traitlets import Any, Bool, Unicode, observe
 
 from jdaviz.configs.imviz.helper import get_top_layer_index
-from jdaviz.core.events import ViewerAddedMessage, ViewerRemovedMessage
+from jdaviz.core.events import ViewerAddedMessage
 from jdaviz.core.registries import tray_registry
-from jdaviz.core.template_mixin import PluginTemplateMixin
-from jdaviz.utils import bqplot_clear_figure
+from jdaviz.core.template_mixin import PluginTemplateMixin, ViewerSelectMixin, Plot
 
 __all__ = ['LineProfileXY']
 
 
 @tray_registry('imviz-line-profile-xy', label="Imviz Line Profiles (XY)")
-class LineProfileXY(PluginTemplateMixin):
+class LineProfileXY(PluginTemplateMixin, ViewerSelectMixin):
     template_file = __file__, "line_profile_xy.vue"
-    viewer_items = List([]).tag(sync=True)
-    selected_viewer = Unicode("").tag(sync=True)
+    uses_active_status = Bool(True).tag(sync=True)
+
     plot_available = Bool(False).tag(sync=True)
     selected_x = Any('').tag(sync=True)
     selected_y = Any('').tag(sync=True)
-    line_plot_across_x = Any('').tag(sync=True, **widget_serialization)
-    line_plot_across_y = Any('').tag(sync=True, **widget_serialization)
+
+    plot_across_x_widget = Unicode().tag(sync=True)
+    plot_across_y_widget = Unicode().tag(sync=True)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._default_viewer = f'{self.app.config}-0'
-
-        self.hub.subscribe(self, ViewerAddedMessage, handler=self._on_viewers_changed)
-        self.hub.subscribe(self, ViewerRemovedMessage, handler=self._on_viewers_changed)
 
-        self._figs = [bqplot.Figure(), bqplot.Figure()]
-        self._on_viewers_changed()  # Populate it on start-up
+        self.plot_across_x = Plot(self)
+        self.plot_across_x.add_line('line', color='gray')
+        self.plot_across_x.figure.axes[0].label = 'Y (pix)'
+        self.plot_across_x_widget = 'IPY_MODEL_'+self.plot_across_x.model_id
+
+        self.plot_across_y = Plot(self)
+        self.plot_across_y.add_line('line', color='gray')
+        self.plot_across_y.figure.axes[0].label = 'X (pix)'
+        self.plot_across_y_widget = 'IPY_MODEL_'+self.plot_across_y.model_id
 
-    def _on_viewers_changed(self, msg=None):
-        self.viewer_items = self.app.get_viewer_ids()
-
-        # Selected viewer was removed but Imviz always has a default viewer to fall back on.
-        if self.selected_viewer not in self.viewer_items:
-            self.selected_viewer = self._default_viewer
+        self.hub.subscribe(self, ViewerAddedMessage, handler=self._on_viewer_added)
 
     def reset_results(self):
         self.plot_available = False
-        self.line_plot_across_x = ''
-        self.line_plot_across_y = ''
-        for fig in self._figs:
-            bqplot_clear_figure(fig)
+        self.plot_across_x.clear_all_marks()
+        self.plot_across_y.clear_all_marks()
+
+    def _create_viewer_callbacks(self, viewer):
+        if not self.is_active:
+            return
 
-    # This is also triggered from viewer code.
-    @observe("selected_viewer")
+        callback = self._viewer_callback(viewer, self._on_viewer_key_event)
+        viewer.add_event_callback(callback, events=['keydown'])
+
+    def _on_viewer_added(self, msg):
+        self._create_viewer_callbacks(self.app.get_viewer_by_id(msg.viewer_id))
+
+    @observe('is_active')
+    def on_is_active_changed(self, *args):
+        # subscribe/unsubscribe to keypress events across all viewers
+        for viewer in self.app._viewer_store.values():
+            if not hasattr(viewer, 'figure'):
+                # table viewer, etc
+                continue
+            callback = self._viewer_callback(viewer, self._on_viewer_key_event)
+
+            if self.is_active:
+                viewer.add_event_callback(callback, events=['keydown'])
+            else:
+                viewer.remove_event_callback(callback)
+
+        if self.is_active:
+            self.vue_draw_plot()
+
+    def _on_viewer_key_event(self, viewer, data):
+        if data['key'] == 'l':
+            image = viewer.active_image_layer.layer
+            x = data['domain']['x']
+            y = data['domain']['y']
+            if x is None or y is None:  # Out of bounds
+                return
+            x, y, _, _ = viewer._get_real_xy(image, x, y)
+            self.selected_x = x
+            self.selected_y = y
+            self.viewer_selected = viewer.reference_id
+            # TODO: remove manual calls to vue_draw_plot and trigger
+            # by changes to selected_x/selected_y as well as viewer_selected
+            self.vue_draw_plot()
+
+    @observe("viewer_selected")
     def vue_draw_plot(self, *args, **kwargs):
         """Draw line profile plots for given Data across given X and Y indices (0-indexed)."""
-        if not self.selected_x or not self.selected_y or not self.plugin_opened:
+        if not self.selected_x or not self.selected_y or not self.is_active:
             return
 
-        viewer = self.app.get_viewer_by_id(self.selected_viewer)
+        viewer = self.viewer.selected_obj
         i = get_top_layer_index(viewer)
         data = viewer.state.layers[i].layer
 
         # Can be str if passed in from Vue.js
         x = int(round(float(self.selected_x)))
         y = int(round(float(self.selected_y)))
 
@@ -77,55 +112,34 @@
 
         comp = data.get_component(data.main_components[0])
         if comp.units:
             y_label = comp.units
         else:
             y_label = 'Value'
 
-        # Clear bqplot figures.
-        fig_x = self._figs[0]
-        bqplot_clear_figure(fig_x)
-        fig_y = self._figs[1]
-        bqplot_clear_figure(fig_y)
-
-        fig_x.title = f'X={x}'
-        fig_x.title_style = {'font-size': '12px'}
-        fig_x.fig_margin = {'top': 60, 'bottom': 60, 'left': 40, 'right': 10}
-        line_x_x_sc = bqplot.LinearScale()
-        line_x_y_sc = bqplot.LinearScale()
-        line_x = bqplot.Lines(x=range(comp.data.shape[0]), y=comp.data[:, x],
-                              scales={'x': line_x_x_sc, 'y': line_x_y_sc}, colors='gray')
-        fig_x.marks = [line_x]
-        fig_x.axes = [bqplot.Axis(scale=line_x_x_sc, label='Y (pix)'),
-                      bqplot.Axis(scale=line_x_y_sc, orientation='vertical', label=y_label)]
-        line_x.scales['x'].min = y_min
-        line_x.scales['x'].max = y_max
+        self.plot_across_x.figure.title = f'X={x}'
+        line_x = self.plot_across_x.marks['line']
+        line_x.x, line_x.y = range(comp.data.shape[0]), comp.data[:, x]
+        line_x.scales['x'].min, line_x.scales['x'].max = y_min, y_max
+        self.plot_across_x.figure.axes[1].label = y_label
+
         y_min = max(int(y_min), 0)
         y_max = min(int(y_max), ny)
         zoomed_data_x = comp.data[y_min:y_max, x]
         if zoomed_data_x.size > 0:
             line_x.scales['y'].min = zoomed_data_x.min() * 0.95
             line_x.scales['y'].max = zoomed_data_x.max() * 1.05
 
-        fig_y.title = f'Y={y}'
-        fig_y.title_style = {'font-size': '12px'}
-        fig_y.fig_margin = {'top': 60, 'bottom': 60, 'left': 40, 'right': 10}
-        line_y_x_sc = bqplot.LinearScale()
-        line_y_y_sc = bqplot.LinearScale()
-        line_y = bqplot.Lines(x=range(comp.data.shape[1]), y=comp.data[y, :],
-                              scales={'x': line_y_x_sc, 'y': line_y_y_sc}, colors='gray')
-        fig_y.marks = [line_y]
-        fig_y.axes = [bqplot.Axis(scale=line_y_x_sc, label='X (pix)'),
-                      bqplot.Axis(scale=line_y_y_sc, orientation='vertical', label=y_label)]
-        line_y.scales['x'].min = x_min
-        line_y.scales['x'].max = x_max
+        self.plot_across_y.figure.title = f'Y={y}'
+        line_y = self.plot_across_y.marks['line']
+        line_y.x, line_y.y = range(comp.data.shape[1]), comp.data[y, :]
+        line_y.scales['x'].min, line_y.scales['x'].max = x_min, x_max
+        self.plot_across_y.figure.axes[1].label = y_label
+
         x_min = max(int(x_min), 0)
         x_max = min(int(x_max), nx)
         zoomed_data_y = comp.data[y, x_min:x_max]
         if zoomed_data_y.size > 0:
             line_y.scales['y'].min = zoomed_data_y.min() * 0.95
             line_y.scales['y'].max = zoomed_data_y.max() * 1.05
 
-        self.line_plot_across_x = fig_x
-        self.line_plot_across_y = fig_y
-        self.bqplot_figs_resize = self._figs
         self.plot_available = True
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,47 @@
 <template>
   <j-tray-plugin
     description='Press l to plot line profiles across X and Y under cursor. You can also manually enter X, Y and then click PLOT.'
     :link="'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#line-profiles'"
+    :uses_active_status="uses_active_status"
+    @plugin-ping="plugin_ping($event)"
     :popout_button="popout_button">
 
-    <v-row>
-      <v-select
-        attach
-        :menu-props="{ left: true }"
-        :items="viewer_items"
-        v-model="selected_viewer"
-        label="Viewer"
-        hint="Select a viewer to plot."
-        persistent-hint
-      ></v-select>
-    </v-row>
+    <plugin-viewer-select
+      :items="viewer_items"
+      :selected.sync="viewer_selected"
+      label="Viewer"
+      :show_if_single_entry="false"
+      hint="Select a viewer to plot."
+      persistent-hint
+    />
 
-    <v-row no-gutters>
-      <v-col>
-        <v-text-field
-          v-model='selected_x'
-          type="number"
-          label="X"
-          hint="Value of X"
-        ></v-text-field>
-      </v-col>
+    <v-row>
+      <v-text-field
+        v-model='selected_x'
+        type="number"
+        label="X"
+        hint="Value of X"
+      ></v-text-field>
     </v-row>
 
-    <v-row no-gutters>
-      <v-col>
-        <v-text-field
-          v-model='selected_y'
-          type="number"
-          label="Y"
-          hint="Value of Y"
-        ></v-text-field>
-      </v-col>
+    <v-row>
+      <v-text-field
+        v-model='selected_y'
+        type="number"
+        label="Y"
+        hint="Value of Y"
+      ></v-text-field>
     </v-row>
 
     <v-row justify="end">
       <v-btn color="primary" text @click="draw_plot">Plot</v-btn>
     </v-row>
 
     <v-row v-if="plot_available">
-      <!-- NOTE: the internal bqplot widget defaults to 480 pixels, so if choosing something else,
-           we will likely need to override that with custom CSS rules in order to avoid the initial
-           rendering of the plot from overlapping with content below -->
-      <jupyter-widget :widget="line_plot_across_x" style="width: 100%; height: 480px" />
+      <jupyter-widget :widget="plot_across_x_widget"/>
       <br/>
-      <jupyter-widget :widget="line_plot_across_y" style="width: 100%; height: 480px" />
+      <jupyter-widget :widget="plot_across_y_widget"/>
     </v-row>
 
   </j-tray-plugin>
 </template>
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/links_control/links_control.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/links_control/links_control.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/links_control/links_control.vue` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/links_control/links_control.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/parsers.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,19 @@
         elif file_obj_lower.endswith('.asdf'):
             if not HAS_ROMAN_DATAMODELS:
                 raise ImportError(
                     "ASDF detected but roman-datamodels is not installed."
                 )
             with rdd.open(file_obj) as pf:
                 _parse_image(app, pf, data_label, ext=ext)
+
+        elif file_obj_lower.endswith('.reg'):
+            # This will load DS9 regions as Subset but only if there is already data.
+            app._jdaviz_helper.load_regions_from_file(file_obj)
+
         else:  # Assume FITS
             with fits.open(file_obj) as pf:
                 _parse_image(app, pf, data_label, ext=ext)
     else:
         _parse_image(app, file_obj, data_label, ext=ext)
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/viewers.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/viewers.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 @viewer_registry("imviz-image-viewer", label="Image 2D (Imviz)")
 class ImvizImageView(JdavizViewerMixin, BqplotImageView, AstrowidgetsImageViewerMixin):
     # categories: zoom resets, zoom, pan, subset, select tools, shortcuts
     tools_nested = [
                     ['jdaviz:homezoom', 'jdaviz:prevzoom'],
                     ['jdaviz:boxzoommatch', 'jdaviz:boxzoom'],
                     ['jdaviz:panzoommatch', 'jdaviz:imagepanzoom'],
-                    ['bqplot:circle', 'bqplot:rectangle', 'bqplot:ellipse',
+                    ['bqplot:circle', 'bqplot:rectangle', 'bqplot:ellipse', 'bqplot:circannulus',
                      'jdaviz:singlepixelregion'],
                     ['jdaviz:blinkonce', 'jdaviz:contrastbias'],
                     ['jdaviz:sidebar_plot', 'jdaviz:sidebar_export', 'jdaviz:sidebar_compass']
                 ]
 
     default_class = None
     _state_cls = FreezableBqplotImageViewerState
@@ -75,27 +75,14 @@
 
         if data['event'] == 'keydown':
             key_pressed = data['key']
 
             if key_pressed in ('b', 'B'):
                 self.blink_once(reversed=key_pressed=='B')  # noqa: E225
 
-            elif key_pressed == 'l' and self.line_profile_xy.plugin_opened:
-                # Same data as mousemove above.
-                image = self.active_image_layer.layer
-                x = data['domain']['x']
-                y = data['domain']['y']
-                if x is None or y is None:  # Out of bounds
-                    return
-                x, y, _, _ = self._get_real_xy(image, x, y)
-                self.line_profile_xy.selected_x = x
-                self.line_profile_xy.selected_y = y
-                self.line_profile_xy.selected_viewer = self.reference_id
-                self.line_profile_xy.vue_draw_plot()
-
     def blink_once(self, reversed=False):
         # Simple blinking of images - this will make it so that only one
         # layer is visible at a time and cycles through the layers.
 
         # Exclude Subsets: They are global
         valid = [ilayer for ilayer, layer in enumerate(self.state.layers)
                  if layer_is_image_data(layer.layer)]
@@ -135,15 +122,15 @@
                 # Update line profile plots too.
                 if self.line_profile_xy is None:
                     try:
                         self.line_profile_xy = self.session.jdaviz_app.get_tray_item_from_name(
                             'imviz-line-profile-xy')
                     except KeyError:  # pragma: no cover
                         return
-                self.line_profile_xy.selected_viewer = self.reference_id
+                self.line_profile_xy.viewer_selected = self.reference_id
                 self.line_profile_xy.vue_draw_plot()
 
     def on_limits_change(self, *args):
         try:
             i = get_top_layer_index(self)
         except IndexError:
             if self.compass is not None:
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_astrowidgets_api.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_astrowidgets_api.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_catalogs.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_catalogs.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_helper.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     returned_data = imviz_helper.get_data(data_label)
     assert len(returned_data.shape) == 2
 
     # new image viewer created
     assert len(imviz_helper.app.get_viewer_ids()) == 2
 
     # there should be no data in the new viewer
-    assert len(imviz_helper.app.get_data_from_viewer(viewer_name)) == 0
+    assert len(imviz_helper.app.get_viewer(viewer_name).data()) == 0
 
     # then add data, and check that data were added to the new viewer
     imviz_helper.app.add_data_to_viewer(viewer_name, data_label)
-    assert len(imviz_helper.app.get_data_from_viewer(viewer_name)) == 1
+    assert len(imviz_helper.app.get_viewer(viewer_name).data()) == 1
 
     # remove data from the new viewer, check that it was removed
     imviz_helper.app.remove_data_from_viewer(viewer_name, data_label)
-    assert len(imviz_helper.app.get_data_from_viewer(viewer_name)) == 0
+    assert len(imviz_helper.app.get_viewer(viewer_name).data()) == 0
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_line_profile_xy.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_line_profile_xy.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,66 +8,67 @@
 
 class TestLineProfileXY(BaseImviz_WCS_NoWCS):
     def test_plugin_linked_by_pixel(self):
         """Go through plugin logic but does not check plot contents."""
         lp_plugin = self.imviz.app.get_tray_item_from_name('imviz-line-profile-xy')
         lp_plugin.plugin_opened = True
 
-        lp_plugin._on_viewers_changed()  # Populate plugin menu items.
-        assert lp_plugin.viewer_items == ['imviz-0']
-        assert lp_plugin.selected_viewer == 'imviz-0'
+        assert lp_plugin.viewer.labels == ['imviz-0']
+        assert lp_plugin.viewer_selected == 'imviz-0'
 
         # Plot attempt with null X/Y should not crash but also no-op.
-        assert not lp_plugin.line_plot_across_x
-        assert not lp_plugin.line_plot_across_y
+        assert len(lp_plugin.plot_across_x.marks['line'].x) == 0
+        assert len(lp_plugin.plot_across_y.marks['line'].x) == 0
         lp_plugin.vue_draw_plot()
         assert not lp_plugin.plot_available
 
         # Mimic "l" key pressed.
-        self.viewer.on_mouse_or_key_event(
-            {'event': 'keydown', 'key': 'l', 'domain': {'x': 5.1, 'y': 5}})
+        lp_plugin._on_viewer_key_event(self.viewer,
+                                       {'event': 'keydown', 'key': 'l',
+                                        'domain': {'x': 5.1, 'y': 5}})
         assert_allclose(lp_plugin.selected_x, 5.1)
         assert_allclose(lp_plugin.selected_y, 5)
-        assert lp_plugin.line_plot_across_x
-        assert lp_plugin.line_plot_across_y
+        assert len(lp_plugin.plot_across_x.marks['line'].x) > 0
+        assert len(lp_plugin.plot_across_y.marks['line'].x) > 0
         assert lp_plugin.plot_available
 
         # Add data with unit
         ndd = NDData(np.ones((10, 10)), unit=u.nJy)
         self.imviz.load_data(ndd, data_label='ndd', show_in_viewer=False)
 
         viewer_2 = self.imviz.create_image_viewer()
         self.imviz.app.add_data_to_viewer(viewer_2.reference_id, 'has_wcs[SCI,1]')
         self.imviz.app.add_data_to_viewer(viewer_2.reference_id, 'ndd[DATA]')
 
         # Blink also triggers viewer takeover and line profile redraw,
         # similar to the "l" key but without touching X and Y.
         viewer_2.blink_once()
-        assert lp_plugin.viewer_items == ['imviz-0', 'imviz-1']
-        assert lp_plugin.selected_viewer == 'imviz-1'
+        assert lp_plugin.viewer.labels == ['imviz-0', 'imviz-1']
+        assert lp_plugin.viewer_selected == 'imviz-1'
         assert_allclose(lp_plugin.selected_x, 5.1)
         assert_allclose(lp_plugin.selected_y, 5)
-        assert lp_plugin.line_plot_across_x
-        assert lp_plugin.line_plot_across_y
+        assert len(lp_plugin.plot_across_x.marks['line'].x) > 0
+        assert len(lp_plugin.plot_across_y.marks['line'].x) > 0
         assert lp_plugin.plot_available
 
         # Wrong input resets plots without error.
         lp_plugin.selected_x = -1
         lp_plugin.vue_draw_plot()
-        assert not lp_plugin.line_plot_across_x
-        assert not lp_plugin.line_plot_across_y
+        assert len(lp_plugin.plot_across_x.marks['line'].x) == 0
+        assert len(lp_plugin.plot_across_y.marks['line'].x) == 0
         assert not lp_plugin.plot_available
 
         # Mimic manual GUI inputs.
         lp_plugin.selected_x = '1.1'
         lp_plugin.selected_y = '9'
-        lp_plugin.selected_viewer = 'imviz-0'
-        assert lp_plugin.line_plot_across_x
-        assert lp_plugin.line_plot_across_y
+        lp_plugin.viewer_selected = 'imviz-0'
+        assert len(lp_plugin.plot_across_x.marks['line'].x) > 0
+        assert len(lp_plugin.plot_across_y.marks['line'].x) > 0
         assert lp_plugin.plot_available
 
         # Nothing should update on "l" when plugin closed.
         lp_plugin.plugin_opened = False
-        self.viewer.on_mouse_or_key_event(
-            {'event': 'keydown', 'key': 'l', 'domain': {'x': 5.1, 'y': 5}})
+        lp_plugin._on_viewer_key_event(self.viewer,
+                                       {'event': 'keydown', 'key': 'l',
+                                        'domain': {'x': 5.1, 'y': 5}})
         lp_plugin.selected_x = '1.1'
         lp_plugin.selected_y = '9'
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_linking.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_links_control.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_links_control.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_parser.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_parser_roman.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_parser_roman.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import pytest
 
 # NOTE: Since this is optional dependency, codecov coverage does not include this test module.
 roman_datamodels = pytest.importorskip("roman_datamodels")
 
 from astropy.utils.data import get_pkg_data_filename
-from erfa.core import ErfaWarning
 from gwcs import WCS as GWCS
 
 
 @pytest.mark.parametrize(
     ('ext_list', 'n_dc'),
     [(None, 5),
      ('data', 1),
      (['data', 'var_rnoise'], 2)])
 def test_roman_wfi_ext_options(imviz_helper, ext_list, n_dc):
     filename = get_pkg_data_filename('data/roman_wfi_image_model.asdf')
-    with pytest.warns(ErfaWarning, match=r".*dubious year"):
-        imviz_helper.load_data(filename, ext=ext_list)
+    imviz_helper.load_data(filename, ext=ext_list)
     dc = imviz_helper.app.data_collection
     assert len(dc) == n_dc
 
     if ext_list is None:
         ext_list = ('data', 'dq', 'err', 'var_poisson', 'var_rnoise')
     elif isinstance(ext_list, str):
         ext_list = (ext_list, )
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_regions.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_regions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-import glue_astronomy
 import numpy as np
+import pytest
 from astropy import units as u
 from astropy.coordinates import SkyCoord, Angle
 from astropy.utils.data import get_pkg_data_filename
-from packaging.version import Version
 from photutils.aperture import CircularAperture, SkyCircularAperture
 from regions import (PixCoord, CircleSkyRegion, RectanglePixelRegion, CirclePixelRegion,
                      EllipsePixelRegion, PointSkyRegion, PolygonPixelRegion,
                      CircleAnnulusPixelRegion, CircleAnnulusSkyRegion, Regions)
 
 from jdaviz.configs.imviz.tests.utils import BaseImviz_WCS_NoWCS
 
-GLUE_ASTRONOMY_LT_0_7_1 = not (Version(glue_astronomy.__version__) >= Version("0.7.1.dev"))
-
 
 class BaseRegionHandler:
     """Test to see if region is loaded.
     Does not check if region is actually at the correct place in display.
     """
     def verify_region_loaded(self, region_label, count=2):
         n = 0
@@ -118,40 +115,55 @@
         assert len(self.imviz.get_interactive_regions()) == 1
 
     def test_regions_sky_has_wcs(self):
         # Mimic interactive region (before)
         self.imviz._apply_interactive_region('bqplot:circle', (1.5, 2.5), (3.6, 4.6))
 
         sky = SkyCoord(ra=337.5202808, dec=-20.833333059999998, unit='deg')
-        # This will become indistinguishable from normal Subset.
+        # These will become indistinguishable from normal Subset.
         my_reg_sky_1 = CircleSkyRegion(sky, Angle(0.5, u.arcsec))
-        # Masked subset.
         my_reg_sky_2 = CircleAnnulusSkyRegion(center=sky, inner_radius=0.0004 * u.deg,
                                               outer_radius=0.0005 * u.deg)
-        # Add them both.
-        bad_regions = self.imviz.load_regions([my_reg_sky_1, my_reg_sky_2], return_bad_regions=True)
+        # Masked subset.
+        my_reg_sky_3 = PolygonPixelRegion(vertices=PixCoord(x=[1, 1, 3, 3, 1], y=[1, 3, 3, 1, 1]))
+        # Add them all.
+        bad_regions = self.imviz.load_regions([my_reg_sky_1, my_reg_sky_2, my_reg_sky_3],
+                                              return_bad_regions=True)
         assert len(bad_regions) == 0
 
         # Mimic interactive regions (after)
         self.imviz._apply_interactive_region('bqplot:ellipse', (-2, 0), (5, 4.5))
         self.imviz._apply_interactive_region('bqplot:rectangle', (0, 0), (10, 10))
 
         # Check interactive regions. We do not check if the translation is correct,
         # that check hopefully is already done in glue-astronomy.
         # Apparently, static region ate up one number...
         subsets = self.imviz.get_interactive_regions()
-        assert list(subsets.keys()) == ['Subset 1', 'Subset 2', 'Subset 4', 'Subset 5'], subsets
+        assert list(subsets.keys()) == ['Subset 1', 'Subset 2', 'Subset 3', 'Subset 5', 'Subset 6'], subsets  # noqa: E501
         assert isinstance(subsets['Subset 1'], CirclePixelRegion)
         assert isinstance(subsets['Subset 2'], CirclePixelRegion)
-        assert isinstance(subsets['Subset 4'], EllipsePixelRegion)
-        assert isinstance(subsets['Subset 5'], RectanglePixelRegion)
+        assert isinstance(subsets['Subset 3'], CircleAnnulusPixelRegion)
+        assert isinstance(subsets['Subset 5'], EllipsePixelRegion)
+        assert isinstance(subsets['Subset 6'], RectanglePixelRegion)
 
         # Check static region
         self.verify_region_loaded('MaskedSubset 1')
 
+    def test_regions_annulus_from_load_data(self):
+        # This file actually will load 2 annuli
+        regfile = get_pkg_data_filename('data/ds9_annulus_01.reg')
+        self.imviz.load_data(regfile)
+        assert len(self.imviz.app.data_collection) == 2  # Make sure not loaded as data
+
+        subsets = self.imviz.get_interactive_regions()
+        subset_names = list(subsets.keys())
+        assert subset_names == ['Subset 1', 'Subset 2']
+        for n in subset_names:
+            assert isinstance(subsets[n], CircleAnnulusPixelRegion)
+
     def test_photutils_pixel(self):
         my_aper = CircularAperture((5, 5), r=2)
         bad_regions = self.imviz.load_regions([my_aper], return_bad_regions=True)
         assert len(bad_regions) == 0
         self.verify_region_loaded('Subset 1')
         assert len(self.imviz.get_interactive_regions()) == 1
 
@@ -169,26 +181,29 @@
     def setup_class(self):
         self.region_file = get_pkg_data_filename(
             'data/ds9.fits.reg', package='regions.io.ds9.tests')
         self.arr = np.ones((1024, 1024))
         self.raw_regions = Regions.read(self.region_file, format='ds9')
 
     def test_ds9_load_all(self, imviz_helper):
+        with pytest.raises(ValueError, match="Cannot load regions without data"):
+            imviz_helper.load_data(self.region_file)
+
         self.viewer = imviz_helper.default_viewer
         imviz_helper.load_data(self.arr, data_label='my_image')
         bad_regions = imviz_helper.load_regions_from_file(self.region_file, return_bad_regions=True)
         assert len(bad_regions) == 1
 
-        # Will load 8/9 and 6 of that become ROIs.
+        # Will load 8/9 and 7 of that become ROIs.
         subsets = imviz_helper.get_interactive_regions()
         assert list(subsets.keys()) == ['Subset 1', 'Subset 2', 'Subset 3',
-                                        'Subset 4', 'Subset 5', 'Subset 6'], subsets
+                                        'Subset 4', 'Subset 5', 'Subset 6', 'Subset 7'], subsets
 
-        for i in (1, 2):  # The other 2 are MaskedSubset
-            self.verify_region_loaded(f'MaskedSubset {i}', count=1)
+        # The other 1 is MaskedSubset
+        self.verify_region_loaded('MaskedSubset 1', count=1)
 
     def test_ds9_load_two_good(self, imviz_helper):
         self.viewer = imviz_helper.default_viewer
         imviz_helper.load_data(self.arr, data_label='my_image')
         bad_regions = imviz_helper.load_regions_from_file(
             self.region_file, max_num_regions=2, return_bad_regions=True)
         assert len(bad_regions) == 0
@@ -230,23 +245,17 @@
         assert isinstance(subsets['Subset 2'], CirclePixelRegion)
 
         # Create a third subset that is an annulus.
         subset_groups = self.imviz.app.data_collection.subset_groups
         new_subset = subset_groups[0].subset_state & ~subset_groups[1].subset_state
         self.viewer.apply_subset_state(new_subset)
 
-        # In older glue-astronomy, annulus is no longer accessible by API
-        # but also should not crash Imviz.
         subsets = self.imviz.get_interactive_regions()
         assert len(self.imviz.app.data_collection.subset_groups) == 3
-        if GLUE_ASTRONOMY_LT_0_7_1:
-            expected_subset_keys = ['Subset 1', 'Subset 2']
-        else:
-            expected_subset_keys = ['Subset 1', 'Subset 2', 'Subset 3']
-            assert isinstance(subsets['Subset 3'], CircleAnnulusPixelRegion)
-        assert list(subsets.keys()) == expected_subset_keys, subsets
+        assert list(subsets.keys()) == ['Subset 1', 'Subset 2', 'Subset 3'], subsets
         assert isinstance(subsets['Subset 1'], CirclePixelRegion)
         assert isinstance(subsets['Subset 2'], CirclePixelRegion)
+        assert isinstance(subsets['Subset 3'], CircleAnnulusPixelRegion)
 
         # Clear the regions for next test.
         self.imviz._delete_all_regions()
         assert len(self.imviz.app.data_collection.subset_groups) == 0
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_simple_aper_phot.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_simple_aper_phot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 import numpy as np
 from astropy import units as u
 from astropy.tests.helper import assert_quantity_allclose
-from glue.core.edit_subset_mode import ReplaceMode
 from numpy.testing import assert_allclose, assert_array_equal
 from photutils.aperture import (ApertureStats, CircularAperture, EllipticalAperture,
                                 RectangularAperture, EllipticalAnnulus)
+from regions import CircleAnnulusPixelRegion, PixCoord
 
 from jdaviz.configs.imviz.plugins.aper_phot_simple.aper_phot_simple import (
     _curve_of_growth, _radial_profile)
 from jdaviz.configs.imviz.tests.utils import BaseImviz_WCS_WCS, BaseImviz_WCS_NoWCS
 
 
 class TestSimpleAperPhot(BaseImviz_WCS_WCS):
@@ -48,24 +48,24 @@
         tbl = self.imviz.get_aperture_photometry_results()
         assert len(tbl) == 1
 
         phot_plugin.dataset_selected = 'has_wcs_2[SCI,1]'
         phot_plugin.current_plot_type = 'Radial Profile (Raw)'
         assert phot_plugin._selected_data is not None
         assert phot_plugin._selected_subset is not None
-        assert phot_plugin.bg_subset.labels == ['Manual', 'Annulus', 'Subset 1']
+        assert phot_plugin.bg_subset.labels == ['Manual', 'Subset 1']
         assert_allclose(phot_plugin.background_value, 0)
         assert_allclose(phot_plugin.counts_factor, 0)
         assert_allclose(phot_plugin.pixel_area, 0)
         assert_allclose(phot_plugin.flux_scaling, 0)
         phot_plugin.vue_do_aper_phot()
         tbl = self.imviz.get_aperture_photometry_results()
         assert len(tbl) == 2
         assert phot_plugin.plot_available
-        assert phot_plugin.radial_plot != ''  # Does not check content
+        assert len(phot_plugin.plot.marks['scatter'].x) > 0
 
         # Check photometry results.
         assert tbl.colnames == [
             'id', 'xcenter', 'ycenter', 'sky_center', 'background', 'sum',
             'sum_aper_area', 'pixarea_tot', 'aperture_sum_counts', 'aperture_sum_counts_err',
             'counts_fac', 'aperture_sum_mag', 'flux_scaling', 'min', 'max', 'mean', 'median',
             'mode', 'std', 'mad_std', 'var', 'biweight_location', 'biweight_midvariance',
@@ -155,24 +155,18 @@
         assert_allclose(phot_plugin.background_value, 1)  # Keeps last value
         phot_plugin.bg_subset_selected = 'Subset 1'
         assert_allclose(phot_plugin.background_value, 1)
         self.imviz.load_data(np.ones((10, 10)) + 1, data_label='twos')
         phot_plugin.dataset_selected = 'twos'
         assert_allclose(phot_plugin.background_value, 2)  # Recalculate based on new Data
 
-        # Check rectangle annulus math
-        phot_plugin.bg_subset_selected = 'Annulus'
-        phot_plugin.subset_selected = 'Subset 3'
-        assert_allclose(phot_plugin.bg_annulus_inner_r, 6.363961030678928)  # half-width = 4.5
-        assert_allclose(phot_plugin.bg_annulus_width, 10)
-
         # Curve of growth
         phot_plugin.current_plot_type = 'Curve of Growth'
         phot_plugin.vue_do_aper_phot()
-        assert phot_plugin._fig.title == 'Curve of growth from aperture center'
+        assert phot_plugin.plot.figure.title == 'Curve of growth from aperture center'
 
 
 class TestSimpleAperPhot_NoWCS(BaseImviz_WCS_NoWCS):
     def test_plugin_no_wcs(self):
         # Most things already tested above, so not re-tested here.
         self.imviz._apply_interactive_region('bqplot:circle', (0, 0), (9, 9))  # Draw a circle
         phot_plugin = self.imviz.app.get_tray_item_from_name('imviz-aper-phot-simple')
@@ -199,70 +193,72 @@
     imviz_helper.load_data(gauss4, data_label='four_gaussians')
     imviz_helper.load_data(ones, data_label='ones')
 
     phot_plugin = imviz_helper.app.get_tray_item_from_name('imviz-aper-phot-simple')
     phot_plugin.dataset_selected = 'ones'
 
     # Mark an object of interest
+    # CirclePixelRegion(center=PixCoord(x=150, y=25), radius=7)
     imviz_helper._apply_interactive_region('bqplot:circle', (143, 18), (157, 32))
+
+    # Load annulus (this used to be part of the plugin but no longer)
+    annulus_1 = CircleAnnulusPixelRegion(
+        PixCoord(x=150, y=25), inner_radius=7, outer_radius=17)
+    imviz_helper.load_regions([annulus_1])
+
     phot_plugin.subset_selected = 'Subset 1'
-    phot_plugin.bg_subset_selected = 'Annulus'
+    phot_plugin.bg_subset_selected = 'Subset 2'
 
     # Check annulus for ones
-    assert_allclose(phot_plugin.bg_annulus_inner_r, 7)  # From circle
-    assert_allclose(phot_plugin.bg_annulus_width, 10)  # Default
     assert_allclose(phot_plugin.background_value, 1)
 
     # Switch data
     phot_plugin.dataset_selected = 'four_gaussians'
-    assert_allclose(phot_plugin.bg_annulus_inner_r, 7)  # Unchanged
-    assert_allclose(phot_plugin.bg_annulus_width, 10)
     assert_allclose(phot_plugin.background_value, 5.745596129482831)  # Changed
 
     # Draw ellipse on another object
+    # EllipsePixelRegion(center=PixCoord(x=20.5, y=37.5), width=41, height=15)
     imviz_helper._apply_interactive_region('bqplot:ellipse', (0, 30), (41, 45))
-    phot_plugin.subset_selected = 'Subset 2'
+
+    # Load annulus (this used to be part of the plugin but no longer)
+    annulus_2 = CircleAnnulusPixelRegion(
+        PixCoord(x=20.5, y=37.5), inner_radius=20.5, outer_radius=30.5)
+    imviz_helper.load_regions([annulus_2])
+
+    # Subset 4 (annulus) should be available for the background but not the aperture
+    assert 'Subset 4' not in phot_plugin.subset.choices
+    assert 'Subset 4' in phot_plugin.bg_subset.choices
+
+    phot_plugin.subset_selected = 'Subset 3'
+    phot_plugin.bg_subset_selected = 'Subset 4'
 
     # Check new annulus for four_gaussians
-    assert_allclose(phot_plugin.bg_annulus_inner_r, 20.5)  # From ellipse half-width
-    assert_allclose(phot_plugin.bg_annulus_width, 10)  # Unchanged
     assert_allclose(phot_plugin.background_value, 5.13918435824334)  # Changed
 
     # Switch to manual, should not change
     phot_plugin.bg_subset_selected = 'Manual'
     assert_allclose(phot_plugin.background_value, 5.13918435824334)
 
     # Switch to Subset, should change a lot because this is not background area
     phot_plugin.bg_subset_selected = 'Subset 1'
     assert_allclose(phot_plugin.background_value, 44.72559981461203)
 
     # Switch back to annulus, should be same as before in same mode
-    phot_plugin.bg_subset_selected = 'Annulus'
-    assert_allclose(phot_plugin.bg_annulus_inner_r, 20.5)
-    assert_allclose(phot_plugin.bg_annulus_width, 10)
+    phot_plugin.bg_subset_selected = 'Subset 4'
     assert_allclose(phot_plugin.background_value, 5.13918435824334)
 
-    # Manually change inner_r
-    phot_plugin.bg_annulus_inner_r = 40
-    assert_allclose(phot_plugin.background_value, 4.783765940615679)
-
-    # Manually change width
-    phot_plugin.bg_annulus_width = 5
-    assert_allclose(phot_plugin.background_value, 4.894003242594493)
-
-    # Move the last created Subset (ellipse) and make sure background updates
-    imviz_helper.app.session.edit_subset_mode.mode = ReplaceMode
-    imviz_helper._apply_interactive_region('bqplot:ellipse', (0, 30), (51, 55))
-    assert_allclose(phot_plugin.bg_annulus_inner_r, 40)
-    assert_allclose(phot_plugin.bg_annulus_width, 5)
-    assert_allclose(phot_plugin.background_value, 4.894003)
-
-    # Bad annulus should not crash plugin
-    phot_plugin.bg_annulus_inner_r = -1
-    assert_allclose(phot_plugin.background_value, 0)
+    # Edit the annulus and make sure background updates
+    subset_plugin = imviz_helper.plugins["Subset Tools"]._obj
+    subset_plugin.subset_selected = "Subset 4"
+    subset_plugin._set_value_in_subset_definition(0, "X Center", "value", 25.5)
+    subset_plugin._set_value_in_subset_definition(0, "Y Center", "value", 42.5)
+    subset_plugin._set_value_in_subset_definition(0, "Inner radius", "value", 40)
+    subset_plugin._set_value_in_subset_definition(0, "Outer radius", "value", 45)
+    subset_plugin.vue_update_subset()
+    assert_allclose(phot_plugin.background_value, 4.89189)
 
 
 # NOTE: Extracting the cutout for radial profile is aperture
 #       shape agnostic, so we use ellipse as representative case.
 # NOTE: This test only tests the radial profile algorithm and does
 #       not care if the actual plugin use centroid or not.
 class TestRadialProfile():
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_subset_centroid.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_subset_centroid.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_tools.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         v2 = self.imviz.create_image_viewer()
         self.imviz.app.add_data_to_viewer('imviz-1', 'has_wcs_1[SCI,1]')
 
         t = v.toolbar.tools['jdaviz:boxzoommatch']
         # original limits (x_min, x_max, y_min, y_max): -0.5 9.5 -0.5 9.5
         original_limits = (v.state.x_min, v.state.x_max, v.state.y_min, v.state.y_max)
         assert_allclose(original_limits, (-0.5, 9.5, -0.5, 9.5))
+        assert_allclose((v2.state.x_min, v2.state.x_max, v2.state.y_min, v2.state.y_max), original_limits)  # noqa
         t.activate()
         t.save_prev_zoom()
         v.state.x_min, v.state.x_max, v.state.y_min, v.state.y_max = (1, 8, 1, 8)
         # second viewer should match these changes
         assert (v2.state.x_min, v2.state.x_max, v2.state.y_min, v2.state.y_max) == (1, 8, 1, 8)
 
         v.toolbar.tools['jdaviz:prevzoom'].activate()
@@ -128,12 +129,41 @@
     viewer.on_mouse_or_key_event({'event': 'keydown', 'key': 'B', 'domain': {'x': 0, 'y': 0}})
     assert label_mouseover.as_text() == ('Pixel x=00.0 y=00.0 Value +2.00000e+00', '', '')
     assert viewer.top_visible_data_label == 'image_2'
 
 
 def test_compass_open_while_load(imviz_helper):
     plg = imviz_helper.plugins['Compass']
-    plg.open_in_tray()
+    plg.plugin_opened = True
 
     # Should not crash even if Compass is open in tray.
     imviz_helper.load_data(np.ones((2, 2)))
     assert len(imviz_helper.app.data_collection) == 1
+
+
+def test_tool_visibility(imviz_helper):
+    imviz_helper.load_data(np.ones((2, 2)))
+    tb = imviz_helper.default_viewer.toolbar
+
+    assert not tb.tools_data['jdaviz:boxzoommatch']['visible']
+
+    assert tb.tools_data['jdaviz:boxzoom']['primary']
+    # activate boxzoom to ensure it remains primary
+    tb.active_tool_id = 'jdaviz:boxzoom'
+
+    imviz_helper.create_image_viewer()
+    imviz_helper.app.set_data_visibility('imviz-1', imviz_helper.app.data_collection[0].label, True)
+
+    assert tb.tools_data['jdaviz:boxzoommatch']['visible']
+    assert tb.active_tool_id == 'jdaviz:boxzoom'
+    assert tb.tools_data['jdaviz:boxzoom']['primary']
+
+    # but the panzoom has updated primary since there was no active tool in that submenu
+    assert tb.tools_data['jdaviz:panzoommatch']['visible']
+    assert tb.tools_data['jdaviz:panzoommatch']['primary']
+
+    # now set the tool to the matched box zoom to ensure it deactivates itself when removing
+    # a viewer
+    tb.active_tool_id = 'jdaviz:boxzoommatch'
+    imviz_helper.destroy_viewer('imviz-1')
+    assert not tb.tools_data['jdaviz:boxzoommatch']['visible']
+    assert tb.active_tool_id is None
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_viewer_tools.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_viewer_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_viewers.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_viewers.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,15 @@
     viewer = imviz_helper.create_image_viewer(viewer_name=desired_name)
     viewer_names = sorted(['imviz-0', actual_name])
     assert viewer.top_visible_data_label == ''
     assert isinstance(viewer, ImvizImageView)
     assert viewer is imviz_helper.app._viewer_store.get(actual_name), list(imviz_helper.app._viewer_store.keys())  # noqa
     assert imviz_helper.app.get_viewer_ids() == viewer_names
 
-    # Make sure plugins that store viewer_items differently are consistent.
-    assert imviz_helper.plugins['Imviz Line Profiles (XY)']._obj.viewer_items == viewer_names
+    # Make sure plugins that store viewer_items are updated.
     assert sorted(imviz_helper.plugins['Compass'].viewer.labels) == viewer_names
 
     imviz_helper.destroy_viewer(actual_name)
     assert imviz_helper.app.get_viewer_ids() == ['imviz-0']
 
 
 def test_get_viewer_created(imviz_helper):
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_wcs_utils.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_wcs_utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/tests/utils.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/imviz/wcs_utils.py` & `jdaviz-3.6.0/jdaviz/configs/imviz/wcs_utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/mosviz/helper.py` & `jdaviz-3.6.0/jdaviz/configs/mosviz/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import warnings
 from copy import deepcopy
 from pathlib import Path
-from time import time
 from zipfile import is_zipfile
 
 import numpy as np
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 from astropy.table import QTable
 from echo import delay_callback
@@ -35,18 +34,15 @@
     _default_spectrum_2d_viewer_reference_name = "spectrum-2d-viewer"
     _default_table_viewer_reference_name = "table-viewer"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         spec1d = self.app.get_viewer(self._default_spectrum_viewer_reference_name)
-        spec1d.scales['x'].observe(self._update_spec2d_x_axis, names=['min', 'max'])
-
         spec2d = self.app.get_viewer(self._default_spectrum_2d_viewer_reference_name)
-        spec2d.scales['x'].observe(self._update_spec1d_x_axis, names=['min', 'max'])
 
         image_viewer = self.app.get_viewer(self._default_image_viewer_reference_name)
 
         # Choose which viewers will have state frozen during a row change.
         # This should be a list of tuples, where each entry has the state as the
         # first item in the tuple, and a list of frozen attributes as the second.
         self._freezable_states = [(spec1d.state, ['x_min', 'x_max']),
@@ -74,20 +70,14 @@
 
         # Listen for new redshifts from the redshift slider (NOT YET IMPLEMENTED)
         self.app.hub.subscribe(self, RedshiftMessage,
                                handler=self._redshift_listener)
 
         self._shared_image = False
 
-        self._scales1d = spec1d.scales['x']
-        self._scales2d = spec2d.scales['x']
-
-        self._panning_warning_triggered = False
-        self._last_panning_warning = 0
-
         self._update_in_progress = False
 
         self._initialize_table()
         self._default_visible_columns = []
 
     def _initialize_table(self, label="MOS Table", table_viewer_reference_name='table-viewer'):
         '''
@@ -136,102 +126,14 @@
 
         # Restore data-layer states from cache, then reset cache
         for (state, attrs), cache in zip(self._freezable_layers, self._frozen_layers_cache):
             state.layers[0].update_from_dict(cache)
 
         self._frozen_layers_cache = []
 
-        # Make sure world flipping has been handled correctly, as internal
-        # callbacks may have been made while limits were frozen.  This is
-        # especially important for NIRISS data.
-        self._update_spec2d_x_axis()
-
-    def _extend_world(self, spec1d, ext):
-        # Extend 1D spectrum world axis to enable panning (within reason) past
-        # the bounds of data
-        world = self.app.data_collection[spec1d]["World 0"].copy()
-        dw = world[1]-world[0]
-        prepend = np.linspace(world[0]-dw*ext, world[0]-dw, ext)
-        dw = world[-1]-world[-2]
-        append = np.linspace(world[-1]+dw, world[-1]+dw*ext, ext)
-        world = np.hstack((prepend, world, append))
-        return world
-
-    def _update_spec2d_x_axis(self, change=None):
-        # This assumes the two spectrum viewers have the same x-axis shape and
-        # wavelength solution, which should always hold
-        table_viewer = self.app.get_viewer(self._default_table_viewer_reference_name)
-
-        if self._update_in_progress or table_viewer.row_selection_in_progress:
-            return
-
-        min_1d = self._scales1d.min
-        max_1d = self._scales1d.max
-
-        spec1d = table_viewer._selected_data[self._default_spectrum_viewer_reference_name]
-        extend_by = int(self.app.data_collection[spec1d]["World 0"].shape[0])
-        world = self._extend_world(spec1d, extend_by)
-
-        # Workaround for flipped data
-        min_world, max_world = ((world[0], world[-1]) if not self._is_world_flipped()
-                                else (world[-1], world[0]))
-
-        # Warn the user if they've panned far enough away from the data
-        # that the viewers will desync
-        if min_1d < min_world or max_1d > max_world:
-            self._show_panning_warning()
-            return
-
-        self._panning_warning_triggered = False
-
-        idx_min = float((np.abs(world - min_1d)).argmin()) - extend_by
-        idx_max = float((np.abs(world - max_1d)).argmin()) - extend_by
-
-        self._update_in_progress = True
-        with self._scales2d.hold_sync():
-            self._scales2d.min = idx_min
-            self._scales2d.max = idx_max
-
-        self._update_in_progress = False
-
-    def _update_spec1d_x_axis(self, change=None):
-        # This assumes the two spectrum viewers have the same x-axis shape and
-        # wavelength solution, which should always hold
-        table_viewer = self.app.get_viewer(self._default_table_viewer_reference_name)
-
-        if self._update_in_progress or table_viewer.row_selection_in_progress:
-            return
-
-        min_2d = self._scales2d.min
-        max_2d = self._scales2d.max
-
-        spec1d = table_viewer._selected_data[self._default_spectrum_viewer_reference_name]
-        extend_by = int(self.app.data_collection[spec1d]["World 0"].shape[0])
-        world = self._extend_world(spec1d, extend_by)
-
-        idx_min = int(np.around(min_2d)) + extend_by
-        idx_max = int(np.around(max_2d)) + extend_by
-
-        # Warn the user if they've panned far enough away from the data
-        # that the viewers will desync
-        # Note: Because of the flipped data workaround, idx_min can be > idx_max
-        max_world = len(world)
-        if not (0 <= idx_min < max_world and 0 <= idx_max < max_world):
-            self._show_panning_warning()
-            return
-
-        self._panning_warning_triggered = False
-
-        self._update_in_progress = True
-        with self._scales1d.hold_sync():
-            self._scales1d.min = world[idx_min]
-            self._scales1d.max = world[idx_max]
-
-        self._update_in_progress = False
-
     def _redshift_listener(self, msg):
         '''Save new redshifts (including from the helper itself)'''
         if self._update_in_progress:
             # then ignore messages for now, the final redshift will be set once the
             # data is loaded and the row change is complete.
             return
 
@@ -251,43 +153,16 @@
         # redshift slider as well as exposing when accessing specviz.get_spectra(...))
         if value is None and row is not None:
             value = self.get_column('Redshift')[row]
 
         if value is not None:
             self.specviz.set_redshift(value)
 
-    def _show_panning_warning(self):
-        now = time()
-
-        # Limit the number of messages that can be send to 1 per 5 seconds
-        panning_warning_timeout = 5
-
-        if (not self._panning_warning_triggered
-                and now > self._last_panning_warning + panning_warning_timeout):
-            self._panning_warning_triggered = True
-            self._last_panning_warning = now
-            msg = ("Warning: panning too far away from the data may desync"
-                   "the 1D and 2D spectrum viewers")
-            msg = SnackbarMessage(msg, color='warning', sender=self)
-            self.app.hub.broadcast(msg)
-
-    def _is_world_flipped(self):
-        spec1d = self.app.get_viewer(
-            self._default_table_viewer_reference_name
-        )._selected_data.get(
-            self._default_spectrum_viewer_reference_name
-        )
-        if not spec1d:
-            return False
-        world = self.app.data_collection[spec1d]["World 0"]
-        return world[0] > world[-1]
-
     def _row_click_message_handler(self, msg):
         self._handle_image_zoom(msg)
-        self._handle_flipped_data()
         # expose the row to vue for each of the viewers
         self.app.state.settings = {**self.app.state.settings, 'mosviz_row': msg.selected_index}
 
     def _handle_image_zoom(self, msg):
         mos_data = self.app.data_collection['MOS Table']
 
         if mos_data.find_component_id("Images") is None:
@@ -313,22 +188,14 @@
                 imview.state.y_min = cur_ycen - height
                 imview.state.x_max = cur_xcen + x_height
                 imview.state.y_max = cur_ycen + height
 
         if center is not None:
             imview.center_on(center)
 
-    def _handle_flipped_data(self):
-        # Workaround for flipped data
-        if self._is_world_flipped():
-            min, max = self._scales2d.max, self._scales2d.min
-            with self._scales2d.hold_sync():
-                self._scales2d.min = min
-                self._scales2d.max = max
-
     def _zoom_to_object_params(self, msg):
 
         table_data = self.app.data_collection['MOS Table']
         specview = self.app.get_viewer(self._default_spectrum_2d_viewer_reference_name)
 
         if ("R.A." not in table_data.component_ids() or
                 "Dec." not in table_data.component_ids()):
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/mosviz/mosviz.yaml` & `jdaviz-3.6.0/jdaviz/configs/mosviz/mosviz.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -39,14 +39,14 @@
             reference: image-viewer
         - container: col
           viewers:
             - name: 2D Spectrum viewer
               plot: mosviz-profile-2d-viewer
               reference: spectrum-2d-viewer
             - name: Spectrum
-              plot: specviz-profile-viewer
+              plot: mosviz-profile-viewer
               reference: spectrum-viewer
       - container: row
         viewers:
         - name: Table viewer
           plot: mosviz-table-viewer
           reference: table-viewer
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/parsers.py` & `jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import warnings
 
 from astropy import units as u
 from astropy.io import fits
 from astropy.io.registry import IORegistryError
 from astropy.wcs import WCS
 from glue.core.data import Data
-from glue.core.link_helpers import LinkSame
+from glue.core.link_helpers import LinkSameWithUnits
 from specutils import Spectrum1D, SpectrumList, SpectrumCollection
 from specutils.io.default_loaders.jwst_reader import identify_jwst_s2d_multi_fits
 
 from jdaviz.configs.imviz.plugins.parsers import get_image_data_iterator
 from jdaviz.core.registries import data_parser_registry
 from jdaviz.core.events import SnackbarMessage
 from jdaviz.utils import standardize_metadata, PRIHDR_KEY
@@ -136,15 +136,15 @@
 
             spec_1d = spectra_1d[index]
             spec_2d = spectra_2d[index]
 
             wc_spec_1d = app.session.data_collection[spec_1d].world_component_ids
             wc_spec_2d = app.session.data_collection[spec_2d].world_component_ids
 
-            wc_spec_ids.append(LinkSame(wc_spec_1d[0], wc_spec_2d[1]))
+            wc_spec_ids.append(LinkSameWithUnits(wc_spec_1d[0], wc_spec_2d[1]))
 
     app.session.data_collection.add_link(wc_spec_ids)
 
 
 @data_parser_registry("mosviz-nirspec-directory-parser")
 def mos_nirspec_directory_parser(app, data_obj, data_labels=None):
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py` & `jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py` & `jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,11 +148,10 @@
         if self._slit_overlay_mark is not None:
             image_figure = self.app.get_viewer(
                 self._default_image_viewer_reference_name
             ).figure
             # We need to do the following instead of just removing directly on
             # the marks otherwise traitlets doesn't register a change in the
             # marks.
-            marks = image_figure.marks.copy()
-            marks.remove(self._slit_overlay_mark)
-            image_figure.marks = marks
+            image_figure.marks.remove(self._slit_overlay_mark)
+            image_figure.send_state('marks')
             self._slit_overlay_mark = None
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py` & `jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_data_loading.py` & `jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_data_loading.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Tests data loading in the Mosviz Jdaviz configuration
 
 from zipfile import ZipFile
 
-from astropy.nddata import CCDData
 import numpy as np
 import pytest
+from astropy.nddata import CCDData
 from specutils import Spectrum1D
 
 from jdaviz.utils import PRIHDR_KEY
 
 
 def test_load_spectrum1d(mosviz_helper, spectrum1d):
     label = "Test 1D Spectrum"
@@ -16,20 +16,22 @@
 
     assert len(mosviz_helper.app.data_collection) == 2
     assert mosviz_helper.app.data_collection[0].label == "MOS Table"
     dc_1 = mosviz_helper.app.data_collection[1]
     assert dc_1.label == label
     assert dc_1.meta['uncertainty_type'] == 'std'
 
-    table = mosviz_helper.app.get_viewer('table-viewer')
+    table = mosviz_helper.app.get_viewer(mosviz_helper._default_table_viewer_reference_name)
     table.widget_table.vue_on_row_clicked(0)
 
-    data = mosviz_helper.app.get_data_from_viewer('spectrum-viewer')
+    data = mosviz_helper.app.get_viewer(mosviz_helper._default_spectrum_viewer_reference_name
+                                        ).data()
 
-    assert isinstance(data[label], Spectrum1D)
+    assert len(data) == 1
+    assert isinstance(data[0], Spectrum1D)
 
     with pytest.raises(AttributeError):
         mosviz_helper.load_1d_spectra([1, 2, 3])
 
 
 def test_load_image(mosviz_helper, mos_image):
     label = "Test Image"
@@ -38,20 +40,22 @@
     assert len(mosviz_helper.app.data_collection) == 2
     assert mosviz_helper.app.data_collection[0].label == "MOS Table"
     dc_1 = mosviz_helper.app.data_collection[1]
     assert dc_1.label == f"{label} 0"
     assert PRIHDR_KEY not in dc_1.meta
     assert dc_1.meta['RADESYS'] == 'ICRS'
 
-    table = mosviz_helper.app.get_viewer('table-viewer')
+    table = mosviz_helper.app.get_viewer(mosviz_helper._default_table_viewer_reference_name)
     table.widget_table.vue_on_row_clicked(0)
 
-    data = mosviz_helper.app.get_data_from_viewer('image-viewer')
+    data = mosviz_helper.app.get_viewer(mosviz_helper._default_image_viewer_reference_name
+                                        ).data(cls=CCDData)
 
-    dataval = data[f"{label} 0"]
+    assert len(data) == 1
+    dataval = data[0]
     assert isinstance(dataval, CCDData)
     assert dataval.shape == (55, 55)
 
 
 def test_load_spectrum_collection(mosviz_helper, spectrum_collection):
     labels = [f"Test Spectrum Collection {i}" for i in range(5)]
     mosviz_helper.load_1d_spectra(spectrum_collection, data_labels=labels, add_redshift_column=True)
@@ -59,70 +63,77 @@
     # +1 for the table viewer
     assert len(mosviz_helper.app.data_collection) == len(spectrum_collection) + 1
     assert mosviz_helper.app.data_collection[0].label == "MOS Table"
     dc_1 = mosviz_helper.app.data_collection[1]
     assert dc_1.label == labels[0]
     assert dc_1.meta['uncertainty_type'] == 'std'
 
-    table = mosviz_helper.app.get_viewer('table-viewer')
+    table = mosviz_helper.app.get_viewer(mosviz_helper._default_table_viewer_reference_name)
     table.select_row(0)
 
-    data = mosviz_helper.app.get_data_from_viewer('spectrum-viewer')
+    data = mosviz_helper.app.get_viewer(mosviz_helper._default_spectrum_viewer_reference_name
+                                        ).data()
 
-    assert isinstance(data[labels[0]], Spectrum1D)
+    assert len(data) == 1
+    assert isinstance(data[0], Spectrum1D)
 
 
 def test_load_list_of_spectrum1d(mosviz_helper, spectrum1d):
     spectra = [spectrum1d] * 3
 
     labels = [f"Test Spectrum 1D {i}" for i in range(3)]
     mosviz_helper.load_1d_spectra(spectra, data_labels=labels, add_redshift_column=True)
 
     assert len(mosviz_helper.app.data_collection) == 4
     assert mosviz_helper.app.data_collection[0].label == "MOS Table"
     dc_1 = mosviz_helper.app.data_collection[1]
     assert dc_1.label == labels[0]
     assert dc_1.meta['uncertainty_type'] == 'std'
 
-    table = mosviz_helper.app.get_viewer('table-viewer')
+    table = mosviz_helper.app.get_viewer(mosviz_helper._default_table_viewer_reference_name)
     table.widget_table.vue_on_row_clicked(0)
 
-    data = mosviz_helper.app.get_data_from_viewer('spectrum-viewer')
+    data = mosviz_helper.app.get_viewer(mosviz_helper._default_spectrum_viewer_reference_name
+                                        ).data()
 
-    assert isinstance(data[labels[0]], Spectrum1D)
+    assert len(data) == 1
+    assert isinstance(data[0], Spectrum1D)
 
 
 def test_load_mos_spectrum2d(mosviz_helper, mos_spectrum2d):
 
     label = "Test 2D Spectrum"
     mosviz_helper.load_data(spectra_2d=mos_spectrum2d, spectra_2d_label=label)
 
     assert len(mosviz_helper.app.data_collection) == 2
     assert mosviz_helper.app.data_collection[0].label == "MOS Table"
     dc_1 = mosviz_helper.app.data_collection[1]
     assert dc_1.label == label
     assert dc_1.meta['INSTRUME'] == 'nirspec'
 
-    table = mosviz_helper.app.get_viewer('table-viewer')
+    table = mosviz_helper.app.get_viewer(mosviz_helper._default_table_viewer_reference_name)
     table.widget_table.vue_on_row_clicked(0)
 
-    data = mosviz_helper.app.get_data_from_viewer('spectrum-2d-viewer')
+    data = mosviz_helper.app.get_viewer(mosviz_helper._default_spectrum_2d_viewer_reference_name
+                                        ).data()
 
-    assert data[label].shape == (1024, 15)
+    assert len(data) == 1
+    assert data[0].shape == (1024, 15)
 
 
 @pytest.mark.parametrize('label', [None, "Test Label"])
 def test_load_multi_image_spec(mosviz_helper, mos_image, spectrum1d, mos_spectrum2d, label):
     spectra1d = [spectrum1d] * 3
     spectra2d = [mos_spectrum2d] * 3
     images = [mos_image] * 3
 
     mosviz_helper.load_data(spectra1d, spectra2d, images=images, images_label=label)
 
-    assert mosviz_helper.app.get_viewer("table-viewer").figure_widget.highlighted == 0
+    assert mosviz_helper.app.get_viewer(mosviz_helper._default_table_viewer_reference_name
+                                        ).figure_widget.highlighted == 0
     assert len(mosviz_helper.app.data_collection) == 10
 
     qtable = mosviz_helper.to_table()
     if label is None:
         assert qtable["Images"][0] == "Image 0"
     else:
         assert qtable["Images"][0] == "Test Label 0"
@@ -130,25 +141,27 @@
 
 def test_load_multi_image_and_spec1d_only(mosviz_helper, mos_image, spectrum1d):
     spectra1d = [spectrum1d] * 3
     images = [mos_image] * 3
 
     mosviz_helper.load_data(spectra_1d=spectra1d, images=images)
 
-    assert mosviz_helper.app.get_viewer("table-viewer").figure_widget.highlighted == 0
+    assert mosviz_helper.app.get_viewer(mosviz_helper._default_table_viewer_reference_name
+                                        ).figure_widget.highlighted == 0
     assert len(mosviz_helper.app.data_collection) == 7
 
 
 def test_load_multi_image_and_spec2d_only(mosviz_helper, mos_image, mos_spectrum2d):
     spectra2d = [mos_spectrum2d] * 3
     images = [mos_image] * 3
 
     mosviz_helper.load_data(spectra_2d=spectra2d, images=images)
 
-    assert mosviz_helper.app.get_viewer("table-viewer").figure_widget.highlighted == 0
+    assert mosviz_helper.app.get_viewer(mosviz_helper._default_table_viewer_reference_name
+                                        ).figure_widget.highlighted == 0
     assert len(mosviz_helper.app.data_collection) == 7
 
 
 @pytest.mark.parametrize('label', [None, "Test Label"])
 def test_load_single_image_multi_spec(mosviz_helper, mos_image, spectrum1d, mos_spectrum2d, label):
     spectra1d = [spectrum1d] * 3
     spectra2d = [mos_spectrum2d] * 3
@@ -166,15 +179,16 @@
     # Test that loading is still possible after previous crash:
     # https://github.com/spacetelescope/jdaviz/issues/364
     with pytest.raises(ValueError, match="incompatible with the dimensions of this data:"):
         mosviz_helper.load_data(spectra1d, spectra2d, images=[mos_image, mos_image])
 
     mosviz_helper.load_data(spectra1d, spectra2d, images=mos_image, images_label=label)
 
-    assert mosviz_helper.app.get_viewer("table-viewer").figure_widget.highlighted == 0
+    assert mosviz_helper.app.get_viewer(mosviz_helper._default_table_viewer_reference_name
+                                        ).figure_widget.highlighted == 0
     assert len(mosviz_helper.app.data_collection) == 8
 
     qtable = mosviz_helper.to_table()
     if label is None:
         assert np.all(qtable["Images"] == "Shared Image")
     else:
         assert np.all(qtable["Images"] == "Test Label")
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_helper.py` & `jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,34 +3,14 @@
 
 import csv
 import pytest
 from numpy.testing import assert_allclose
 from jdaviz.configs.specviz2d.helper import Specviz2d
 
 
-def test_viewer_axis_link(mosviz_helper, mos_spectrum1d, mos_spectrum2d):
-    label1d = "Test 1D Spectrum"
-    mosviz_helper.load_1d_spectra(mos_spectrum1d, data_labels=label1d)
-
-    label2d = "Test 2D Spectrum"
-    mosviz_helper.load_2d_spectra(mos_spectrum2d, data_labels=label2d, add_redshift_column=True)
-
-    table = mosviz_helper.app.get_viewer('table-viewer')
-    table.widget_table.vue_on_row_clicked(0)
-
-    scale_2d = mosviz_helper.app.get_viewer('spectrum-2d-viewer').scales['x']
-    scale_1d = mosviz_helper.app.get_viewer('spectrum-viewer').scales['x']
-
-    scale_2d.min = 200.0
-    assert scale_1d.min == mos_spectrum1d.spectral_axis.value[200]
-
-    scale_1d.max = 7564
-    assert scale_2d.max == 800.0
-
-
 def test_to_csv(tmp_path, mosviz_helper, spectrum_collection):
     labels = [f"Test Spectrum Collection {i}" for i in range(5)]
     mosviz_helper.load_1d_spectra(spectrum_collection, data_labels=labels, add_redshift_column=True)
 
     mosviz_helper.to_csv(filename=str(tmp_path / "MOS_data.csv"))
 
     found_rows = 0
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_parsers.py` & `jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py` & `jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz/helper.py` & `jdaviz-3.6.0/jdaviz/configs/specviz/helper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import warnings
 
 from astropy import units as u
+from astropy.utils.decorators import deprecated_renamed_argument, deprecated
 from regions.core.core import Region
 from glue.core.subset_group import GroupedSubset
 from specutils import SpectralRegion, Spectrum1D
 
 from jdaviz.core.helpers import ConfigHelper
 from jdaviz.core.events import RedshiftMessage
 from jdaviz.configs.default.plugins.line_lists.line_list_mixin import LineListMixin
@@ -36,14 +37,15 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Listen for new redshifts from the redshift slider
         self.app.hub.subscribe(self, RedshiftMessage,
                                handler=self._redshift_listener)
 
+    @deprecated(since="3.6", alternative="load_data")
     def load_spectrum(self, data, data_label=None, format=None, show_in_viewer=True,
                       concat_by_file=False):
         """
         Loads a data file or `~specutils.Spectrum1D` object into Specviz.
 
         Parameters
         ----------
@@ -57,44 +59,68 @@
         show_in_viewer : bool
             Show data in viewer(s).
         concat_by_file : bool
             If True and there is more than one available extension, concatenate
             the extensions within each spectrum file passed to the parser and
             add a concatenated spectrum to the data collection.
         """
+        self.load_data(data, data_label, format, show_in_viewer, concat_by_file)
+
+    def load_data(self, data, data_label=None, format=None, show_in_viewer=True,
+                  concat_by_file=False):
+        """
+        Load data into Specviz.
+
+        Parameters
+        ----------
+        data : str, `~specutils.Spectrum1D`, or `~specutils.SpectrumList`
+            Spectrum1D, SpectrumList, or path to compatible data file.
+        data_label : str
+            The Glue data label found in the ``DataCollection``.
+        format : str
+            Loader format specification used to indicate data format in
+            `~specutils.Spectrum1D.read` io method.
+        show_in_viewer : bool
+            Show data in viewer(s).
+        concat_by_file : bool
+            If True and there is more than one available extension, concatenate
+            the extensions within each spectrum file passed to the parser and
+            add a concatenated spectrum to the data collection.
+        """
         super().load_data(data,
                           parser_reference='specviz-spectrum1d-parser',
                           data_label=data_label,
                           format=format,
                           show_in_viewer=show_in_viewer,
                           concat_by_file=concat_by_file)
 
-    def get_spectra(self, data_label=None, subset_to_apply=None, apply_slider_redshift="Warn"):
+    @deprecated_renamed_argument("subset_to_apply", "spectral_subset", "3.6")
+    def get_spectra(self, data_label=None, spectral_subset=None, apply_slider_redshift="Warn"):
         """Returns the current data loaded into the main viewer
 
         """
         spectra = {}
         # Just to save line length
         get_data_method = self.app._jdaviz_helper.get_data
         viewer = self.app.get_viewer(self._default_spectrum_viewer_reference_name)
         function_kwargs = {'function': getattr(viewer.state, "function")} if self.app.config == 'cubeviz' else {}  # noqa
         all_subsets = self.app.get_subsets(object_only=True)
 
         if data_label is not None:
             spectrum = get_data_method(data_label=data_label,
-                                       spectral_subset=subset_to_apply,
+                                       spectral_subset=spectral_subset,
                                        cls=Spectrum1D)
             spectra[data_label] = spectrum
         else:
             for layer_state in viewer.state.layers:
                 lyr = layer_state.layer
-                if subset_to_apply is not None:
-                    if lyr.label == subset_to_apply:
+                if spectral_subset is not None:
+                    if lyr.label == spectral_subset:
                         spectrum = get_data_method(data_label=lyr.data.label,
-                                                   spectral_subset=subset_to_apply,
+                                                   spectral_subset=spectral_subset,
                                                    cls=Spectrum1D,
                                                    **function_kwargs)
                         spectra[lyr.data.label] = spectrum
                     else:
                         continue
                 else:
                     if (isinstance(lyr, GroupedSubset) and lyr.label in all_subsets.keys() and
@@ -134,26 +160,32 @@
                               "keyword option to True or False.")
 
             if data_label is not None:
                 output_spectra = output_spectra[data_label]
 
             return output_spectra
 
-    def get_spectral_regions(self):
+    def get_spectral_regions(self, use_display_units=False):
         """
         A simple wrapper around the app-level call to retrieve only spectral
         subsets, which are now returned as SpectralRegions by default.
 
+        Parameters
+        ----------
+        use_display_units : bool, optional
+            Whether to convert to the display units defined in the
+            :ref:`Unit Conversion <unit-conversion>` plugin.
+
         Returns
         -------
         spec_regs : dict
             Mapping from the names of the subsets to the subsets expressed
             as `specutils.SpectralRegion` objects.
         """
-        return self.app.get_subsets(spectral_only=True)
+        return self.app.get_subsets(spectral_only=True, use_display_units=use_display_units)
 
     def x_limits(self, x_min=None, x_max=None):
         """Sets the limits of the x-axis
 
         Parameters
         ----------
         x_min
@@ -277,27 +309,30 @@
             return
 
         # Examples of values for fmt are '0.1e' or '0.2f'
         self.app.get_viewer(
             self._default_spectrum_viewer_reference_name
         ).figure.axes[axis].tick_format = fmt
 
-    def get_data(self, data_label=None, spectral_subset=None, cls=None, **kwargs):
+    def get_data(self, data_label=None, spectral_subset=None, cls=None,
+                 use_display_units=False, **kwargs):
         """
         Returns data with name equal to data_label of type cls with subsets applied from
-        subset_to_apply.
+        spectral_subset.
 
         Parameters
         ----------
         data_label : str, optional
             Provide a label to retrieve a specific data set from data_collection.
         spectral_subset : str, optional
             Spectral subset applied to data.
         cls : `~specutils.Spectrum1D`, optional
             The type that data will be returned as.
+        use_display_units: bool, optional
+            Whether to convert to the display units defined in the <unit-conversion> plugin.
 
         Returns
         -------
         data : cls
             Data is returned as type cls with subsets applied.
 
         """
@@ -318,8 +353,9 @@
         elif spatial_subset or function:
             raise ValueError('kwargs spatial subset and function are not valid in specviz')
         else:
             spatial_subset = None
             function = None
 
         return self._get_data(data_label=data_label, spatial_subset=spatial_subset,
-                              spectral_subset=spectral_subset, function=function, cls=cls)
+                              spectral_subset=spectral_subset, function=function,
+                              cls=cls, use_display_units=use_display_units)
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py` & `jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 import warnings
 
 import numpy as np
 from glue.core.message import (SubsetDeleteMessage,
                                SubsetUpdateMessage)
 from glue_jupyter.common.toolbar_vuetify import read_icon
 from traitlets import Bool, List, Float, Unicode, observe
+from astropy.utils.decorators import deprecated
 from astropy import units as u
 from specutils import analysis, Spectrum1D
 from specutils.manipulation import extract_region
 
 from jdaviz.core.custom_traitlets import FloatHandleEmpty
 from jdaviz.core.events import (AddDataMessage,
                                 RemoveDataMessage,
                                 SpectralMarksChangedMessage,
                                 LineIdentifyMessage,
-                                RedshiftMessage)
+                                RedshiftMessage,
+                                GlobalDisplayUnitChanged,
+                                SnackbarMessage)
 from jdaviz.core.marks import (LineAnalysisContinuum,
                                LineAnalysisContinuumCenter,
                                LineAnalysisContinuumLeft,
                                LineAnalysisContinuumRight,
                                ShadowLine)
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import (PluginTemplateMixin,
@@ -86,20 +89,20 @@
     * ``continuum`` (:class:`~jdaviz.core.template_mixin.SubsetSelect`):
       Subset to use for the continuum, or ``Surrounding`` to use a region surrounding the
       subset set in ``spectral_subset``.
     * :attr:`width`:
       Width, relative to the overall line spectral region, to fit the linear continuum
       (excluding the region containing the line). If 1, will use endpoints within line region
       only.
-    * :meth:`show_continuum_marks`
     * :meth:`get_results`
 
     """
     dialog = Bool(False).tag(sync=True)
     template_file = __file__, "line_analysis.vue"
+    uses_active_status = Bool(True).tag(sync=True)
 
     spatial_subset_items = List().tag(sync=True)
     spatial_subset_selected = Unicode().tag(sync=True)
 
     continuum_subset_items = List().tag(sync=True)
     continuum_subset_selected = Unicode().tag(sync=True)
 
@@ -125,27 +128,27 @@
 
         self.update_results(None)
 
         self.continuum = SubsetSelect(self,
                                       'continuum_subset_items',
                                       'continuum_subset_selected',
                                       default_text='Surrounding',
-                                      allowed_type='spectral')
+                                      filters=['is_spectral'])
 
         # when accessing the selected data, access the spectrum-viewer version
         self.dataset._viewers = [self._default_spectrum_viewer_reference_name]
         # require entries to be in spectrum-viewer (not other cubeviz images, etc)
         self.dataset.add_filter('layer_in_spectrum_viewer')
 
         if self.app.state.settings.get("configuration") == "cubeviz":
             self.spatial_subset = SubsetSelect(self,
                                                'spatial_subset_items',
                                                'spatial_subset_selected',
                                                default_text=SPATIAL_DEFAULT_TEXT,
-                                               allowed_type='spatial')
+                                               filters=['is_spatial'])
         else:
             self.spatial_subset = None
 
         self.hub.subscribe(self, AddDataMessage,
                            handler=self._on_viewer_data_changed)
         self.hub.subscribe(self, RemoveDataMessage,
                            handler=self._on_viewer_data_changed)
@@ -154,14 +157,16 @@
                            handler=self._on_viewer_subsets_changed)
         self.hub.subscribe(self, SubsetUpdateMessage,
                            handler=self._on_viewer_subsets_changed)
         self.hub.subscribe(self, SpectralMarksChangedMessage,
                            handler=self._on_plotted_lines_changed)
         self.hub.subscribe(self, LineIdentifyMessage,
                            handler=self._on_identified_line_changed)
+        self.hub.subscribe(self, GlobalDisplayUnitChanged,
+                           handler=self._on_global_display_unit_changed)
 
     @property
     def user_api(self):
         return PluginUserApi(self, expose=('dataset', 'spatial_subset', 'spectral_subset',
                                            'continuum', 'width',
                                            'show_continuum_marks', 'get_results'))
 
@@ -176,14 +181,15 @@
         get_data_kwargs = {'data_label': msg.data.label}
         if self.config == 'cubeviz':
             get_data_kwargs['function'] = getattr(viewer.state, 'function', None)
         viewer_data = self.app._jdaviz_helper.get_data(**get_data_kwargs)
 
         # If no data is currently plotted, don't attempt to update
         if viewer_data is None:
+            self.disabled_msg = 'Line Analysis unavailable without spectral data'
             return
 
         if viewer_data.spectral_axis.unit == u.pix:
             # disable the plugin until we can address this properly (either using the wavelength
             # solution to support pixels in line-lists, or properly displaying the extracted
             # 1d spectrum in wavelength-space)
             self.disabled_msg = 'Line Analysis unavailable when x-axis is in pixels'
@@ -198,38 +204,34 @@
         ----------
         msg : `glue.core.Message`
             The glue message passed to this callback method.
         """
         if (msg.subset.label in [self.spectral_subset_selected,
                                  self.spatial_subset_selected,
                                  self.continuum_subset_selected]
-                and self.plugin_opened):
+                and self.is_active):
             self._calculate_statistics()
 
-    @observe('plugin_opened')
-    def _on_plugin_opened_changed(self, *args):
+    def _on_global_display_unit_changed(self, msg):
+        if self.is_active:
+            self._calculate_statistics()
+
+    @observe('is_active')
+    def _is_active_changed(self, msg):
         if self.disabled_msg:
             return
-        # toggle continuum lines in spectrum viewer based on whether this plugin
-        # is currently open in the tray
-        self.show_continuum_marks(self.plugin_opened)
-
-    def show_continuum_marks(self, show=True):
-        """
-        Show (or hide) the marks indicating the continuum on the spectrum viewer.
 
-        Parameters
-        ----------
-        show : bool
-            Whether to show (or hide) the marks
-        """
         for pos, mark in self.marks.items():
-            mark.visible = show
-        if show:
-            self._calculate_statistics(ignore_plugin_closed=True)
+            mark.visible = self.is_active
+        if self.is_active:
+            self._calculate_statistics()
+
+    @deprecated(since="3.6", alternative="keep_active")
+    def show_continuum_marks(self):
+        self.keep_active = True
 
     @property
     def marks(self):
         marks = {}
         viewer = self.app.get_viewer(self._default_spectrum_viewer_reference_name)
         for mark in viewer.figure.marks:
             if isinstance(mark, LineAnalysisContinuum):
@@ -243,17 +245,17 @@
 
         if not len(marks):
             if not viewer.state.reference_data:
                 # we don't have data yet for scales, defer initializing
                 return {}
             # then haven't been initialized yet, so initialize with empty
             # marks that will be populated once the first analysis is done.
-            marks = {'left': LineAnalysisContinuumLeft(viewer, visible=self.plugin_opened),
-                     'center': LineAnalysisContinuumCenter(viewer, visible=self.plugin_opened),
-                     'right': LineAnalysisContinuumRight(viewer, visible=self.plugin_opened)}
+            marks = {'left': LineAnalysisContinuumLeft(viewer, visible=self.is_active),
+                     'center': LineAnalysisContinuumCenter(viewer, visible=self.is_active),
+                     'right': LineAnalysisContinuumRight(viewer, visible=self.is_active)}
             shadows = [ShadowLine(mark, shadow_width=2) for mark in marks.values()]
             # NOTE: += won't trigger the figure to notice new marks
             viewer.figure.marks = viewer.figure.marks + shadows + list(marks.values())
 
         return marks
 
     def update_results(self, results=None, mark_x={}, mark_y={}):
@@ -271,15 +273,15 @@
         # user-facing API call to force updating and retrieving results, even if the plugin
         # is closed
 
         if not self.spectral_subset_valid:
             valid, spec_range, subset_range = self._check_dataset_spectral_subset_valid(return_ranges=True)  # noqa
             raise ValueError(f"spectral subset '{self.spectral_subset.selected}' {subset_range} is outside data range of '{self.dataset.selected}' {spec_range}")  # noqa
 
-        self._calculate_statistics(ignore_plugin_closed=True)
+        self._calculate_statistics()
         return self.results
 
     def _on_plotted_lines_changed(self, msg):
         self.line_marks = msg.marks
         self.line_items = msg.names_rest
         if self.selected_line not in self.line_items:
             # default to identified line if available
@@ -300,47 +302,55 @@
         """
         Run the line analysis functions on the selected data/subset and
         display the results.
         """
         if not hasattr(self, 'dataset') or self.app._jdaviz_helper is None or self.dataset_selected == '':  # noqa
             # during initial init, this can trigger before the component is initialized
             return
+        if self.disabled_msg != '':
+            self.update_results(None)
+            return
 
         # call directly since this observe may be triggered before the spectral_subset_valid
         # traitlet is updated
         if not self._check_dataset_spectral_subset_valid():
             # skip gracefully, if the user called from get_results, and error would be raised there
             self.update_results(None)
             return
 
         # show spinner with overlay
         self.results_computing = True
+        full_spectrum = self.dataset.selected_spectrum_for_spatial_subset(self.spatial_subset_selected,  # noqa
+                                                                          use_display_units=True)
 
-        full_spectrum = self.dataset.selected_spectrum_for_spatial_subset(self.spatial_subset_selected)  # noqa
-
-        if (full_spectrum is None or self.width == "" or
-                (not self.plugin_opened and not kwargs.get('ignore_plugin_closed'))):
+        if full_spectrum is None or self.width == "":
             # this can happen DURING a unit conversion change
             self.update_results(None)
             return
 
         spectral_axis = full_spectrum.spectral_axis
+        if spectral_axis.unit == u.pix:
+            # plugin should be disabled so not get this far, but can still get here
+            # before the disabled message is set
+            self.update_results(None)
+            return
 
         if self.continuum_subset_selected == self.spectral_subset_selected:
             # already raised a validation error in the UI
             self.update_results(None)
             return
 
-        sr = self.app.get_subsets().get(self.spectral_subset_selected)
         if self.spectral_subset_selected == "Entire Spectrum":
             spectrum = full_spectrum
         else:
+            sr = self.app.get_subsets(self.spectral_subset_selected,
+                                      simplify_spectral=True, use_display_units=True)
             spectrum = extract_region(full_spectrum, sr, return_single_spectrum=True)
-            sr_lower = spectrum.spectral_axis[spectrum.spectral_axis.value >= sr.lower.value][0]
-            sr_upper = spectrum.spectral_axis[spectrum.spectral_axis.value <= sr.upper.value][-1]
+            sr_lower = np.nanmin(spectrum.spectral_axis[spectrum.spectral_axis.value >= sr.lower.value])  # noqa
+            sr_upper = np.nanmax(spectrum.spectral_axis[spectrum.spectral_axis.value <= sr.upper.value])  # noqa
 
         # compute continuum
         if self.continuum_subset_selected == "Surrounding" and self.spectral_subset_selected == "Entire Spectrum": # noqa
             # we know we'll just use the endpoints, so let's be efficient and not even
             # try extracting from the region
             continuum_mask = np.array([0, len(spectral_axis)-1])
             mark_x = {'left': np.array([]),
@@ -379,15 +389,16 @@
 
         else:
             # we'll access the mask of the continuum and then apply that to the spectrum.  For a
             # spatially-collapsed spectrum in cubeviz, this will access the mask from the full
             # cube, but still apply that to the spatially-collapsed spectrum.
             continuum_mask = ~self._specviz_helper.get_data(
                 self.dataset.selected,
-                spectral_subset=self.continuum_subset_selected).mask
+                spectral_subset=self.continuum_subset_selected,
+                use_display_units=False).mask
             spectral_axis_nanmasked = spectral_axis.value.copy()
             spectral_axis_nanmasked[~continuum_mask] = np.nan
             if self.spectral_subset_selected == "Entire Spectrum":
                 mark_x = {'left': spectral_axis_nanmasked,
                           'center': spectral_axis.value,
                           'right': []}
             else:
@@ -443,18 +454,28 @@
                     # Perform integration in frequency space
                     freq_spec = Spectrum1D(
                         spectral_axis=spec_subtracted.spectral_axis.to(u.Hz,
                                                                        equivalencies=u.spectral()),
                         flux=spec_subtracted.flux,
                         uncertainty=spec_subtracted.uncertainty)
 
-                    raw_result = analysis.line_flux(freq_spec)
+                    try:
+                        raw_result = analysis.line_flux(freq_spec)
+                    except ValueError as e:
+                        # can happen if interpolation out-of-bounds or any error from specutils
+                        # let's avoid the whole app crashing and instead expose the error to the
+                        # user
+                        self.hub.broadcast(SnackbarMessage(
+                            f"failed to calculate line analysis statistics: {e}", sender=self,
+                            color="warning"))
+                        self.update_results(None)
+                        return
+
                     # When flux is equivalent to Jy, lineflux result should be shown in W/m2
                     if flux_unit.is_equivalent(u.Jy/u.sr):
-
                         final_unit = u.Unit('W/(m2 sr)')
                     else:
                         final_unit = u.Unit('W/m2')
 
                     temp_result = raw_result.to(final_unit)
                     if getattr(raw_result, 'uncertainty', None) is not None:
                         temp_result.uncertainty = raw_result.uncertainty.to(final_unit)
@@ -465,15 +486,25 @@
                         flux_unit.is_equivalent(u.Unit('W/(m2 m sr)'))):
                     # Perform integration in wavelength space using MKS unit (meters)
                     wave_spec = Spectrum1D(
                         spectral_axis=spec_subtracted.spectral_axis.to(u.m,
                                                                        equivalencies=u.spectral()),
                         flux=spec_subtracted.flux,
                         uncertainty=spec_subtracted.uncertainty)
-                    raw_result = analysis.line_flux(wave_spec)
+                    try:
+                        raw_result = analysis.line_flux(wave_spec)
+                    except ValueError as e:
+                        # can happen if interpolation out-of-bounds or any error from specutils
+                        # let's avoid the whole app crashing and instead expose the error to the
+                        # user
+                        self.hub.broadcast(SnackbarMessage(
+                            f"failed to calculate line analysis statistics: {e}", sender=self,
+                            color="warning"))
+                        self.update_results(None)
+                        return
                     # When flux is equivalent to Jy, lineflux result should be shown in W/m2
                     if flux_unit.is_equivalent(u.Unit('W/(m2 m)'/u.sr)):
                         final_unit = u.Unit('W/(m2 sr)')
                     else:
                         final_unit = u.Unit('W/m2')
 
                     temp_result = raw_result.to(final_unit)
@@ -517,16 +548,16 @@
             self.selected_line = self.identified_line
 
         self.update_results(temp_results, mark_x, mark_y)
 
     def _compute_redshift_for_selected_line(self):
         index = self.line_items.index(self.selected_line)
         line_mark = self.line_marks[index]
-        rest_value = (line_mark.rest_value * line_mark._x_unit).to_value(u.AA,
-                                                                         equivalencies=u.spectral())
+        rest_value = (line_mark.rest_value * line_mark.xunit).to_value(u.AA,
+                                                                       equivalencies=u.spectral())
         return (self.results_centroid - rest_value) / rest_value
 
     @observe('sync_identify')
     def _sync_identify_changed(self, event={}):
         if not event.get('new', self.sync_identify):
             return
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue` & `jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 <template>
   <j-tray-plugin
     description="Return statistics for a single spectral line."
     :link="'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#line-analysis'"
+    :uses_active_status="uses_active_status"
+    @plugin-ping="plugin_ping($event)"
+    :keep_active.sync="keep_active"
     :disabled_msg="disabled_msg"
     :popout_button="popout_button">
 
     <j-plugin-section-header>Line</j-plugin-section-header>
     <v-row>
       <j-docs-link>Choose a region that defines the spectral line.</j-docs-link>
     </v-row>
@@ -129,59 +132,61 @@
           indeterminate
           color="spinner"
           size="50"
           width="6"
         ></v-progress-circular>
       </div>
 
-      <j-plugin-section-header>Redshift from Centroid</j-plugin-section-header>
-      <v-row>
-        <j-docs-link>Assign the centroid reported above to the observed wavelength of a given line and set the resulting redshift.  Lines must be loaded and plotted through the Line Lists plugin first.</j-docs-link>
-      </v-row>
-      <v-row class="row-no-outside-padding">
-        <v-col cols=2>
-          <j-tooltip tipid='plugin-line-analysis-sync-identify'>
-            <v-btn icon @click="() => sync_identify = !sync_identify" style="margin-top: 14px">
-              <img :class="sync_identify ? 'color-to-accent' : 'invert-if-dark'" :src="sync_identify ? sync_identify_icon_enabled : sync_identify_icon_disabled" width="20"/>
+      <div v-if="line_items.length > 0">
+        <j-plugin-section-header>Redshift from Centroid</j-plugin-section-header>
+        <v-row>
+          <j-docs-link>Assign the centroid reported above to the observed wavelength of a given line and set the resulting redshift.  Lines must be loaded and plotted through the Line Lists plugin first.</j-docs-link>
+        </v-row>
+        <v-row class="row-no-outside-padding">
+          <v-col cols=2>
+            <j-tooltip tipid='plugin-line-analysis-sync-identify'>
+              <v-btn icon @click="() => sync_identify = !sync_identify" style="margin-top: 14px">
+                <img :class="sync_identify ? 'color-to-accent' : 'invert-if-dark'" :src="sync_identify ? sync_identify_icon_enabled : sync_identify_icon_disabled" width="20"/>
+              </v-btn>
+            </j-tooltip>
+          </v-col>
+          <v-col cols=10>
+            <v-select
+              :menu-props="{ left: true }"
+              attach
+              :items="line_items"
+              v-model="selected_line"
+              label="Line"
+              hint="Select reference line."
+              persistent-hint
+            ></v-select>
+          </v-col>
+        </v-row>
+
+        <v-row v-if="selected_line">
+          <v-text-field
+            :value='selected_line_redshift'
+            class="mt-0 pt-0"
+            type="number"
+            label="Redshift"
+            hint="Redshift that will be applied by assigning centroid to the selected line."
+            persistent-hint
+            disabled
+          ></v-text-field>
+        </v-row>
+
+        <v-row justify="end">
+          <j-tooltip tipid='plugin-line-analysis-assign'>
+            <v-btn 
+            color="accent"
+            style="padding-left: 8px; padding-right: 8px;"
+            text
+            :disabled="!selected_line"
+            @click="line_assign">
+              Assign
             </v-btn>
           </j-tooltip>
-        </v-col>
-        <v-col cols=10>
-          <v-select
-            :menu-props="{ left: true }"
-            attach
-            :items="line_items"
-            v-model="selected_line"
-            label="Line"
-            hint="Select reference line."
-            persistent-hint
-          ></v-select>
-        </v-col>
-      </v-row>
-
-      <v-row v-if="selected_line">
-        <v-text-field
-          :value='selected_line_redshift'
-          class="mt-0 pt-0"
-          type="number"
-          label="Redshift"
-          hint="Redshift that will be applied by assigning centroid to the selected line."
-          persistent-hint
-          disabled
-        ></v-text-field>
-      </v-row>
-
-      <v-row justify="end">
-        <j-tooltip tipid='plugin-line-analysis-assign'>
-          <v-btn 
-           color="accent"
-           style="padding-left: 8px; padding-right: 8px;"
-           text
-           :disabled="!selected_line"
-           @click="line_assign">
-            Assign
-          </v-btn>
-        </j-tooltip>
-      </v-row>
+        </v-row>
+      </div>
     </div>  
   </j-tray-plugin>
 </template>
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py` & `jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+from numpy.testing import assert_allclose
 import pytest
 from astropy import units as u
 from astropy.table import QTable
 from glue.core.roi import XRangeROI
 from glue.core.edit_subset_mode import NewMode
 from regions import RectanglePixelRegion, PixCoord
 from specutils import Spectrum1D
@@ -10,27 +11,27 @@
 from jdaviz.configs.specviz.plugins.line_analysis.line_analysis import _coerce_unit
 from jdaviz.core.events import LineIdentifyMessage
 from jdaviz.core.marks import LineAnalysisContinuum
 
 
 def test_plugin(specviz_helper, spectrum1d):
     label = "Test 1D Spectrum"
-    specviz_helper.load_spectrum(spectrum1d, data_label=label)
+    specviz_helper.load_data(spectrum1d, data_label=label)
 
     plugin = specviz_helper.app.get_tray_item_from_name('specviz-line-analysis')
-    plugin.open_in_tray()
+    plugin.keep_active = True
 
     # continuum should be created, plotted, and visible
     sv = specviz_helper.app.get_viewer('spectrum-viewer')
     continuum_marks = [m for m in sv.figure.marks if isinstance(m, LineAnalysisContinuum)]
     assert len(continuum_marks) == 3
     assert np.all([cm.visible for cm in continuum_marks])
 
-    # closing tray/plugin should hide the continuum
-    specviz_helper.app.state.drawer = False
+    # disabling keep_active should hide the continuum
+    plugin.keep_active = False
     assert np.all([cm.visible is False for cm in continuum_marks])
 
     # add a region and rerun stats for that region
     sv.apply_roi(XRangeROI(6500, 7400))
     specviz_helper.app.state.drawer = True
 
     assert 'Subset 1' in plugin.spectral_subset.labels
@@ -59,15 +60,15 @@
 
     # create a spectral region
     spectrum_viewer = cubeviz_helper.app.get_viewer('spectrum-viewer')
     spectrum_viewer.apply_roi(XRangeROI(3.623e-7, 3.627e-7))  # meters
     cubeviz_helper.app.state.drawer = True
 
     plugin = cubeviz_helper.app.get_tray_item_from_name('specviz-line-analysis')
-    plugin.open_in_tray()
+    plugin.keep_active = True
 
     plugin.spatial_subset_selected = 'Subset 1'
     plugin.spectral_subset_selected = 'Subset 2'
     plugin.continuum_subset_selected = 'Surrounding'
     plugin.width = 1
 
     for result in plugin.results:
@@ -75,21 +76,21 @@
         assert not np.isnan(float(result['result']))
         # Check the unit is not dimensionless
         assert u.Unit(result['unit']) != u.dimensionless_unscaled
 
 
 def test_user_api(specviz_helper, spectrum1d):
     label = "Test 1D Spectrum"
-    specviz_helper.load_spectrum(spectrum1d, data_label=label)
+    specviz_helper.load_data(spectrum1d, data_label=label)
 
     sv = specviz_helper.app.get_viewer('spectrum-viewer')
     sv.apply_roi(XRangeROI(6500, 7400))
 
     la = specviz_helper.plugins['Line Analysis']
-    la.open_in_tray()
+    la.keep_active = True
 
     # spectral subset does not support multiselect
     assert "multiselect" not in la.spectral_subset.__repr__()
     with pytest.raises(ValueError):
         la.spectral_subset.select_all()
     with pytest.raises(ValueError):
         la.spectral_subset.select_none()
@@ -105,36 +106,37 @@
     assert la.spectral_subset.selected == 'Subset 1'
 
     la.get_results()
 
 
 def test_line_identify(specviz_helper, spectrum1d):
     label = "Test 1D Spectrum"
-    specviz_helper.load_spectrum(spectrum1d, data_label=label)
+    specviz_helper.load_data(spectrum1d, data_label=label)
 
     lt = QTable()
     lt['linename'] = ['O III', 'Halpha']
     lt['rest'] = [5007, 6563]*u.AA
     lt['listname'] = 'Test List'
     specviz_helper.load_line_list(lt)
 
     ll_plugin = specviz_helper.app.get_tray_item_from_name('g-line-list')
     la_plugin = specviz_helper.app.get_tray_item_from_name('specviz-line-analysis')
+    la_plugin.plugin_opened = True
     rest_names = [line['name_rest'] for line in ll_plugin.list_contents['Test List']['lines']]
 
     # will default to no selection
     assert la_plugin.selected_line == ''
 
     # check redshift
     assert la_plugin.selected_line_redshift == 0.0
 
     # but selecting a line from line-list (or clicking) should change the dropdown value
     # since sync is enabled by default
     assert la_plugin.sync_identify is True
-    # think this is the problem and we need to send the rest name here!
+
     msg = LineIdentifyMessage(rest_names[1],
                               sender=specviz_helper)
     specviz_helper.app.session.hub.broadcast(msg)
     assert la_plugin.selected_line == rest_names[1]
 
     # and changing the dropdown should change the identified line
     la_plugin.selected_line = rest_names[0]
@@ -158,15 +160,20 @@
     la_plugin.identified_line = ''
     la_plugin.sync_identify = False
     la_plugin.sync_identify = True
     assert la_plugin.identified_line == "O III 5007.0"
 
     # manually update redshift
     la_plugin.vue_line_assign()
-    assert la_plugin.selected_line_redshift == -1.0
+    assert_allclose(la_plugin.results_centroid, 7307.4232674401555)
+    line_mark = la_plugin.line_marks[la_plugin.line_items.index(la_plugin.selected_line)]
+    assert_allclose(line_mark.rest_value, 5007)
+    z = la_plugin._compute_redshift_for_selected_line()
+    assert_allclose(z, (la_plugin.results_centroid - line_mark.rest_value)/line_mark.rest_value)
+    assert_allclose(la_plugin.selected_line_redshift, z)
 
 
 def test_coerce_unit():
     q_input = 1 * u.Unit('1E-20 erg m / (Angstrom cm**2 s)')
     q_input.uncertainty = 0.1 * u.Unit('1E-20 erg m / (Angstrom cm**2 s)')
     q_coerced = _coerce_unit(q_input)
     assert q_coerced.unit == u.Unit('erg / (cm**2 s)')
@@ -176,18 +183,18 @@
     q_input.uncertainty = None
     q_coerced = _coerce_unit(q_input)
     assert not hasattr(q_coerced, 'uncertainty')
 
 
 def test_continuum_surrounding_spectral_subset(specviz_helper, spectrum1d):
     label = "Test 1D Spectrum"
-    specviz_helper.load_spectrum(spectrum1d, data_label=label)
+    specviz_helper.load_data(spectrum1d, data_label=label)
 
     plugin = specviz_helper.app.get_tray_item_from_name('specviz-line-analysis')
-    plugin.open_in_tray()
+    plugin.keep_active = True
 
     # continuum should be created, plotted, and visible
     sv = specviz_helper.app.get_viewer('spectrum-viewer')
     continuum_marks = [m for m in sv.figure.marks if isinstance(m, LineAnalysisContinuum)]
     assert len(continuum_marks) == 3
     assert np.all([cm.visible for cm in continuum_marks])
 
@@ -203,18 +210,18 @@
 
     # Values have not yet been validated
     np.testing.assert_allclose(float(plugin.results[0]['result']), 2.153181e-13, atol=1e-15)
 
 
 def test_continuum_spectral_same_value(specviz_helper, spectrum1d):
     label = "Test 1D Spectrum"
-    specviz_helper.load_spectrum(spectrum1d, data_label=label)
+    specviz_helper.load_data(spectrum1d, data_label=label)
 
     plugin = specviz_helper.app.get_tray_item_from_name('specviz-line-analysis')
-    plugin.open_in_tray()
+    plugin.keep_active = True
 
     # continuum should be created, plotted, and visible
     sv = specviz_helper.app.get_viewer('spectrum-viewer')
     continuum_marks = [m for m in sv.figure.marks if isinstance(m, LineAnalysisContinuum)]
     assert len(continuum_marks) == 3
     assert np.all([cm.visible for cm in continuum_marks])
 
@@ -230,18 +237,18 @@
 
     # continuum and spectral cannot be the same value
     assert plugin.results[0]['result'] == ''
 
 
 def test_continuum_surrounding_invalid_width(specviz_helper, spectrum1d):
     label = "Test 1D Spectrum"
-    specviz_helper.load_spectrum(spectrum1d, data_label=label)
+    specviz_helper.load_data(spectrum1d, data_label=label)
 
     plugin = specviz_helper.app.get_tray_item_from_name('specviz-line-analysis')
-    plugin.open_in_tray()
+    plugin.keep_active = True
 
     # continuum should be created, plotted, and visible
     sv = specviz_helper.app.get_viewer('spectrum-viewer')
     continuum_marks = [m for m in sv.figure.marks if isinstance(m, LineAnalysisContinuum)]
     assert len(continuum_marks) == 3
     assert np.all([cm.visible for cm in continuum_marks])
 
@@ -255,18 +262,18 @@
     plugin.spectral_subset_selected = 'Subset 1'
     plugin.width = 11
     assert plugin.results[0]['result'] == ''
 
 
 def test_continuum_subset_spectral_entire(specviz_helper, spectrum1d):
     label = "Test 1D Spectrum"
-    specviz_helper.load_spectrum(spectrum1d, data_label=label)
+    specviz_helper.load_data(spectrum1d, data_label=label)
 
     plugin = specviz_helper.app.get_tray_item_from_name('specviz-line-analysis')
-    plugin.open_in_tray()
+    plugin.keep_active = True
 
     # continuum should be created, plotted, and visible
     sv = specviz_helper.app.get_viewer('spectrum-viewer')
     continuum_marks = [m for m in sv.figure.marks if isinstance(m, LineAnalysisContinuum)]
     assert len(continuum_marks) == 3
     assert np.all([cm.visible for cm in continuum_marks])
 
@@ -282,18 +289,18 @@
 
     # Values have not yet been validated
     np.testing.assert_allclose(float(plugin.results[0]['result']), -2.79572e-13, atol=1e-15)
 
 
 def test_continuum_subset_spectral_subset2(specviz_helper, spectrum1d):
     label = "Test 1D Spectrum"
-    specviz_helper.load_spectrum(spectrum1d, data_label=label)
+    specviz_helper.load_data(spectrum1d, data_label=label)
 
     plugin = specviz_helper.app.get_tray_item_from_name('specviz-line-analysis')
-    plugin.open_in_tray()
+    plugin.keep_active = True
 
     # continuum should be created, plotted, and visible
     sv = specviz_helper.app.get_viewer('spectrum-viewer')
     continuum_marks = [m for m in sv.figure.marks if isinstance(m, LineAnalysisContinuum)]
     assert len(continuum_marks) == 3
     assert np.all([cm.visible for cm in continuum_marks])
 
@@ -315,18 +322,18 @@
 
     # Values have not yet been validated
     np.testing.assert_allclose(float(plugin.results[0]['result']), 1.482418e-14, atol=1e-16)
 
 
 def test_continuum_surrounding_no_right(specviz_helper, spectrum1d):
     label = "Test 1D Spectrum"
-    specviz_helper.load_spectrum(spectrum1d, data_label=label)
+    specviz_helper.load_data(spectrum1d, data_label=label)
 
     plugin = specviz_helper.app.get_tray_item_from_name('specviz-line-analysis')
-    plugin.open_in_tray()
+    plugin.keep_active = True
 
     # continuum should be created, plotted, and visible
     sv = specviz_helper.app.get_viewer('spectrum-viewer')
     continuum_marks = [m for m in sv.figure.marks if isinstance(m, LineAnalysisContinuum)]
     assert len(continuum_marks) == 3
     assert np.all([cm.visible for cm in continuum_marks])
 
@@ -343,18 +350,18 @@
 
     # Values have not yet been validated
     np.testing.assert_allclose(float(plugin.results[0]['result']), 4.204513e-14, atol=1e-16)
 
 
 def test_continuum_surrounding_no_left(specviz_helper, spectrum1d):
     label = "Test 1D Spectrum"
-    specviz_helper.load_spectrum(spectrum1d, data_label=label)
+    specviz_helper.load_data(spectrum1d, data_label=label)
 
     plugin = specviz_helper.app.get_tray_item_from_name('specviz-line-analysis')
-    plugin.open_in_tray()
+    plugin.keep_active = True
 
     # continuum should be created, plotted, and visible
     sv = specviz_helper.app.get_viewer('spectrum-viewer')
     continuum_marks = [m for m in sv.figure.marks if isinstance(m, LineAnalysisContinuum)]
     assert len(continuum_marks) == 3
     assert np.all([cm.visible for cm in continuum_marks])
 
@@ -371,18 +378,18 @@
 
     # Values have not yet been validated
     np.testing.assert_allclose(float(plugin.results[0]['result']), 7.570859e-14, atol=1e-16)
 
 
 def test_subset_changed(specviz_helper, spectrum1d):
     label = "Test 1D Spectrum"
-    specviz_helper.load_spectrum(spectrum1d, data_label=label)
+    specviz_helper.load_data(spectrum1d, data_label=label)
 
     plugin = specviz_helper.app.get_tray_item_from_name('specviz-line-analysis')
-    plugin.open_in_tray()
+    plugin.keep_active = True
 
     # continuum should be created, plotted, and visible
     sv = specviz_helper.app.get_viewer('spectrum-viewer')
     continuum_marks = [m for m in sv.figure.marks if isinstance(m, LineAnalysisContinuum)]
     assert len(continuum_marks) == 3
     assert np.all([cm.visible for cm in continuum_marks])
 
@@ -402,20 +409,20 @@
 
     # Values have not yet been validated
     np.testing.assert_allclose(float(plugin.results[0]['result']), 2.153181e-13, atol=1e-15)
 
 
 def test_invalid_subset(specviz_helper, spectrum1d):
     # 6000-8000
-    specviz_helper.load_spectrum(spectrum1d, data_label="right_spectrum")
+    specviz_helper.load_data(spectrum1d, data_label="right_spectrum")
 
     # 5000-7000
     sp2 = Spectrum1D(spectral_axis=spectrum1d.spectral_axis - 1000*spectrum1d.spectral_axis.unit,
                      flux=spectrum1d.flux * 1.25)
-    specviz_helper.load_spectrum(sp2, data_label="left_spectrum")
+    specviz_helper.load_data(sp2, data_label="left_spectrum")
 
     # apply subset that overlaps on left_spectrum, but not right_spectrum
     # NOTE: using a subset that overlaps the right_spectrum (reference) results in errors when
     # retrieving the subset (https://github.com/spacetelescope/jdaviz/issues/1868)
     specviz_helper.app.get_viewer('spectrum-viewer').apply_roi(XRangeROI(5000, 6000))
 
     plugin = specviz_helper.plugins['Line Analysis']
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py` & `jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,16 @@
     '''
     Returns the line flux calculation by opening the Line Analysis Plugin
     Assumes the plugin hasn't been opened yet
     '''
     # Open the plugin and force the calculation
     viz_helper.app.state.drawer = True
     line_analysis_plugin = viz_helper.app.get_tray_item_from_name('specviz-line-analysis')
-    line_analysis_plugin.open_in_tray()
+    line_analysis_plugin.keep_active = True
+
     # Retrieve Results
     for result in line_analysis_plugin.results:
         if result['function'] == 'Line Flux':
             return result
 
 
 @pytest.mark.filterwarnings(r"ignore:.* contains multiple slashes")
@@ -95,15 +96,15 @@
 @pytest.mark.filterwarnings(r"ignore:.* contains multiple slashes")
 @pytest.mark.parametrize('test_case', unit_flux_gaussian_test_cases)
 def test_unit_gaussian(specviz_helper, test_case):
     '''
     Test an Area 1 Gaussian and ensure the result returns in W/m2
     Test provided by Patrick Ogle
     '''
-    specviz_helper.load_spectrum(test_case)
+    specviz_helper.load_data(test_case)
 
     lineflux_result = _calculate_line_flux(specviz_helper)
     assert_quantity_allclose(float(lineflux_result['result']) * u.Unit(lineflux_result['unit']),
                              1*u.Unit('W/m2'))
 
 
 @pytest.mark.filterwarnings(r"ignore:.* contains multiple slashes")
@@ -113,11 +114,11 @@
     Test provided by Patrick Ogle
     '''
     # unit-flux gaussian in wavelength space, mixed units, per steradian
     lam_a = np.arange(1, 2, 0.001)*u.Angstrom
     flx_wave = _gauss_with_unity_area(lam_a.value, mn, sig)*1E3*u.erg/u.s/u.cm**2/u.Angstrom/u.sr
     fl_wave = Spectrum1D(spectral_axis=lam_a, flux=flx_wave)
 
-    specviz_helper.load_spectrum(fl_wave)
+    specviz_helper.load_data(fl_wave)
     lineflux_result = _calculate_line_flux(specviz_helper)
     assert_quantity_allclose(float(lineflux_result['result']) * u.Unit(lineflux_result['unit']),
                              1*u.Unit('W/(m2sr)'))
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz/plugins/parsers.py` & `jdaviz-3.6.0/jdaviz/configs/specviz/plugins/parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,40 +72,28 @@
             for i in range(len(data)):
                 temp_labels.append(f"{data_label} {i}")
             data_label = temp_labels
         elif len(data_label) != len(data):
             raise ValueError(f"Length of data labels list ({len(data_label)}) is different"
                              f" than length of list of data ({len(data)})")
 
-    # If there's already visible data in the viewer, convert units if needed
-    current_unit = None
-    if spectrum_viewer_reference_name in app.get_viewer_reference_names():
-        sv = app.get_viewer(spectrum_viewer_reference_name)
-        for layer_state in sv.state.layers:
-            if layer_state.visible:
-                current_unit = sv.state.x_display_unit
-
     with app.data_collection.delay_link_manager_update():
         # these are used to build a combined spectrum with all
         # input spectra included (taken from https://github.com/spacetelescope/
         # dat_pyinthesky/blob/main/jdat_notebooks/MRS_Mstar_analysis/
         # JWST_Mstar_dataAnalysis_analysis.ipynb)
         wlallorig = []
         fnuallorig = []
         dfnuallorig = []
 
         for i, spec in enumerate(data):
 
             wave_units = spec.spectral_axis.unit
             flux_units = spec.flux.unit
 
-            if current_unit is not None and spec.spectral_axis.unit != current_unit:
-                spec = Spectrum1D(flux=spec.flux,
-                                  spectral_axis=spec.spectral_axis.to(current_unit))
-
             # Make metadata layout conform with other viz.
             spec.meta = standardize_metadata(spec.meta)
 
             app.add_data(spec, data_label[i])
 
             # handle display, with the SpectrumList special case in mind.
             if show_in_viewer:
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz/plugins/viewers.py` & `jdaviz-3.6.0/jdaviz/configs/specviz/plugins/viewers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 import warnings
 
 import numpy as np
 from astropy import table
 from astropy import units as u
+from astropy.nddata import StdDevUncertainty, VarianceUncertainty, InverseVariance
 from glue.core import BaseData
 from glue.core.subset import Subset
+from glue.core.subset_group import GroupedSubset
 from glue.config import data_translator
 from glue_jupyter.bqplot.profile import BqplotProfileView
 from glue.core.exceptions import IncompatibleAttribute
 from matplotlib.colors import cnames
 from specutils import Spectrum1D
 
 from jdaviz.core.events import SpectralMarksChangedMessage, LineIdentifyMessage
 from jdaviz.core.registries import viewer_registry
 from jdaviz.core.marks import SpectralLine, LineUncertainties, ScatterMask, OffscreenLinesMarks
 from jdaviz.core.linelists import load_preset_linelist, get_available_linelists
 from jdaviz.core.freezable_state import FreezableProfileViewerState
 from jdaviz.configs.default.plugins.viewers import JdavizViewerMixin
+from jdaviz.utils import get_subset_type
 
 __all__ = ['SpecvizProfileView']
 
 
+uncertainty_str_to_cls_mapping = {
+    "std": StdDevUncertainty,
+    "var": VarianceUncertainty,
+    "ivar": InverseVariance
+}
+
+
 @viewer_registry("specviz-profile-viewer", label="Profile 1D (Specviz)")
 class SpecvizProfileView(JdavizViewerMixin, BqplotProfileView):
     # categories: zoom resets, zoom, pan, subset, select tools, shortcuts
     tools_nested = [
                     ['jdaviz:homezoom', 'jdaviz:prevzoom'],
                     ['jdaviz:boxzoom', 'jdaviz:xrangezoom', 'jdaviz:yrangezoom'],
                     ['jdaviz:panzoom', 'jdaviz:panzoom_x', 'jdaviz:panzoom_y'],
@@ -34,18 +44,19 @@
                 ]
 
     default_class = Spectrum1D
     spectral_lines = None
     _state_cls = FreezableProfileViewerState
 
     def __init__(self, *args, **kwargs):
+        default_tool_priority = kwargs.pop('default_tool_priority', [])
         super().__init__(*args, **kwargs)
 
         self._subscribe_to_layers_update()
-        self.initialize_toolbar(default_tool_priority=['jdaviz:selectslice'])
+        self.initialize_toolbar(default_tool_priority=default_tool_priority)
         self._offscreen_lines_marks = OffscreenLinesMarks(self)
         self.figure.marks = self.figure.marks + self._offscreen_lines_marks.marks
 
         self.state.add_callback('show_uncertainty', self._show_uncertainty_changed)
 
         self.display_mask = False
 
@@ -346,28 +357,43 @@
             Alpha value for plotting.
 
         Returns
         -------
         result : bool
             `True` if successful, `False` otherwise.
         """
+        # If this is the first loaded data, set things up for unit conversion.
+        if len(self.layers) == 0:
+            reset_plot_axes = True
+        else:
+            reset_plot_axes = False
+
         # The base class handles the plotting of the main
         # trace representing the spectrum itself.
         result = super().add_data(data, color, alpha, **layer_state)
 
+        if reset_plot_axes:
+            x_units = data.get_component(self.state.x_att.label).units
+            y_units = data.get_component("flux").units
+            self.state.x_display_unit = x_units if len(x_units) else None
+            self.state.y_display_unit = y_units if len(y_units) else None
+            self.set_plot_axes()
+
         self._plot_uncertainties()
 
         self._plot_mask()
 
         # Set default linewidth on any created spectral subset layers
         # NOTE: this logic will need updating if we add support for multiple cubes as this assumes
         # that new data entries (from model fitting or gaussian smooth, etc) will only be spectra
         # and all subsets affected will be spectral
         for layer in self.state.layers:
-            if "Subset" in layer.layer.label and layer.layer.data.label == data.label:
+            if (isinstance(layer.layer, GroupedSubset)
+                    and get_subset_type(layer.layer) == 'spectral'
+                    and layer.layer.data.label == data.label):
                 layer.linewidth = 3
 
         return result
 
     def _plot_mask(self):
         if not self.display_mask:
             return
@@ -429,14 +455,19 @@
 
             comps = [str(component) for component in lyr.components]
 
             # Ignore data that does not have an uncertainty component
             if "uncertainty" in comps:  # noqa
                 error = np.array(lyr['uncertainty'].data)
 
+                # ensure that the uncertainties are represented as stddev:
+                uncertainty_type_str = lyr.meta.get('uncertainty_type', 'stddev')
+                uncert_cls = uncertainty_str_to_cls_mapping[uncertainty_type_str]
+                error = uncert_cls(error).represent_as(StdDevUncertainty).array
+
                 data_obj = lyr.data.get_object()
                 data_x = data_obj.spectral_axis.value
                 data_y = data_obj.flux.value
 
                 # The shaded band around the spectrum trace is bounded by
                 # two lines, above and below the spectrum trace itself.
                 data_x_list = np.ndarray.tolist(data_x)
@@ -472,29 +503,28 @@
                                                     close_path=False
                                                     )
 
                 # Add error lines to viewer
                 self.figure.marks = list(self.figure.marks) + [error_line_mark]
 
     def set_plot_axes(self):
-        # Get data to be used for axes labels
-        data = self.data()[0]
-
         # Set axes labels for the spectrum viewer
-        spectral_axis_unit_type = str(data.spectral_axis.unit.physical_type).title()
-        # flux_unit_type = data.flux.unit.physical_type.title()
         flux_unit_type = "Flux density"
-
-        if data.spectral_axis.unit.is_equivalent(u.m):
+        x_disp_unit = self.state.x_display_unit
+        x_unit = u.Unit(x_disp_unit) if x_disp_unit else u.dimensionless_unscaled
+        if x_unit.is_equivalent(u.m):
             spectral_axis_unit_type = "Wavelength"
-        elif data.spectral_axis.unit.is_equivalent(u.pixel):
-            spectral_axis_unit_type = "pixel"
+        elif x_unit.is_equivalent(u.Hz):
+            spectral_axis_unit_type = "Frequency"
+        elif x_unit.is_equivalent(u.pixel):
+            spectral_axis_unit_type = "Pixel"
+        else:
+            spectral_axis_unit_type = str(x_unit.physical_type).title()
 
-        label_0 = f"{spectral_axis_unit_type} [{data.spectral_axis.unit.to_string()}]"
-        self.figure.axes[0].label = label_0
-        self.figure.axes[1].label = f"{flux_unit_type} [{data.flux.unit.to_string()}]"
+        self.figure.axes[0].label = f"{spectral_axis_unit_type} [{self.state.x_display_unit}]"
+        self.figure.axes[1].label = f"{flux_unit_type} [{self.state.y_display_unit}]"
 
         # Make it so y axis label is not covering tick numbers.
         self.figure.axes[1].label_offset = "-50"
 
         # Set Y-axis to scientific notation
         self.figure.axes[1].tick_format = '0.1e'
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz/specviz.yaml` & `jdaviz-3.6.0/jdaviz/configs/specviz/specviz.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz/tests/test_helper.py` & `jdaviz-3.6.0/jdaviz/configs/specviz/tests/test_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,70 +6,68 @@
 from astropy.tests.helper import assert_quantity_allclose
 from glue.core.roi import XRangeROI
 from glue.core.edit_subset_mode import OrMode, AndMode, AndNotMode
 from specutils import Spectrum1D, SpectrumList, SpectrumCollection
 from astropy.utils.data import download_file
 
 from jdaviz.app import Application
-from jdaviz.configs.specviz.plugins.unit_conversion import unit_conversion as uc
 from jdaviz.core.marks import LineUncertainties
 from jdaviz import Specviz
 
 
 class TestSpecvizHelper:
     @pytest.fixture(autouse=True)
     def setup_class(self, specviz_helper, spectrum1d, multi_order_spectrum_list):
         self.spec_app = specviz_helper
         self.spec = spectrum1d
         self.spec_list = SpectrumList([spectrum1d] * 3)
         self.multi_order_spectrum_list = multi_order_spectrum_list
 
         self.label = "Test 1D Spectrum"
-        self.spec_app.load_spectrum(spectrum1d, data_label=self.label)
+        self.spec_app.load_data(spectrum1d, data_label=self.label)
 
     def test_load_spectrum1d(self):
         # starts with a single loaded spectrum1d object:
         assert len(self.spec_app.app.data_collection) == 1
         dc_0 = self.spec_app.app.data_collection[0]
         assert dc_0.label == self.label
         assert dc_0.meta['uncertainty_type'] == 'std'
 
-        data = self.spec_app.app.get_data_from_viewer('spectrum-viewer')
+        data = self.spec_app.get_data()
 
-        assert isinstance(list(data.values())[0], Spectrum1D)
-        assert list(data.keys())[0] == self.label
+        assert isinstance(data, Spectrum1D)
 
     def test_load_spectrum_list_no_labels(self):
         # now load three more spectra from a SpectrumList, without labels
-        self.spec_app.load_spectrum(self.spec_list)
+        self.spec_app.load_data(self.spec_list)
         assert len(self.spec_app.app.data_collection) == 4
         for i in (1, 2, 3):
             assert "specviz_data" in self.spec_app.app.data_collection[i].label
 
     def test_load_spectrum_list_with_labels(self):
         # now load three more spectra from a SpectrumList, with labels:
         labels = ["List test 1", "List test 2", "List test 3"]
-        self.spec_app.load_spectrum(self.spec_list, data_label=labels)
+        self.spec_app.load_data(self.spec_list, data_label=labels)
         assert len(self.spec_app.app.data_collection) == 4
 
     def test_load_multi_order_spectrum_list(self):
         assert len(self.spec_app.app.data_collection) == 1
         # now load ten spectral orders from a SpectrumList:
-        self.spec_app.load_spectrum(self.multi_order_spectrum_list)
+        self.spec_app.load_data(self.multi_order_spectrum_list)
         assert len(self.spec_app.app.data_collection) == 11
 
     def test_mismatched_label_length(self):
         with pytest.raises(ValueError, match='Length'):
             labels = ["List test 1", "List test 2"]
-            self.spec_app.load_spectrum(self.spec_list, data_label=labels)
+            self.spec_app.load_data(self.spec_list, data_label=labels)
 
     def test_load_spectrum_collection(self):
         with pytest.raises(TypeError):
             collection = SpectrumCollection([1]*u.AA)
-            self.spec_app.load_spectrum(collection)
+            self.spec_app.load_data(collection)
 
     def test_get_spectra(self):
         with pytest.warns(UserWarning, match='Applying the value from the redshift slider'):
             spectra = self.spec_app.get_spectra()
 
         assert_quantity_allclose(spectra[self.label].flux,
                                  self.spec.flux, atol=1e-5*u.Unit(self.spec.flux.unit))
@@ -243,23 +241,23 @@
 def test_get_spectra_no_spectra_label_redshift_error(specviz_helper, spectrum1d):
     label = "label"
     with pytest.raises(ValueError):
         specviz_helper.get_spectra(data_label=label, apply_slider_redshift=True)
 
 
 def test_add_spectrum_after_subset(specviz_helper, spectrum1d):
-    specviz_helper.load_spectrum(spectrum1d, data_label="test")
+    specviz_helper.load_data(spectrum1d, data_label="test")
     specviz_helper.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(6200, 7000))
     new_spec = specviz_helper.get_spectra(apply_slider_redshift=True)["test"]*0.9
-    specviz_helper.load_spectrum(new_spec, data_label="test2")
+    specviz_helper.load_data(new_spec, data_label="test2")
 
 
 def test_get_spectral_regions_unit(specviz_helper, spectrum1d):
     # Ensure units we put in are the same as the units we get out
-    specviz_helper.load_spectrum(spectrum1d)
+    specviz_helper.load_data(spectrum1d)
     specviz_helper.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(6200, 7000))
 
     subsets = specviz_helper.get_spectral_regions()
     reg = subsets.get('Subset 1')
 
     assert spectrum1d.spectral_axis.unit == reg.lower.unit
     assert spectrum1d.spectral_axis.unit == reg.upper.unit
@@ -273,15 +271,15 @@
     label_mouseover._viewer_mouse_event(spec_viewer,
                                         {'event': 'mousemove', 'domain': {'x': 6100, 'y': 12.5}})
     assert label_mouseover.as_text() == ('', '', '')
     assert label_mouseover.icon == ''
 
     # If the reference (visible) data changes via unit conversion,
     # check that the region's units convert too
-    specviz_helper.load_spectrum(spectrum1d)
+    specviz_helper.load_data(spectrum1d)  # Originally Angstrom
 
     # Also check coordinates info panel.
     # x=0 -> 6000 A, x=1 -> 6222.222 A
     label_mouseover._viewer_mouse_event(spec_viewer,
                                         {'event': 'mousemove', 'domain': {'x': 6100, 'y': 12.5}})
     assert label_mouseover.as_text() == ('Cursor 6.10000e+03, 1.25000e+01',
                                          'Wave 6.00000e+03 Angstrom (0 pix)',  # actual 0.4
@@ -289,51 +287,46 @@
     assert label_mouseover.icon == 'a'
 
     label_mouseover._viewer_mouse_event(spec_viewer,
                                         {'event': 'mousemove', 'domain': {'x': None, 'y': 12.5}})
     assert label_mouseover.as_text() == ('', '', '')
     assert label_mouseover.icon == ''
 
-    # Convert the wavelength axis to microns
-    new_spectral_axis = "micron"
-    conv_func = uc.UnitConversion.process_unit_conversion
-    converted_spectrum = conv_func(specviz_helper.app, spectrum=spectrum1d,
-                                   new_spectral_axis=new_spectral_axis)
-
-    # Add this new data and clear the other, making the converted spectrum our reference
-    specviz_helper.app.add_data(converted_spectrum, "Converted Spectrum")
-    specviz_helper.app.add_data_to_viewer("spectrum-viewer",
-                                          "Converted Spectrum",
-                                          clear_other_data=True)
+    # Convert the wavelength axis to micron
+    new_spectral_axis = "um"
+    specviz_helper.plugins['Unit Conversion'].spectral_unit = new_spectral_axis
 
-    specviz_helper.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(0.6, 0.7))
+    spec_viewer.apply_roi(XRangeROI(0.6, 0.7))
 
-    # TODO: Is this test still relevant with the upcoming glue unit conversion changes?
     # Retrieve the Subset
-    # subsets = specviz_helper.get_spectral_regions()
-    # reg = subsets.get('Subset 1')
-    #
-    # assert reg.lower.unit == u.Unit(new_spectral_axis)
-    # assert reg.upper.unit == u.Unit(new_spectral_axis)
+    subsets = specviz_helper.get_spectral_regions(use_display_units=False)
+    reg = subsets.get('Subset 1')
+    assert reg.lower.unit == u.Angstrom
+    assert reg.upper.unit == u.Angstrom
+
+    subsets = specviz_helper.get_spectral_regions(use_display_units=True)
+    reg = subsets.get('Subset 1')
+    assert reg.lower.unit == u.um
+    assert reg.upper.unit == u.um
 
     # Coordinates info panel should show new unit
     label_mouseover._viewer_mouse_event(spec_viewer,
                                         {'event': 'mousemove', 'domain': {'x': 0.61, 'y': 12.5}})
     label_mouseover.as_text() == ('Cursor 6.10000e-01, 1.25000e+01',
                                   'Wave 6.00000e-01 micron (0 pix)',
                                   'Flux 1.24967e+01 Jy')
-    assert label_mouseover.icon == 'b'
+    assert label_mouseover.icon == 'a'
 
     label_mouseover._viewer_mouse_event(spec_viewer, {'event': 'mouseleave'})
     assert label_mouseover.as_text() == ('', '', '')
     assert label_mouseover.icon == ''
 
 
 def test_subset_default_thickness(specviz_helper, spectrum1d):
-    specviz_helper.load_spectrum(spectrum1d)
+    specviz_helper.load_data(spectrum1d)
 
     sv = specviz_helper.app.get_viewer('spectrum-viewer')
     sv.toolbar.active_tool = sv.toolbar.tools['bqplot:xrange']
     from glue.core.roi import XRangeROI
     sv.apply_roi(XRangeROI(2.5, 3.5))
     # _on_layers_update is not triggered within CI
     sv._on_layers_update()
@@ -353,15 +346,15 @@
     with ZipFile(fn, 'r') as sample_data_zip:
         sample_data_zip.extractall(tmpdir.strpath)
     data_path = str(tmpdir.join('NIRISS_for_parser_p0171'))
 
     # Load two NIRISS x1d files from FITS. They have 19 and 20 EXTRACT1D
     # extensions per file, for a total of 39 spectra to load:
     with pytest.warns(UserWarning, match='SRCTYPE is missing or UNKNOWN in JWST x1d loader'):
-        specviz_helper.load_spectrum(data_path)
+        specviz_helper.load_data(data_path)
 
     # NOTE: the length was 3 before specutils 1.9 (https://github.com/astropy/specutils/pull/982)
     expected_len = 39
     assert len(specviz_helper.app.data_collection) == expected_len
 
     for data in specviz_helper.app.data_collection:
         assert data.main_components[:2] == ['flux', 'uncertainty']
@@ -380,20 +373,20 @@
     data_path = str(tmpdir.join('NIRISS_for_parser_p0171'))
 
     # Load two x1d files from FITS. They have 19 and 20 EXTRACT1D
     # extensions per file, for a total of 39 spectra to load. Also concatenate
     # spectra common to each file into one "Combined" spectrum to load per file.
     # Now the total is (19 EXTRACT 1D + 1 Combined) + (20 EXTRACT 1D + 1 Combined) = 41.
     with pytest.warns(UserWarning, match='SRCTYPE is missing or UNKNOWN in JWST x1d loader'):
-        specviz_helper.load_spectrum(data_path, concat_by_file=True)
+        specviz_helper.load_data(data_path, concat_by_file=True)
     assert len(specviz_helper.app.data_collection) == 41
 
 
 def test_plot_uncertainties(specviz_helper, spectrum1d):
-    specviz_helper.load_spectrum(spectrum1d)
+    specviz_helper.load_data(spectrum1d)
 
     specviz_viewer = specviz_helper.app.get_viewer("spectrum-viewer")
 
     assert len([m for m in specviz_viewer.figure.marks if isinstance(m, LineUncertainties)]) == 0
 
     specviz_viewer.state.show_uncertainty = True
     uncert_marks = [m for m in specviz_viewer.figure.marks if isinstance(m, LineUncertainties)]
@@ -419,31 +412,31 @@
         plugin = plugin_api._obj
         for attr in plugin_api._expose:
             assert hasattr(plugin, attr)
 
 
 def test_data_label_as_posarg(specviz_helper, spectrum1d):
     # Passing in data_label keyword as posarg.
-    specviz_helper.load_spectrum(spectrum1d, 'my_spec')
+    specviz_helper.load_data(spectrum1d, 'my_spec')
     assert specviz_helper.app.data_collection[0].label == 'my_spec'
 
 
 def test_spectra_partial_overlap(specviz_helper):
     spec_viewer = specviz_helper.app.get_viewer('spectrum-viewer')
 
     wave_1 = np.linspace(6000, 7000, 10) * u.AA
     flux_1 = ([1200] * wave_1.size) * u.nJy
     sp_1 = Spectrum1D(flux=flux_1, spectral_axis=wave_1)
 
     wave_2 = wave_1 + (800 * u.AA)
     flux_2 = ([60] * wave_2.size) * u.nJy
     sp_2 = Spectrum1D(flux=flux_2, spectral_axis=wave_2)
 
-    specviz_helper.load_spectrum(sp_1, data_label='left')
-    specviz_helper.load_spectrum(sp_2, data_label='right')
+    specviz_helper.load_data(sp_1, data_label='left')
+    specviz_helper.load_data(sp_2, data_label='right')
 
     # Test mouseover outside of left but in range for right.
     # Should show right spectrum even when mouse is near left flux.
     label_mouseover = specviz_helper.app.session.application._tools['g-coords-info']
     label_mouseover._viewer_mouse_event(spec_viewer,
                                         {'event': 'mousemove', 'domain': {'x': 7022, 'y': 1000}})
     assert label_mouseover.as_text() == ('Cursor 7.02200e+03, 1.00000e+03',
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz2d/helper.py` & `jdaviz-3.6.0/jdaviz/configs/specviz2d/helper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import numpy as np
-
 from jdaviz.configs.specviz import Specviz
 from jdaviz.core.helpers import ConfigHelper
 from jdaviz.core.events import SnackbarMessage
 from jdaviz.configs.default.plugins.line_lists.line_list_mixin import LineListMixin
 from jdaviz.configs.specviz2d.plugins.spectral_extraction.spectral_extraction import SpectralExtraction  # noqa
 
 __all__ = ['Specviz2d']
@@ -16,108 +14,24 @@
     _default_spectrum_viewer_reference_name = "spectrum-viewer"
     _default_spectrum_2d_viewer_reference_name = "spectrum-2d-viewer"
     _default_table_viewer_reference_name = "table-viewer"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        spec1d = self.app.get_viewer(self._default_spectrum_viewer_reference_name)
-        spec1d.scales['x'].observe(self._update_spec2d_x_axis)
-
-        spec2d = self.app.get_viewer(self._default_spectrum_2d_viewer_reference_name)
-        spec2d.scales['x'].observe(self._update_spec1d_x_axis)
-
     @property
     def specviz(self):
         """
         A Specviz helper (`~jdaviz.configs.specviz.helper.Specviz`) for the Jdaviz
         application that is wrapped by Specviz2d.
         """
         if not hasattr(self, '_specviz'):
             self._specviz = Specviz(app=self.app)
         return self._specviz
 
-    def _extend_world(self, spec1d, ext):
-        # Extend 1D spectrum world axis to enable panning (within reason) past
-        # the bounds of data
-        world = self.app.data_collection[spec1d]["World 0"].copy()
-        dw = world[1]-world[0]
-        prepend = np.linspace(world[0]-dw*ext, world[0]-dw, ext)
-        dw = world[-1]-world[-2]
-        append = np.linspace(world[-1]+dw, world[-1]+dw*ext, ext)
-        world = np.hstack((prepend, world, append))
-        return world
-
-    def _update_spec2d_x_axis(self, change):
-        # This assumes the two spectrum viewers have the same x-axis shape and
-        # wavelength solution, which should always hold
-        if change['old'] is None:
-            pass
-        else:
-            name = change['name']
-            if name not in ['min', 'max']:
-                return
-            new_val = change['new']
-            spec1d = self.app.get_viewer(
-                self._default_spectrum_viewer_reference_name
-            ).state.reference_data.label
-            extend_by = int(self.app.data_collection[spec1d]["World 0"].shape[0])
-            world = self._extend_world(spec1d, extend_by)
-
-            # Warn the user if they've panned far enough away from the data
-            # that the viewers will desync
-            if new_val > world[-1] or new_val < world[0]:
-                self.app.hub.broadcast(SnackbarMessage(
-                    "Panning too far away from the data may desync the 1D and 2D spectrum viewers.",
-                    color='warning', sender=self))
-
-            idx = float((np.abs(world - new_val)).argmin()) - extend_by
-            scales = self.app.get_viewer(self._default_spectrum_2d_viewer_reference_name).scales
-            old_idx = getattr(scales['x'], name)
-            if idx != old_idx:
-                setattr(scales['x'], name, idx)
-
-    def _update_spec1d_x_axis(self, change):
-        if self.app.get_viewer(
-                self._default_spectrum_viewer_reference_name
-        ).state.reference_data is None:
-            return
-
-        # This assumes the two spectrum viewers have the same x-axis shape and
-        # wavelength solution, which should always hold
-        if change['old'] is None:
-            pass
-        else:
-            name = change['name']
-            if name not in ['min', 'max']:
-                return
-            new_idx = int(np.around(change['new']))
-            spec1d = self.app.get_viewer(
-                self._default_spectrum_viewer_reference_name
-            ).state.reference_data.label
-            extend_by = int(self.app.data_collection[spec1d]["World 0"].shape[0])
-            world = self._extend_world(spec1d, extend_by)
-
-            scales = self.app.get_viewer(
-                self._default_spectrum_viewer_reference_name
-            ).scales
-            old_val = getattr(scales['x'], name)
-
-            # Warn the user if they've panned far enough away from the data
-            # that the viewers will desync
-            try:
-                val = world[new_idx+extend_by]
-            except IndexError:
-                val = old_val
-                self.app.hub.broadcast(SnackbarMessage(
-                    "Panning too far away from the data may desync the 1D and 2D spectrum viewers.",
-                    color='warning', sender=self))
-            if val != old_val:
-                setattr(scales['x'], name, val)
-
     def load_data(self, spectrum_2d=None, spectrum_1d=None, spectrum_1d_label=None,
                   spectrum_2d_label=None, show_in_viewer=True, ext=1,
                   transpose=False):
         """
         Load and parse a pair of corresponding 1D and 2D spectra.
 
         Parameters
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/parsers.py` & `jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py` & `jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
                                         AddResults)
 from jdaviz.core.user_api import PluginUserApi
 from jdaviz.core.custom_traitlets import IntHandleEmpty, FloatHandleEmpty
 from jdaviz.core.marks import PluginLine
 
 from astropy.modeling import models
 from astropy.nddata import StdDevUncertainty, VarianceUncertainty, UnknownUncertainty
-from astropy import units
 from specreduce import tracing
 from specreduce import background
 from specreduce import extract
 
 __all__ = ['SpectralExtraction']
 
 _model_cls = {'Spline': models.Spline1D,
@@ -92,14 +91,15 @@
     * ``ext_add_results`` (:class:`~jdaviz.core.template_mixin.AddResults`)
     * :meth:`import_extract`
     * :meth:`export_extract`
     * :meth:`export_extract_spectrum`
     """
     dialog = Bool(False).tag(sync=True)
     template_file = __file__, "spectral_extraction.vue"
+    uses_active_status = Bool(True).tag(sync=True)
 
     active_step = Unicode().tag(sync=True)
     interactive_extract = Bool(True).tag(sync=True)
 
     # TRACE
     trace_trace_items = List().tag(sync=True)
     trace_trace_selected = Unicode().tag(sync=True)
@@ -393,36 +393,29 @@
 
         Parameters
         ----------
         step : str
             Step in the extraction process to visualize.  Must be one of: 'trace', 'bg', 'ext'.
         """
         if step is not None:
-            self.plugin_opened = True
             if step == 'trace':
                 self._interaction_in_trace_step()
             elif step == 'bg':
                 self._interaction_in_bg_step()
             elif step == 'ext':
                 self._interaction_in_ext_step()
             else:
                 raise ValueError("step must be one of: trace, bg, ext")
 
-    def clear_marks(self):
-        """
-        Manually clear the live-preview marks.
-        """
-        self.plugin_opened = False
-
-    @observe('plugin_opened', 'interactive_extract')
+    @observe('is_active', 'interactive_extract')
     def _update_plugin_marks(self, *args):
         if not self._do_marks:
             return
 
-        if not self.plugin_opened:
+        if not (self.is_active):
             for step, mark in self.marks.items():
                 mark.visible = False
             return
 
         if self.active_step == '':
             # on load, default to 'extract' (this will then trigger the observe to update the marks)
             self._interaction_in_ext_step()
@@ -472,43 +465,43 @@
 
         if not viewer2d.state.reference_data:
             # we don't have data yet for scales, defer initializing
             return {}
 
         # the marks haven't been initialized yet, so initialize with empty
         # marks that will be populated once the first analysis is done.
-        self._marks = {'trace': PluginLine(viewer2d, visible=self.plugin_opened),
-                       'ext_lower': PluginLine(viewer2d, visible=self.plugin_opened),
-                       'ext_upper': PluginLine(viewer2d, visible=self.plugin_opened),
-                       'bg1_center': PluginLine(viewer2d, visible=self.plugin_opened,
+        self._marks = {'trace': PluginLine(viewer2d, visible=self.is_active),
+                       'ext_lower': PluginLine(viewer2d, visible=self.is_active),
+                       'ext_upper': PluginLine(viewer2d, visible=self.is_active),
+                       'bg1_center': PluginLine(viewer2d, visible=self.is_active,
                                                 line_style='dotted'),
-                       'bg1_lower': PluginLine(viewer2d, visible=self.plugin_opened),
-                       'bg1_upper': PluginLine(viewer2d, visible=self.plugin_opened),
-                       'bg2_center': PluginLine(viewer2d, visible=self.plugin_opened,
+                       'bg1_lower': PluginLine(viewer2d, visible=self.is_active),
+                       'bg1_upper': PluginLine(viewer2d, visible=self.is_active),
+                       'bg2_center': PluginLine(viewer2d, visible=self.is_active,
                                                 line_style='dotted'),
-                       'bg2_lower': PluginLine(viewer2d, visible=self.plugin_opened),
-                       'bg2_upper': PluginLine(viewer2d, visible=self.plugin_opened)}
+                       'bg2_lower': PluginLine(viewer2d, visible=self.is_active),
+                       'bg2_upper': PluginLine(viewer2d, visible=self.is_active)}
         # NOTE: += won't trigger the figure to notice new marks
         viewer2d.figure.marks = viewer2d.figure.marks + list(self._marks.values())
 
-        self._marks['extract'] = PluginLine(viewer1d, visible=self.plugin_opened)
-        self._marks['bg_spec'] = PluginLine(viewer1d, visible=self.plugin_opened, stroke_width=1)  # noqa
+        self._marks['extract'] = PluginLine(viewer1d, visible=self.is_active)
+        self._marks['bg_spec'] = PluginLine(viewer1d, visible=self.is_active, stroke_width=1)  # noqa
 
         # NOTE: += won't trigger the figure to notice new marks
         viewer1d.figure.marks = viewer1d.figure.marks + [self._marks['extract'],
                                                          self._marks['bg_spec']]
 
         return self._marks
 
     @observe('trace_dataset_selected', 'trace_type_selected',
              'trace_trace_selected', 'trace_offset', 'trace_order',
              'trace_pixel', 'trace_peak_method_selected',
              'trace_do_binning', 'trace_bins', 'trace_window', 'active_step')
     def _interaction_in_trace_step(self, event={}):
-        if not self.plugin_opened or not self._do_marks:
+        if not self.is_active or not self._do_marks:
             return
         if event.get('name', '') == 'active_step' and event.get('new') != 'trace':
             return
 
         try:
             trace = self.export_trace(add_data=False)
         except Exception:
@@ -521,15 +514,15 @@
         self.active_step = 'trace'
         self._update_plugin_marks()
 
     @observe('bg_dataset_selected', 'bg_type_selected',
              'bg_trace_selected', 'bg_trace_pixel',
              'bg_separation', 'bg_width', 'bg_statistic_selected', 'active_step')
     def _interaction_in_bg_step(self, event={}):
-        if not self.plugin_opened or not self._do_marks:
+        if not self.is_active or not self._do_marks:
             return
         if event.get('name', '') == 'active_step' and event.get('new') != 'bg':
             return
 
         try:
             trace = self._get_bg_trace()
         except Exception:
@@ -577,15 +570,15 @@
 
         self.active_step = 'bg'
         self._update_plugin_marks()
 
     @observe('ext_dataset_selected', 'ext_trace_selected',
              'ext_type_selected', 'ext_width', 'active_step')
     def _interaction_in_ext_step(self, event={}):
-        if not self.plugin_opened or not self._do_marks:
+        if not self.is_active or not self._do_marks:
             return
         if event.get('name', '') == 'active_step' and event.get('new') != 'ext':
             return
 
         try:
             trace = self._get_ext_trace()
         except Exception:
@@ -825,18 +818,14 @@
             defined in the plugin.
         """
         spec = self.export_bg(**kwargs).bkg_spectrum()
 
         if add_data:
             self.bg_spec_add_results.add_results_from_plugin(spec, replace=False)
 
-        # TEMPORARY: override spectral axis to be in pixels until properly supporting plotting
-        # in wavelength/frequency
-        spec._spectral_axis = np.arange(len(spec.spectral_axis)) * units.pix
-
         return spec
 
     def vue_create_bg_spec(self, *args):
         self.export_bg_spectrum(add_data=True)
 
     def export_bg_sub(self, add_data=False, **kwargs):
         """
@@ -920,18 +909,14 @@
         add_data : bool
             Whether to add the resulting spectrum to the application, according to the options
             defined in the plugin.
         """
         extract = self.export_extract(**kwargs)
         spectrum = extract.spectrum
 
-        # TEMPORARY: override spectral axis to be in pixels until properly supporting plotting
-        # in wavelength/frequency
-        spectrum._spectral_axis = np.arange(len(spectrum.spectral_axis)) * units.pix
-
         if add_data:
             self.ext_add_results.add_results_from_plugin(spectrum, replace=False)
 
         return spectrum
 
     def vue_extract_spectrum(self, *args):
         self.export_extract_spectrum(add_data=True)
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue` & `jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 <template>
   <j-tray-plugin
     description="2D to 1D spectral extraction."
     :link="'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#spectral-extraction'"
+    :uses_active_status="uses_active_status"
+    @plugin-ping="plugin_ping($event)"
+    :keep_active.sync="keep_active"
     :popout_button="popout_button">
 
     <v-row>
       <v-expansion-panels popout>
         <v-expansion-panel>
           <v-expansion-panel-header v-slot="{ open }">
             <span style="padding: 6px">Settings</span>
@@ -155,15 +158,15 @@
             hint="Method to use for identifying the peak cross-dispersion pixel in each bin"
             persistent-hint
           ></v-select>
         </v-row>
       </div>
 
       <v-row>
-        <v-expansion-panels popout>
+        <v-expansion-panels accordion>
           <v-expansion-panel>
             <v-expansion-panel-header v-slot="{ open }">
               <span style="padding: 6px">Export Trace</span>
             </v-expansion-panel-header>
             <v-expansion-panel-content>
               <plugin-add-results
                 :label.sync="trace_results_label"
@@ -269,15 +272,15 @@
           label="Statistic"
           hint="Statistic to use over the background window."
           persistent-hint
         ></v-select>
       </v-row>
 
       <v-row>
-        <v-expansion-panels popout>
+        <v-expansion-panels accordion>
           <v-expansion-panel>
             <v-expansion-panel-header v-slot="{ open }">
               <span style="padding: 6px">Export Background Image</span>
             </v-expansion-panel-header>
             <v-expansion-panel-content>
               <plugin-add-results
                 :label.sync="bg_results_label"
@@ -293,15 +296,15 @@
                 @click:action="create_bg_img"
               ></plugin-add-results>
             </v-expansion-panel-content>
           </v-expansion-panel>
         </v-expansion-panels>
       </v-row>
       <v-row>
-        <v-expansion-panels popout>
+        <v-expansion-panels accordion>
           <v-expansion-panel>
             <v-expansion-panel-header v-slot="{ open }">
               <span style="padding: 6px">Export Background Spectrum</span>
             </v-expansion-panel-header>
             <v-expansion-panel-content>
               <plugin-add-results
                 :label.sync="bg_spec_results_label"
@@ -317,15 +320,15 @@
                 @click:action="create_bg_spec"
               ></plugin-add-results>
             </v-expansion-panel-content>
           </v-expansion-panel>
         </v-expansion-panels>
       </v-row>
       <v-row>
-        <v-expansion-panels popout>
+        <v-expansion-panels accordion>
           <v-expansion-panel>
             <v-expansion-panel-header v-slot="{ open }">
               <span style="padding: 6px">Export Background-Subtracted Image</span>
             </v-expansion-panel-header>
             <v-expansion-panel-content>
               <plugin-add-results
                 :label.sync="bg_sub_results_label"
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py` & `jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     pext = specviz2d_helper.app.get_tray_item_from_name('spectral-extraction')
 
     # test trace marks - won't be created until after opening the plugin
     sp2dv = specviz2d_helper.app.get_viewer('spectrum-2d-viewer')
     assert len(sp2dv.figure.marks) == 2
 
-    pext.open_in_tray()
+    pext.keep_active = True
     assert len(sp2dv.figure.marks) == 11
     assert pext.marks['trace'].visible is True
     assert len(pext.marks['trace'].x) > 0
 
     # create FlatTrace
     pext.trace_type_selected = 'Flat'
     pext.trace_pixel = 28
@@ -152,15 +152,15 @@
 @pytest.mark.filterwarnings('ignore')
 def test_user_api(specviz2d_helper):
     fn = download_file('https://stsci.box.com/shared/static/exnkul627fcuhy5akf2gswytud5tazmw.fits', cache=True)  # noqa
 
     specviz2d_helper.load_data(spectrum_2d=fn)
 
     pext = specviz2d_helper.plugins['Spectral Extraction']
-    pext.open_in_tray()
+    pext.keep_active = True
 
     # test that setting a string to an AddResults object redirects to the label
     pext.bg_sub_add_results = 'override label'
     assert pext.bg_sub_add_results.label == 'override label'
     pext.bg_sub_add_results.label = 'override label 2'
     assert "override label 2" in pext.bg_sub_add_results.__repr__()
     assert "override label 2" in pext.bg_sub_add_results._obj.auto_label.__repr__()
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz2d/specviz2d.yaml` & `jdaviz-3.6.0/jdaviz/configs/specviz2d/specviz2d.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -17,24 +17,23 @@
   - g-metadata-viewer
   - g-plot-options
   - g-subset-plugin
   - g-markers
   - spectral-extraction
   - g-gaussian-smooth
   - g-model-fitting
-  - g-unit-conversion
   - g-line-list
   - specviz-line-analysis
   - g-export-plot
 viewer_area:
   - container: col
     children:
       - container: row
         viewers:
           - name: 2D Spectrum viewer
             plot: mosviz-profile-2d-viewer
             reference: spectrum-2d-viewer
       - container: row
         viewers:
           - name: Spectrum
-            plot: specviz-profile-viewer
+            plot: mosviz-profile-viewer
             reference: spectrum-viewer
```

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz2d/tests/test_helper.py` & `jdaviz-3.6.0/jdaviz/configs/specviz2d/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/configs/specviz2d/tests/test_parsers.py` & `jdaviz-3.6.0/jdaviz/configs/specviz2d/tests/test_parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,17 +75,17 @@
     assert label_mouseover.as_text() == ('Pixel x=00000.0 y=00000.0 Value +3.74540e-01', '', '')
     assert label_mouseover.icon == 'a'
 
     viewer_1d = specviz2d_helper.app.get_viewer('spectrum-viewer')
     # need to trigger a mouseleave or mouseover to reset the traitlets
     label_mouseover._viewer_mouse_event(viewer_1d, {'event': 'mouseenter'})
     label_mouseover._viewer_mouse_event(viewer_1d,
-                                        {'event': 'mousemove', 'domain': {'x': 6.5, 'y': 3}})
-    assert label_mouseover.as_text() == ('Cursor 6.50000e+00, 3.00000e+00',
-                                         'Wave 6.00000e+00 pix',
+                                        {'event': 'mousemove', 'domain': {'x': 7.2e-6, 'y': 3}})
+    assert label_mouseover.as_text() == ('Cursor 7.20000e-06, 3.00000e+00',
+                                         'Wave 7.00000e-06 m (6 pix)',
                                          'Flux -3.59571e+00')
     assert label_mouseover.icon == 'b'
 
 
 def test_1d_parser(specviz2d_helper, spectrum1d):
     specviz2d_helper.load_data(spectrum_1d=spectrum1d)
     assert len(specviz2d_helper.app.data_collection) == 1
```

### Comparing `jdaviz-3.5.0/jdaviz/conftest.py` & `jdaviz-3.6.0/jdaviz/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
         sc.append(spectrum1d)
 
     return SpectrumList(sc)
 
 
 def _create_spectrum1d_cube_with_fluxunit(fluxunit=u.Jy, shape=(2, 2, 4), with_uncerts=False):
-
+    # nz=2 nx=2 ny=4
     flux = np.arange(np.prod(shape)).reshape(shape) * fluxunit
     wcs_dict = {"CTYPE1": "RA---TAN", "CTYPE2": "DEC--TAN", "CTYPE3": "WAVE-LOG",
                 "CRVAL1": 205, "CRVAL2": 27, "CRVAL3": 4.622e-7,
                 "CDELT1": -0.0001, "CDELT2": 0.0001, "CDELT3": 8e-11,
                 "CRPIX1": 0, "CRPIX2": 0, "CRPIX3": 0}
     w = WCS(wcs_dict)
     if with_uncerts:
@@ -214,25 +214,25 @@
 
 @pytest.fixture
 def spectrum1d_cube_custom_fluxunit():
     return _create_spectrum1d_cube_with_fluxunit
 
 
 @pytest.fixture
-def mos_spectrum1d():
+def mos_spectrum1d(mos_spectrum2d):
     '''
     A specially defined Spectrum1d that matches the corresponding spectrum2d below.
 
     TODO: this fixture should be replaced by the global spectrum1d fixture defined in
     jdaviz/conftest.py AFTER reforming the spectrum2d fixture below to match the
     global spectrum1d fixture.
 
     Unless linking the two is required, try to use the global spectrum1d fixture.
     '''
-    spec_axis = np.linspace(6000, 8000, 1024) * u.AA
+    spec_axis = mos_spectrum2d.spectral_axis
     np.random.seed(42)
     flux = (np.random.randn(len(spec_axis.value)) +
             10*np.exp(-0.001*(spec_axis.value-6563)**2) +
             spec_axis.value/500) * u.Jy
 
     return Spectrum1D(spectral_axis=spec_axis, flux=flux)
```

### Comparing `jdaviz-3.5.0/jdaviz/container.vue` & `jdaviz-3.6.0/jdaviz/container.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/core/astrowidgets_api.py` & `jdaviz-3.6.0/jdaviz/core/astrowidgets_api.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/core/config.py` & `jdaviz-3.6.0/jdaviz/core/config.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/core/custom_traitlets.py` & `jdaviz-3.6.0/jdaviz/core/custom_traitlets.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/core/data_formats.py` & `jdaviz-3.6.0/jdaviz/core/data_formats.py`

 * *Files 10% similar despite different names*

```diff
@@ -150,31 +150,36 @@
     filename : str (path-like)
         Name for a local data file.
     ext : int
         Extension from the FITS file.
 
     Returns
     -------
-    helper_name : str
-        Name of the best-guess helper for ``filename``.
+    helper_name : list of str
+        Name of the best-guess compatible helpers for ``filename``.
+
+    Fits HDUList : astropy.io.fits.HDUList
+        The HDUList of the file opened to identify the helper
     """
     supported_dtypes = [
         Spectrum1D,
         SpectrumList,
         SpectrumCollection,
         CCDData
     ]
 
     if filename.lower().endswith('asdf'):
         # ASDF files are only supported in jdaviz for
         # Roman WFI 2D images, so suggest imviz:
-        return 'imviz'
+        return (['imviz'], None)
 
-    header = fits.getheader(filename, ext=ext)
-    data = fits.getdata(filename, ext=ext)
+    # Must use memmap=False to force close all handles and allow file overwrite
+    hdul = fits.open(filename, memmap=False)
+    data = hdul[ext]
+    header = data.header
     wcs = _get_wcs(filename, header)
     has_spectral_axis = 'spectral' in wcs.world_axis_object_classes
 
     n_axes = (
         int(has_spectral_axis) +
 
         sum([component[0] in ['celestial', 'angle']
@@ -197,18 +202,18 @@
     # If CCDData is the only match:
     if len(possible_formats) == 1:
         only_key, only_value = possible_formats.popitem()
         if only_key == CCDData:
             # could be 2D spectrum or 2D image. break tie with WCS:
             if has_spectral_axis:
                 if n_axes > 1:
-                    return 'specviz2d'
-                return 'specviz'
+                    return (['specviz2d'], hdul)
+                return (['specviz'], hdul)
             elif not isinstance(data, fits.BinTableHDU):
-                return 'imviz'
+                return (['imviz'], hdul)
 
     # Ensure specviz is chosen when ``data`` is a table or recarray
     # and there's a "known" spectral column name:
     if isinstance(data, (fits.BinTableHDU, fits.fitsrec.FITS_rec)):
         # now catch spectra in FITS tables, looking for
         # columns with "wave" or "flux" in the names:
         table_columns = [getattr(col, 'name', col).lower() for col in data.columns]
@@ -226,49 +231,49 @@
             found_col.startswith(known_col)
             for known_col in known_spectral_columns
             for found_col in table_columns
         ]
 
         # if at least one spectral column is found:
         if sum(found_spectral_columns):
-            return 'specviz'
+            return (['specviz'], hdul)
 
     # If the data could be spectral:
     for cls in [Spectrum1D, SpectrumList]:
         if cls in possible_formats.keys():
             recognized_spectrum_format = possible_formats[cls][0].lower()
 
             # first catch known JWST spectrum types:
             if (n_axes == 3 and
                     recognized_spectrum_format.find('s3d') > -1):
-                return 'cubeviz'
+                return (['cubeviz'], hdul)
             elif (n_axes == 2 and
                   recognized_spectrum_format.find('x1d') > -1):
-                return 'specviz'
+                return (['specviz'], hdul)
 
             # we intentionally don't choose specviz2d for
             # data recognized as 's2d' as we did with the cases above,
             # because 2D data products could be 2D spectra *or* 2D images
             # that the registry recognizes as s2d.
 
             # Use WCS to break the tie below:
             elif n_axes == 2:
                 if has_spectral_axis:
-                    return 'specviz2d'
-                return 'imviz'
+                    return (['specviz2d'], hdul)
+                return (['imviz'], hdul)
 
             elif n_axes == 1:
-                return 'specviz'
+                return (['specviz'], hdul)
 
     try:
         # try using the specutils registry:
         valid_format, config = identify_data(filename)
-        return config
+        return ([config], hdul)
     except ValueError:
         # if file type not recognized:
         pass
 
     if n_axes == 2 and not has_spectral_axis:
         # at this point, non-spectral 2D data are likely images:
-        return 'imviz'
+        return (['imviz'], hdul)
 
     raise ValueError(f"No helper could be auto-identified for {filename}.")
```

### Comparing `jdaviz-3.5.0/jdaviz/core/events.py` & `jdaviz-3.6.0/jdaviz/core/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import astropy.units as u
 from glue.core.message import Message
 
 __all__ = ['NewViewerMessage', 'ViewerAddedMessage', 'ViewerRemovedMessage', 'LoadDataMessage',
            'AddDataMessage', 'SnackbarMessage', 'RemoveDataMessage',
            'AddLineListMessage', 'RowLockMessage',
            'SliceSelectSliceMessage',
            'SliceToolStateMessage',
            'TableClickMessage', 'LinkUpdatedMessage', 'ExitBatchLoadMessage',
-           'MarkersChangedMessage', 'CanvasRotationChangedMessage']
+           'MarkersChangedMessage', 'CanvasRotationChangedMessage',
+           'GlobalDisplayUnitChanged']
 
 
 class NewViewerMessage(Message):
     """Message to trigger viewer creation in the application."""
     def __init__(self, cls, data, x_attr=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -333,7 +335,23 @@
     @property
     def angle(self):
         return self._angle
 
     @property
     def flip_horizontal(self):
         return self._flip_horizontal
+
+
+class GlobalDisplayUnitChanged(Message):
+    '''Message generated when the global app-wide display unit is changed'''
+    def __init__(self, axis, unit, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._axis = axis
+        self._unit = unit
+
+    @property
+    def axis(self):
+        return self._axis
+
+    @property
+    def unit(self):
+        return u.Unit(self._unit)
```

### Comparing `jdaviz-3.5.0/jdaviz/core/freezable_state.py` & `jdaviz-3.6.0/jdaviz/core/freezable_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from glue.viewers.profile.state import ProfileViewerState
 from glue_jupyter.bqplot.image.state import BqplotImageViewerState
 from glue.viewers.matplotlib.state import DeferredDrawCallbackProperty as DDCProperty
 
 __all__ = ['FreezableState', 'FreezableProfileViewerState', 'FreezableBqplotImageViewerState']
 
 
-class FreezableState():
+class FreezableState:
     _frozen_state = []
 
     def __setattr__(self, k, v):
         if k[0] == '_' or k not in self._frozen_state:
             super().__setattr__(k, v)
         elif getattr(self, k) is None:
             # still allow Nones to be updated to initial values
```

### Comparing `jdaviz-3.5.0/jdaviz/core/helpers.py` & `jdaviz-3.6.0/jdaviz/core/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import warnings
 from contextlib import contextmanager
 from inspect import isclass
 
 import numpy as np
 import astropy.units as u
 from astropy.wcs.wcsapi import BaseHighLevelWCS
-from astropy.nddata import CCDData
+from astropy.nddata import CCDData, StdDevUncertainty
 from regions.core.core import Region
 from glue.core import HubListener
 from glue.core.edit_subset_mode import NewMode
 from glue.core.message import SubsetCreateMessage, SubsetDeleteMessage
 from glue.core.subset import Subset, MaskSubsetState
 from glue.config import data_translator
 from ipywidgets.widgets import widget_serialization
@@ -408,16 +408,56 @@
         Shows Jdaviz in a sidecar in a new tab to the right
         """
         warnings.warn('show_in_new_tab has been replaced with show(loc="sidecar:tab-after")',
                       DeprecationWarning)
         return self.show(loc="sidecar:tab-after", title=title)
 
     def _get_data(self, data_label=None, spatial_subset=None, spectral_subset=None,
-                  mask_subset=None, function=None, cls=None):
-        # Start validity checks
+                  mask_subset=None, function=None, cls=None, use_display_units=False):
+        def _handle_display_units(data, use_display_units):
+            if use_display_units:
+                if isinstance(data, Spectrum1D):
+                    spectral_unit = self.app._get_display_unit('spectral')
+                    if not spectral_unit:
+                        return data
+                    if self.app.config == 'cubeviz' and spectral_unit == 'deg':
+                        # this happens before the correct axis is set for the spectrum-viewer
+                        # and would result in a unit-conversion error if attempting to convert
+                        # to the display units.  This should only ever be temporary during
+                        # app intialization.
+                        return data
+                    flux_unit = self.app._get_display_unit('flux')
+                    # TODO: any other attributes (meta, wcs, etc)?
+                    # TODO: implement uncertainty.to upstream
+                    uncertainty = data.uncertainty
+                    if uncertainty is not None:
+                        # convert the uncertainties to StdDevUncertainties, since
+                        # that is assumed in a few places in jdaviz:
+                        if uncertainty.unit is None:
+                            uncertainty.unit = data.flux.unit
+                        if hasattr(uncertainty, 'represent_as'):
+                            new_uncert = uncertainty.represent_as(
+                                StdDevUncertainty
+                            ).quantity.to(flux_unit)
+                        else:
+                            # if not specified as NDUncertainty, assume stddev:
+                            new_uncert = uncertainty.quantity.to(flux_unit)
+                        new_uncert = StdDevUncertainty(new_uncert, unit=flux_unit)
+                    else:
+                        new_uncert = None
+
+                    data = Spectrum1D(spectral_axis=data.spectral_axis.to(spectral_unit,
+                                                                          u.spectral()),
+                                      flux=data.flux.to(flux_unit,
+                                                        u.spectral_density(data.spectral_axis)),
+                                      uncertainty=new_uncert)
+                else:  # pragma: nocover
+                    raise NotImplementedError(f"converting {data.__class__.__name__} to display units is not supported")  # noqa
+            return data
+
         list_of_valid_function_values = ('minimum', 'maximum', 'mean',
                                          'median', 'sum')
         if function and function not in list_of_valid_function_values:
             raise ValueError(f"function {function} not in list of valid"
                              f" function values {list_of_valid_function_values}")
 
         list_of_valid_subset_names = [x.label for x in self.app.data_collection.subset_groups]
@@ -467,15 +507,15 @@
             if 'Trace' in data.meta:
                 if cls is not None:  # pragma: no cover
                     raise ValueError("cls not supported for Trace object")
                 data = data.get_object()
             else:
                 data = data.get_object(cls=cls, **object_kwargs)
 
-            return data
+            return _handle_display_units(data, use_display_units)
 
         if not cls and spatial_subset:
             raise AttributeError(f"A valid cls must be provided to"
                                  f" apply subset {spatial_subset} to data. "
                                  f"Instead, {cls} was given.")
         elif not cls and mask_subset:
             raise AttributeError(f"A valid cls must be provided to"
@@ -524,35 +564,40 @@
                               f" Exception: {e}")
             if spatial_subset or function:
                 # Return collapsed Spectrum1D object with spectral subset mask applied
                 data.mask = spec_subset.mask
             else:
                 data = spec_subset
 
-        return data
+        return _handle_display_units(data, use_display_units)
 
-    def get_data(self, data_label=None, cls=None):
+    def get_data(self, data_label=None, cls=None, use_display_units=False, **kwargs):
         """
         Returns data with name equal to data_label of type cls.
 
         Parameters
         ----------
         data_label : str, optional
             Provide a label to retrieve a specific data set from data_collection.
         cls : `~specutils.Spectrum1D`, `~astropy.nddata.CCDData`, optional
             The type that data will be returned as.
+        use_display_units : bool, optional
+            Whether to convert to the display units defined in the <unit-conversion> plugin.
+        kwargs : dict
+            For Cubeviz, you could also pass in ``function`` (str) to collapse
+            the cube into 1D spectrum using provided function.
 
         Returns
         -------
         data : cls
-            Data is returned as type cls.
+            Data is returned as type ``cls``.
 
         """
-        return self._get_data(data_label=data_label, spatial_subset=None,
-                              spectral_subset=None, function=None, cls=None)
+        return self._get_data(data_label=data_label,
+                              cls=cls, use_display_units=use_display_units, **kwargs)
 
 
 class ImageConfigHelper(ConfigHelper):
     """`ConfigHelper` that uses an image viewer as its primary viewer.
     For example, Imviz and Cubeviz.
     """
 
@@ -654,20 +699,25 @@
         bad_regions : list of (obj, str) or `None`
             If requested (see ``return_bad_regions`` option), return a
             list of ``(region, reason)`` tuples for region objects that failed to load.
             If all the regions loaded successfully, this list will be empty.
             If not requested, return `None`.
 
         """
+        if len(self.app.data_collection) == 0:
+            raise ValueError('Cannot load regions without data.')
+
         from photutils.aperture import (CircularAperture, SkyCircularAperture,
                                         EllipticalAperture, SkyEllipticalAperture,
-                                        RectangularAperture, SkyRectangularAperture)
+                                        RectangularAperture, SkyRectangularAperture,
+                                        CircularAnnulus, SkyCircularAnnulus)
         from regions import (Regions, CirclePixelRegion, CircleSkyRegion,
                              EllipsePixelRegion, EllipseSkyRegion,
-                             RectanglePixelRegion, RectangleSkyRegion)
+                             RectanglePixelRegion, RectangleSkyRegion,
+                             CircleAnnulusPixelRegion, CircleAnnulusSkyRegion)
         from jdaviz.core.region_translators import regions2roi, aperture2regions
 
         # If user passes in one region obj instead of list, try to be smart.
         if not isinstance(regions, (list, tuple, Regions)):
             regions = [regions]
 
         n_loaded = 0
@@ -684,31 +734,35 @@
             data = self.app.data_collection[refdata_label]
 
         # TODO: Make this work for data cube.
         # https://github.com/glue-viz/glue-astronomy/issues/75
         has_wcs = data_has_valid_wcs(data, ndim=2)
 
         for region in regions:
-            if isinstance(region, (SkyCircularAperture, SkyEllipticalAperture,
-                                   SkyRectangularAperture, CircleSkyRegion,
-                                   EllipseSkyRegion, RectangleSkyRegion)) and not has_wcs:
+            if (isinstance(region, (SkyCircularAperture, SkyEllipticalAperture,
+                                    SkyRectangularAperture, SkyCircularAnnulus,
+                                    CircleSkyRegion, EllipseSkyRegion,
+                                    RectangleSkyRegion, CircleAnnulusSkyRegion))
+                    and not has_wcs):
                 bad_regions.append((region, 'Sky region provided but data has no valid WCS'))
                 continue
 
             # photutils: Convert to regions shape first
             if isinstance(region, (CircularAperture, SkyCircularAperture,
                                    EllipticalAperture, SkyEllipticalAperture,
-                                   RectangularAperture, SkyRectangularAperture)):
+                                   RectangularAperture, SkyRectangularAperture,
+                                   CircularAnnulus, SkyCircularAnnulus)):
                 region = aperture2regions(region)
 
             # regions: Convert to ROI.
             # NOTE: Out-of-bounds ROI will succeed; this is native glue behavior.
             if isinstance(region, (CirclePixelRegion, CircleSkyRegion,
                                    EllipsePixelRegion, EllipseSkyRegion,
-                                   RectanglePixelRegion, RectangleSkyRegion)):
+                                   RectanglePixelRegion, RectangleSkyRegion,
+                                   CircleAnnulusPixelRegion, CircleAnnulusSkyRegion)):
                 state = regions2roi(region, wcs=data.coords)
 
                 # TODO: Do we want user to specify viewer? Does it matter?
                 self.app.session.edit_subset_mode._mode = NewMode
                 self.default_viewer.apply_roi(state)
                 self.app.session.edit_subset_mode.edit_subset = None  # No overwrite next iteration # noqa
```

### Comparing `jdaviz-3.5.0/jdaviz/core/linelists.py` & `jdaviz-3.6.0/jdaviz/core/linelists.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/core/marks.py` & `jdaviz-3.6.0/jdaviz/core/marks.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 from astropy import units as u
 from bqplot import LinearScale
 from bqplot.marks import Lines, Label, Scatter
 from copy import deepcopy
 from glue.core import HubListener
 from specutils import Spectrum1D
 
+from jdaviz.core.events import GlobalDisplayUnitChanged
 from jdaviz.core.events import (SliceToolStateMessage, LineIdentifyMessage,
                                 SpectralMarksChangedMessage,
                                 RedshiftMessage)
 
 __all__ = ['OffscreenLinesMarks', 'BaseSpectrumVerticalLine', 'SpectralLine',
            'SliceIndicatorMarks', 'ShadowMixin', 'ShadowLine', 'ShadowLabelFixedY',
-           'PluginMark', 'PluginLine', 'PluginScatter',
+           'PluginMark', 'LinesAutoUnit', 'PluginLine', 'PluginScatter',
            'LineAnalysisContinuum', 'LineAnalysisContinuumCenter',
            'LineAnalysisContinuumLeft', 'LineAnalysisContinuumRight',
            'LineUncertainties', 'ScatterMask', 'SelectedSpaxel', 'MarkersMark']
 
 
 class OffscreenLinesMarks(HubListener):
     def __init__(self, viewer):
@@ -54,19 +55,93 @@
                     oob_left += 1
                 elif m.x[0] > self.viewer.state.x_max:
                     oob_right += 1
         self.left.text = [f'\u25c0 {oob_left}' if oob_left > 0 else '']
         self.right.text = [f'{oob_right} \u25b6' if oob_right > 0 else '']
 
 
-class BaseSpectrumVerticalLine(Lines, HubListener):
+class PluginMark():
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.xunit = None
+        self.yunit = None
+        # whether to update existing marks when global display units are changed
+        self.auto_update_units = True
+        self.hub.subscribe(self, GlobalDisplayUnitChanged,
+                           handler=self._on_global_display_unit_changed)
+
+        if self.xunit is None:
+            self.set_x_unit()
+        if self.yunit is None:
+            self.set_y_unit()
+
+    @property
+    def hub(self):
+        return self.viewer.hub
+
+    def update_xy(self, x, y):
+        self.x = np.asarray(x)
+        self.y = np.asarray(y)
+
+    def append_xy(self, x, y):
+        self.x = np.append(self.x, x)
+        self.y = np.append(self.y, y)
+
+    def set_x_unit(self, unit=None):
+        if unit is None:
+            if not hasattr(self.viewer.state, 'x_display_unit'):
+                return
+            unit = self.viewer.state.x_display_unit
+        unit = u.Unit(unit)
+
+        if self.xunit is not None and not np.all([s == 0 for s in self.x.shape]):
+            x = (self.x * self.xunit).to_value(unit, u.spectral())
+            self.xunit = unit
+            self.x = x
+        self.xunit = unit
+
+    def set_y_unit(self, unit=None):
+        if unit is None:
+            if not hasattr(self.viewer.state, 'y_display_unit'):
+                return
+            unit = self.viewer.state.y_display_unit
+        unit = u.Unit(unit)
+
+        if self.yunit is not None and not np.all([s == 0 for s in self.y.shape]):
+            if self.viewer.default_class is Spectrum1D:
+                spec = self.viewer.state.reference_data.get_object(cls=Spectrum1D)
+                eqv = u.spectral_density(spec.spectral_axis)
+                y = (self.y * self.yunit).to_value(unit, equivalencies=eqv)
+            else:
+                y = (self.y * self.yunit).to_value(unit)
+            self.yunit = unit
+            self.y = y
+
+        self.yunit = unit
+
+    def _on_global_display_unit_changed(self, msg):
+        if not self.auto_update_units:
+            return
+        if self.viewer.__class__.__name__ in ['SpecvizProfileView', 'CubevizProfileView']:
+            axis_map = {'spectral': 'x', 'flux': 'y'}
+        elif self.viewer.__class__.__name__ == 'MosvizProfile2DView':
+            axis_map = {'spectral': 'x'}
+        else:
+            return
+        axis = axis_map.get(msg.axis, None)
+        if axis is not None:
+            getattr(self, f'set_{axis}_unit')(msg.unit)
+
+    def clear(self):
+        self.update_xy([], [])
+
+
+class BaseSpectrumVerticalLine(Lines, PluginMark, HubListener):
     def __init__(self, viewer, x, **kwargs):
-        # we'll store the current units so that we can automatically update the
-        # positioning on a change to the x-units
-        self._x_unit = viewer.state.reference_data.get_object(cls=Spectrum1D).spectral_axis.unit
+        self.viewer = viewer
 
         # the location of the marker will need to update automatically if the
         # underlying data changes (through a unit conversion, for example)
         viewer.state.add_callback("reference_data",
                                   self._update_reference_data)
 
         scales = viewer.scales
@@ -79,22 +154,22 @@
     def _update_reference_data(self, reference_data):
         if reference_data is None:
             return
         self._update_data(reference_data.get_object(cls=Spectrum1D).spectral_axis)
 
     def _update_data(self, x_all):
         # the x-units may have changed.  We want to convert the internal self.x
-        # from self._x_unit to the new units (x_all.unit)
+        # from self.xunit to the new units (x_all.unit)
         new_unit = x_all.unit
-        if new_unit == self._x_unit:
+        if new_unit == self.xunit:
             return
-        old_quant = self.x[0]*self._x_unit
+        old_quant = self.x[0]*self.xunit
         x = old_quant.to_value(x_all.unit, equivalencies=u.spectral())
         self.x = [x, x]
-        self._x_unit = new_unit
+        self.xunit = new_unit
 
 
 class SpectralLine(BaseSpectrumVerticalLine):
     """
     Subclass on bqplot Lines, mostly so that we can erase spectral lines
     by eliminating any SpectralLines objects from a figures marks list. Also
     lets us do wavelength redshifting here on mark creation.
@@ -106,15 +181,15 @@
 
         # table_index is same as name_rest elsewhere
         self.table_index = kwargs.pop("table_index", None)
 
         # setting redshift will set self.x and enable the obs_value property,
         # but to do that we need x_unit set first (would normally be assigned
         # in the super init)
-        self._x_unit = viewer.state.reference_data.get_object(cls=Spectrum1D).spectral_axis.unit
+        self.xunit = u.Unit(viewer.state.x_display_unit)
         self.redshift = redshift
 
         viewer.session.hub.subscribe(self, LineIdentifyMessage,
                                      handler=self._process_identify_change)
 
         super().__init__(viewer=viewer, x=self.obs_value, stroke_width=1,
                          fill='none', close_path=False, **kwargs)
@@ -127,31 +202,36 @@
     def rest_value(self):
         return self._rest_value
 
     @property
     def obs_value(self):
         return self.x[0]
 
+    def set_x_unit(self, unit=None):
+        prev_unit = self.xunit
+        super().set_x_unit(unit=unit)
+        self._rest_value = (self._rest_value * prev_unit).to_value(unit, u.spectral())
+
     @property
     def redshift(self):
         return self._redshift
 
     @redshift.setter
     def redshift(self, redshift):
         self._redshift = redshift
-        if str(self._x_unit.physical_type) == 'length':
+        if str(self.xunit.physical_type) == 'length':
             obs_value = self._rest_value*(1+redshift)
-        elif str(self._x_unit.physical_type) == 'frequency':
+        elif str(self.xunit.physical_type) == 'frequency':
             obs_value = self._rest_value/(1+redshift)
         else:
             # catch all for anything else (wavenumber, energy, etc)
-            rest_angstrom = (self._rest_value*self._x_unit).to_value(u.Angstrom,
-                                                                     equivalencies=u.spectral())
+            rest_angstrom = (self._rest_value*self.xunit).to_value(u.Angstrom,
+                                                                   equivalencies=u.spectral())
             obs_angstrom = rest_angstrom*(1+redshift)
-            obs_value = (obs_angstrom*u.Angstrom).to_value(self._x_unit,
+            obs_value = (obs_angstrom*u.Angstrom).to_value(self.xunit,
                                                            equivalencies=u.spectral())
         self.x = [obs_value, obs_value]
 
     @property
     def identify(self):
         return self._identify
 
@@ -164,22 +244,22 @@
         self.stroke_width = 3 if identify else 1
 
     def _process_identify_change(self, msg):
         self.identify = msg.name_rest == self.table_index
 
     def _update_data(self, x_all):
         new_unit = x_all.unit
-        if new_unit == self._x_unit:
+        if new_unit == self.xunit:
             return
 
-        old_quant = self._rest_value*self._x_unit
+        old_quant = self._rest_value*self.xunit
         self._rest_value = old_quant.to_value(new_unit, equivalencies=u.spectral())
         # re-compute self.x from current redshift (instead of converting that as well)
         self.redshift = self._redshift
-        self._x_unit = new_unit
+        self.xunit = new_unit
 
 
 class SliceIndicatorMarks(BaseSpectrumVerticalLine, HubListener):
     """Subclass on bqplot Lines to handle slice/wavelength indicator.
     """
     def __init__(self, viewer, slice=0, **kwargs):
         self._viewer = viewer
@@ -264,15 +344,15 @@
             return
 
         self.visible = True
         self.label.visible = self._show_wavelength
         self.colors = ["#c75109" if self._active else "#007BA1"]
         self.opacities = [1.0 if self._active else 0.9]
 
-    def _on_change_state(self, msg):
+    def _on_change_state(self, msg={}):
         if isinstance(msg, dict):
             changes = msg
         else:
             changes = msg.change
 
         for k, v in changes.items():
             if k == 'active':
@@ -375,29 +455,33 @@
 
 
 class ShadowSpatialSpectral(Lines, HubListener, ShadowMixin):
     """
     Shadow the mark of a spatial subset collapsed spectrum, with the mask from a spectral subset,
     and the styling from the spatial subset.
     """
-    def __init__(self, spatial_spectrum_mark, spectral_subset_mark):
+    def __init__(self, spatial_spectrum_mark, spectral_subset_mark, spatial_uuid, spectral_uuid,
+                 data_uuid):
         # spatial_spectrum_mark: Lines mark corresponding to the spatially-collapsed spectrum
         # from a spatial subset
         # spectral_subset_mark: Lines mark on the FULL cube corresponding to the glue-highlight
         # of the spectral subset
         super().__init__(scales=spatial_spectrum_mark.scales, marker=None)
 
         self._spatial_mark_id = self._get_id(spatial_spectrum_mark)
         self._setup_shadowing(spatial_spectrum_mark,
                               ['scales', 'y', 'visible', 'line_style'],
                               ['x'])
+        self.spatial_uuid = spatial_uuid
 
         self._spectral_mark_id = self._get_id(spectral_subset_mark)
         self._setup_shadowing(spectral_subset_mark,
                               ['stroke_width', 'x', 'y', 'visible', 'opacities', 'colors'])
+        self.spectral_uuid = spectral_uuid
+        self.data_uuid = data_uuid
 
     @property
     def spatial_spectrum_mark(self):
         return self._shadowing[self._spatial_mark_id]
 
     @property
     def spectral_subset_mark(self):
@@ -480,41 +564,40 @@
 
         if change['name'] in ('x', 'scales'):
             # then the position of the label on the plot has changed, so re-determine whether
             # it should be aligned to the left or right
             self._update_align()
 
 
-class PluginMark():
-    def update_xy(self, x, y):
-        self.x = np.asarray(x)
-        self.y = np.asarray(y)
-
-    def append_xy(self, x, y):
-        self.x = np.append(self.x, x)
-        self.y = np.append(self.y, y)
-
-    def clear(self):
-        self.update_xy([], [])
+class LinesAutoUnit(PluginMark, Lines, HubListener):
+    def __init__(self, viewer, *args, **kwargs):
+        self.viewer = viewer
+        super().__init__(*args, **kwargs)
 
 
 class PluginLine(Lines, PluginMark, HubListener):
     def __init__(self, viewer, x=[], y=[], **kwargs):
+        self.viewer = viewer
         # color is same blue as import button
         super().__init__(x=x, y=y, colors=["#007BA1"], scales=viewer.scales, **kwargs)
 
 
 class PluginScatter(Scatter, PluginMark, HubListener):
     def __init__(self, viewer, x=[], y=[], **kwargs):
+        self.viewer = viewer
         # color is same blue as import button
         super().__init__(x=x, y=y, colors=["#007BA1"], scales=viewer.scales, **kwargs)
 
 
 class LineAnalysisContinuum(PluginLine):
-    pass
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        # units do not need to be updated because the plugin itself reruns
+        # the computation and automatically changes the arrays themselves
+        self.auto_update_units = False
 
 
 class LineAnalysisContinuumCenter(LineAnalysisContinuum):
     def __init__(self, viewer, x=[], y=[], **kwargs):
         super().__init__(viewer, x, y, **kwargs)
         self.stroke_width = 1
 
@@ -525,17 +608,17 @@
         self.stroke_width = 5
 
 
 class LineAnalysisContinuumRight(LineAnalysisContinuumLeft):
     pass
 
 
-class LineUncertainties(Lines):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+class LineUncertainties(LinesAutoUnit):
+    def __init__(self, viewer, *args, **kwargs):
+        super().__init__(viewer, *args, **kwargs)
 
 
 class ScatterMask(Scatter):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
 
@@ -544,7 +627,17 @@
         super().__init__(**kwargs)
 
 
 class MarkersMark(PluginScatter):
     def __init__(self, viewer, **kwargs):
         kwargs.setdefault('marker', 'circle')
         super().__init__(viewer, **kwargs)
+
+
+class HistogramMark(Lines):
+    def __init__(self, min_max_value, scales, **kwargs):
+        # Vertical line in LinearScale
+        y = [0, 1]
+        colors = ["#c75d2c"]
+        line_style = "solid"
+        super().__init__(x=min_max_value, y=y, scales=scales, colors=colors, line_style=line_style,
+                         **kwargs)
```

### Comparing `jdaviz-3.5.0/jdaviz/core/region_translators.py` & `jdaviz-3.6.0/jdaviz/core/region_translators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The ``region_translators`` module houses translations of
 :ref:`regions:shapes` to :ref:`photutils:photutils-aperture` apertures.
 """
 from astropy import units as u
 from astropy.coordinates import Angle
-from glue.core.roi import CircularROI, EllipticalROI, RectangularROI
+from glue.core.roi import CircularROI, EllipticalROI, RectangularROI, CircularAnnulusROI
 from photutils.aperture import (CircularAperture, SkyCircularAperture,
                                 EllipticalAperture, SkyEllipticalAperture,
                                 RectangularAperture, SkyRectangularAperture,
                                 CircularAnnulus, SkyCircularAnnulus,
                                 EllipticalAnnulus, SkyEllipticalAnnulus,
                                 RectangularAnnulus, SkyRectangularAnnulus)
 from regions import (CirclePixelRegion, CircleSkyRegion,
@@ -111,15 +111,16 @@
     >>> from regions import CirclePixelRegion, PixCoord
     >>> from jdaviz.core.region_translators import regions2roi
     >>> region_shape = CirclePixelRegion(center=PixCoord(x=42, y=43), radius=4.2)
     >>> regions2roi(region_shape)  # doctest: +ELLIPSIS
     <glue.core.roi.CircularROI object at ...>
 
     """
-    if isinstance(region_shape, (CircleSkyRegion, EllipseSkyRegion, RectangleSkyRegion)):
+    if isinstance(region_shape, (CircleSkyRegion, EllipseSkyRegion, RectangleSkyRegion,
+                                 CircleAnnulusSkyRegion)):
         if wcs is None:
             raise ValueError(f'WCS must be provided for {region_shape}')
 
         # Convert sky to pixel region first, if necessary.
         region_shape = region_shape.to_pixel(wcs)
 
     if isinstance(region_shape, CirclePixelRegion):
@@ -136,14 +137,18 @@
         xmin = region_shape.center.x - half_w
         xmax = region_shape.center.x + half_w
         ymin = region_shape.center.y - half_h
         ymax = region_shape.center.y + half_h
         roi = RectangularROI(
             xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax,
             theta=region_shape.angle.to_value(u.radian))
+    elif isinstance(region_shape, CircleAnnulusPixelRegion):
+        roi = CircularAnnulusROI(
+            xc=region_shape.center.x, yc=region_shape.center.y,
+            inner_radius=region_shape.inner_radius, outer_radius=region_shape.outer_radius)
     else:
         raise NotImplementedError(f'{region_shape.__class__.__name__} is not supported')
 
     return roi
 
 
 def regions2aperture(region_shape):
```

### Comparing `jdaviz-3.5.0/jdaviz/core/registries.py` & `jdaviz-3.6.0/jdaviz/core/registries.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/core/template_mixin.py` & `jdaviz-3.6.0/jdaviz/core/template_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 from astropy.coordinates.sky_coordinate import SkyCoord
 from astropy.table import QTable
 from astropy.table.row import Row as QTableRow
 import astropy.units as u
+import bqplot
+from contextlib import contextmanager
 import numpy as np
+import threading
+import time
 
 from functools import cached_property
 from ipyvuetify import VuetifyTemplate
 from glue.config import colormaps
 from glue.core import HubListener
 from glue.core.message import (DataCollectionAddMessage,
                                DataCollectionDeleteMessage,
                                SubsetCreateMessage,
                                SubsetDeleteMessage,
                                SubsetUpdateMessage)
-from glue.core.subset import RoiSubsetState
+from glue.core.roi import CircularAnnulusROI
+from glue_jupyter.bqplot.image import BqplotImageView
 from glue_jupyter.widgets.linked_dropdown import get_choices as _get_glue_choices
 from specutils import Spectrum1D
 from traitlets import Any, Bool, HasTraits, List, Unicode, observe
 
 from ipywidgets import widget_serialization
 from ipypopout import PopoutButton
 
 from jdaviz import __version__
 from jdaviz.core.events import (AddDataMessage, RemoveDataMessage,
                                 ViewerAddedMessage, ViewerRemovedMessage)
 from jdaviz.core.user_api import UserApiWrapper, PluginUserApi
+from jdaviz.utils import get_subset_type
 
 
 __all__ = ['show_widget', 'TemplateMixin', 'PluginTemplateMixin',
-           'BasePluginComponent', 'SelectPluginComponent',
+           'ViewerPropertiesMixin',
+           'BasePluginComponent', 'SelectPluginComponent', 'UnitSelectPluginComponent',
            'PluginSubcomponent',
            'SubsetSelect', 'SpatialSubsetSelectMixin', 'SpectralSubsetSelectMixin',
            'DatasetSpectralSubsetValidMixin',
            'ViewerSelect', 'ViewerSelectMixin',
            'LayerSelect', 'LayerSelectMixin',
            'DatasetSelect', 'DatasetSelectMixin',
            'Table', 'TableMixin',
+           'Plot', 'PlotMixin',
            'AutoTextField', 'AutoTextFieldMixin',
            'AddResults', 'AddResultsMixin',
            'PlotOptionsSyncState',
            'SPATIAL_DEFAULT_TEXT']
 
 SPATIAL_DEFAULT_TEXT = "Entire Cube"
 GLUE_STATES_WITH_HELPERS = ('size_att', 'cmap_att')
@@ -86,27 +94,40 @@
         else:
             raise ValueError("Unrecognized popout anchor")
 
     else:
         raise ValueError(f"Unrecognized display location: {loc}")
 
 
-def _subset_type(subset):
-    while hasattr(subset.subset_state, 'state1'):
-        # this assumes no mixing between spatial and spectral subsets and just
-        # taking the first component (down the hierarchical tree) to determine the type
-        subset = subset.subset_state.state1
+class ViewerPropertiesMixin:
+    # assumes that self.app is defined by the class
+    @cached_property
+    def spectrum_viewer(self):
+        if hasattr(self, '_default_spectrum_viewer_reference_name'):
+            viewer_reference = self._default_spectrum_viewer_reference_name
+        else:
+            viewer_reference = self.app._get_first_viewer_reference_name(
+                require_spectrum_viewer=True
+            )
 
-    if isinstance(subset.subset_state, RoiSubsetState):
-        return 'spatial'
-    else:
-        return 'spectral'
+        return self.app.get_viewer(viewer_reference)
+
+    @cached_property
+    def spectrum_2d_viewer(self):
+        if hasattr(self, '_default_spectrum_2d_viewer_reference_name'):
+            viewer_reference = self._default_spectrum_2d_viewer_reference_name
+        else:
+            viewer_reference = self.app._get_first_viewer_reference_name(
+                require_spectrum_2d_viewer=True
+            )
+
+        return self.app.get_viewer(viewer_reference)
 
 
-class TemplateMixin(VuetifyTemplate, HubListener):
+class TemplateMixin(VuetifyTemplate, HubListener, ViewerPropertiesMixin):
     config = Unicode("").tag(sync=True)
     vdocs = Unicode("").tag(sync=True)
     popout_button = Any().tag(sync=True, **widget_serialization)
 
     def __new__(cls, *args, **kwargs):
         """
         Overload object creation so that we can inject a reference to the
@@ -190,28 +211,64 @@
 
 
 class PluginTemplateMixin(TemplateMixin):
     """
     This base class can be inherited by all sidebar/tray plugins to expose common functionality.
     """
     disabled_msg = Unicode("").tag(sync=True)
-    plugin_opened = Bool(False).tag(sync=True)
+    plugin_opened = Bool(False).tag(sync=True)  # noqa any instance of the plugin is open (recently sent an "alive" ping)
+    uses_active_status = Bool(False).tag(sync=True)  # noqa whether the plugin has live-preview marks, set to True in plugins to expose keep_active switch
+    keep_active = Bool(False).tag(sync=True)  # noqa whether the live-preview marks show regardless of active state, inapplicable unless uses_active_status is True
+    is_active = Bool(False).tag(sync=True)  # noqa read-only: whether the previews should be shown according to plugin_opened and keep_active
 
     def __init__(self, **kwargs):
         self._viewer_callbacks = {}
+        self._inactive_thread = None  # thread checking for alive pings to control plugin_opened
+        self._ping_timestamp = 0
         super().__init__(**kwargs)
-        self.app.state.add_callback('tray_items_open', self._mxn_update_plugin_opened)
-        self.app.state.add_callback('drawer', self._mxn_update_plugin_opened)
 
     @property
     def user_api(self):
         # plugins should override this to pass their own list of expose functionality, which
         # can even be dependent on config, etc.
         return PluginUserApi(self, expose=[])
 
+    def vue_plugin_ping(self, ping_timestamp):
+        self._ping_timestamp = ping_timestamp
+
+        # we've received a ping, so immediately set plugin_opened state to True
+        if not self.plugin_opened:
+            self.plugin_opened = True
+
+        if self._inactive_thread is not None and self._inactive_thread.is_alive():
+            # a thread already exists to check for pings, the latest ping will allow
+            # the existing while-loop to continue
+            return
+
+        # create a thread to monitor for pings.  If a ping hasn't been received in the
+        # expected time, then plugin_opened will be set to False.
+        self._inactive_thread = threading.Thread(target=self._watch_active)
+        self._inactive_thread.start()
+
+    def _watch_active(self):
+        # expected_delay_ms should match value in setTimeout in tray_plugin.vue
+        # NOTE: could control with a traitlet, but then would need to pass through each
+        # <j-tray-plugin> component
+        expected_delay_ms = 200
+        # plugin_ping (ms) set by setTimeout in tray_plugin.vue
+        # time.time() is in s, so need to convert to ms
+        while time.time()*1000 - self._ping_timestamp < 2 * expected_delay_ms:
+            # at least one plugin has sent an "alive" ping within twice of the expected
+            # interval, wait a full (double) interval and then check again
+            time.sleep(2 * expected_delay_ms / 1000)
+
+        # "alive" ping has not been received within the expected time, consider all instances
+        # of the plugin to be closed
+        self.plugin_opened = False
+
     def _viewer_callback(self, viewer, plugin_method):
         """
         Cached access to callbacks to a plugin method to attach to a viewer.
 
         To define a callback:
         def _on_callback(self, viewer, data):
 
@@ -226,29 +283,39 @@
             return lambda data: plugin_method(viewer, data)
 
         key = f'{viewer.reference_id}:{plugin_method.__name__}'
         if key not in self._viewer_callbacks.keys():
             self._viewer_callbacks[key] = plugin_viewer_callback(viewer, plugin_method)
         return self._viewer_callbacks.get(key)
 
-    def _mxn_update_plugin_opened(self, new_value):
-        app_state = self.app.state
-        tray_names_open = [app_state.tray_items[i]['name'] for i in app_state.tray_items_open]
-        self.plugin_opened = app_state.drawer and self._registry_name in tray_names_open
-
     def open_in_tray(self):
         """
         Open the plugin in the sidebar/tray (and open the sidebar if it is not already).
         """
         app_state = self.app.state
         app_state.drawer = True
         index = [ti['name'] for ti in app_state.tray_items].index(self._registry_name)
         if index not in app_state.tray_items_open:
             app_state.tray_items_open = app_state.tray_items_open + [index]
 
+    @observe('plugin_opened', 'keep_active')
+    def _update_is_active(self, *args):
+        self.is_active = self.keep_active or self.plugin_opened
+
+    @contextmanager
+    def as_active(self):
+        """
+        Context manager to temporarily enable keep_active and enable live-previews and keypress
+        events, even if the plugin UI is not opened.
+        """
+        _keep_active = self.keep_active
+        self.keep_active = True
+        yield
+        self.keep_active = _keep_active
+
     def show(self, loc="inline", title=None):  # pragma: no cover
         """Display the plugin UI.
 
         Parameters
         ----------
         loc : str
             The display location determines where to present the viz app.
@@ -290,15 +357,15 @@
         If "sidecar" is requested in the "classic" Jupyter notebook, the plugin will appear inline,
         as only JupyterLab has a mechanism to have multiple tabs.
         """
         title = title if title is not None else self._registry_label
         show_widget(self, loc=loc, title=title)
 
 
-class BasePluginComponent(HubListener):
+class BasePluginComponent(HubListener, ViewerPropertiesMixin):
     """
     This base class handles attaching traitlets from the plugin itself to logic
     handled within the component, support for caching and clearing caches on properties,
     and common properties for accessing the app, etc.
     """
     def __init__(self, plugin, **kwargs):
         self._plugin_traitlets = {k: v for k, v in kwargs.items() if v is not None}
@@ -372,36 +439,14 @@
 
             return d
 
         return [_dict_from_viewer(viewer, self.app._viewer_item_by_id(vid))
                 for vid, viewer in self.app._viewer_store.items()
                 if viewer.__class__.__name__ != 'MosvizTableViewer']
 
-    @cached_property
-    def spectrum_viewer(self):
-        if hasattr(self, '_default_spectrum_viewer_reference_name'):
-            viewer_reference = self._default_spectrum_viewer_reference_name
-        else:
-            viewer_reference = self.app._get_first_viewer_reference_name(
-                require_spectrum_viewer=True
-            )
-
-        return self._plugin.app.get_viewer(viewer_reference)
-
-    @cached_property
-    def spectrum_2d_viewer(self):
-        if hasattr(self, '_default_spectrum_2d_viewer_reference_name'):
-            viewer_reference = self._default_spectrum_2d_viewer_reference_name
-        else:
-            viewer_reference = self.app._get_first_viewer_reference_name(
-                require_spectrum_2d_viewer=True
-            )
-
-        return self._plugin.app.get_viewer(viewer_reference)
-
 
 class SelectPluginComponent(BasePluginComponent, HasTraits):
     """
     Plugin select, with support for single or multi-selection.
 
     Useful API methods/attributes:
 
@@ -470,14 +515,18 @@
         # defining __eq__ without defining __hash__ makes the object unhashable
         return super().__hash__()
 
     @property
     def choices(self):
         return self.labels
 
+    @choices.setter
+    def choices(self, choices=[]):
+        self.items = [{'label': choice} for choice in choices]
+
     @property
     def is_multiselect(self):
         if not hasattr(self, 'multiselect'):
             return False
         else:
             return self.multiselect
 
@@ -638,14 +687,56 @@
                 raise ValueError(f"not all items in {event['new']} are one of {self.labels}, reverting selection to {event['old']}")  # noqa
         else:
             if event['new'] not in self.labels + ['']:
                 self.selected = event['old']
                 raise ValueError(f"{event['new']} not one of {self.labels}, reverting selection to {event['old']}")  # noqa
 
 
+class UnitSelectPluginComponent(SelectPluginComponent):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.add_observe('items', lambda _: self._clear_cache('unit_choices'))
+        self._addl_unit_strings = []
+
+    @cached_property
+    def unit_choices(self):
+        return [u.Unit(lbl) for lbl in self.labels]
+
+    @property
+    def addl_unit_choices(self):
+        return [u.Unit(choice) for choice in self._addl_unit_strings]
+
+    def _selected_changed(self, event):
+        self._clear_cache()
+        if event['new'] in self.labels + ['']:
+            # the string is an exact match, no converting necessary
+            return
+        elif not len(self.labels):
+            raise ValueError("no valid unit choices")
+        try:
+            new_u = u.Unit(event['new'])
+        except ValueError:
+            self.selected = event['old']
+            raise ValueError(f"{event['new']} could not be converted to a valid unit, reverting selection to {event['old']}")  # noqa
+        if new_u not in self.unit_choices:
+            if new_u in self.addl_unit_choices:
+                # append this one (as the valid string representation) to the list of user-choices
+                addl_index = self.addl_unit_choices.index(new_u)
+                self.choices = self.choices + [self._addl_unit_strings[addl_index]]
+                # clear the cache so we can find the appropriate entry in unit_choices
+                self._clear_cache('unit_choices')
+            else:
+                self.selected = event['old']
+                raise ValueError(f"{event['new']} not one of {self.labels}, reverting selection to {event['old']}")  # noqa
+
+        # convert to default string representation from the valid choices
+        ind = self.unit_choices.index(new_u)
+        self.selected = self.labels[ind]
+
+
 class LayerSelect(SelectPluginComponent):
     """
     Plugin select for layers, with support for single or multi-selection.
 
     Useful API methods/attributes:
 
     * :meth:`~SelectPluginComponent.choices`
@@ -688,15 +779,15 @@
         :show_if_single_entry="true"
         label="Layer"
         hint="Select layer."
       />
     """
     def __init__(self, plugin, items, selected, viewer,
                  multiselect=None,
-                 default_text=None, manual_options=[], allowed_type=None,
+                 default_text=None, manual_options=[],
                  default_mode='first'):
         """
         Parameters
         ----------
         plugin
             the parent plugin object
         items : str
@@ -880,16 +971,15 @@
 
     * ``selected_min_max(cube)`` (quantity, only applicable for spectral subsets)
 
     To use in a plugin:
 
     * create (empty) traitlets in the plugin
     * register with all the automatic logic in the plugin's init by passing the string names
-      of the respective traitlets.  Pass ``allowed_type='spectral'`` or ``allowed_type='spatial'``
-      to only support spectral or spatial subsets, respectively.
+      of the respective traitlets.
     * use component in plugin template (see below)
     * refer to properties above based on the interally stored reference to the
       instantiated object of this component
     * observe the traitlets created and defined in the plugin, as necessary
 
     Example template (label and hint are optional)::
 
@@ -899,15 +989,15 @@
         :show_if_single_entry="true"
         label="Subset"
         hint="Select subset."
       />
 
     """
     def __init__(self, plugin, items, selected, selected_has_subregions=None,
-                 viewers=None, default_text=None, manual_options=[], allowed_type=None,
+                 viewers=None, default_text=None, manual_options=[], filters=[],
                  default_mode='default_text'):
         """
         Parameters
         ----------
         plugin
             the parent plugin object
         items : str
@@ -918,35 +1008,31 @@
             the name of the selected_has_subregions traitlet defined in ``plugin``, optional
         viewers : list
             the reference names or ids of the viewer to extract the subregion.  If not provided o
             None, will loop through all references.
         default_text : str or None
             the text to show for no selection.  If not provided or None, no entry will be provided
             in the dropdown for no selection.
-        manual_options: list
+        manual_options : list
             list of options to provide that are not automatically populated by subsets.  If
             ``default`` text is provided but not in ``manual_options`` it will still be included as
             the first item in the list.
-        allowed_type : str or None
-            whether to filter to 'spatial' or 'spectral' types of subsets.  If not provided or None,
-            will include both entries.
+        filters : list
+            list of strings (for built-in filters) or callables to filter to only valid options.
         """
         super().__init__(plugin,
                          items=items,
                          selected=selected,
+                         filters=filters,
                          selected_has_subregions=selected_has_subregions,
                          viewers=viewers,
                          default_text=default_text,
                          manual_options=manual_options,
                          default_mode=default_mode)
 
-        if allowed_type not in [None, 'spatial', 'spectral']:
-            raise ValueError("allowed_type must be None, 'spatial', or 'spectral'")
-        self._allowed_type = allowed_type
-
         if selected_has_subregions is not None:
             self.selected_has_subregions = False
 
         self.hub.subscribe(self, SubsetUpdateMessage,
                            handler=lambda msg: self._update_subset(msg.subset, msg.attribute))
         self.hub.subscribe(self, SubsetDeleteMessage,
                            handler=lambda msg: self._delete_subset(msg.subset))
@@ -961,33 +1047,48 @@
 
     def _subset_to_dict(self, subset):
         # find layer artist in default spectrum-viewer
         for viewer in self.viewers:
             for layer in viewer.layers:
                 if layer.layer.label == subset.label:
                     color = layer.state.color
-                    subset_type = _subset_type(subset)
-                    return {"label": subset.label, "color": color, "type": subset_type}
+                    type = get_subset_type(subset)
+                    return {"label": subset.label, "color": color, "type": type}
         return {"label": subset.label, "color": False, "type": False}
 
     def _delete_subset(self, subset):
         # NOTE: calling .remove will not trigger traitlet update
         self.items = [s for s in self.items
                       if s['label'] != subset.label]
         if self.selected not in self.labels:
             self._apply_default_selection()
 
-    def _update_subset(self, subset, attribute=None):
-        if self._allowed_type is not None and _subset_type(subset) != self._allowed_type:
-            return
+    def _is_valid_item(self, subset):
+        def is_spectral(subset):
+            return get_subset_type(subset) == 'spectral'
+
+        def is_spatial(subset):
+            return get_subset_type(subset) == 'spatial'
+
+        def is_not_composite(subset):
+            return not hasattr(subset.subset_state, 'state1')
+
+        def is_not_annulus(subset):
+            # this will be considered "not an annulus" if it is composite, even
+            # if that composite subset contains an annulus
+            return (not is_not_composite(subset)
+                    or not isinstance(subset.subset_state.roi, CircularAnnulusROI))
 
+        return super()._is_valid_item(subset, locals())
+
+    def _update_subset(self, subset, attribute=None):
         if subset.label not in self.labels:
             # NOTE: this logic will need to be revisited if generic renaming of subsets is added
             # see https://github.com/spacetelescope/jdaviz/pull/1175#discussion_r829372470
-            if subset.label.startswith('Subset'):
+            if subset.label.startswith('Subset') and self._is_valid_item(subset):
                 # NOTE: += will not trigger traitlet update
                 self.items = self.items + [self._subset_to_dict(subset)]  # noqa
         else:
             # 'type' can be passed manually rather than coming from SubsetUpdateMessage.attribute
             if attribute in ('style', 'type'):
                 # TODO: may need to add label and then rebuild the entire list if/when
                 # we add support for renaming subsets
@@ -1010,37 +1111,37 @@
             else:
                 self.selected_has_subregions = len(self.selected_obj.subregions) > 1
 
     @cached_property
     def selected_obj(self):
         if self.selected in self.manual_options or self.selected not in self.labels:
             return None
-        subset_type = self.selected_item['type']
-        # NOTE: we use reference names here instead of IDs since get_subsets_from_viewer requires
+        # NOTE: we use reference names here instead of IDs since get_subsets requires
         # that.  For imviz, this will mean we won't be able to loop through each of the viewers,
         # but the original viewer should have access to all the subsets.
         for viewer_ref in self.viewer_refs:
-            match = self.app.get_subsets_from_viewer(viewer_ref,
-                                                     subset_type=subset_type).get(self.selected)
+            match = self.app.get_subsets(self.selected)
             if match is not None:
                 return match
 
     @property
     def selected_subset_state(self):
         subset_group = [s for s in self.app.data_collection.subset_groups if
                         s.label == self.selected][0]
         return subset_group.subset_state
 
     @property
     def selected_subset_mask(self):
         get_data_kwargs = {'data_label': self.plugin.dataset.selected}
-        if self._allowed_type:
-            get_data_kwargs[f'{self._allowed_type}_subset'] = self.selected
+        if 'is_spectral' in self.filters:
+            get_data_kwargs['spectral_subset'] = self.selected
+        elif 'is_spatial' in self.filters:
+            get_data_kwargs['spatial_subset'] = self.selected
 
-        if self.app.config == 'cubeviz' and self._allowed_type == 'spectral':
+        if self.app.config == 'cubeviz' and 'is_spectral' in self.filters:
             viewer_ref = getattr(self.plugin,
                                  '_default_spectrum_viewer_reference_name',
                                  self.viewers[0].reference_id)
             get_data_kwargs['function'] = self.app.get_viewer(viewer_ref).state.function
 
         subset = self.app._jdaviz_helper.get_data(**get_data_kwargs)
 
@@ -1088,15 +1189,15 @@
         spectrum_viewer = kwargs.get('spectrum_viewer_reference_name')
         self.spectral_subset = SubsetSelect(self,
                                             'spectral_subset_items',
                                             'spectral_subset_selected',
                                             'spectral_subset_selected_has_subregions',
                                             viewers=[spectrum_viewer],
                                             default_text='Entire Spectrum',
-                                            allowed_type='spectral')
+                                            filters=['is_spectral'])
 
 
 class SpatialSubsetSelectMixin(VuetifyTemplate, HubListener):
     """
     Applies the SubsetSelect component as a mixin in the base plugin.  This
     automatically adds traitlets as well as new properties to the plugin with minimal
     extra code.  For multiple instances or custom traitlet names/defaults, use the
@@ -1125,15 +1226,15 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.spatial_subset = SubsetSelect(self,
                                            'spatial_subset_items',
                                            'spatial_subset_selected',
                                            'spatial_subset_selected_has_subregions',
                                            default_text='No Subset',
-                                           allowed_type='spatial')
+                                           filters=['is_spatial'])
 
 
 class DatasetSpectralSubsetValidMixin(VuetifyTemplate, HubListener):
     """
     Adds a traitlet tracking whether self.dataset and self.spectral_subset
     overlap in the spectral axis.
 
@@ -1405,14 +1506,16 @@
         ----------
         plugin
             the parent plugin object
         items : str
             the name of the items traitlet defined in ``plugin``
         selected : str
             the name of the selected traitlet defined in ``plugin``
+        filters : list
+            list of strings (for built-in filters) or callables to filter to only valid options.
         default_text : str or None
             the text to show for no selection.  If not provided or None, no entry will be provided
             in the dropdown for no selection.
         manual_options: list
             list of options to provide that are not automatically populated by datasets.  If
             ``default`` text is provided but not in ``manual_options`` it will still be included as
             the first item in the list.
@@ -1441,15 +1544,15 @@
 
         # add additional callback for subsets
         # We have to use SubsetUpdateMessage instead of SubsetCreateMessage to ensure it has already
         # been added to data_collection.subset_groups.  To avoid extra calls to _on_data_changed
         # for changes in style, etc, we'll try to filter out extra messages in advance.
         def _subset_update(msg):
             if msg.attribute == 'subset_state':
-                if _subset_type(msg.subset) == 'spatial':
+                if get_subset_type(msg.subset) == 'spatial':
                     self._on_data_changed()
 
         self.hub.subscribe(self, SubsetUpdateMessage,
                            handler=_subset_update)
         self._include_spatial_subsets = True
 
     @property
@@ -1481,24 +1584,30 @@
         match = self.app._jdaviz_helper.get_data(data_label=self.selected)
         if match is not None:
             return match
         # handle the case of empty Application with no viewer, we'll just pull directly
         # from the data collection
         return self.get_object(cls=self.default_data_cls)
 
-    def selected_spectrum_for_spatial_subset(self, spatial_subset=SPATIAL_DEFAULT_TEXT):
+    def selected_spectrum_for_spatial_subset(self,
+                                             spatial_subset=SPATIAL_DEFAULT_TEXT,
+                                             use_display_units=True):
         if spatial_subset == SPATIAL_DEFAULT_TEXT:
             spatial_subset = None
         return self.plugin._specviz_helper.get_data(data_label=self.selected,
-                                                    spatial_subset=spatial_subset)
+                                                    spatial_subset=spatial_subset,
+                                                    use_display_units=use_display_units)
 
     def _is_valid_item(self, data):
         def not_from_plugin(data):
             return data.meta.get('Plugin', None) is None
 
+        def not_from_this_plugin(data):
+            return data.meta.get('Plugin', None) != self.plugin.__class__.__name__
+
         def not_from_plugin_model_fitting(data):
             return data.meta.get('Plugin', None) != 'ModelFitting'
 
         def has_metadata(data):
             return hasattr(data, 'meta') and isinstance(data.meta, dict) and len(data.meta)
 
         def layer_in_viewers(data):
@@ -1548,15 +1657,15 @@
 
         manual_items = [{'label': label} for label in self.manual_options]
         self.items = manual_items + [_dc_to_dict(data) for data in self.app.data_collection
                                      if self._is_valid_item(data)]
         if getattr(self, '_include_spatial_subsets', False):
             # allow for spatial subsets to be listed
             self.items = self.items + [_dc_to_dict(subset) for subset in self.app.data_collection.subset_groups  # noqa
-                                       if _subset_type(subset) == 'spatial']
+                                       if get_subset_type(subset) == 'spatial']
         self._apply_default_selection()
         # future improvement: only clear cache if the selected data entry was changed?
         self._clear_cache(*self._cached_properties)
 
 
 class DatasetSelectMixin(VuetifyTemplate, HubListener):
     """
@@ -1674,17 +1783,17 @@
     label = Unicode().tag(sync=True)
     label_default = Unicode().tag(sync=True)
     label_auto = Bool(True).tag(sync=True)
     label_invalid_msg = Unicode('').tag(sync=True)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.auto_label = AddResults(self, 'label',
-                                     'label_default', 'label_auto',
-                                     'label_invalid_msg')
+        self.auto_label = AutoTextField(self, 'label',
+                                        'label_default', 'label_auto',
+                                        'label_invalid_msg')
 
 
 class AddResults(BasePluginComponent):
     """
     Plugin component for providing a data-label and selecting a viewer to add the results from
     the plugin.
 
@@ -1827,54 +1936,87 @@
         self.label_overwrite = False
 
     def add_results_from_plugin(self, data_item, replace=None, label=None):
         """
         Add ``data_item`` to the app's data_collection according to the default or user-provided
         label and adds to any requested viewers.
         """
+
+        # Note that we can only preserve one of percentile or vmin+vmax
+        ignore_attributes = ("layer", "attribute", "percentile")
+
         if self.label_invalid_msg:
             raise ValueError(self.label_invalid_msg)
 
         if label is None:
             label = self.label
 
-        if replace is None:
-            replace = self.viewer.selected_reference != 'spectrum-viewer'
-
-        if self.label_overwrite and len(self.add_to_viewer_items) <= 2:
+        if self.label_overwrite:
             # the switch for add_to_viewer is hidden, and so the loaded state of the overwritten
             # entry should be the same as the original entry (to avoid deleting reference data)
-            viewer_reference = self.add_to_viewer_items[-1]['reference']
-            viewer_item = self.app._viewer_item_by_reference(viewer_reference)
-            viewer = self.app.get_viewer(viewer_reference)
-            viewer_loaded_labels = [layer.layer.label for layer in viewer.layers]
-            add_to_viewer_selected = viewer_reference if label in viewer_loaded_labels else 'None'  # noqa
-            visible = label in viewer_item['visible_layers']
+            add_to_viewer_refs = []
+            add_to_viewer_vis = []
+            preserved_attributes = []
+            for viewer_select_item in self.add_to_viewer_items[1:]:
+                # index 0 is for "None"
+                viewer_ref = viewer_select_item['reference']
+                viewer_item = self.app._viewer_item_by_reference(viewer_ref)
+                viewer = self.app.get_viewer(viewer_ref)
+                for layer in viewer.layers:
+                    if layer.layer.label != label:
+                        continue
+                    else:
+                        add_to_viewer_refs.append(viewer_ref)
+                        add_to_viewer_vis.append(label in viewer_item['visible_layers'])
+                        preserve_these = {}
+                        for att in layer.state.as_dict():
+                            # Can't set cmap_att, size_att, etc
+                            if att not in ignore_attributes and "_att" not in att:
+                                preserve_these[att] = getattr(layer.state, att)
+                        preserved_attributes.append(preserve_these)
         else:
-            add_to_viewer_selected = self.add_to_viewer_selected
-            visible = True
+            if self.add_to_viewer_selected == 'None':
+                add_to_viewer_refs = []
+                add_to_viewer_vis = []
+                preserved_attributes = []
+            else:
+                add_to_viewer_refs = [self.add_to_viewer_selected]
+                add_to_viewer_vis = [True]
+                preserved_attributes = [{}]
 
         if label in self.app.data_collection:
-            if add_to_viewer_selected != 'None':
-                self.app.remove_data_from_viewer(self.viewer.selected_reference, label)
+            for viewer_ref in add_to_viewer_refs:
+                self.app.remove_data_from_viewer(viewer_ref, label)
             self.app.data_collection.remove(self.app.data_collection[label])
 
         if not hasattr(data_item, 'meta'):
             data_item.meta = {}
         data_item.meta['Plugin'] = self._plugin.__class__.__name__
         if self.app.config == 'mosviz':
             data_item.meta['mosviz_row'] = self.app.state.settings['mosviz_row']
         self.app.add_data(data_item, label)
 
-        if add_to_viewer_selected != 'None':
+        for viewer_ref, visible, preserved in zip(add_to_viewer_refs, add_to_viewer_vis,
+                                                  preserved_attributes):
             # replace the contents in the selected viewer with the results from this plugin
-            # TODO: switch to an instance/classname check?
-            self.app.add_data_to_viewer(self.viewer.selected_id,
+            this_viewer = self.app.get_viewer(viewer_ref)
+            if replace is not None:
+                this_replace = replace
+            else:
+                this_replace = isinstance(this_viewer, BqplotImageView)
+
+            self.app.add_data_to_viewer(viewer_ref,
                                         label,
-                                        visible=visible, clear_other_data=replace)
+                                        visible=visible, clear_other_data=this_replace)
+
+            if preserved != {}:
+                layer_state = [layer.state for layer in this_viewer.layers if
+                               layer.layer.label == label][0]
+                for att in preserved:
+                    setattr(layer_state, att, preserved[att])
 
         # update overwrite warnings, etc
         self._on_label_changed()
 
 
 class AddResultsMixin(VuetifyTemplate, HubListener):
     """
@@ -2465,7 +2607,98 @@
         self.clear_table()
 
     def export_table(self):
         """
         Export the QTable representation of the table.
         """
         return self.table.export_table()
+
+
+class Plot(PluginSubcomponent):
+    """
+    Plot subcomponent.  For most cases where a plugin only requires a single plot, use the mixin
+    instead.
+
+    To use in a plugin, define ``plugin.plot = Plot(plugin)``, create a ``plot_widget`` Unicode
+    traitlet, and set ``plugin.plot_widget = 'IPY_MODEL_'+self.plot.model_id``.
+
+    To render in the plugin's vue file::
+
+      <jupyter-widget :widget="plot_widget"></jupyter-widget>
+
+    """
+    template_file = __file__, "../components/plugin_plot.vue"
+
+    figure = Any().tag(sync=True, **widget_serialization)
+
+    def __init__(self, plugin, *args, **kwargs):
+        super().__init__(plugin, 'Plot', *args, **kwargs)
+        self.figure = bqplot.Figure()
+        self._marks = {}
+
+        self.figure.axes = [bqplot.Axis(scale=bqplot.LinearScale(), label='x'),
+                            bqplot.Axis(scale=bqplot.LinearScale(),
+                                        orientation='vertical', label='y')]
+
+        self.figure.title_style = {'font-size': '12px'}
+        self.figure.fig_margin = {'top': 60, 'bottom': 60, 'left': 40, 'right': 10}
+
+        plugin.bqplot_figs_resize += [self.figure]
+
+    @property
+    def marks(self):
+        return self._marks
+
+    def clear_marks(self, *mark_labels):
+        for mark_label, mark in self.marks.items():
+            if mark_label in mark_labels:
+                mark.x, mark.y = [], []
+
+    def clear_all_marks(self):
+        self.clear_marks(*self.marks.keys())
+
+    def _add_mark(self, cls, label, **kwargs):
+        if label in self._marks:
+            raise ValueError(f"mark with label '{label}' already exists")
+        mark = cls(scales={'x': self.figure.axes[0].scale,
+                           'y': self.figure.axes[1].scale},
+                   **kwargs)
+        self.figure.marks = self.figure.marks + [mark]
+        self._marks[label] = mark
+        return mark
+
+    def add_line(self, label, x=[], y=[], **kwargs):
+        return self._add_mark(bqplot.Lines, label, x=x, y=y,
+                              colors=kwargs.pop('color', kwargs.pop('colors', 'gray')),
+                              **kwargs)
+
+    def add_scatter(self, label, x=[], y=[], **kwargs):
+        return self._add_mark(bqplot.Scatter, label, x=x, y=y,
+                              colors=kwargs.pop('color', kwargs.pop('colors', 'gray')),
+                              **kwargs)
+
+
+class PlotMixin(VuetifyTemplate, HubListener):
+    """
+    Plot subcomponent mixin.
+
+    In addition to ``plot``, this provides the following methods at the plugin-level:
+
+    * :meth:`clear_plot`
+
+    To render in the plugin's vue file::
+
+      <jupyter-widget :widget="plot_widget"></jupyter-widget>
+
+    """
+    plot_widget = Unicode().tag(sync=True)
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.plot = Plot(self)
+        self.plot_widget = 'IPY_MODEL_'+self.plot.model_id
+
+    def clear_plot(self):
+        """
+        Clear all data from the current plot.
+        """
+        self.plot.clear_plot()
```

### Comparing `jdaviz-3.5.0/jdaviz/core/tests/test_custom_traitlets.py` & `jdaviz-3.6.0/jdaviz/core/tests/test_custom_traitlets.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/core/tests/test_data_menu.py` & `jdaviz-3.6.0/jdaviz/core/tests/test_data_menu.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,19 +25,19 @@
      ['mast:JWST/product/jw02732-o004_t004_miri_ch1-shortmediumlong_x1d.fits',
       'specviz']
 ]
 
 
 def test_data_menu_toggles(specviz_helper, spectrum1d):
     # load 2 data entries
-    specviz_helper.load_spectrum(spectrum1d, data_label="test")
+    specviz_helper.load_data(spectrum1d, data_label="test")
     app = specviz_helper.app
     sv = app.get_viewer('spectrum-viewer')
     new_spec = specviz_helper.get_spectra(apply_slider_redshift=True)["test"]*0.9
-    specviz_helper.load_spectrum(new_spec, data_label="test2")
+    specviz_helper.load_data(new_spec, data_label="test2")
 
     # check that both are enabled in the data menu
     selected_data_items = app._viewer_item_by_id('specviz-0')['selected_data_items']
     data_ids = list(selected_data_items.keys())
     assert len(data_ids) == 2
     assert np.all([visible == 'visible' for visible in selected_data_items.values()])
     assert len(sv.layers) == 2
@@ -106,21 +106,10 @@
 @pytest.mark.filterwarnings(r"ignore::astropy.wcs.wcs.FITSFixedWarning")
 @pytest.mark.parametrize(
     "uri, expected_helper", example_uri_helper
 )
 def test_auto_config_detection(uri, expected_helper):
     url = f'https://mast.stsci.edu/api/v0.1/Download/file/?uri={uri}'
     fn = download_file(url, timeout=100)
-    helper_name = identify_helper(fn)
+    helper_name, hdul = identify_helper(fn)
+    hdul.close()
     assert helper_name == expected_helper
-
-
-@pytest.mark.remote_data
-@pytest.mark.filterwarnings(r"ignore::astropy.wcs.wcs.FITSFixedWarning")
-def test_auto_config_manga():
-    # Check that MaNGA cubes go to cubeviz. This file is
-    # originally from
-    # https://data.sdss.org/sas/dr14/manga/spectro/redux/v2_1_2/7495/stack/manga-7495-12704-LOGCUBE.fits.gz
-    URL = 'https://stsci.box.com/shared/static/28a88k1qfipo4yxc4p4d40v4axtlal8y.fits'
-    fn = download_file(URL, cache=True, timeout=100)
-    helper_name = identify_helper(fn)
-    assert helper_name == 'cubeviz'
```

### Comparing `jdaviz-3.5.0/jdaviz/core/tests/test_helpers.py` & `jdaviz-3.6.0/jdaviz/core/tests/test_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     def setup_class(self, specviz_helper, spectrum1d, multi_order_spectrum_list):
         self.spec_app = specviz_helper
         self.spec = spectrum1d
         self.label = "Test 1D Spectrum"
 
         self.spec2 = spectrum1d._copy(spectral_axis=spectrum1d.spectral_axis+1000*u.AA)
         self.label2 = "Test 1D Spectrum 2"
-        self.spec_app.load_spectrum(spectrum1d, data_label=self.label)
-        self.spec_app.load_spectrum(self.spec2, data_label=self.label2)
+        self.spec_app.load_data(spectrum1d, data_label=self.label)
+        self.spec_app.load_data(self.spec2, data_label=self.label2)
 
         # Add 3 subsets to cover different parts of spec and spec2
         self.spec_app.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(6000, 6500))
         self.spec_app.app.session.edit_subset_mode.mode = NewMode
 
         self.spec_app.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(6700, 7200))
         self.spec_app.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(8200, 8800))
```

### Comparing `jdaviz-3.5.0/jdaviz/core/tests/test_region_translators.py` & `jdaviz-3.6.0/jdaviz/core/tests/test_region_translators.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/core/tests/test_template_mixin.py` & `jdaviz-3.6.0/jdaviz/core/tests/test_template_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 def test_spectralsubsetselect(specviz_helper, spectrum1d):
     # apply mask to spectrum to check selected subset is masked:
     mask = spectrum1d.flux < spectrum1d.flux.mean()
     spectrum1d.mask = mask
 
-    specviz_helper.load_spectrum(spectrum1d)
+    specviz_helper.load_data(spectrum1d)
     sv = specviz_helper.app.get_viewer('spectrum-viewer')
     # create a "Subset 1" entry
     sv.apply_roi(XRangeROI(6500, 7400))
 
     # model fitting uses the mixin
     p = specviz_helper.app.get_tray_item_from_name('g-model-fitting')
     assert len(p.spectral_subset.labels) == 2  # Entire Spectrum, Subset 1
```

### Comparing `jdaviz-3.5.0/jdaviz/core/tests/test_tools.py` & `jdaviz-3.6.0/jdaviz/core/tests/test_tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-import numpy as np
 from numpy.testing import assert_allclose
-from glue.core import Data
 
 
-def test_boxzoom(cubeviz_helper, spectral_cube_wcs):
-    data = Data(flux=np.ones((128, 128, 256)), label='Test Flux', coords=spectral_cube_wcs)
-    cubeviz_helper.app.data_collection.append(data)
-
-    cubeviz_helper.app.add_data_to_viewer('spectrum-viewer', 'Test Flux')
-    cubeviz_helper.app.add_data_to_viewer('flux-viewer', 'Test Flux')
+def test_boxzoom(cubeviz_helper, image_cube_hdu_obj_microns):
+    cubeviz_helper.load_data(image_cube_hdu_obj_microns, data_label="Test Flux")
 
     flux_viewer = cubeviz_helper.app.get_viewer('flux-viewer')
 
     assert flux_viewer.state.y_min == -0.5
-    assert flux_viewer.state.y_max == 127.5
+    assert flux_viewer.state.y_max == 8.5
     assert flux_viewer.state.x_min == -0.5
-    assert flux_viewer.state.x_max == 127.5
+    assert flux_viewer.state.x_max == 9.5
 
     t = flux_viewer.toolbar.tools['jdaviz:boxzoom']
     t.activate()
-    t.interact.selected_x = [10, 20]
-    t.interact.selected_y = [20, 60]
+    t.interact.selected_x = [1, 4]
+    t.interact.selected_y = [2, 6]
 
-    assert t.get_x_axis_with_aspect_ratio() == (-5., 35.)
+    assert_allclose(t.get_x_axis_with_aspect_ratio(), [0.277778, 4.722222], rtol=1e-6)
 
 
 def _get_lims(viewer):
     return [viewer.state.x_min, viewer.state.x_max,
             viewer.state.y_min, viewer.state.y_max]
```

### Comparing `jdaviz-3.5.0/jdaviz/core/tools.py` & `jdaviz-3.6.0/jdaviz/core/tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,42 +5,126 @@
 from glue.config import viewer_tool
 from glue.core import HubListener
 from glue.viewers.common.tool import Tool
 from glue_jupyter.bqplot.common.tools import (CheckableTool,
                                               HomeTool, BqplotPanZoomMode,
                                               BqplotPanZoomXMode, BqplotPanZoomYMode,
                                               BqplotRectangleMode, BqplotCircleMode,
-                                              BqplotEllipseMode, BqplotXRangeMode,
-                                              BqplotYRangeMode, BqplotSelectionTool,
+                                              BqplotEllipseMode, BqplotCircularAnnulusMode,
+                                              BqplotXRangeMode, BqplotYRangeMode,
+                                              BqplotSelectionTool,
                                               INTERACT_COLOR)
 from bqplot.interacts import BrushSelector, BrushIntervalSelector
 
 from jdaviz.core.events import LineIdentifyMessage, SpectralMarksChangedMessage
+from jdaviz.core.marks import SpectralLine
 
 __all__ = []
 
-ICON_DIR = os.path.join(os.path.dirname(__file__), '..', 'data', 'icons')
+ICON_DIR = os.path.normpath(os.path.join(os.path.dirname(__file__), '..', 'data', 'icons'))
 
 
 # Override icons for built-in tools from glue-jupyter
 BqplotRectangleMode.icon = os.path.join(ICON_DIR, 'select_xy.svg')
 BqplotCircleMode.icon = os.path.join(ICON_DIR, 'select_circle.svg')
 BqplotEllipseMode.icon = os.path.join(ICON_DIR, 'select_ellipse.svg')
+BqplotCircularAnnulusMode.icon = os.path.join(ICON_DIR, 'select_annulus.svg')
 BqplotXRangeMode.icon = os.path.join(ICON_DIR, 'select_x.svg')
 BqplotYRangeMode.icon = os.path.join(ICON_DIR, 'select_y.svg')
 
 
 class _BaseZoomHistory:
     # Mixin for custom zoom tools to be able to save their previous zoom state
     # which is then used by the PrevZoom tool
     def save_prev_zoom(self):
         self.viewer._prev_limits = (self.viewer.state.x_min, self.viewer.state.x_max,
                                     self.viewer.state.y_min, self.viewer.state.y_max)
 
 
+class _MatchedZoomMixin:
+    match_axes = ('x', 'y')
+    disable_matched_zoom_in_other_viewer = False
+
+    def _is_matched_viewer(self, viewer):
+        return True
+
+    def _iter_matched_viewers(self, include_self=False):
+        for viewer in self.viewer.session.application.viewers:
+            if viewer is self.viewer and not include_self:
+                continue
+            elif self._is_matched_viewer(viewer):
+                yield viewer
+
+    def _map_limits(self, from_viewer, to_viewer, limits={}):
+        return limits
+
+    def _post_activate(self):
+        return
+
+    @property
+    def match_keys(self):
+        keys = []
+        for ax in self.match_axes:
+            keys += [f'{ax}_min', f'{ax}_max']
+        return keys
+
+    def activate(self):
+        if self.disable_matched_zoom_in_other_viewer:
+            # mapping limits are not guaranteed to roundtrip, so we need to disable
+            # any linked tool in the "other" viewer
+            for viewer in self._iter_matched_viewers(include_self=False):
+                if isinstance(viewer.toolbar.active_tool, _MatchedZoomMixin):
+                    viewer.toolbar.active_tool_id = None
+
+        super().activate()
+        for k in self.match_keys:
+            self.viewer.state.add_callback(k, self.on_limits_change)
+
+        self._post_activate()
+
+        # Trigger a sync so the initial limits match
+        self.on_limits_change()
+
+    def deactivate(self):
+        for k in self.match_keys:
+            self.viewer.state.remove_callback(k, self.on_limits_change)
+
+        super().deactivate()
+
+    def on_limits_change(self, *args):
+        # from_lims: limits in the viewer belonging to the tool
+        from_lims = {k: getattr(self.viewer.state, k) for k in self.match_keys}
+
+        for viewer in self._iter_matched_viewers(include_self=False):
+            # orig_lims: limits in this "matched" viewer
+            # to_lims: proposed new limits for this "matched" viewer
+            orig_lims = {k: getattr(viewer.state, k) for k in self.match_keys}
+            to_lims = self._map_limits(self.viewer, viewer, from_lims)
+            with delay_callback(viewer.state, *self.match_keys):
+                for ax in self.match_axes:
+                    # to avoid recursion we'll only update the state if there is a change
+                    # outside a tolerance set by some fraction of the limits range
+                    if None in orig_lims.values():
+                        orig_range = np.inf
+                    else:
+                        orig_range = abs(orig_lims.get(f'{ax}_max') - orig_lims.get(f'{ax}_min'))
+                    to_range = abs(to_lims.get(f'{ax}_max') - to_lims.get(f'{ax}_min'))
+                    tol = 1e-6 * min(orig_range, to_range)
+
+                    for k in (f'{ax}_min', f'{ax}_max'):
+                        value = to_lims.get(k)
+                        orig_value = orig_lims.get(k)
+                        if not np.isnan(value) and (orig_value is None or
+                                                    abs(value-orig_lims.get(k, np.inf)) > tol):
+                            setattr(viewer.state, k, value)
+
+    def is_visible(self):
+        return len(self.viewer.jdaviz_app._viewer_store) > 1
+
+
 @viewer_tool
 class PrevZoom(Tool, _BaseZoomHistory):
     icon = os.path.join(ICON_DIR, 'zoom_back.svg')
     tool_id = 'jdaviz:prevzoom'
     action_text = 'Previous zoom'
     tool_tip = 'Back to previous zoom level'
 
@@ -246,14 +330,17 @@
         if not len(lines_x):
             return
         ind = np.argmin(abs(lines_x - data['domain']['x']))
         # find line closest to mouse position and transmit event
         msg = LineIdentifyMessage(self.line_names[ind], sender=self)
         self.viewer.session.hub.broadcast(msg)
 
+    def is_visible(self):
+        return len([m for m in self.viewer.figure.marks if isinstance(m, SpectralLine)]) > 0
+
 
 class _BaseSidebarShortcut(Tool):
     plugin_name = None  # define in subclass
     viewer_attr = 'viewer'
 
     def activate(self):
         plugin = self.viewer.jdaviz_app.get_tray_item_from_name(self.plugin_name)
```

### Comparing `jdaviz-3.5.0/jdaviz/core/user_api.py` & `jdaviz-3.6.0/jdaviz/core/user_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import astropy.units as u
+
 __all__ = ['UserApiWrapper', 'PluginUserApi']
 
 
 class UserApiWrapper:
     """
     This is an API wrapper around an internal object.  For a full list of attributes/methods,
     call dir(object).
@@ -34,20 +36,23 @@
             return super().__setattr__(attr, value)
 
         if attr in self._readonly:
             raise AttributeError("cannot set read-only item")
 
         exp_obj = getattr(self._obj, attr)
         from jdaviz.core.template_mixin import (SelectPluginComponent,
+                                                UnitSelectPluginComponent,
                                                 PlotOptionsSyncState,
                                                 AddResults,
                                                 AutoTextField)
         if isinstance(exp_obj, SelectPluginComponent):
             # this allows setting the selection directly without needing to access the underlying
             # .selected traitlet
+            if isinstance(exp_obj, UnitSelectPluginComponent) and isinstance(value, u.Unit):
+                value = value.to_string()
             exp_obj.selected = value
             return
         elif isinstance(exp_obj, AddResults):
             exp_obj.auto_label.value = value
             return
         elif isinstance(exp_obj, AutoTextField):
             exp_obj.value = value
@@ -77,11 +82,13 @@
     call help(plugin_object.attribute).
 
     For example::
       help(plugin_object.show)
     """
     def __init__(self, plugin, expose=[], readonly=[]):
         expose = list(set(list(expose) + ['open_in_tray', 'show']))
+        if plugin.uses_active_status:
+            expose += ['keep_active', 'as_active']
         super().__init__(plugin, expose, readonly)
 
     def __repr__(self):
         return f'<{self._obj._registry_label} API>'
```

### Comparing `jdaviz-3.5.0/jdaviz/core/validunits.py` & `jdaviz-3.6.0/jdaviz/core/validunits.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import astropy.units as u
-import numpy as np
+from astropy import units as u
 
 __all__ = ['units_to_strings', 'create_spectral_equivalencies_list',
            'create_flux_equivalencies_list']
 
 
 def units_to_strings(unit_list):
     """Convert equivalencies into readable versions of the units.
@@ -15,85 +14,75 @@
         to `astropy.units`.
 
     Returns
     -------
     result : list
         A list of the units with their best (i.e., most readable) string version.
     """
-    return [u.Unit(unit).name
-            if u.Unit(unit) == u.Unit("Angstrom")
-            else u.Unit(unit).long_names[0] if (
-                hasattr(u.Unit(unit), "long_names") and len(u.Unit(unit).long_names) > 0)
-            else u.Unit(unit).to_string()
-            for unit in unit_list]
+    return [u.Unit(unit).to_string() for unit in unit_list]
 
 
-def create_spectral_equivalencies_list(spectrum,
+def create_spectral_equivalencies_list(spectral_axis_unit,
                                        exclude=[u.jupiterRad, u.earthRad, u.solRad,
-                                                u.lyr, u.AU, u.pc]):
-    """Get all possible conversions from current spectral_axis_unit.
-    """
-    if spectrum.spectral_axis.unit == u.pix:
+                                                u.lyr, u.AU, u.pc, u.Bq, u.micron, u.lsec]):
+    """Get all possible conversions from current spectral_axis_unit."""
+    if spectral_axis_unit in (u.pix, u.dimensionless_unscaled):
         return []
 
     # Get unit equivalencies.
-    curr_spectral_axis_unit_equivalencies = u.Unit(
-        spectrum.spectral_axis.unit).find_equivalent_units(
-        equivalencies=u.spectral())
+    try:
+        curr_spectral_axis_unit_equivalencies = spectral_axis_unit.find_equivalent_units(
+            equivalencies=u.spectral())
+    except u.core.UnitConversionError:
+        return []
 
     # Get local units.
-    locally_defined_spectral_axis_units = ['angstrom', 'nanometer',
-                                           'micron', 'hertz', 'erg']
+    locally_defined_spectral_axis_units = ['Angstrom', 'nm',
+                                           'um', 'Hz', 'erg']
     local_units = [u.Unit(unit) for unit in locally_defined_spectral_axis_units]
 
     # Remove overlap units.
     curr_spectral_axis_unit_equivalencies = list(set(curr_spectral_axis_unit_equivalencies)
-                                                 - set(local_units+exclude))
+                                                 - set(local_units + exclude))
 
     # Convert equivalencies into readable versions of the units and sorted alphabetically.
     spectral_axis_unit_equivalencies_titles = sorted(units_to_strings(
         curr_spectral_axis_unit_equivalencies))
 
     # Concatenate both lists with the local units coming first.
-    spectral_axis_unit_equivalencies_titles = sorted(units_to_strings(
-        local_units)) + spectral_axis_unit_equivalencies_titles
-
-    return spectral_axis_unit_equivalencies_titles
+    return sorted(units_to_strings(local_units)) + spectral_axis_unit_equivalencies_titles
 
 
-def create_flux_equivalencies_list(spectrum):
-    """Get all possible conversions for flux from current flux units.
-    """
-    if ((spectrum.flux.unit == u.count) or (spectrum.spectral_axis.unit == u.pix)):
+def create_flux_equivalencies_list(flux_unit, spectral_axis_unit):
+    """Get all possible conversions for flux from current flux units."""
+    if ((flux_unit in (u.count, (u.MJy / u.sr), u.dimensionless_unscaled))
+            or (spectral_axis_unit in (u.pix, u.dimensionless_unscaled))):
         return []
 
-    # Get unit equivalencies.
-    curr_flux_unit_equivalencies = u.Unit(
-        spectrum.flux.unit).find_equivalent_units(
-            equivalencies=u.spectral_density(np.sum(spectrum.spectral_axis)),
+    # Get unit equivalencies. Value passed into u.spectral_density() is irrelevant.
+    try:
+        curr_flux_unit_equivalencies = flux_unit.find_equivalent_units(
+            equivalencies=u.spectral_density(1 * spectral_axis_unit),
             include_prefix_units=False)
+    except u.core.UnitConversionError:
+        return []
 
     # Get local units.
     locally_defined_flux_units = ['Jy', 'mJy', 'uJy',
                                   'W / (m2 Hz)',
                                   'eV / (s m2 Hz)',
                                   'erg / (s cm2)',
-                                  'erg / (s cm2 um)',
                                   'erg / (s cm2 Angstrom)',
                                   'erg / (s cm2 Hz)',
-                                  'ph / (s cm2 um)',
                                   'ph / (s cm2 Angstrom)',
                                   'ph / (s cm2 Hz)']
     local_units = [u.Unit(unit) for unit in locally_defined_flux_units]
 
     # Remove overlap units.
     curr_flux_unit_equivalencies = list(set(curr_flux_unit_equivalencies)
                                         - set(local_units))
 
     # Convert equivalencies into readable versions of the units and sort them alphabetically.
     flux_unit_equivalencies_titles = sorted(units_to_strings(curr_flux_unit_equivalencies))
 
     # Concatenate both lists with the local units coming first.
-    flux_unit_equivalencies_titles = (sorted(units_to_strings(local_units)) +
-                                      flux_unit_equivalencies_titles)
-
-    return flux_unit_equivalencies_titles
+    return sorted(units_to_strings(local_units)) + flux_unit_equivalencies_titles
```

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/checktoradial.svg` & `jdaviz-3.6.0/jdaviz/data/icons/checktoradial.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/compass.svg` & `jdaviz-3.6.0/jdaviz/data/icons/compass.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/line_select.svg` & `jdaviz-3.6.0/jdaviz/data/icons/line_select.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/line_select_disabled.svg` & `jdaviz-3.6.0/jdaviz/data/icons/line_select_disabled.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/pan.svg` & `jdaviz-3.6.0/jdaviz/data/icons/pan.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/pan2.svg` & `jdaviz-3.6.0/jdaviz/data/icons/pan2.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/panzoom_match.svg` & `jdaviz-3.6.0/jdaviz/data/icons/panzoom_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/pixelspectra.svg` & `jdaviz-3.6.0/jdaviz/data/icons/pixelspectra.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/radialtocheck.svg` & `jdaviz-3.6.0/jdaviz/data/icons/radialtocheck.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/select_circle.svg` & `jdaviz-3.6.0/jdaviz/data/icons/select_circle.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/select_ellipse.svg` & `jdaviz-3.6.0/jdaviz/data/icons/select_ellipse.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/select_lasso.svg` & `jdaviz-3.6.0/jdaviz/data/icons/select_lasso.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/select_single_pixel.svg` & `jdaviz-3.6.0/jdaviz/data/icons/select_single_pixel.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/select_xy.svg` & `jdaviz-3.6.0/jdaviz/data/icons/select_xy.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/slice.svg` & `jdaviz-3.6.0/jdaviz/data/icons/slice.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/spectral_range.svg` & `jdaviz-3.6.0/jdaviz/data/icons/spectral_range.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/icons/zoom_box_match.svg` & `jdaviz-3.6.0/jdaviz/data/icons/zoom_box_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/Atomic-ISO.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/Atomic-ISO.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/Atomic-Ionic.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/Atomic-Ionic.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/CO.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/CO.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/Common_nebular.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/Common_nebular.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/Common_stellar.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/Common_stellar.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/DEV_NOTES.txt` & `jdaviz-3.6.0/jdaviz/data/linelists/DEV_NOTES.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/H-He.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/H-He.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/H-Paschen-Brackett.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/H-Paschen-Brackett.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/H2-ISO.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/H2-ISO.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/H2-alt.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/H2-alt.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/H2.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/H2.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/HeI-HeII.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/HeI-HeII.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/JWST_line_list_original.txt` & `jdaviz-3.6.0/jdaviz/data/linelists/JWST_line_list_original.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/PAH.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/PAH.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/SDSS-IV.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/SDSS-IV.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/SDSS.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/SDSS.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/UV_linelist_vacuum.csv` & `jdaviz-3.6.0/jdaviz/data/linelists/UV_linelist_vacuum.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/data/linelists/linelist_metadata.json` & `jdaviz-3.6.0/jdaviz/data/linelists/linelist_metadata.json`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/jdaviz_cli.ipynb` & `jdaviz-3.6.0/jdaviz/jdaviz_cli.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/models/physical_models.py` & `jdaviz-3.6.0/jdaviz/models/physical_models.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/tests/coveragerc` & `jdaviz-3.6.0/jdaviz/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/tests/test_app.py` & `jdaviz-3.6.0/jdaviz/tests/test_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,33 +49,34 @@
     class Customviz(Specviz):
         _default_configuration = config
         _default_spectrum_viewer_reference_name = 'h'
 
     viz = Customviz()
     assert viz.app.get_viewer_reference_names() == ['h', 'k']
 
-    viz.load_spectrum(spectrum1d, data_label='example label')
-    assert not len(viz.app.get_data_from_viewer("h", "non-existent label"))
+    viz.load_data(spectrum1d, data_label='example label')
+    with pytest.raises(ValueError):
+        viz.get_data("non-existent label")
 
 
 def test_duplicate_data_labels(specviz_helper, spectrum1d):
-    specviz_helper.load_spectrum(spectrum1d, data_label="test")
-    specviz_helper.load_spectrum(spectrum1d, data_label="test")
+    specviz_helper.load_data(spectrum1d, data_label="test")
+    specviz_helper.load_data(spectrum1d, data_label="test")
     dc = specviz_helper.app.data_collection
     assert dc[0].label == "test"
     assert dc[1].label == "test (1)"
-    specviz_helper.load_spectrum(spectrum1d, data_label="test_1")
-    specviz_helper.load_spectrum(spectrum1d, data_label="test")
+    specviz_helper.load_data(spectrum1d, data_label="test_1")
+    specviz_helper.load_data(spectrum1d, data_label="test")
     assert dc[2].label == "test_1"
     assert dc[3].label == "test (2)"
 
 
 def test_duplicate_data_labels_with_brackets(specviz_helper, spectrum1d):
-    specviz_helper.load_spectrum(spectrum1d, data_label="test[test]")
-    specviz_helper.load_spectrum(spectrum1d, data_label="test[test]")
+    specviz_helper.load_data(spectrum1d, data_label="test[test]")
+    specviz_helper.load_data(spectrum1d, data_label="test[test]")
     dc = specviz_helper.app.data_collection
     assert len(dc) == 2
     assert dc[0].label == "test[test]"
     assert dc[1].label == "test[test] (1)"
 
 
 def test_return_data_label_is_none(specviz_helper):
@@ -101,42 +102,42 @@
     assert data_label == "myimage"
 
 
 def test_unique_name_variations(specviz_helper, spectrum1d):
     data_label = specviz_helper.app.return_unique_name(None)
     assert data_label == "Unknown"
 
-    specviz_helper.load_spectrum(spectrum1d, data_label="test[flux]")
+    specviz_helper.load_data(spectrum1d, data_label="test[flux]")
     data_label = specviz_helper.app.return_data_label("test[flux]", ext="flux")
     assert data_label == "test[flux][flux]"
 
     data_label = specviz_helper.app.return_data_label("test", ext="flux")
     assert data_label == "test[flux] (1)"
 
 
 def test_substring_in_label(specviz_helper, spectrum1d):
-    specviz_helper.load_spectrum(spectrum1d, data_label="M31")
-    specviz_helper.load_spectrum(spectrum1d, data_label="M32")
+    specviz_helper.load_data(spectrum1d, data_label="M31")
+    specviz_helper.load_data(spectrum1d, data_label="M32")
     data_label = specviz_helper.app.return_data_label("M")
     assert data_label == "M"
 
 
 @pytest.mark.parametrize('data_label', ('111111', 'aaaaa', '///(#$@)',
                                         'two  spaces  repeating',
                                         'word42word42word  two  spaces'))
 def test_edge_cases(specviz_helper, spectrum1d, data_label):
     dc = specviz_helper.app.data_collection
 
-    specviz_helper.load_spectrum(spectrum1d, data_label=data_label)
-    specviz_helper.load_spectrum(spectrum1d, data_label=data_label)
+    specviz_helper.load_data(spectrum1d, data_label=data_label)
+    specviz_helper.load_data(spectrum1d, data_label=data_label)
     assert dc[1].label == f"{data_label} (1)"
 
-    specviz_helper.load_spectrum(spectrum1d, data_label=data_label)
+    specviz_helper.load_data(spectrum1d, data_label=data_label)
     assert dc[2].label == f"{data_label} (2)"
 
 
 def test_case_that_used_to_break_return_label(specviz_helper, spectrum1d):
-    specviz_helper.load_spectrum(spectrum1d, data_label="this used to break (1)")
-    specviz_helper.load_spectrum(spectrum1d, data_label="this used to break")
+    specviz_helper.load_data(spectrum1d, data_label="this used to break (1)")
+    specviz_helper.load_data(spectrum1d, data_label="this used to break")
     dc = specviz_helper.app.data_collection
     assert dc[0].label == "this used to break (1)"
     assert dc[1].label == "this used to break (2)"
```

### Comparing `jdaviz-3.5.0/jdaviz/tests/test_data_formats.py` & `jdaviz-3.6.0/jdaviz/tests/test_data_formats.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/tests/test_metadata.py` & `jdaviz-3.6.0/jdaviz/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/tests/test_subsets.py` & `jdaviz-3.6.0/jdaviz/tests/test_subsets.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import numpy as np
 import pytest
 from astropy import units as u
 from astropy.tests.helper import assert_quantity_allclose
 from glue.core import Data
-from glue.core.roi import CircularROI, EllipticalROI, RectangularROI, XRangeROI
-
-from glue.core.edit_subset_mode import AndMode, AndNotMode, OrMode, XorMode
-from regions import PixCoord, CirclePixelRegion, RectanglePixelRegion, EllipsePixelRegion
-
+from glue.core.roi import CircularROI, CircularAnnulusROI, EllipticalROI, RectangularROI, XRangeROI
+from glue.core.subset_group import GroupedSubset
+from glue.core.edit_subset_mode import AndMode, AndNotMode, OrMode, XorMode, NewMode
+from regions import (PixCoord, CirclePixelRegion, RectanglePixelRegion, EllipsePixelRegion,
+                     CircleAnnulusPixelRegion)
 from numpy.testing import assert_allclose
-from specutils import SpectralRegion
+from specutils import SpectralRegion, Spectrum1D
 
 from jdaviz.core.marks import ShadowSpatialSpectral
+from jdaviz.utils import get_subset_type
 
 
 def test_region_from_subset_2d(cubeviz_helper):
     data = Data(flux=np.ones((128, 128)), label='Test 2D Flux')
     cubeviz_helper.app.data_collection.append(data)
 
     subset_plugin = cubeviz_helper.app.get_tray_item_from_name('g-subset-plugin')
 
     cubeviz_helper.app.add_data_to_viewer('flux-viewer', 'Test 2D Flux')
 
     cubeviz_helper.app.get_viewer('flux-viewer').apply_roi(EllipticalROI(1, 3.5, 1.2, 3.3))
 
-    subsets = cubeviz_helper.app.get_subsets_from_viewer('flux-viewer')
-    reg = subsets.get('Subset 1')
+    subsets = cubeviz_helper.app.get_subsets()
+    reg = subsets.get('Subset 1')[0]['region']
 
     assert len(subsets) == 1
     assert isinstance(reg, EllipsePixelRegion)
 
     assert_allclose(reg.center.x, 1)
     assert_allclose(reg.center.y, 3.5)
     assert_allclose(reg.width, 2.4)
@@ -97,27 +98,27 @@
     for key in ("orig", "value"):
         assert subset_plugin._get_value_from_subset_definition(0, "Xmin", key) == 2
         assert subset_plugin._get_value_from_subset_definition(0, "Xmax", key) == 3.5
         assert subset_plugin._get_value_from_subset_definition(0, "Ymin", key) == 0
         assert subset_plugin._get_value_from_subset_definition(0, "Ymax", key) == 3.3
         assert subset_plugin._get_value_from_subset_definition(0, "Angle", key) == 45
 
-    subsets = cubeviz_helper.app.get_subsets_from_viewer('flux-viewer')
-    reg = subsets.get('Subset 1')
+    subsets = cubeviz_helper.app.get_subsets()
+    reg = subsets.get('Subset 1')[0]['region']
 
     assert_allclose(reg.center.x, 2.75)
     assert_allclose(reg.center.y, 1.65)
     assert_allclose(reg.width, 1.5)
     assert_allclose(reg.height, 3.3)
     assert_allclose(reg.angle.to_value(u.deg), 45)  # Might be stored in radians
 
     # Move the rectangle
     subset_plugin.set_center((3, 2), update=True)
-    subsets = cubeviz_helper.app.get_subsets_from_viewer('flux-viewer')
-    reg = subsets.get('Subset 1')
+    subsets = cubeviz_helper.app.get_subsets()
+    reg = subsets.get('Subset 1')[0]['region']
     assert_allclose(reg.center.x, 3)
     assert_allclose(reg.center.y, 2)
     assert_allclose(reg.width, 1.5)
     assert_allclose(reg.height, 3.3)
     assert_allclose(reg.angle.to_value(u.deg), 45)  # Might be stored in radians
 
     # Circular Subset
@@ -131,24 +132,22 @@
     for key in ("orig", "value"):
         assert subset_plugin._get_value_from_subset_definition(0, "X Center", key) == 3
         assert subset_plugin._get_value_from_subset_definition(0, "Y Center", key) == 4
         assert subset_plugin._get_value_from_subset_definition(0, "Radius", key) == 2.4
 
 
 def test_region_from_subset_profile(cubeviz_helper, spectral_cube_wcs):
-    data = Data(flux=np.ones((128, 128, 256)), label='Test 1D Flux', coords=spectral_cube_wcs)
+    data = Spectrum1D(flux=np.ones((128, 128, 256)) * u.nJy, wcs=spectral_cube_wcs)
     subset_plugin = cubeviz_helper.app.get_tray_item_from_name('g-subset-plugin')
 
-    cubeviz_helper.app.data_collection.append(data)
-
-    cubeviz_helper.app.add_data_to_viewer('spectrum-viewer', 'Test 1D Flux')
+    cubeviz_helper.load_data(data, data_label='Test 1D Flux')
 
     cubeviz_helper.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(5, 15.5))
 
-    subsets = cubeviz_helper.app.get_subsets_from_viewer('spectrum-viewer', subset_type='spectral')
+    subsets = cubeviz_helper.app.get_subsets(spectral_only=True)
     reg = subsets.get('Subset 1')
 
     assert len(subsets) == 1
     assert isinstance(reg, SpectralRegion)
     assert_quantity_allclose(reg.lower, 5.0 * u.Hz)
     assert_quantity_allclose(reg.upper, 15.5 * u.Hz)
 
@@ -165,86 +164,129 @@
     # "orig" is unchanged until user clicks Update button.
     assert subset_plugin._get_value_from_subset_definition(0, "Lower bound", "orig") == 5
     subset_plugin.vue_update_subset()
     for key in ("orig", "value"):
         assert subset_plugin._get_value_from_subset_definition(0, "Lower bound", key) == 10
         assert subset_plugin._get_value_from_subset_definition(0, "Upper bound", key) == 15.5
 
-    subsets = cubeviz_helper.app.get_subsets_from_viewer('spectrum-viewer', subset_type='spectral')
+    subsets = cubeviz_helper.app.get_subsets(spectral_only=True)
     reg = subsets.get('Subset 1')
 
     assert_quantity_allclose(reg.lower, 10.0 * u.Hz)
     assert_quantity_allclose(reg.upper, 15.5 * u.Hz)
 
     # Move the Subset.
     subset_plugin.set_center(10, update=True)
-    subsets = cubeviz_helper.app.get_subsets_from_viewer('spectrum-viewer', subset_type='spectral')
+    subsets = cubeviz_helper.app.get_subsets(spectral_only=True)
     reg = subsets.get('Subset 1')
     assert_quantity_allclose(reg.lower, 7.25 * u.Hz)
     assert_quantity_allclose(reg.upper, 12.75 * u.Hz)
 
 
 def test_region_spectral_spatial(cubeviz_helper, spectral_cube_wcs):
-    data = Data(flux=np.ones((128, 128, 256)), label='Test Flux', coords=spectral_cube_wcs)
-    cubeviz_helper.app.data_collection.append(data)
-
-    cubeviz_helper.app.add_data_to_viewer('spectrum-viewer', 'Test Flux')
-    cubeviz_helper.app.add_data_to_viewer('flux-viewer', 'Test Flux')
+    data = Spectrum1D(flux=np.ones((128, 128, 256)) * u.nJy, wcs=spectral_cube_wcs)
+    cubeviz_helper.load_data(data, data_label="Test Flux")
 
     # use gaussian smooth plugin as a regression test for
     # https://github.com/spacetelescope/jdaviz/issues/1853
     cubeviz_helper.plugins['Gaussian Smooth'].smooth(add_data=True)
 
-    spectrum_viewer = cubeviz_helper.app.get_viewer("spectrum-viewer")
+    spectrum_viewer_name = cubeviz_helper._default_spectrum_viewer_reference_name
+    spectrum_viewer = cubeviz_helper.app.get_viewer(spectrum_viewer_name)
     spectrum_viewer.apply_roi(XRangeROI(5, 15.5))
 
     # should be no spatial-spectral intersection marks yet
     assert len([m for m in spectrum_viewer.figure.marks if isinstance(m, ShadowSpatialSpectral)]) == 0  # noqa
 
     flux_viewer = cubeviz_helper.app.get_viewer("flux-viewer")
     # We set the active tool here to trigger a reset of the Subset state to "Create New"
     flux_viewer.toolbar.active_tool = flux_viewer.toolbar.tools['bqplot:rectangle']
     flux_viewer.apply_roi(RectangularROI(1, 3.5, -0.2, 3.3))
 
-    assert len([m for m in spectrum_viewer.figure.marks if isinstance(m, ShadowSpatialSpectral)]) == 1  # noqa
+    assert len([m for m in spectrum_viewer.figure.marks if isinstance(m, ShadowSpatialSpectral)]) == 2  # noqa
 
-    subsets = cubeviz_helper.app.get_subsets_from_viewer('spectrum-viewer', subset_type='spectral')
+    subsets = cubeviz_helper.app.get_subsets(spectral_only=True)
     reg = subsets.get('Subset 1')
 
     assert len(subsets) == 1
     assert isinstance(reg, SpectralRegion)
 
     assert_quantity_allclose(reg.lower, 5.0 * u.Hz)
     assert_quantity_allclose(reg.upper, 15.5 * u.Hz)
 
-    subsets = cubeviz_helper.app.get_subsets_from_viewer('flux-viewer', subset_type='spatial')
-    reg = subsets.get('Subset 2')
+    subsets = cubeviz_helper.app.get_subsets(spatial_only=True)
+    reg = subsets.get('Subset 2')[0]['region']
 
     assert len(subsets) == 1
     assert isinstance(reg, RectanglePixelRegion)
     assert_allclose(reg.center.x, 2.25)
     assert_allclose(reg.center.y, 1.55)
     assert_allclose(reg.width, 2.5)
     assert_allclose(reg.height, 3.5)
 
     # add another spectral subset to ensure the spatial-spectral intersection marks are created as
     # expected
     # reset the tool to force a new selection instead of the default "replace"
     spectrum_viewer.toolbar.active_tool = spectrum_viewer.toolbar.tools['jdaviz:panzoom']
     spectrum_viewer.toolbar.active_tool = spectrum_viewer.toolbar.tools['bqplot:xrange']
     spectrum_viewer.apply_roi(XRangeROI(3, 16))
+    assert len([m for m in spectrum_viewer.figure.marks if isinstance(m, ShadowSpatialSpectral)]) == 4  # noqa
+
+    # Delete the spatial subset to make sure ALL ShadowSpatialSpectral marks are removed
+    dc = cubeviz_helper.app.data_collection
+    dc.remove_subset_group(dc.subset_groups[1])
+
+    assert len([m for m in spectrum_viewer.figure.marks if isinstance(m, ShadowSpatialSpectral)]) == 0  # noqa
+
+    spectrum_viewer.session.edit_subset_mode._mode = NewMode
+    flux_viewer.toolbar.active_tool = flux_viewer.toolbar.tools['bqplot:rectangle']
+    flux_viewer.apply_roi(RectangularROI(1, 3.5, -0.2, 3.3))
+
+    assert len([m for m in spectrum_viewer.figure.marks if isinstance(m, ShadowSpatialSpectral)]) == 4  # noqa
+
+    # This creates a composite subset, which tests if ShadowSpatialSpectral marks are added
+    # to those types of subsets as well
+    spectrum_viewer.session.edit_subset_mode._mode = OrMode
+    flux_viewer.toolbar.active_tool = flux_viewer.toolbar.tools['bqplot:rectangle']
+    flux_viewer.apply_roi(RectangularROI(0, 2, 2, 4))
+
+    assert len([m for m in spectrum_viewer.figure.marks if isinstance(m, ShadowSpatialSpectral)]) == 4  # noqa
+
+    # Delete one of the spectral subsets to make sure the other is still applied as two
+    # ShadowSpatialSpectral objects. One for the data's spatial subset and the other for the
+    # smoothed data's spatial subset
+    dc.remove_subset_group(dc.subset_groups[0])
+
     assert len([m for m in spectrum_viewer.figure.marks if isinstance(m, ShadowSpatialSpectral)]) == 2  # noqa
 
+    # Make sure that ShadowSpectralSpatial objects become invisible with data
+    cubeviz_helper.app.set_data_visibility(cubeviz_helper._default_spectrum_viewer_reference_name,
+                                           dc[-1].label, visible=False)
+    assert len([m for m in spectrum_viewer.figure.marks if isinstance(m, ShadowSpatialSpectral) and m.visible]) == 1  # noqa
+    cubeviz_helper.app.set_data_visibility(cubeviz_helper._default_spectrum_viewer_reference_name,
+                                           dc[-1].label, visible=True)
+
+    assert len([m for m in spectrum_viewer.figure.marks if isinstance(m, ShadowSpatialSpectral)]) == 2  # noqa
+
+    # Test that removing and adding the data from the viewer removes and adds
+    # the shadow marks accordingly
+    cubeviz_helper.app.remove_data_from_viewer(spectrum_viewer_name, dc[-1].label)
+    assert len([m for m in spectrum_viewer.figure.marks if isinstance(m, ShadowSpatialSpectral)]) == 1  # noqa
+    cubeviz_helper.app.add_data_to_viewer(spectrum_viewer_name, dc[-1].label)
+    assert len([m for m in spectrum_viewer.figure.marks if isinstance(m, ShadowSpatialSpectral)]) == 2  # noqa
+
+    # Remove the smoothed data to make sure the ShadowSpatialSpectral object still applies to
+    # the original data's spatial subset
+    dc.remove(dc[-1])
+    assert len([m for m in spectrum_viewer.figure.marks if isinstance(m, ShadowSpatialSpectral)]) == 1  # noqa
 
-def test_disjoint_spatial_subset(cubeviz_helper, spectral_cube_wcs):
-    data = Data(flux=np.ones((128, 128, 256)), label='Test Flux', coords=spectral_cube_wcs)
-    cubeviz_helper.app.data_collection.append(data)
 
-    cubeviz_helper.app.add_data_to_viewer('spectrum-viewer', 'Test Flux')
-    cubeviz_helper.app.add_data_to_viewer('flux-viewer', 'Test Flux')
+def test_disjoint_spatial_subset(cubeviz_helper, spectral_cube_wcs):
+    data = Spectrum1D(flux=np.ones((128, 128, 256)) * u.nJy, wcs=spectral_cube_wcs)
+    cubeviz_helper.load_data(data, data_label="Test Flux")
 
     flux_viewer = cubeviz_helper.app.get_viewer("flux-viewer")
     flux_viewer.apply_roi(CircularROI(xc=3, yc=4, radius=1))
 
     mf = cubeviz_helper.plugins['Model Fitting']
     assert len(mf.spatial_subset.choices) == 2  # 'Entire Cube' and Subset 1
     assert len(mf.spectral_subset.choices) == 1  # 'Entire Spectrum'
@@ -256,19 +298,16 @@
     # regression test for https://github.com/spacetelescope/jdaviz/pull/2058
     assert len(mf.spatial_subset.choices) == 2  # 'Entire Cube' and Subset 1
     assert len(mf.spectral_subset.choices) == 1  # 'Entire Spectrum'
 
 
 def test_disjoint_spectral_subset(cubeviz_helper, spectral_cube_wcs):
     subset_plugin = cubeviz_helper.app.get_tray_item_from_name('g-subset-plugin')
-    data = Data(flux=np.ones((128, 128, 256)), label='Test Flux', coords=spectral_cube_wcs)
-    cubeviz_helper.app.data_collection.append(data)
-
-    cubeviz_helper.app.add_data_to_viewer('spectrum-viewer', 'Test Flux')
-    cubeviz_helper.app.add_data_to_viewer('flux-viewer', 'Test Flux')
+    data = Spectrum1D(flux=np.ones((128, 128, 256)) * u.nJy, wcs=spectral_cube_wcs)
+    cubeviz_helper.load_data(data, data_label="Test Flux")
 
     spec_viewer = cubeviz_helper.app.get_viewer("spectrum-viewer")
     spec_viewer.apply_roi(XRangeROI(5, 15.5))
 
     # Add second region to Subset 1
     cubeviz_helper.app.session.edit_subset_mode.mode = OrMode
     spec_viewer.apply_roi(XRangeROI(30, 35))
@@ -325,18 +364,18 @@
     reg = cubeviz_helper.app.get_subsets("Subset 1")
     rectangle1 = RectanglePixelRegion(center=PixCoord(x=27.5, y=27.5),
                                       width=5, height=5, angle=0.0 * u.deg)
     assert reg[-1] == {'name': 'RectangularROI', 'glue_state': 'AndNotState', 'region': rectangle1,
                        'subset_state': reg[-1]['subset_state']}
 
     cubeviz_helper.app.session.edit_subset_mode.mode = OrMode
-    viewer.apply_roi(EllipticalROI(30, 30, 3, 6))
+    viewer.apply_roi(EllipticalROI(xc=30, yc=30, radius_x=3, radius_y=6))
     reg = cubeviz_helper.app.get_subsets("Subset 1")
     ellipse1 = EllipsePixelRegion(center=PixCoord(x=30, y=30),
-                                  width=3, height=6, angle=0.0 * u.deg)
+                                  width=6, height=12, angle=0.0 * u.deg)
     assert reg[-1] == {'name': 'EllipticalROI', 'glue_state': 'OrState', 'region': ellipse1,
                        'subset_state': reg[-1]['subset_state']}
 
     cubeviz_helper.app.session.edit_subset_mode.mode = AndMode
     viewer.apply_roi(RectangularROI(20, 25, 20, 25))
     reg = cubeviz_helper.app.get_subsets("Subset 1")
     rectangle2 = RectanglePixelRegion(center=PixCoord(x=22.5, y=22.5),
@@ -377,29 +416,29 @@
     reg = cubeviz_helper.app.get_subsets("Subset 1")
     rectangle1 = RectanglePixelRegion(center=PixCoord(x=27.5, y=27.5),
                                       width=5, height=5, angle=0.0 * u.deg)
     assert reg[-1] == {'name': 'RectangularROI', 'glue_state': 'AndNotState', 'region': rectangle1,
                        'subset_state': reg[-1]['subset_state']}
 
     cubeviz_helper.app.session.edit_subset_mode.mode = AndNotMode
-    viewer.apply_roi(EllipticalROI(30, 30, 3, 6))
+    viewer.apply_roi(EllipticalROI(xc=30, yc=30, radius_x=3, radius_y=6))
     reg = cubeviz_helper.app.get_subsets("Subset 1")
     ellipse1 = EllipsePixelRegion(center=PixCoord(x=30, y=30),
-                                  width=3, height=6, angle=0.0 * u.deg)
+                                  width=6, height=12, angle=0.0 * u.deg)
     assert reg[-1] == {'name': 'EllipticalROI', 'glue_state': 'AndNotState', 'region': ellipse1,
                        'subset_state': reg[-1]['subset_state']}
 
     regions_list = cubeviz_helper.app.get_subsets("Subset 1", object_only=True)
     assert len(regions_list) == 3
-    assert regions_list[-1].width == 3
+    assert regions_list[-1].width == 6
 
     regions_list = cubeviz_helper.app.get_subsets("Subset 1", spatial_only=True,
                                                   object_only=True)
     assert len(regions_list) == 3
-    assert regions_list[-1].width == 3
+    assert regions_list[-1].width == 6
 
     spatial_list = cubeviz_helper.app.get_subsets("Subset 1", spatial_only=True)
     assert len(spatial_list) == 3
 
     subset_plugin = cubeviz_helper.app.get_tray_item_from_name('g-subset-plugin')
     assert subset_plugin.subset_selected == "Subset 1"
     assert subset_plugin.subset_types == ['CircularROI', 'RectangularROI', 'EllipticalROI']
@@ -417,57 +456,69 @@
 
     # Make sure changes were not propagated
     reg = cubeviz_helper.app.get_subsets("Subset 1")
     assert reg[0]['subset_state'].roi.radius == 5
     assert reg[1]['subset_state'].roi.xmin == 25
     assert reg[1]['subset_state'].roi.xmax == 30
 
+    for layer in viewer.state.layers:
+        if isinstance(layer.layer, GroupedSubset):
+            assert get_subset_type(layer.layer.subset_state) == 'spatial'
+
 
 def test_composite_region_with_imviz(imviz_helper, image_2d_wcs):
     arr = np.ones((10, 10))
 
     data_label = 'image-data'
-    viewer = imviz_helper.app.get_viewer('imviz-0')
+    viewer = imviz_helper.default_viewer
     imviz_helper.load_data(arr, data_label=data_label, show_in_viewer=True)
     viewer.apply_roi(CircularROI(xc=5, yc=5, radius=2))
     reg = imviz_helper.app.get_subsets("Subset 1")
     circle1 = CirclePixelRegion(center=PixCoord(x=5, y=5), radius=2)
     assert reg[-1] == {'name': 'CircularROI', 'glue_state': 'RoiSubsetState', 'region': circle1,
                        'subset_state': reg[-1]['subset_state']}
 
     imviz_helper.app.session.edit_subset_mode.mode = AndNotMode
-    viewer.apply_roi(RectangularROI(2, 4, 2, 4))
+    viewer.apply_roi(RectangularROI(xmin=2, xmax=4, ymin=2, ymax=4))
     reg = imviz_helper.app.get_subsets("Subset 1")
     rectangle1 = RectanglePixelRegion(center=PixCoord(x=3, y=3),
                                       width=2, height=2, angle=0.0 * u.deg)
     assert reg[-1] == {'name': 'RectangularROI', 'glue_state': 'AndNotState', 'region': rectangle1,
                        'subset_state': reg[-1]['subset_state']}
 
     imviz_helper.app.session.edit_subset_mode.mode = AndNotMode
-    viewer.apply_roi(EllipticalROI(3, 3, 3, 6))
+    viewer.apply_roi(EllipticalROI(xc=3, yc=3, radius_x=3, radius_y=6))
     reg = imviz_helper.app.get_subsets("Subset 1")
     ellipse1 = EllipsePixelRegion(center=PixCoord(x=3, y=3),
-                                  width=3, height=6, angle=0.0 * u.deg)
+                                  width=6, height=12, angle=0.0 * u.deg)
     assert reg[-1] == {'name': 'EllipticalROI', 'glue_state': 'AndNotState', 'region': ellipse1,
                        'subset_state': reg[-1]['subset_state']}
 
+    imviz_helper.app.session.edit_subset_mode.mode = OrMode
+    viewer.apply_roi(CircularAnnulusROI(xc=5, yc=5, inner_radius=2.5, outer_radius=5))
+    reg = imviz_helper.app.get_subsets("Subset 1")
+    ann1 = CircleAnnulusPixelRegion(center=PixCoord(x=5, y=5), inner_radius=2.5, outer_radius=5)
+    assert reg[-1] == {'name': 'CircularAnnulusROI', 'glue_state': 'OrState', 'region': ann1,
+                       'subset_state': reg[-1]['subset_state']}
+
     subset_plugin = imviz_helper.app.get_tray_item_from_name('g-subset-plugin')
     assert subset_plugin.subset_selected == "Subset 1"
-    assert subset_plugin.subset_types == ['CircularROI', 'RectangularROI', 'EllipticalROI']
-    assert subset_plugin.glue_state_types == ['AndState', 'AndNotState', 'AndNotState']
+    assert subset_plugin.subset_types == ['CircularROI', 'RectangularROI', 'EllipticalROI',
+                                          'CircularAnnulusROI']
+    assert subset_plugin.glue_state_types == ['AndState', 'AndNotState', 'AndNotState', 'OrState']
 
 
 def test_with_invalid_subset_name(cubeviz_helper):
     subset_name = "Test"
     with pytest.raises(ValueError, match=f'{subset_name} not in '):
         cubeviz_helper.app.get_subsets(subset_name=subset_name)
 
 
 def test_composite_region_from_subset_2d(specviz_helper, spectrum1d):
-    specviz_helper.load_spectrum(spectrum1d)
+    specviz_helper.load_data(spectrum1d)
     viewer = specviz_helper.app.get_viewer(specviz_helper._default_spectrum_viewer_reference_name)
     viewer.apply_roi(XRangeROI(6000, 7000))
     reg = specviz_helper.app.get_subsets("Subset 1", simplify_spectral=False)
     subset1 = SpectralRegion(6000 * spectrum1d.spectral_axis.unit,
                              7000 * spectrum1d.spectral_axis.unit)
     assert reg[-1]['region'].lower == subset1.lower and reg[-1]['region'].upper == subset1.upper
     assert reg[-1]['glue_state'] == 'RangeSubsetState'
@@ -500,17 +551,24 @@
     assert reg[-1]['glue_state'] == 'AndState'
 
     subset_plugin = specviz_helper.app.get_tray_item_from_name('g-subset-plugin')
     assert subset_plugin.subset_selected == "Subset 1"
     assert subset_plugin.subset_types == ['Range', 'Range', 'Range', 'Range']
     assert subset_plugin.glue_state_types == ['AndState', 'AndNotState', 'OrState', 'AndState']
 
+    subset_plugin.vue_simplify_subset()
+    assert subset_plugin.glue_state_types == ["RangeSubsetState", "OrState"]
+
+    for layer in viewer.state.layers:
+        if isinstance(layer.layer, GroupedSubset):
+            assert get_subset_type(layer.layer.subset_state) == 'spectral'
+
 
 def test_edit_composite_spectral_subset(specviz_helper, spectrum1d):
-    specviz_helper.load_spectrum(spectrum1d)
+    specviz_helper.load_data(spectrum1d)
     viewer = specviz_helper.app.get_viewer(specviz_helper._default_spectrum_viewer_reference_name)
 
     viewer.apply_roi(XRangeROI(6200, 6800))
     specviz_helper.app.session.edit_subset_mode.mode = OrMode
     viewer.apply_roi(XRangeROI(7200, 7600))
 
     specviz_helper.app.session.edit_subset_mode.mode = XorMode
@@ -543,10 +601,115 @@
     # This should be prevented by the _check_inputs method
     subset_plugin._set_value_in_subset_definition(0, "Lower bound", "value", 8000)
     subset_plugin.vue_update_subset()
     reg2 = specviz_helper.app.get_subsets("Subset 1")
     assert reg.lower.value == reg2.lower.value
     assert reg.upper.value == reg2.upper.value
 
+    assert subset_plugin.can_simplify
+
     viewer.apply_roi(XRangeROI(7800, 8000))
     with pytest.raises(ValueError, match="AND mode should overlap with existing subset"):
         specviz_helper.app.get_subsets("Subset 1")
+
+
+def test_edit_composite_spectral_with_xor(specviz_helper, spectrum1d):
+    specviz_helper.load_data(spectrum1d)
+    viewer = specviz_helper.app.get_viewer(specviz_helper._default_spectrum_viewer_reference_name)
+
+    viewer.apply_roi(XRangeROI(6400, 6600))
+    specviz_helper.app.session.edit_subset_mode.mode = OrMode
+    viewer.apply_roi(XRangeROI(7200, 7400))
+
+    viewer.apply_roi(XRangeROI(7600, 7800))
+
+    specviz_helper.app.session.edit_subset_mode.mode = XorMode
+    viewer.apply_roi(XRangeROI(6700, 7700))
+    reg = specviz_helper.app.get_subsets("Subset 1")
+
+    assert reg[0].lower.value == 6400 and reg[0].upper.value == 6600
+    assert reg[1].lower.value == 6700 and reg[1].upper.value == 7200
+    assert reg[2].lower.value == 7400 and reg[2].upper.value == 7600
+    assert reg[3].lower.value == 7700 and reg[3].upper.value == 7800
+
+
+def test_overlapping_spectral_regions(specviz_helper, spectrum1d):
+    specviz_helper.load_data(spectrum1d)
+    viewer = specviz_helper.app.get_viewer(specviz_helper._default_spectrum_viewer_reference_name)
+
+    viewer.apply_roi(XRangeROI(6400, 7400))
+    specviz_helper.app.session.edit_subset_mode.mode = AndNotMode
+    viewer.apply_roi(XRangeROI(6600, 7200))
+
+    specviz_helper.app.session.edit_subset_mode.mode = OrMode
+    viewer.apply_roi(XRangeROI(6600, 7300))
+
+    subset_plugin = specviz_helper.app.get_tray_item_from_name('g-subset-plugin')
+    assert subset_plugin.can_simplify
+    subset_plugin.vue_simplify_subset()
+
+    reg = specviz_helper.app.get_subsets("Subset 1")
+    assert reg.lower.value == 6400 and reg.upper.value == 7400
+
+
+def test_only_overlapping_spectral_regions(specviz_helper, spectrum1d):
+    specviz_helper.load_data(spectrum1d)
+    viewer = specviz_helper.app.get_viewer(specviz_helper._default_spectrum_viewer_reference_name)
+
+    viewer.apply_roi(XRangeROI(6400, 6600))
+    assert specviz_helper.app.is_there_overlap_spectral_subset("Subset 1") is False
+    specviz_helper.app.session.edit_subset_mode.mode = OrMode
+    viewer.apply_roi(XRangeROI(7000, 7400))
+
+    viewer.apply_roi(XRangeROI(6600, 7300))
+
+    viewer.apply_roi(XRangeROI(7600, 7800))
+
+    subset_plugin = specviz_helper.app.get_tray_item_from_name('g-subset-plugin')
+    assert subset_plugin.can_simplify
+    subset_plugin.vue_simplify_subset()
+
+    reg = specviz_helper.app.get_subsets("Subset 1")
+    assert reg[0].lower.value == 6400 and reg[0].upper.value == 7400
+    assert reg[1].lower.value == 7600 and reg[1].upper.value == 7800
+
+
+def test_overlapping_in_specviz2d(specviz2d_helper, mos_spectrum2d):
+    specviz2d_helper.load_data(spectrum_2d=mos_spectrum2d)
+    viewer = specviz2d_helper.app.get_viewer(
+        specviz2d_helper._default_spectrum_2d_viewer_reference_name)
+
+    viewer.apply_roi(XRangeROI(6400, 7400))
+    specviz2d_helper.app.session.edit_subset_mode.mode = AndNotMode
+    viewer.apply_roi(XRangeROI(6600, 7200))
+
+    specviz2d_helper.app.session.edit_subset_mode.mode = OrMode
+    viewer.apply_roi(XRangeROI(6600, 7300))
+
+    subset_plugin = specviz2d_helper.app.get_tray_item_from_name('g-subset-plugin')
+    assert subset_plugin.can_simplify
+    subset_plugin.vue_simplify_subset()
+
+    reg = specviz2d_helper.app.get_subsets("Subset 1")
+    assert reg.lower.value == 6400 and reg.upper.value == 7400
+
+
+def test_only_overlapping_in_specviz2d(specviz2d_helper, mos_spectrum2d):
+    specviz2d_helper.load_data(spectrum_2d=mos_spectrum2d)
+    viewer = specviz2d_helper.app.get_viewer(
+        specviz2d_helper._default_spectrum_2d_viewer_reference_name)
+
+    viewer.apply_roi(XRangeROI(6400, 6600))
+    specviz2d_helper.app.session.edit_subset_mode.mode = OrMode
+    viewer.apply_roi(XRangeROI(7000, 7400))
+
+    viewer.apply_roi(XRangeROI(6600, 7300))
+
+    viewer.apply_roi(XRangeROI(7600, 7800))
+
+    subset_plugin = specviz2d_helper.app.get_tray_item_from_name('g-subset-plugin')
+    assert subset_plugin.can_simplify
+    subset_plugin.vue_simplify_subset()
+
+    reg = specviz2d_helper.app.get_subsets("Subset 1")
+    assert reg[0].lower.value == 6400 and reg[0].upper.value == 7400
+    assert reg[1].lower.value == 7600 and reg[1].upper.value == 7800
```

### Comparing `jdaviz-3.5.0/jdaviz/tests/test_utils.py` & `jdaviz-3.6.0/jdaviz/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/tests/test_viewer_ids.py` & `jdaviz-3.6.0/jdaviz/tests/test_viewer_ids.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/jdaviz/utils.py` & `jdaviz-3.6.0/jdaviz/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 import time
 import threading
 from collections import deque
 
 import matplotlib.pyplot as plt
-
 from astropy.io import fits
 from ipyvue import watch
 from glue.config import settings
+from glue.core.subset import RangeSubsetState, RoiSubsetState
+
 
 __all__ = ['SnackbarQueue', 'enable_hot_reloading', 'bqplot_clear_figure',
-           'standardize_metadata', 'ColorCycler', 'alpha_index']
+           'standardize_metadata', 'ColorCycler', 'alpha_index', 'get_subset_type']
 
 # For Metadata Viewer plugin internal use only.
 PRIHDR_KEY = '_primary_header'
 COMMENTCARD_KEY = '_fits_comment_card'
 
 
 class SnackbarQueue:
@@ -256,7 +257,37 @@
         cycle_index = self.counter % len(self.default_color_palette)
         color = self.default_color_palette[cycle_index]
 
         return color
 
     def reset(self):
         self.counter = -1
+
+
+def get_subset_type(subset):
+    """
+    Determine the subset type of a subset or layer
+
+    Parameters
+    ----------
+    subset : glue.core.subset.Subset or glue.core.subset_group.GroupedSubset
+        should have ``subset_state`` as an attribute, otherwise will return ``None``.
+
+    Returns
+    -------
+    subset_type : str or None
+        'spatial', 'spectral', or None
+    """
+    if not hasattr(subset, 'subset_state'):
+        return None
+
+    while hasattr(subset.subset_state, 'state1'):
+        # this assumes no mixing between spatial and spectral subsets and just
+        # taking the first component (down the hierarchical tree) to determine the type
+        subset = subset.subset_state.state1
+
+    if isinstance(subset.subset_state, RoiSubsetState):
+        return 'spatial'
+    elif isinstance(subset.subset_state, RangeSubsetState):
+        return 'spectral'
+    else:
+        return None
```

### Comparing `jdaviz-3.5.0/jdaviz.egg-info/PKG-INFO` & `jdaviz-3.6.0/jdaviz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: jdaviz
-Version: 3.5.0
+Version: 3.6.0
 Summary: Astronomical data analysis development leveraging the Jupyter platform
-Author-email: JDADF Developers <rosteen@stsci.edu>
+Home-page: https://jdaviz.readthedocs.io/en/latest/
+Author: JDADF Developers
+Author-email: JDADF Developers <help@stsci.edu>
 Project-URL: Homepage, https://jdaviz.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: all
 Provides-Extra: roman
 License-File: LICENSE.rst
 
 .. image:: docs/logos/jdaviz.svg
     :width: 400
     :alt: Jdaviz logo
     :align: center
@@ -89,15 +92,15 @@
 
 ``jdaviz`` provides a command-line tool to start the web application. To see the syntax and usage,
 from a terminal, type:
 
 .. code-block:: bash
 
     jdaviz --help
-    jdaviz specviz /path/to/data/spectral_file
+    jdaviz --layout=specviz /path/to/data/spectral_file
 
 For more information on the command line interfaces for each tool, see the
 `Jdaviz docs <https://jdaviz.readthedocs.io/en/latest/index.html>`_.
 
 
 In a Jupyter Notebook
 +++++++++++++++++++++
```

### Comparing `jdaviz-3.5.0/jdaviz.egg-info/SOURCES.txt` & `jdaviz-3.6.0/jdaviz.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 .bandit.yaml
 .flake8
 .gitignore
+.mailmap
 .readthedocs.yaml
 CHANGES.rst
 CITATION.cff
 CODE_OF_CONDUCT.md
 LICENSE.rst
 MANIFEST.in
 README.rst
 conftest.py
 licenses
 pyproject.toml
+setup.cfg
 setup.py
 tox.ini
 .github/CODEOWNERS
 .github/PULL_REQUEST_TEMPLATE.md
 .github/labeler.yml
 .github/ISSUE_TEMPLATE/bug_report.yaml
 .github/ISSUE_TEMPLATE/config.yml
@@ -22,21 +24,24 @@
 .github/workflows/changelog_check.yml
 .github/workflows/ci_cron_weekly.yml
 .github/workflows/ci_workflows.yml
 .github/workflows/codeql-analysis.yml
 .github/workflows/open_actions.yml
 .github/workflows/predeps_workflows.yml
 .github/workflows/publish.yml
+.github/workflows/standalone.yml
 jdaviz/__init__.py
+jdaviz/_astropy_init.py
 jdaviz/app.py
 jdaviz/app.vue
 jdaviz/cli.py
 jdaviz/conftest.py
 jdaviz/container.vue
 jdaviz/jdaviz_cli.ipynb
+jdaviz/jdaviz_cli_launcher.ipynb
 jdaviz/utils.py
 jdaviz/version.py
 jdaviz.egg-info/PKG-INFO
 jdaviz.egg-info/SOURCES.txt
 jdaviz.egg-info/dependency_links.txt
 jdaviz.egg-info/entry_points.txt
 jdaviz.egg-info/not-zip-safe
@@ -49,27 +54,29 @@
 jdaviz/components/layer_viewer_icon.vue
 jdaviz/components/number_uncertainty.vue
 jdaviz/components/play_pause_widget.vue
 jdaviz/components/plugin_add_results.vue
 jdaviz/components/plugin_auto_label.vue
 jdaviz/components/plugin_dataset_select.vue
 jdaviz/components/plugin_layer_select.vue
+jdaviz/components/plugin_plot.vue
 jdaviz/components/plugin_popout.vue
 jdaviz/components/plugin_section_header.vue
 jdaviz/components/plugin_subset_select.vue
 jdaviz/components/plugin_table.vue
 jdaviz/components/plugin_viewer_select.vue
 jdaviz/components/toolbar_nested.py
 jdaviz/components/toolbar_nested.vue
 jdaviz/components/tooltip.vue
 jdaviz/components/tray_plugin.vue
 jdaviz/components/viewer_data_select.vue
 jdaviz/components/viewer_data_select_item.vue
 jdaviz/configs/__init__.py
 jdaviz/configs/cubeviz/__init__.py
+jdaviz/configs/cubeviz/cubeviz.ipynb
 jdaviz/configs/cubeviz/cubeviz.yaml
 jdaviz/configs/cubeviz/helper.py
 jdaviz/configs/cubeviz/plugins/__init__.py
 jdaviz/configs/cubeviz/plugins/parsers.py
 jdaviz/configs/cubeviz/plugins/tools.py
 jdaviz/configs/cubeviz/plugins/viewers.py
 jdaviz/configs/cubeviz/plugins/moment_maps/__init__.py
@@ -82,18 +89,20 @@
 jdaviz/configs/cubeviz/plugins/slice/slice.vue
 jdaviz/configs/cubeviz/plugins/slice/tests/__init__.py
 jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py
 jdaviz/configs/cubeviz/plugins/tests/__init__.py
 jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py
 jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py
 jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py
+jdaviz/configs/cubeviz/plugins/tests/test_export_plots.py
 jdaviz/configs/cubeviz/plugins/tests/test_parsers.py
 jdaviz/configs/cubeviz/plugins/tests/test_regions.py
 jdaviz/configs/cubeviz/plugins/tests/test_tools.py
 jdaviz/configs/default/__init__.py
+jdaviz/configs/default/default.ipynb
 jdaviz/configs/default/default.yaml
 jdaviz/configs/default/plugins/__init__.py
 jdaviz/configs/default/plugins/viewers.py
 jdaviz/configs/default/plugins/collapse/__init__.py
 jdaviz/configs/default/plugins/collapse/collapse.py
 jdaviz/configs/default/plugins/collapse/collapse.vue
 jdaviz/configs/default/plugins/collapse/tests/__init__.py
@@ -149,14 +158,15 @@
 jdaviz/configs/default/plugins/subset_tools/subset_tools.py
 jdaviz/configs/default/plugins/subset_tools/subset_tools.vue
 jdaviz/configs/default/plugins/viewer_creator/__init__.py
 jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py
 jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue
 jdaviz/configs/imviz/__init__.py
 jdaviz/configs/imviz/helper.py
+jdaviz/configs/imviz/imviz.ipynb
 jdaviz/configs/imviz/imviz.yaml
 jdaviz/configs/imviz/wcs_utils.py
 jdaviz/configs/imviz/plugins/__init__.py
 jdaviz/configs/imviz/plugins/parsers.py
 jdaviz/configs/imviz/plugins/tools.py
 jdaviz/configs/imviz/plugins/viewers.py
 jdaviz/configs/imviz/plugins/aper_phot_simple/__init__.py
@@ -200,37 +210,42 @@
 jdaviz/configs/imviz/tests/test_simple_aper_phot.py
 jdaviz/configs/imviz/tests/test_subset_centroid.py
 jdaviz/configs/imviz/tests/test_tools.py
 jdaviz/configs/imviz/tests/test_viewer_tools.py
 jdaviz/configs/imviz/tests/test_viewers.py
 jdaviz/configs/imviz/tests/test_wcs_utils.py
 jdaviz/configs/imviz/tests/utils.py
+jdaviz/configs/imviz/tests/data/ds9_annulus_01.reg
 jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf
 jdaviz/configs/imviz/tests/data/roman_wfi_image_model.asdf
 jdaviz/configs/mosviz/__init__.py
 jdaviz/configs/mosviz/helper.py
+jdaviz/configs/mosviz/mosviz.ipynb
 jdaviz/configs/mosviz/mosviz.yaml
 jdaviz/configs/mosviz/plugins/__init__.py
 jdaviz/configs/mosviz/plugins/parsers.py
+jdaviz/configs/mosviz/plugins/tools.py
 jdaviz/configs/mosviz/plugins/viewers.py
 jdaviz/configs/mosviz/plugins/row_lock/__init__.py
 jdaviz/configs/mosviz/plugins/row_lock/row_lock.py
 jdaviz/configs/mosviz/plugins/row_lock/row_lock.vue
 jdaviz/configs/mosviz/plugins/slit_overlay/__init__.py
 jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py
 jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.vue
 jdaviz/configs/mosviz/plugins/slit_overlay/tests/__init__.py
 jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py
 jdaviz/configs/mosviz/tests/__init__.py
 jdaviz/configs/mosviz/tests/test_data_loading.py
 jdaviz/configs/mosviz/tests/test_helper.py
 jdaviz/configs/mosviz/tests/test_parsers.py
 jdaviz/configs/mosviz/tests/test_source_identifier_extract.py
+jdaviz/configs/mosviz/tests/test_tools.py
 jdaviz/configs/specviz/__init__.py
 jdaviz/configs/specviz/helper.py
+jdaviz/configs/specviz/specviz.ipynb
 jdaviz/configs/specviz/specviz.yaml
 jdaviz/configs/specviz/plugins/__init__.py
 jdaviz/configs/specviz/plugins/parsers.py
 jdaviz/configs/specviz/plugins/viewers.py
 jdaviz/configs/specviz/plugins/line_analysis/__init__.py
 jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py
 jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue
@@ -261,62 +276,70 @@
 jdaviz/core/astrowidgets_api.py
 jdaviz/core/config.py
 jdaviz/core/custom_traitlets.py
 jdaviz/core/data_formats.py
 jdaviz/core/events.py
 jdaviz/core/freezable_state.py
 jdaviz/core/helpers.py
+jdaviz/core/launcher.py
 jdaviz/core/linelists.py
 jdaviz/core/marks.py
 jdaviz/core/region_translators.py
 jdaviz/core/registries.py
 jdaviz/core/style_widget.py
 jdaviz/core/template_mixin.py
 jdaviz/core/tools.py
 jdaviz/core/user_api.py
 jdaviz/core/validunits.py
 jdaviz/core/tests/__init__.py
+jdaviz/core/tests/test_autoconfig.py
 jdaviz/core/tests/test_custom_traitlets.py
 jdaviz/core/tests/test_data_menu.py
 jdaviz/core/tests/test_helpers.py
 jdaviz/core/tests/test_region_translators.py
 jdaviz/core/tests/test_template_mixin.py
 jdaviz/core/tests/test_tools.py
 jdaviz/data/icons/blink.svg
 jdaviz/data/icons/checktoradial.svg
 jdaviz/data/icons/compass.svg
 jdaviz/data/icons/contrast.svg
 jdaviz/data/icons/home.svg
+jdaviz/data/icons/home_match.svg
 jdaviz/data/icons/image.svg
 jdaviz/data/icons/left-east.svg
 jdaviz/data/icons/line_select.svg
 jdaviz/data/icons/line_select_disabled.svg
 jdaviz/data/icons/pan.svg
 jdaviz/data/icons/pan2.svg
 jdaviz/data/icons/pan_x.svg
+jdaviz/data/icons/pan_x_match.svg
 jdaviz/data/icons/pan_y.svg
+jdaviz/data/icons/pan_y_match.svg
 jdaviz/data/icons/panzoom_match.svg
 jdaviz/data/icons/pixelspectra.svg
 jdaviz/data/icons/radialtocheck.svg
 jdaviz/data/icons/right-east.svg
+jdaviz/data/icons/select_annulus.svg
 jdaviz/data/icons/select_circle.svg
 jdaviz/data/icons/select_ellipse.svg
 jdaviz/data/icons/select_lasso.svg
 jdaviz/data/icons/select_single_pixel.svg
 jdaviz/data/icons/select_x.svg
 jdaviz/data/icons/select_xy.svg
 jdaviz/data/icons/select_y.svg
 jdaviz/data/icons/slice.svg
 jdaviz/data/icons/spectral_range.svg
 jdaviz/data/icons/tune.svg
 jdaviz/data/icons/zoom_back.svg
 jdaviz/data/icons/zoom_box.svg
 jdaviz/data/icons/zoom_box_match.svg
 jdaviz/data/icons/zoom_xrange.svg
+jdaviz/data/icons/zoom_xrange_match.svg
 jdaviz/data/icons/zoom_yrange.svg
+jdaviz/data/icons/zoom_yrange_match.svg
 jdaviz/data/linelists/Atomic-ISO.csv
 jdaviz/data/linelists/Atomic-Ionic.csv
 jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv
 jdaviz/data/linelists/CO-band-heads.csv
 jdaviz/data/linelists/CO.csv
 jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv
 jdaviz/data/linelists/Common_Galactic_700A-2000A.csv
@@ -379,17 +402,32 @@
 notebooks/concepts/mosviz_concept.ipynb
 notebooks/concepts/mosviz_generate_photometry.ipynb
 notebooks/concepts/mosviz_niriss_parser.ipynb
 notebooks/concepts/mosviz_overplot_slit.ipynb
 notebooks/concepts/pypi_metrics.ipynb
 notebooks/concepts/specviz_from_list.ipynb
 notebooks/concepts/specviz_from_splot.ipynb
+notebooks/concepts/specviz_glue_unit_conversion.ipynb
 notebooks/concepts/specviz_line_lists.ipynb
 notebooks/concepts/specviz_minimal.ipynb
 notebooks/concepts/specviz_spectrum_list.ipynb
-notebooks/concepts/specviz_unit_conversion.ipynb
 share/jupyter/nbconvert/templates/jdaviz-default/ansi.js
 share/jupyter/nbconvert/templates/jdaviz-default/app.html
 share/jupyter/nbconvert/templates/jdaviz-default/conf.json
 share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2
 share/jupyter/nbconvert/templates/jdaviz-default/util.js
-share/jupyter/voila/templates/jdaviz-default/index.html.j2
+share/jupyter/voila/templates/jdaviz-default/index.html.j2
+standalone/entitlements.plist
+standalone/jdaviz-cli-entrypoint.py
+standalone/jdaviz.spec
+standalone/test.py
+standalone/hooks/hook-bqplot.py
+standalone/hooks/hook-debugpy.py
+standalone/hooks/hook-glue.py
+standalone/hooks/hook-glue_jupyter.py
+standalone/hooks/hook-ipypopout.py
+standalone/hooks/hook-jdaviz.py
+standalone/hooks/hook-jupyter_client.py
+standalone/hooks/hook-mistune.py
+standalone/hooks/hook-photutils.py
+standalone/hooks/hook-regions.py
+standalone/hooks/hook-skimage.py
```

### Comparing `jdaviz-3.5.0/jdaviz.egg-info/requires.txt` & `jdaviz-3.6.0/jdaviz.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 packaging
 astropy>=4.3
 matplotlib
 traitlets>=5.0.5
 bqplot>=0.12.37
 bqplot-image-gl>=1.4.11
-glue-core!=1.10,!=1.9.0,>=1.6.0
-glue-jupyter>=0.15.0
+glue-core>=1.11
+glue-jupyter>=0.17
 echo>=0.5.0
 ipykernel>=6.19.4
 ipyvue>=1.6
 ipyvuetify>=1.7.0
 ipysplitpanes>=0.1.0
 ipygoldenlayout>=0.3.0
 ipywidgets>=8.0.6
-voila>=0.4
+voila<0.5,>=0.4
 pyyaml>=5.4.1
 specutils>=1.9
 specreduce<1.4.0,>=1.3.0
 photutils>=1.4
-glue-astronomy>=0.7
+glue-astronomy>=0.10
 asteval>=0.9.23
 idna
 vispy>=0.6.5
 asdf>=2.14.3
 stdatamodels>=1.3
 gwcs>=0.16.1
 regions>=0.6
@@ -30,21 +30,21 @@
 sidecar>=0.5.2
 ipypopout>=0.0.11
 astroquery
 
 [:python_version == "3.9"]
 y_py<0.5.5
 
-[docs]
-sphinx-rtd-theme
-sphinx-astropy
+[all]
+opencv-python
 
-[docs:python_version < "3.11"]
-tomli
+[docs]
+sphinx-astropy[confv2]>=1.9.1
+sphinx_design
 
 [roman]
-roman_datamodels>=0.14.2
+roman_datamodels>=0.16.1
 
 [test]
 pytest
 pytest-astropy
 pytest-tornasync
```

### Comparing `jdaviz-3.5.0/licenses/GINGA_LICENSE.txt` & `jdaviz-3.6.0/licenses/GINGA_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/licenses/IMEXAM_LICENSE.txt` & `jdaviz-3.6.0/licenses/IMEXAM_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/licenses/IPYFILECHOOSER_LICENSE.rst` & `jdaviz-3.6.0/licenses/IPYFILECHOOSER_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/licenses/TEMPLATE_LICENCE.rst` & `jdaviz-3.6.0/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/CubevizExample.ipynb` & `jdaviz-3.6.0/notebooks/CubevizExample.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9911390692640693%*

 * *Differences: {"'cells'": '{15: {\'source\': ["data = '*

 * *            'cubeviz.get_data(\'jw02732-o004_t004_miri_ch1-shortmediumlong_s3d.fits[SCI]\')"]}, '*

 * *            "18: {'source': {insert: [(0, 'spectra_dict = "*

 * *            "cubeviz.specviz.get_spectra(apply_slider_redshift=True)\\n')], delete: [0]}}, insert: "*

 * *            "[(7, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), ('source', "*

 * *            '["Alternatively, the data and the configuration can be autodetected and loaded '*

 * *            'simu […]*

```diff
@@ -85,14 +85,21 @@
                 "    cubeviz.load_data(f'{data_dir}/{fn}')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "Alternatively, the data and the configuration can be autodetected and loaded simultaneously by calling `jdaviz.open(f'{data_dir}/{fn}')`"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "The upper left viewer containing the FLUX cube is the default viewer that is accessible as follows."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -144,15 +151,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "data = cubeviz.app.get_data_from_viewer('flux-viewer', 'contents[FLUX]')"
+                "data = cubeviz.get_data('jw02732-o004_t004_miri_ch1-shortmediumlong_s3d.fits[SCI]')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -176,15 +183,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "spectra_dict = cubeviz.specviz.get_spectra()\n",
+                "spectra_dict = cubeviz.specviz.get_spectra(apply_slider_redshift=True)\n",
                 "spectra_dict"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -221,13 +228,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.8"
+            "version": "3.10.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `jdaviz-3.5.0/notebooks/ImvizDitheredExample.ipynb` & `jdaviz-3.6.0/notebooks/ImvizDitheredExample.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998397435897436%*

 * *Differences: {"'cells'": '{30: {\'source\': ["data = imviz.get_data(\'acs_47tuc_1[SCI,1]\')"]}}'}*

```diff
@@ -297,15 +297,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "0a4e02ef",
             "metadata": {},
             "outputs": [],
             "source": [
-                "data = imviz.app.get_data_from_viewer('imviz-0', 'acs_47tuc_1[SCI,1]')"
+                "data = imviz.get_data('acs_47tuc_1[SCI,1]')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "164a1a40",
             "metadata": {},
```

### Comparing `jdaviz-3.5.0/notebooks/ImvizExample.ipynb` & `jdaviz-3.6.0/notebooks/ImvizExample.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9956519717261905%*

 * *Differences: {"'cells'": '{31: {\'source\': ["data = '*

 * *            'imviz.get_data(\'jw02727-o002_t062_nircam_clear-f090w_i2d[DATA]\')"]}, insert: [(11, '*

 * *            "OrderedDict([('cell_type', 'markdown'), ('id', '99d4bdef'), ('metadata', "*

 * *            'OrderedDict()), (\'source\', ["Alternatively, the data and the configuration can be '*

 * *            'autodetected and loaded simultaneously by calling '*

 * *            '`jdaviz.open(f\'{data_dir}/{fn}\')`"])]))]}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.10'}}"}*

```diff
@@ -150,14 +150,22 @@
             "outputs": [],
             "source": [
                 "imviz.show()"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "99d4bdef",
+            "metadata": {},
+            "source": [
+                "Alternatively, the data and the configuration can be autodetected and loaded simultaneously by calling `jdaviz.open(f'{data_dir}/{fn}')`"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "3e78efeb",
             "metadata": {},
             "source": [
                 "The first thing you will probably notice is that the image doesn't take up the entire viewer area. \n",
                 "If you press the \"b\" key to blink to the other loaded image, you will see that this image is \n",
                 "zoomed correctly by default. The odd default zoom on the other is because the images are linked\n",
                 "by pixel when loaded. We can instead link by WCS (world coordinates) so that the images\n",
@@ -336,15 +344,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "0a4e02ef",
             "metadata": {},
             "outputs": [],
             "source": [
-                "data = imviz.app.get_data_from_viewer('imviz-0', 'jw02727-o002_t062_nircam_clear-f090w_i2d[DATA]')"
+                "data = imviz.get_data('jw02727-o002_t062_nircam_clear-f090w_i2d[DATA]')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "164a1a40",
             "metadata": {},
@@ -716,13 +724,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.10.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `jdaviz-3.5.0/notebooks/MosvizExample.ipynb` & `jdaviz-3.6.0/notebooks/MosvizExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/MosvizNIRISSExample.ipynb` & `jdaviz-3.6.0/notebooks/MosvizNIRISSExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/Specviz2dExample.ipynb` & `jdaviz-3.6.0/notebooks/Specviz2dExample.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9838789682539683%*

 * *Differences: {"'cells'": "{insert: [(8, OrderedDict([('cell_type', 'markdown'), ('id', '795bc520'), "*

 * *            '(\'metadata\', OrderedDict()), (\'source\', ["Alternatively, the data and the '*

 * *            'configuration can be autodetected and loaded simultaneously by calling '*

 * *            '`jdaviz.open(f\'{data_dir}/{fn}\')`"])]))]}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.10'}}"}*

```diff
@@ -92,14 +92,22 @@
             "execution_count": null,
             "id": "ec94837b",
             "metadata": {},
             "outputs": [],
             "source": [
                 "specviz2d.load_data(f'{data_dir}/{fn}')"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "795bc520",
+            "metadata": {},
+            "source": [
+                "Alternatively, the data and the configuration can be autodetected and loaded simultaneously by calling `jdaviz.open(f'{data_dir}/{fn}')`"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -110,13 +118,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.10.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `jdaviz-3.5.0/notebooks/SpecvizExample.ipynb` & `jdaviz-3.6.0/notebooks/SpecvizExample.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9898809523809524%*

 * *Differences: {"'cells'": "{1: {'metadata': {replace: OrderedDict([('tags', [])])}}, 3: {'metadata': {replace: "*

 * *            "OrderedDict([('tags', [])])}}, 6: {'metadata': {replace: OrderedDict([('tags', "*

 * *            "[])])}}, 8: {'metadata': {replace: OrderedDict([('tags', [])])}}, 11: {'metadata': "*

 * *            "{replace: OrderedDict([('tags', [])])}, 'source': {insert: [(1, "*

 * *            '"specviz.get_data(data_label=\'myfile\', spectral_subset=\'Subset 1\')")], delete: '*

 * *            "[1]}}, 13: {'metadata': {replac […]*

```diff
@@ -9,15 +9,17 @@
                 "\n",
                 "## Setup"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "import warnings\n",
                 "import tempfile\n",
                 "\n",
                 "import astropy.units as u\n",
                 "from astroquery.mast import Observations\n",
@@ -33,15 +35,17 @@
             "source": [
                 "## Create Specviz via Helper"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "from jdaviz import Specviz\n",
                 "specviz = Specviz()"
             ]
         },
         {
@@ -59,15 +63,17 @@
             "source": [
                 "This will show Specviz inline in the notebook"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "specviz.show()"
             ]
         },
         {
             "cell_type": "markdown",
@@ -87,15 +93,17 @@
                 "version. You can turn off caching by setting `cache=False` in the `download_file` call to\n",
                 "force it to re-download the file if desired."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "data_dir = tempfile.gettempdir()\n",
                 "#data_dir = \"/User/username/Data/\"\n",
                 "\n",
                 "fn = \"jw02732-o004_t004_miri_ch1-shortmediumlong_x1d.fits\"\n",
                 "result = Observations.download_file(f\"mast:JWST/product/{fn}\", local_path=f'{data_dir}/{fn}')\n",
@@ -103,44 +111,55 @@
                 "specviz.load_spectrum(f'{data_dir}/{fn}', \"myfile\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "Alternatively, the data and the configuration can be autodetected and loaded simultaneously by calling `jdaviz.open(f'{data_dir}/{fn}')`"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## Subset Retrieval\n",
                 "User Task: Select a subset in the viewer above\n",
                 "\n",
                 "After defining regions in your spectra, you can retrieve your subsets through different means. To retrieve your subset by name:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "# Returns a version of the whole spectra, with a mask applied\n",
-                "specviz.get_spectra(data_label='myfile', subset_to_apply='Subset 1')"
+                "specviz.get_data(data_label='myfile', spectral_subset='Subset 1')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Or, if you've defined multiple regions, you can retrieve all defined regions/subsets via:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
-                "specviz.app.get_subsets_from_viewer('spectrum-viewer')"
+                "specviz.get_spectra()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Screenshot Saving"
@@ -277,13 +296,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.8"
+            "version": "3.10.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `jdaviz-3.5.0/notebooks/concepts/cubeviz_contour_overlay.ipynb` & `jdaviz-3.6.0/notebooks/concepts/cubeviz_contour_overlay.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/cubeviz_data_interactions.ipynb` & `jdaviz-3.6.0/notebooks/concepts/cubeviz_data_interactions.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999465811965812%*

 * *Differences: {"'cells'": '{12: {\'source\': {insert: [(2, "spec_data = '*

 * *            'app.get_viewer(\'spectrum-viewer\').data()\\n")], delete: [2]}}, 14: {\'source\': '*

 * *            '{insert: [(0, "spec = '*

 * *            "app._jdaviz_helper.get_data('6de4c8ee5659e87a302e3de595074ba5[FLUX]', "*

 * *            'function=\'sum\')\\n")], delete: [0]}}, 24: {\'source\': {insert: [(3, "image_data = '*

 * *            'app.get_viewer(\'flux-viewer\').data()[0]\\n")], delete: [3]}}}'}*

```diff
@@ -145,15 +145,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from specutils import Spectrum1D\n",
                 "\n",
-                "spec_data = app.get_data_from_viewer('spectrum-viewer')\n",
+                "spec_data = app.get_viewer('spectrum-viewer').data()\n",
                 "\n",
                 "# The returned data from `get_data` is in list format, as it's \n",
                 "# possible for there to be several data plotted in the viewer\n",
                 "spec = spec_data[0]\n",
                 "spec"
             ]
         },
@@ -166,15 +166,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "spec = app.get_data_from_viewer('spectrum-viewer', '6de4c8ee5659e87a302e3de595074ba5[FLUX]')\n",
+                "spec = app._jdaviz_helper.get_data('6de4c8ee5659e87a302e3de595074ba5[FLUX]', function='sum')\n",
                 "spec"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -263,15 +263,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import matplotlib.pyplot as plt\n",
                 "\n",
                 "# The returned data object is a `CCData` class to represent the 2D nature of the image data.\n",
-                "image_data = app.get_data_from_viewer('flux-viewer')\n",
+                "image_data = app.get_viewer('flux-viewer').data()[0]\n",
                 "\n",
                 "f, ax = plt.subplots()\n",
                 "\n",
                 "ax.imshow(image_data[0], origin='center')"
             ]
         },
         {
```

### Comparing `jdaviz-3.5.0/notebooks/concepts/cubeviz_fitting.ipynb` & `jdaviz-3.6.0/notebooks/concepts/cubeviz_fitting.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/cubeviz_ndarray_gif.ipynb` & `jdaviz-3.6.0/notebooks/concepts/imviz_load_3d_slices.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9640830592105263%*

 * *Differences: {"'cells'": "{0: {'id': '852e11d6', 'source': {insert: [(0, '# Imviz: Load 3D cube as 2D "*

 * *            "slices\\n'), (2, 'This showcases how Imviz can load 3D cube as 2D slices at "*

 * *            "`axis=0`.')], delete: [5, 4, 2, 1, 0]}}, 1: {'id': '662e9783', 'source': ['import "*

 * *            "numpy as np\\n', '\\n', 'from jdaviz import Imviz']}, 2: {'id': 'e2e74c3a', 'source': "*

 * *            "['# Generate the cube.\\n', 'arr = np.stack([np.random.random((10, 10)) for _ in "*

 * *            "range(5)])\\n', 'arr.sh […]*

```diff
@@ -1,193 +1,211 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "f07603dd",
+            "id": "852e11d6",
             "metadata": {},
             "source": [
-                "# Cubeviz with Numpy Cube and GIF\n",
+                "# Imviz: Load 3D cube as 2D slices\n",
                 "\n",
-                "This concept notebook shows Cubeviz loading:\n",
-                "\n",
-                "  * plain Numpy array, and\n",
-                "  * GIF animation as a playable cube"
+                "This showcases how Imviz can load 3D cube as 2D slices at `axis=0`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0adf0be6",
+            "id": "662e9783",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from jdaviz import Cubeviz"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "3bd69931",
-            "metadata": {},
-            "source": [
-                "## From array\n",
-                "\n",
-                "For `flux-viewer`, `(0, 0)` of first slice should have value of zero and should be at bottom left. Cubeviz requires the input cube to have axes order of `(x, y, z)`.\n",
+                "import numpy as np\n",
                 "\n",
-                "For `uncert-viewer`, the values are all random."
+                "from jdaviz import Imviz"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5fb6ab3e",
+            "id": "e2e74c3a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import numpy as np"
+                "# Generate the cube.\n",
+                "arr = np.stack([np.random.random((10, 10)) for _ in range(5)])\n",
+                "arr.shape"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b52e2b0c",
+            "id": "e75f616e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "a = np.arange(5 * 8 * 10).reshape((8, 5, 10))  # x, y, z\n",
-                "b = np.random.random(a.shape)"
+                "imviz = Imviz()\n",
+                "imviz.load_data(arr, data_label='my_slices')\n",
+                "imviz.show()"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "385d69c9",
+            "cell_type": "markdown",
+            "id": "05c24b87",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "cubeviz = Cubeviz()"
+                "## You can also load it one slice at a time..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3cd294b2",
+            "id": "b07b7fd2",
             "metadata": {},
             "outputs": [],
             "source": [
-                "cubeviz.load_data(a, data_label='ordered')\n",
-                "cubeviz.load_data(b, data_label='random', data_type='uncert', override_cube_limit=True)"
+                "imviz2 = Imviz()\n",
+                "imviz2.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d088e647",
+            "id": "d38aa230",
             "metadata": {},
             "outputs": [],
             "source": [
-                "cubeviz.show()"
+                "with imviz2.batch_load():\n",
+                "    for i in range(arr.shape[0]):\n",
+                "        data = arr[i, :, :]\n",
+                "        imviz2.load_data(data, data_label=f'a_{i}')"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "65427228",
+            "id": "11626756",
             "metadata": {},
             "source": [
-                "### But what about roundtripping?"
+                "## This is not Cubeviz, so...\n",
+                "\n",
+                "You have to plot the line profile manually, as follows."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "873089bb",
+            "id": "fa2ede51",
             "metadata": {},
             "outputs": [],
             "source": [
-                "data = cubeviz.app.get_data_from_viewer('flux-viewer', 'ordered')\n",
-                "orig_cube = data.get_object(statistic=None)\n",
-                "orig_cube.shape  # Input was (8, 5, 10)  # x, y, z"
+                "import matplotlib.pyplot as plt\n",
+                "\n",
+                "%matplotlib inline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "dfe43427",
+            "id": "f18e7353",
             "metadata": {},
             "outputs": [],
             "source": [
-                "cubeviz.load_data(orig_cube.flux.value * 0.1, \"roundtrip_test\", override_cube_limit=True)"
+                "collapsed_mean = arr.mean(axis=(1, 2))\n",
+                "collapsed_mean.shape"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1f7e9209",
+            "id": "0ea2c32e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "data_2 = cubeviz.app.get_data_from_viewer('flux-viewer', 'roundtrip_test')\n",
-                "data_2.shape"
+                "plt.plot(collapsed_mean, '-o')\n",
+                "plt.title('Mean across slices')\n",
+                "plt.xlabel('Slice index')\n",
+                "plt.ylabel('Value');"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "014f2ab7",
+            "id": "8b692944-ec27-4e72-9601-114ba040f6e7",
             "metadata": {},
             "source": [
-                "## From GIF\n",
+                "## What else can you do doo doo doo doo?\n",
                 "\n",
-                "The GIF is from https://media4.giphy.com/media/J5pnZ53pj4cmu30Rx5/giphy.gif. This needs `imageio` and Pillow to be installed as well."
+                "This requires `PIL` package to be installed."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "e8d9092e-86c3-489d-b48c-e103d276eae0",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from astropy.utils.data import download_file\n",
+                "from PIL import Image, ImageSequence\n",
+                "from skimage.color import rgb2gray"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fab04442",
+            "id": "006260b6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "filename = 'baby_shark.gif'"
+                "imviz3 = Imviz()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c89c8d5f",
+            "id": "1f01e094-785d-4a15-a90b-b65e10d69fff",
             "metadata": {},
             "outputs": [],
             "source": [
-                "cubeviz2 = Cubeviz()"
+                "gif_file = download_file('https://media4.giphy.com/media/J5pnZ53pj4cmu30Rx5/giphy.gif', cache=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "137fdde0",
+            "id": "ce2667c4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "cubeviz2.load_data(filename)"
+                "im = Image.open(gif_file)\n",
+                "i = 0\n",
+                "\n",
+                "with imviz3.batch_load():\n",
+                "    for frame in ImageSequence.Iterator(im):\n",
+                "        if i % 10 != 0:  # Skip some\n",
+                "            i += 1\n",
+                "            continue\n",
+                "        data = np.asarray(frame)[::-1, :]\n",
+                "        if data.ndim == 3:\n",
+                "            data = rgb2gray(data)\n",
+                "        imviz3.load_data(data, data_label=f'frame_{i}', do_link=False)\n",
+                "        i += 1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ab4eca75",
-            "metadata": {
-                "scrolled": false
-            },
+            "id": "fb573f18-970b-4555-9ca7-4156b99a7b57",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "cubeviz2.show()"
+                "imviz3.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4d1af33f",
+            "id": "7f408020",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `jdaviz-3.5.0/notebooks/concepts/cubeviz_spectral_fitting.ipynb` & `jdaviz-3.6.0/notebooks/concepts/cubeviz_spectral_fitting.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb` & `jdaviz-3.6.0/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb` & `jdaviz-3.6.0/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb` & `jdaviz-3.6.0/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998148148148148%*

 * *Differences: {"'cells'": '{26: {\'source\': {insert: [(1, "app.get_viewer(\'image-viewer\').data()")], delete: '*

 * *            '[1]}}}'}*

```diff
@@ -276,15 +276,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# can I access the data back out? \n",
-                "app.get_data_from_viewer('image-viewer')"
+                "app.get_viewer('image-viewer').data()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Option 2 - Create the viewer programmatically and also load some data\n",
```

### Comparing `jdaviz-3.5.0/notebooks/concepts/imviz_color_display.ipynb` & `jdaviz-3.6.0/notebooks/concepts/imviz_color_display.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/imviz_compass_mpl.ipynb` & `jdaviz-3.6.0/notebooks/concepts/imviz_compass_mpl.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/imviz_custom_colormap.ipynb` & `jdaviz-3.6.0/notebooks/concepts/imviz_custom_colormap.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/imviz_dithered_gwcs.ipynb` & `jdaviz-3.6.0/notebooks/concepts/imviz_dithered_gwcs.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/imviz_edit_subset_programmatic.ipynb` & `jdaviz-3.6.0/notebooks/concepts/imviz_edit_subset_programmatic.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/imviz_line_profiles.ipynb` & `jdaviz-3.6.0/notebooks/concepts/imviz_line_profiles.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/imviz_load_3d_slices.ipynb` & `jdaviz-3.6.0/notebooks/concepts/imviz_load_fits_hdu.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9604745370370371%*

 * *Differences: {"'cells'": "{0: {'id': '5164a543-c0cc-406a-a698-3a6a7477c43d', 'source': ['# Loading individual "*

 * *            "HDUs with Imviz']}, 1: {'id': '76247920-501d-4085-a2ec-67ed2a29a347', 'source': "*

 * *            "{insert: [(0, 'from astropy.io import fits\\n'), (1, 'from astropy.utils.data import "*

 * *            "download_file\\n')], delete: [0]}}, 2: {'id': '1a214c0e-ddec-41b4-a289-3d1dbe975f64', "*

 * *            '\'source\': ["jwf277w = '*

 * *            "download_file('https://stsci.box.com/shared/static/iao1zxtigyrhq7 […]*

```diff
@@ -1,214 +1,179 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "852e11d6",
+            "id": "5164a543-c0cc-406a-a698-3a6a7477c43d",
             "metadata": {},
             "source": [
-                "# Imviz: Load 3D cube as 2D slices\n",
-                "\n",
-                "This showcases how Imviz can load 3D cube as 2D slices at `axis=0`."
+                "# Loading individual HDUs with Imviz"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "662e9783",
+            "id": "76247920-501d-4085-a2ec-67ed2a29a347",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import numpy as np\n",
+                "from astropy.io import fits\n",
+                "from astropy.utils.data import download_file\n",
                 "\n",
                 "from jdaviz import Imviz"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e2e74c3a",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# Generate the cube.\n",
-                "arr = np.stack([np.random.random((10, 10)) for _ in range(5)])\n",
-                "arr.shape"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "e75f616e",
+            "id": "1a214c0e-ddec-41b4-a289-3d1dbe975f64",
             "metadata": {},
             "outputs": [],
             "source": [
-                "imviz = Imviz()\n",
-                "imviz.load_data(arr, data_label='my_slices')\n",
-                "imviz.show()"
+                "jwf277w = download_file('https://stsci.box.com/shared/static/iao1zxtigyrhq7k3wtu5nchrxzlhj9kv.fits', cache=True)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "05c24b87",
+            "id": "2004d08e-9056-4cd4-a77e-bd0d6a4e8eb3",
             "metadata": {},
             "source": [
-                "## You can also load it one slice at a time..."
+                "FITS info would show this:\n",
+                "\n",
+                "    No.    Name      Ver    Type      Cards   Dimensions   Format\n",
+                "      0  PRIMARY       1 PrimaryHDU     263   ()\n",
+                "      1  SCI           1 ImageHDU        85   (2048, 2048)   float32\n",
+                "      2  ERR           1 ImageHDU        10   (2048, 2048)   float32\n",
+                "      3  DQ            1 ImageHDU        11   (2048, 2048)   int32 (rescales to uint32)\n",
+                "      ..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b07b7fd2",
+            "id": "d375cdcf-1930-4ef0-a693-fa33436abf3d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "imviz2 = Imviz()\n",
-                "imviz2.show()"
+                "pf = fits.open(jwf277w)\n",
+                "pf.info()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d38aa230",
+            "id": "254e547f-a7f1-4a3c-913c-3674b7ac93da",
             "metadata": {},
             "outputs": [],
             "source": [
-                "with imviz2.batch_load():\n",
-                "    for i in range(arr.shape[0]):\n",
-                "        data = arr[i, :, :]\n",
-                "        imviz2.load_data(data, data_label=f'a_{i}')"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "11626756",
-            "metadata": {},
-            "source": [
-                "## This is not Cubeviz, so...\n",
-                "\n",
-                "You have to plot the line profile manually, as follows."
+                "imviz = Imviz()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fa2ede51",
+            "id": "28c4f536",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import matplotlib.pyplot as plt\n",
-                "\n",
-                "%matplotlib inline"
+                "# This is the recommended way and you will get GWCS from\n",
+                "# the ASDF extension for all the loaded HDUs.\n",
+                "imviz.load_data(jwf277w, ext=('SCI', 1))\n",
+                "imviz.load_data(jwf277w, ext=('ERR', 1))\n",
+                "imviz.load_data(jwf277w, ext=('DQ', 1))"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "f18e7353",
+            "cell_type": "raw",
+            "id": "0e8a5744",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "collapsed_mean = arr.mean(axis=(1, 2))\n",
-                "collapsed_mean.shape"
+                "# If you must load HDU objects themselves individually, you will\n",
+                "# only get WCS if it is in the immediate FITS header.\n",
+                "imviz.load_data(pf[1], data_label='ext_1')\n",
+                "imviz.load_data(pf[2], data_label='ext_2')\n",
+                "imviz.load_data(pf[3], data_label='ext_3')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0ea2c32e",
+            "id": "ffba41b3-b843-441b-aa3e-7d8efc9bc7a5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "plt.plot(collapsed_mean, '-o')\n",
-                "plt.title('Mean across slices')\n",
-                "plt.xlabel('Slice index')\n",
-                "plt.ylabel('Value');"
+                "imviz.show()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "8b692944-ec27-4e72-9601-114ba040f6e7",
+            "id": "7dddb1d6",
             "metadata": {},
             "source": [
-                "## What else can you do doo doo doo doo?\n",
+                "To programmatically control Plot Options so you can set some stuff for all data at once, see https://jdaviz.readthedocs.io/en/latest/api/jdaviz.configs.default.plugins.plot_options.plot_options.PlotOptions.html.\n",
                 "\n",
-                "This requires `PIL` package to be installed."
+                "The example below sets the same colormap for all images."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e8d9092e-86c3-489d-b48c-e103d276eae0",
+            "id": "436974df",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from astropy.utils.data import download_file\n",
-                "from PIL import Image, ImageSequence\n",
-                "from skimage.color import rgb2gray"
+                "plot_options = imviz.plugins['Plot Options']"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "006260b6",
+            "id": "2b1d2bdf",
             "metadata": {},
             "outputs": [],
             "source": [
-                "imviz3 = Imviz()"
+                "dir(plot_options)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1f01e094-785d-4a15-a90b-b65e10d69fff",
+            "id": "dabf30e4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "gif_file = download_file('https://media4.giphy.com/media/J5pnZ53pj4cmu30Rx5/giphy.gif', cache=True)"
+                "plot_options.select_all()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ce2667c4",
+            "id": "a57719f5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "im = Image.open(gif_file)\n",
-                "i = 0\n",
-                "\n",
-                "with imviz3.batch_load():\n",
-                "    for frame in ImageSequence.Iterator(im):\n",
-                "        if i % 10 != 0:  # Skip some\n",
-                "            i += 1\n",
-                "            continue\n",
-                "        data = np.asarray(frame)[::-1, :]\n",
-                "        if data.ndim == 3:\n",
-                "            data = rgb2gray(data)\n",
-                "        imviz3.load_data(data, data_label=f'frame_{i}', do_link=False)\n",
-                "        i += 1"
+                "plot_options.image_colormap = 'Viridis'"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "fb573f18-970b-4555-9ca7-4156b99a7b57",
+            "cell_type": "markdown",
+            "id": "b1cce96a",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "imviz3.show()"
+                "Close the FITS file pointer when you are done with this notebook."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7f408020",
+            "id": "cf112d5f-e10a-420e-9144-d8883d8dc2cf",
             "metadata": {},
             "outputs": [],
-            "source": []
+            "source": [
+                "pf.close()"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `jdaviz-3.5.0/notebooks/concepts/imviz_load_fits_hdu.ipynb` & `jdaviz-3.6.0/notebooks/concepts/specviz_line_lists.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8119334539371303%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict([('scrolled', False)])}, 'source': {insert: "*

 * *            "[(0, '#from jdaviz.app import Application\\n'), (1, 'from jdaviz import Specviz\\n'), "*

 * *            '(3, "#app = Application(configuration=\'cubeviz\')\\n"), (4, \'specviz = '*

 * *            "Specviz()\\n'), (5, 'specviz.show()')], delete: [3, 1, 0]}, delete: ['id']}, 1: "*

 * *            "{'metadata': {replace: OrderedDict([('scrolled', False)])}, 'source': ['from "*

 * *            "astropy.utils.data import […]*

```diff
@@ -1,196 +1,186 @@
 {
     "cells": [
         {
-            "cell_type": "markdown",
-            "id": "5164a543-c0cc-406a-a698-3a6a7477c43d",
-            "metadata": {},
-            "source": [
-                "# Loading individual HDUs with Imviz"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
-            "id": "76247920-501d-4085-a2ec-67ed2a29a347",
-            "metadata": {},
+            "metadata": {
+                "scrolled": false
+            },
             "outputs": [],
             "source": [
-                "from astropy.io import fits\n",
-                "from astropy.utils.data import download_file\n",
+                "#from jdaviz.app import Application\n",
+                "from jdaviz import Specviz\n",
                 "\n",
-                "from jdaviz import Imviz"
+                "#app = Application(configuration='cubeviz')\n",
+                "specviz = Specviz()\n",
+                "specviz.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1a214c0e-ddec-41b4-a289-3d1dbe975f64",
-            "metadata": {},
+            "metadata": {
+                "scrolled": false
+            },
             "outputs": [],
             "source": [
-                "jwf277w = download_file('https://stsci.box.com/shared/static/iao1zxtigyrhq7k3wtu5nchrxzlhj9kv.fits', cache=True)"
+                "from astropy.utils.data import download_file\n",
+                "\n",
+                "# This file is originally from https://data.sdss.org/sas/dr14/manga/spectro/redux/v2_1_2/7495/stack/manga-7495-12704-LOGCUBE.fits.gz\n",
+                "# but has been modified to correct some inconsistencies in the way units are parsed\n",
+                "fn = download_file('https://stsci.box.com/shared/static/28a88k1qfipo4yxc4p4d40v4axtlal8y.fits', cache=True)\n",
+                "specviz.app.load_data(fn)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2004d08e-9056-4cd4-a77e-bd0d6a4e8eb3",
             "metadata": {},
             "source": [
-                "FITS info would show this:\n",
+                "### Adding line lists via code in cells\n",
                 "\n",
-                "    No.    Name      Ver    Type      Cards   Dimensions   Format\n",
-                "      0  PRIMARY       1 PrimaryHDU     263   ()\n",
-                "      1  SCI           1 ImageHDU        85   (2048, 2048)   float32\n",
-                "      2  ERR           1 ImageHDU        10   (2048, 2048)   float32\n",
-                "      3  DQ            1 ImageHDU        11   (2048, 2048)   int32 (rescales to uint32)\n",
-                "      ..."
+                "Line lists are expected to be input as an astropy `QTable`, with at minimum \"linename\" and \"rest\" fields. The user can optionally specify a \"color\" column if they want each line to be a different color. \n",
+                "\n",
+                "The first step is to load the line list into the specviz instance using `specviz.load_line_list(lines)`. A line list as described as above is required, and there is an optional `replace` parameter that, if set to True, replaces any existing lines with those input. The default behavior is to add newly loaded lines to the existing list.\n",
+                "\n",
+                "Note that the line list functionality is all actually happening under the hood in the spectrum viewer (and thus could also be used in e.g. Cubeviz); the Specviz methods are convenience wrappers. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d375cdcf-1930-4ef0-a693-fa33436abf3d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pf = fits.open(jwf277w)\n",
-                "pf.info()"
+                "from astropy.table import QTable\n",
+                "import astropy.units as u\n",
+                "\n",
+                "lt = QTable()\n",
+                "lt['linename'] = ['Halpha', 'Hbeta']\n",
+                "lt['rest'] = [6.563e-7, 4.862e-7]*u.m\n",
+                "\n",
+                "specviz.load_line_list(lt)\n",
+                "specviz.spectral_lines"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "254e547f-a7f1-4a3c-913c-3674b7ac93da",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "imviz = Imviz()"
+                "If the loaded table has a `listname` column, the lines will show up in the Line List UI under that heading. Otherwise, they will by default show up under the `Custom` heading."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "28c4f536",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# This is the recommended way and you will get GWCS from\n",
-                "# the ASDF extension for all the loaded HDUs.\n",
-                "imviz.load_data(jwf277w, ext=('SCI', 1))\n",
-                "imviz.load_data(jwf277w, ext=('ERR', 1))\n",
-                "imviz.load_data(jwf277w, ext=('DQ', 1))"
+                "lt = QTable()\n",
+                "lt['linename'] = ['Test1', 'Test2']\n",
+                "lt['rest'] = [6.8e-7, 4.4e-7]*u.m\n",
+                "lt['listname'] = \"Test\"\n",
+                "\n",
+                "specviz.load_line_list(lt)\n",
+                "specviz.spectral_lines"
             ]
         },
         {
-            "cell_type": "raw",
-            "id": "0e8a5744",
+            "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# If you must load HDU objects themselves individually, you will\n",
-                "# only get WCS if it is in the immediate FITS header.\n",
-                "imviz.load_data(pf[1], data_label='ext_1')\n",
-                "imviz.load_data(pf[2], data_label='ext_2')\n",
-                "imviz.load_data(pf[3], data_label='ext_3')"
+                "Adding the lines to the plot is as simple as calling the `plot_spectral_lines` function:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ffba41b3-b843-441b-aa3e-7d8efc9bc7a5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "imviz.show()"
+                "specviz.plot_spectral_lines()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7dddb1d6",
             "metadata": {},
             "source": [
-                "To programmatically control Plot Options so you can set some stuff for all data at once, see https://jdaviz.readthedocs.io/en/latest/api/jdaviz.configs.default.plugins.plot_options.plot_options.PlotOptions.html.\n",
-                "\n",
-                "The example below sets the same colormap for all images."
+                "And one can erase all spectral lines from the plot as below:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "436974df",
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_options = imviz.plugins['Plot Options']"
+                "specviz.erase_spectral_lines()"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "2b1d2bdf",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "dir(plot_options)"
+                "### Preset line lists\n",
+                "\n",
+                "We also include with the jdaviz package a set of predefined line lists that can be loaded and plotted by the user. The names of these lists, which can be accessed via `specviz.available_linelists`, can be passed to `specviz.load_line_list` instead of passing in a QTable. The `replace` keyword still works as above."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "dabf30e4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_options.select_all()"
+                "specviz.available_linelists"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a57719f5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_options.image_colormap = 'Viridis'"
+                "specviz.load_line_list(\"Common Nebular\", replace=True)"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "b1cce96a",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Close the FITS file pointer when you are done with this notebook."
+                "specviz.spectral_lines"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "cf112d5f-e10a-420e-9144-d8883d8dc2cf",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pf.close()"
+                "specviz.plot_spectral_lines()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python 3",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.4"
+            "version": "3.8.2"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 4
 }
```

### Comparing `jdaviz-3.5.0/notebooks/concepts/imviz_roman_asdf.ipynb` & `jdaviz-3.6.0/notebooks/concepts/imviz_roman_asdf.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997996794871795%*

 * *Differences: {"'cells'": "{18: {'source': ['data = imviz.get_data(imviz.app.data_collection[0].label)']}}"}*

```diff
@@ -198,15 +198,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "0a4e02ef",
             "metadata": {},
             "outputs": [],
             "source": [
-                "data = imviz.app.get_data_from_viewer('imviz-0', imviz.app.data_collection[0].label)"
+                "data = imviz.get_data(imviz.app.data_collection[0].label)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "164a1a40",
             "metadata": {},
```

### Comparing `jdaviz-3.5.0/notebooks/concepts/imviz_simple_aper_phot.ipynb` & `jdaviz-3.6.0/notebooks/concepts/imviz_simple_aper_phot.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/mosviz_concept.ipynb` & `jdaviz-3.6.0/notebooks/concepts/mosviz_concept.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999338624338625%*

 * *Differences: {"'cells'": '{62: {\'source\': {insert: [(2, "currspec = '*

 * *            'mosviz.get_data(\'spectrum-added-by-plugin\')\\n")], delete: [2]}}}'}*

```diff
@@ -633,15 +633,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Assuming the user has done something with a glue plugin that adds another spectrum to the spectrum view\n",
                 "\n",
-                "currspec = mosviz.app.get_data_from_viewer('spectrum-viewer', 'spectrum-added-by-plugin')\n",
+                "currspec = mosviz.get_data('spectrum-added-by-plugin')\n",
                 "\n",
                 "... do something with currspec ..."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `jdaviz-3.5.0/notebooks/concepts/mosviz_generate_photometry.ipynb` & `jdaviz-3.6.0/notebooks/concepts/mosviz_generate_photometry.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/mosviz_niriss_parser.ipynb` & `jdaviz-3.6.0/notebooks/concepts/mosviz_niriss_parser.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/mosviz_overplot_slit.ipynb` & `jdaviz-3.6.0/notebooks/concepts/mosviz_overplot_slit.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/pypi_metrics.ipynb` & `jdaviz-3.6.0/notebooks/concepts/pypi_metrics.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/specviz_from_list.ipynb` & `jdaviz-3.6.0/notebooks/concepts/specviz_from_list.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/specviz_from_splot.ipynb` & `jdaviz-3.6.0/notebooks/concepts/specviz_from_splot.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/specviz_minimal.ipynb` & `jdaviz-3.6.0/notebooks/concepts/specviz_minimal.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/specviz_spectrum_list.ipynb` & `jdaviz-3.6.0/notebooks/concepts/specviz_spectrum_list.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/notebooks/concepts/specviz_unit_conversion.ipynb` & `jdaviz-3.6.0/jdaviz/jdaviz_cli_launcher.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7408730158730159%*

 * *Differences: {"'cells'": "{0: {'source': ['from jdaviz.core.launcher import show_launcher\\n', '\\n', "*

 * *            "'show_launcher()']}, delete: [2, 0]}",*

 * * "'metadata'": '{\'kernelspec\': {\'display_name\': "Python 3.10.10 (\'envmain\': venv)"}, '*

 * *               "'language_info': {'version': '3.10.10'}, 'vscode': OrderedDict([('interpreter', "*

 * *               "OrderedDict([('hash', "*

 * *               "'f917e879dca01012f092e44ceeb72fc316d3b188a12a493299dc2bd49905dadb')]))])}",*

 * * "'nbformat_minor'": '2'}*

```diff
@@ -2,60 +2,40 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from jdaviz.configs.specviz.helper import Specviz\n",
-                "import specutils\n",
-                "import astropy.units as u\n",
-                "import numpy as np"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "spec_url = 'https://dr14.sdss.org/optical/spectrum/view/data/format=fits/spec=lite?plateid=1323&mjd=52797&fiberid=12'\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "scrolled": false
-            },
-            "outputs": [],
-            "source": [
-                "specviz = Specviz()\n",
-                "spec = specutils.Spectrum1D.read(spec_url)\n",
-                "specviz.load_spectrum(spec)\n",
+                "from jdaviz.core.launcher import show_launcher\n",
                 "\n",
-                "specviz.show()"
+                "show_launcher()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3.10.10 ('envmain': venv)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.5"
+            "version": "3.10.10"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "f917e879dca01012f092e44ceeb72fc316d3b188a12a493299dc2bd49905dadb"
+            }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 2
 }
```

### Comparing `jdaviz-3.5.0/pyproject.toml` & `jdaviz-3.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [project]
 name = "jdaviz"
 description = "Astronomical data analysis development leveraging the Jupyter platform"
 requires-python = ">=3.8"
 authors = [
-    { name = "JDADF Developers", email = "rosteen@stsci.edu" },
+    { name = "JDADF Developers", email = "help@stsci.edu" },
 ]
 dependencies = [
     "packaging",
     "astropy>=4.3",
     "matplotlib",
     "traitlets>=5.0.5",
     "bqplot>=0.12.37",
     "bqplot-image-gl>=1.4.11",
-    "glue-core>=1.6.0,!=1.9.0,!=1.10",
-    "glue-jupyter>=0.15.0",
+    "glue-core>=1.11",
+    "glue-jupyter>=0.17",
     "echo>=0.5.0",
     "ipykernel>=6.19.4",
     "ipyvue>=1.6",
     "ipyvuetify>=1.7.0",
     "ipysplitpanes>=0.1.0",
     "ipygoldenlayout>=0.3.0",
     "ipywidgets>=8.0.6",
-    "voila>=0.4",
+    "voila>=0.4,<0.5",
     "pyyaml>=5.4.1",
     "specutils>=1.9",
     "specreduce>=1.3.0,<1.4.0",
     "photutils>=1.4",
-    "glue-astronomy>=0.7",
+    "glue-astronomy>=0.10",
     "asteval>=0.9.23",
     "idna",
     "vispy>=0.6.5",
     "asdf>=2.14.3",
     "stdatamodels>=1.3",
     "gwcs>=0.16.1",
     "regions>=0.6",
@@ -62,26 +62,28 @@
 default = "jdaviz.configs.default"
 cubeviz = "jdaviz.configs.cubeviz"
 specviz = "jdaviz.configs.specviz"
 mosviz = "jdaviz.configs.mosviz"
 imviz = "jdaviz.configs.imviz"
 
 [project.optional-dependencies]
+all = [
+    "opencv-python",
+]
 test = [
     "pytest",
     "pytest-astropy",
     "pytest-tornasync",
 ]
 docs = [
-    "sphinx-rtd-theme",
-    "sphinx-astropy",
-    "tomli; python_version <\"3.11\""
+    "sphinx-astropy[confv2]>=1.9.1",
+    "sphinx_design"
 ]
 roman = [
-    "roman_datamodels>=0.14.2",
+    "roman_datamodels>=0.16.1",
 ]
 
 [build-system]
 requires = [
     "setuptools>=61.2",
     "setuptools_scm",
     "wheel",
@@ -103,14 +105,15 @@
     "data/*",
     "data/*/*",
     "*.vue",
     "components/*.vue",
     "configs/*/*/*/*.vue",
     "configs/*/*.yaml",
     "jdaviz_cli.ipynb",
+    "jdaviz_cli_launcher.ipynb",
 ]
 "jdaviz.configs.imviz.tests" = [
     "data/*",
 ]
 
 [tool.pytest.ini_options]
 testpaths = [
@@ -134,14 +137,16 @@
     "ignore:specutils uses the deprecated entry point asdf_extensions",
     "ignore::DeprecationWarning:glue",
     "ignore::DeprecationWarning:bqplot",
     "ignore::DeprecationWarning:bqplot_image_gl",
     "ignore::DeprecationWarning:bqscales",
     "ignore::DeprecationWarning:traittypes",
     "ignore::DeprecationWarning:voila",
+    "ignore::DeprecationWarning:asteval",
+    "ignore::FutureWarning:asteval",
     "ignore:::specutils.spectra.spectrum1d",
 ]
 
 [tool.coverage.run]
 omit = [
     "jdaviz/_astropy_init*",
     "jdaviz/conftest.py",
```

### Comparing `jdaviz-3.5.0/setup.py` & `jdaviz-3.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js` & `jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/app.html` & `jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/app.html`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2` & `jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/util.js` & `jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/util.js`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/share/jupyter/voila/templates/jdaviz-default/index.html.j2` & `jdaviz-3.6.0/share/jupyter/voila/templates/jdaviz-default/index.html.j2`

 * *Files identical despite different names*

### Comparing `jdaviz-3.5.0/tox.ini` & `jdaviz-3.6.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 isolated_build = true
 
 [testenv]
 # Suppress display of matplotlib plots generated during docs build
 setenv =
     MPLBACKEND=agg
     JUPYTER_PLATFORM_DIRS=1
-    devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/scipy-wheels-nightly/simple
+    devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/scientific-python-nightly-wheels/simple
 
 # Pass through the following environment variables which may be needed for the CI
 passenv = HOME,WINDIR,LC_ALL,LC_CTYPE,CC,CI
 
 # Run the tests in a temporary directory to make sure that we don't import
 # this package from the source tree
 changedir = .tmp/{envname}
@@ -46,31 +46,30 @@
     devdeps: numpy>=0.0.dev0
     devdeps: git+https://github.com/astropy/regions.git
     devdeps: git+https://github.com/astropy/specutils.git
     devdeps: git+https://github.com/astropy/photutils.git
     devdeps: git+https://github.com/spacetelescope/gwcs.git
     devdeps: git+https://github.com/asdf-format/asdf.git
     devdeps: git+https://github.com/astropy/asdf-astropy.git
-    # FIXME: https://github.com/spacetelescope/stdatamodels/issues/159
-    #devdeps: git+https://github.com/spacetelescope/stdatamodels.git
+    devdeps: git+https://github.com/spacetelescope/stdatamodels.git
     devdeps: git+https://github.com/bqplot/bqplot.git@0.12.x
     devdeps: git+https://github.com/glue-viz/glue.git
-    devdeps: git+https://github.com/voila-dashboards/voila.git
+    # FIXME: https://github.com/spacetelescope/jdaviz/pull/2268
+    #devdeps: git+https://github.com/voila-dashboards/voila.git
     devdeps: git+https://github.com/glue-viz/bqplot-image-gl.git
     devdeps: git+https://github.com/glue-viz/glue-jupyter.git
     devdeps: git+https://github.com/glue-viz/glue-astronomy.git
     # TODO: Enable this when specreduce becomes stable.
     #devdeps: git+https://github.com/astropy/specreduce.git
 
 # The following indicates which extras_require from setup.cfg will be installed
 extras =
     test
     romandeps: roman
-    # Uncomment when we have all again in setup.cfg
-    #alldeps: all
+    alldeps: all
 
 commands =
     devdeps: pip install -U -i https://pypi.anaconda.org/astropy/simple astropy --pre
     jupyter --paths
     pip freeze
     !cov: pytest --pyargs jdaviz {toxinidir}/docs {posargs}
     cov: pytest --pyargs jdaviz {toxinidir}/docs --cov jdaviz --cov-config={toxinidir}/pyproject.toml {posargs}
```

