# Comparing `tmp/otter-grader-5.0.1.tar.gz` & `tmp/otter-grader-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter-grader-5.0.1.tar", last modified: Wed Jul 19 03:36:39 2023, max compression
+gzip compressed data, was "otter-grader-5.0.2.tar", last modified: Fri Jul 28 01:46:35 2023, max compression
```

## Comparing `otter-grader-5.0.1.tar` & `otter-grader-5.0.2.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-19 03:36:10.000000 otter-grader-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-19 03:36:10.000000 otter-grader-5.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-19 03:36:39.489056 otter-grader-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-19 03:36:10.000000 otter-grader-5.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/assign/
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/cell_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/feature_toggle.py
--rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/question_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/assign/r_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/r_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/r_adapter/cell_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/r_adapter/rmarkdown_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/r_adapter/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/r_adapter/tests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/tests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/check/
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/check/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/check/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/check/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/check/validate_export/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/check/validate_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/check/validate_export/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/execute/
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-19 03:36:37.000000 otter-grader-5.0.1/otter/execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/execute/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/execute/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/export/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/export/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/base_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/export/exporters/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/export/exporters/templates/via_html/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_html/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_html/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_html.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/export/exporters/templates/via_latex/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_latex/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_latex/index.tex.j2
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_latex.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/export/exporters/templates/via_latex_xecjk/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_latex_xecjk/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_latex_xecjk.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/via_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/via_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/generate/
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.477056 otter-grader-5.0.1/otter/generate/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/generate/templates/common/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/generate/templates/common/run_autograder
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/generate/templates/common/run_otter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/generate/templates/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/generate/templates/python/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/generate/templates/r/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/generate/templates/r/setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/generate/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/generate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/grade/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/grade/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/grade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/grade/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/grade/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/abstract_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/plugins/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/plugins/builtin/gmail_notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/builtin/gmail_notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/plugins/builtin/gmail_notifications/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/builtin/gmail_notifications/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/builtin/grade_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/builtin/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/run/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/run/run_autograder/
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/run_autograder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/run_autograder/autograder_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/run/run_autograder/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/run_autograder/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/run_autograder/runners/abstract_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/run_autograder/runners/python_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/run_autograder/runners/r_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/run_autograder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/test_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/test_files/abstract_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/test_files/exception_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/test_files/metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/test_files/ok_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/test_files/ottr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-19 03:36:37.000000 otter-grader-5.0.1/otter/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/otter_grader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-19 03:36:39.000000 otter-grader-5.0.1/otter_grader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-19 03:36:39.000000 otter-grader-5.0.1/otter_grader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 03:36:39.000000 otter-grader-5.0.1/otter_grader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-19 03:36:39.000000 otter-grader-5.0.1/otter_grader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-19 03:36:39.000000 otter-grader-5.0.1/otter_grader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 03:36:39.000000 otter-grader-5.0.1/otter_grader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-19 03:36:37.000000 otter-grader-5.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 03:36:39.489056 otter-grader-5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-19 03:36:10.000000 otter-grader-5.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/test_assign/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_assign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_assign/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/test_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_check/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_check/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_check/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    20296 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/test_execute/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_execute/test_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_execute/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/test_export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_export/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/test_generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_generate/test_autograder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_generate/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_generate/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/test_grade/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_grade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_grade/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/test_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_run/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-28 01:46:05.000000 otter-grader-5.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-28 01:46:05.000000 otter-grader-5.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-28 01:46:35.260630 otter-grader-5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-28 01:46:05.000000 otter-grader-5.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.248629 otter-grader-5.0.2/otter/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/assign/
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/cell_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/feature_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/question_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/assign/r_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/r_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/r_adapter/cell_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/r_adapter/rmarkdown_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/r_adapter/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/r_adapter/tests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/tests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/check/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/check/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/check/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/check/validate_export/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/check/validate_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-28 01:46:32.000000 otter-grader-5.0.2/otter/check/validate_export/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/execute/
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/execute/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/execute/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/export/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/base_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/export/exporters/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/export/exporters/templates/via_html/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_html/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_html/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_html.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/export/exporters/templates/via_latex/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_latex/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_latex/index.tex.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_latex.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/export/exporters/templates/via_latex_xecjk/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_latex_xecjk/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_latex_xecjk.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/via_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/via_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.244629 otter-grader-5.0.2/otter/generate/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/generate/templates/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/generate/templates/common/run_autograder
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/generate/templates/common/run_otter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/generate/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/generate/templates/python/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/generate/templates/r/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/generate/templates/r/setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/generate/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/generate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/grade/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/grade/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/grade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/grade/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/grade/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/abstract_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/plugins/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/plugins/builtin/gmail_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/builtin/gmail_notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/plugins/builtin/gmail_notifications/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/builtin/gmail_notifications/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/builtin/grade_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/builtin/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/run/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/run/run_autograder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/run_autograder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/run_autograder/autograder_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/run/run_autograder/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/run_autograder/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/run_autograder/runners/abstract_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/run_autograder/runners/python_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/run_autograder/runners/r_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/run_autograder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/test_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/test_files/abstract_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/test_files/exception_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/test_files/metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/test_files/ok_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/test_files/ottr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-28 01:46:33.000000 otter-grader-5.0.2/otter/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter_grader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-28 01:46:34.000000 otter-grader-5.0.2/otter_grader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-28 01:46:35.000000 otter-grader-5.0.2/otter_grader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 01:46:34.000000 otter-grader-5.0.2/otter_grader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-28 01:46:34.000000 otter-grader-5.0.2/otter_grader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-28 01:46:34.000000 otter-grader-5.0.2/otter_grader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 01:46:34.000000 otter-grader-5.0.2/otter_grader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-28 01:46:05.000000 otter-grader-5.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 01:46:35.260630 otter-grader-5.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-28 01:46:05.000000 otter-grader-5.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/test_assign/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_assign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_assign/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/test_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_check/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_check/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_check/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20296 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/test_execute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_execute/test_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_execute/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/test_export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_export/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/test_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_generate/test_autograder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_generate/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_generate/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/test_grade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_grade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-07-28 01:46:32.000000 otter-grader-5.0.2/test/test_grade/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/test_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_run/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_utils.py
```

### Comparing `otter-grader-5.0.1/LICENSE` & `otter-grader-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/PKG-INFO` & `otter-grader-5.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-grader
-Version: 5.0.1
+Version: 5.0.2
 Summary: Python and Jupyter Notebook autograder
 Home-page: https://github.com/ucbds-infra/otter-grader
 Author: Christopher Pyles
 Author-email: otter-grader@berkeley.edu
 License: BSD-3-Clause
 Description: # Otter-Grader
```

### Comparing `otter-grader-5.0.1/README.md` & `otter-grader-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/api.py` & `otter-grader-5.0.2/otter/api.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/__init__.py` & `otter-grader-5.0.2/otter/assign/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/assignment.py` & `otter-grader-5.0.2/otter/assign/assignment.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/blocks.py` & `otter-grader-5.0.2/otter/assign/blocks.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/cell_factory.py` & `otter-grader-5.0.2/otter/assign/cell_factory.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/feature_toggle.py` & `otter-grader-5.0.2/otter/assign/feature_toggle.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/notebook_transformer.py` & `otter-grader-5.0.2/otter/assign/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/output.py` & `otter-grader-5.0.2/otter/assign/output.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/plugins.py` & `otter-grader-5.0.2/otter/assign/plugins.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/question_config.py` & `otter-grader-5.0.2/otter/assign/question_config.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/r_adapter/cell_factory.py` & `otter-grader-5.0.2/otter/assign/r_adapter/cell_factory.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/r_adapter/rmarkdown_converter.py` & `otter-grader-5.0.2/otter/assign/r_adapter/rmarkdown_converter.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/r_adapter/solutions.py` & `otter-grader-5.0.2/otter/assign/r_adapter/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/r_adapter/tests_manager.py` & `otter-grader-5.0.2/otter/assign/r_adapter/tests_manager.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/solutions.py` & `otter-grader-5.0.2/otter/assign/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/tests_manager.py` & `otter-grader-5.0.2/otter/assign/tests_manager.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/assign/utils.py` & `otter-grader-5.0.2/otter/assign/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/check/__init__.py` & `otter-grader-5.0.2/otter/check/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/check/logs.py` & `otter-grader-5.0.2/otter/check/logs.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/check/notebook.py` & `otter-grader-5.0.2/otter/check/notebook.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/check/utils.py` & `otter-grader-5.0.2/otter/check/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/check/validate_export/__main__.py` & `otter-grader-5.0.2/otter/check/validate_export/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
     try:
         with zipfile.ZipFile(args.zip_path, "r") as zf:
             nb_path = zf.extract(args.nb_arcname, path=nb_dir)
 
         results = grade_notebook(
             nb_path,
+            test_dir=args.tests_dir,
             tests_glob=glob(args.tests_dir + "/*.py"),
             cwd=os.getcwd()
         )
 
         with open(args.results_path, "wb") as f:
             dill.dump(results, f)
```

### Comparing `otter-grader-5.0.1/otter/cli.py` & `otter-grader-5.0.2/otter/cli.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/execute/__init__.py` & `otter-grader-5.0.2/otter/execute/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/execute/checker.py` & `otter-grader-5.0.2/otter/execute/checker.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/execute/preprocessor.py` & `otter-grader-5.0.2/otter/execute/preprocessor.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/export/__init__.py` & `otter-grader-5.0.2/otter/export/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/export/exporters/__init__.py` & `otter-grader-5.0.2/otter/export/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/export/exporters/base_exporter.py` & `otter-grader-5.0.2/otter/export/exporters/base_exporter.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/export/exporters/templates/via_html/index.html.j2` & `otter-grader-5.0.2/otter/export/exporters/templates/via_html/index.html.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/export/exporters/templates/via_html.tpl` & `otter-grader-5.0.2/otter/export/exporters/templates/via_html.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/export/exporters/templates/via_latex/index.tex.j2` & `otter-grader-5.0.2/otter/export/exporters/templates/via_latex/index.tex.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/export/exporters/templates/via_latex.tpl` & `otter-grader-5.0.2/otter/export/exporters/templates/via_latex.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2` & `otter-grader-5.0.2/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/export/exporters/templates/via_latex_xecjk.tpl` & `otter-grader-5.0.2/otter/export/exporters/templates/via_latex_xecjk.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/export/exporters/utils.py` & `otter-grader-5.0.2/otter/export/exporters/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/export/exporters/via_html.py` & `otter-grader-5.0.2/otter/export/exporters/via_html.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/export/exporters/via_latex.py` & `otter-grader-5.0.2/otter/export/exporters/via_latex.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/generate/__init__.py` & `otter-grader-5.0.2/otter/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/generate/templates/python/setup.sh` & `otter-grader-5.0.2/otter/generate/templates/python/setup.sh`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/generate/templates/r/setup.sh` & `otter-grader-5.0.2/otter/generate/templates/r/setup.sh`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/generate/token.py` & `otter-grader-5.0.2/otter/generate/token.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/generate/utils.py` & `otter-grader-5.0.2/otter/generate/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/grade/Dockerfile` & `otter-grader-5.0.2/otter/grade/Dockerfile`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/grade/__init__.py` & `otter-grader-5.0.2/otter/grade/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/grade/containers.py` & `otter-grader-5.0.2/otter/grade/containers.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/grade/utils.py` & `otter-grader-5.0.2/otter/grade/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/plugins/__init__.py` & `otter-grader-5.0.2/otter/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/plugins/abstract_plugin.py` & `otter-grader-5.0.2/otter/plugins/abstract_plugin.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/plugins/builtin/gmail_notifications/__init__.py` & `otter-grader-5.0.2/otter/plugins/builtin/gmail_notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py` & `otter-grader-5.0.2/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/plugins/builtin/grade_override.py` & `otter-grader-5.0.2/otter/plugins/builtin/grade_override.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/plugins/builtin/rate_limiting.py` & `otter-grader-5.0.2/otter/plugins/builtin/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/run/__init__.py` & `otter-grader-5.0.2/otter/run/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/run/run_autograder/__init__.py` & `otter-grader-5.0.2/otter/run/run_autograder/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/run/run_autograder/autograder_config.py` & `otter-grader-5.0.2/otter/run/run_autograder/autograder_config.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/run/run_autograder/runners/__init__.py` & `otter-grader-5.0.2/otter/run/run_autograder/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/run/run_autograder/runners/abstract_runner.py` & `otter-grader-5.0.2/otter/run/run_autograder/runners/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/run/run_autograder/runners/python_runner.py` & `otter-grader-5.0.2/otter/run/run_autograder/runners/python_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/run/run_autograder/runners/r_runner.py` & `otter-grader-5.0.2/otter/run/run_autograder/runners/r_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/test_files/__init__.py` & `otter-grader-5.0.2/otter/test_files/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/test_files/abstract_test.py` & `otter-grader-5.0.2/otter/test_files/abstract_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/test_files/exception_test.py` & `otter-grader-5.0.2/otter/test_files/exception_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/test_files/metadata_test.py` & `otter-grader-5.0.2/otter/test_files/metadata_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/test_files/ok_test.py` & `otter-grader-5.0.2/otter/test_files/ok_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/utils.py` & `otter-grader-5.0.2/otter/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/otter/version.py` & `otter-grader-5.0.2/otter/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Version and printable logo"""
 
 import sys
 
 from textwrap import dedent
 
 
-__version__ = "5.0.1"
+__version__ = "5.0.2"
 
 
 LOGO_WITH_VERSION = fr"""
   _________        __          __               
  /  _____  \    __|  |__    __|  |__               
 |  /     \  |  |__    __|  |__    __|   _______    _  _____
 | |       | |     |  |        |  |     |  ___  |  | |/ ____|
```

### Comparing `otter-grader-5.0.1/otter_grader.egg-info/PKG-INFO` & `otter-grader-5.0.2/otter_grader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-grader
-Version: 5.0.1
+Version: 5.0.2
 Summary: Python and Jupyter Notebook autograder
 Home-page: https://github.com/ucbds-infra/otter-grader
 Author: Christopher Pyles
 Author-email: otter-grader@berkeley.edu
 License: BSD-3-Clause
 Description: # Otter-Grader
```

### Comparing `otter-grader-5.0.1/otter_grader.egg-info/SOURCES.txt` & `otter-grader-5.0.2/otter_grader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/setup.py` & `otter-grader-5.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/test/test_api.py` & `otter-grader-5.0.2/test/test_api.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/test/test_assign/test_integration.py` & `otter-grader-5.0.2/test/test_assign/test_integration.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/test/test_check/test_cli.py` & `otter-grader-5.0.2/test/test_check/test_cli.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/test/test_check/test_logs.py` & `otter-grader-5.0.2/test/test_check/test_logs.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/test/test_check/test_notebook.py` & `otter-grader-5.0.2/test/test_check/test_notebook.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/test/test_cli.py` & `otter-grader-5.0.2/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/test/test_execute/test_checker.py` & `otter-grader-5.0.2/test/test_execute/test_checker.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/test/test_execute/test_integration.py` & `otter-grader-5.0.2/test/test_execute/test_integration.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/test/test_export/test_integration.py` & `otter-grader-5.0.2/test/test_export/test_integration.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/test/test_generate/test_autograder.py` & `otter-grader-5.0.2/test/test_generate/test_autograder.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/test/test_generate/test_token.py` & `otter-grader-5.0.2/test/test_generate/test_token.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/test/test_generate/test_utils.py` & `otter-grader-5.0.2/test/test_generate/test_utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.1/test/test_grade/test_integration.py` & `otter-grader-5.0.2/test/test_grade/test_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pandas as pd
 import pytest
 import re
 import shutil
 import zipfile
 
 from glob import glob
+from python_on_whales import docker
 from unittest import mock
 
 from otter.generate import main as generate
 from otter.grade import main as grade
 from otter.run.run_autograder.autograder_config import AutograderConfig
 from otter.utils import loggers
 
@@ -99,15 +100,15 @@
     """
     grade(
         name = ASSIGNMENT_NAME,
         paths = [FILE_MANAGER.get_path("network/")],
         output_dir = "test/",
         autograder = AG_ZIP_PATH,
         containers = 5,
-        no_network=True,
+        no_network = True,
     )
 
     df_test = pd.read_csv("test/final_grades.csv")
 
     # sort by filename
     df_test = df_test.sort_values("file").reset_index(drop=True)
 
@@ -186,26 +187,26 @@
     }])
 
     notebook_path = FILE_MANAGER.get_path("notebooks/passesAll.ipynb")
 
     kw_expected = {
         "num_containers": 1,
         "base_image": "ubuntu:22.04",
-        "tag": "foo",
+        "tag": ASSIGNMENT_NAME,
         "no_kill": False,
         "pdf_dir": None,
         "timeout": None,
         "network": True,
         "config": AutograderConfig(),
     }
 
     mocked_launch_grade.return_value = [df]
 
     output = grade(
-        name = "foo",
+        name = ASSIGNMENT_NAME,
         paths = [notebook_path],
         output_dir = "test/",
         # the value of the autograder argument doesn't matter, it just needs to be a valid file path
         autograder = notebook_path,
         containers = 1,
     )
 
@@ -228,15 +229,15 @@
         "q7": 1.0,
         "percent_correct": 1.0,
         "file": "passesAll.ipynb",
     }])]
 
     notebook_path = FILE_MANAGER.get_path("notebooks/passesAll.ipynb")
     grade(
-        name = "foo",
+        name = ASSIGNMENT_NAME,
         paths = [notebook_path],
         output_dir = "test/",
         # the value of the autograder argument doesn't matter, it just needs to be a valid file path
         autograder = notebook_path,
         containers = 1,
         pdfs = True,
         ext = "zip",
@@ -257,15 +258,15 @@
     Checks that overriding otter_config.json configurations with CLI flags works.
     """
     notebook_path = FILE_MANAGER.get_path("notebooks/passesAll.ipynb")
     with zipfile.ZipFile(ZIP_SUBM_PATH, "x") as zf:
         zf.write(notebook_path, arcname="passesAll.ipynb")
 
     output = grade(
-        name = "foo",
+        name = ASSIGNMENT_NAME,
         paths = [ZIP_SUBM_PATH],
         output_dir = "test/",
         # the value of the autograder argument doesn't matter, it just needs to be a valid file path
         autograder = AG_ZIP_PATH,
         ext = "zip",
     )
```

### Comparing `otter-grader-5.0.1/test/test_run/test_integration.py` & `otter-grader-5.0.2/test/test_run/test_integration.py`

 * *Files identical despite different names*

