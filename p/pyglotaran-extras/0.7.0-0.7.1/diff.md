# Comparing `tmp/pyglotaran_extras-0.7.0.tar.gz` & `tmp/pyglotaran_extras-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglotaran_extras-0.7.0.tar", last modified: Sat Apr 15 19:53:14 2023, max compression
+gzip compressed data, was "pyglotaran_extras-0.7.1.tar", last modified: Thu Jul 27 22:24:03 2023, max compression
```

## Comparing `pyglotaran_extras-0.7.0.tar` & `pyglotaran_extras-0.7.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.220532 pyglotaran_extras-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-15 19:53:14.220532 pyglotaran_extras-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.204531 pyglotaran_extras-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.200531 pyglotaran_extras-0.7.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.208531 pyglotaran_extras-0.7.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/_templates/autosummary/exception.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/_templates/autosummary/function.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/_templates/autosummary/method.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/api_docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.208531 pyglotaran_extras-0.7.0/pyglotaran_extras/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.208531 pyglotaran_extras-0.7.0/pyglotaran_extras/deprecation/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/deprecation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/deprecation/deprecation_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.212531 pyglotaran_extras-0.7.0/pyglotaran_extras/inspect/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/inspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/inspect/a_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/inspect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.212531 pyglotaran_extras-0.7.0/pyglotaran_extras/io/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/io/load_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/io/setup_case_study.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.212531 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_coherent_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_concentrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_doas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_irf_dispersion_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyglotaran_extras/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.208531 pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-15 19:53:13.000000 pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-15 19:53:14.000000 pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:53:13.000000 pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-15 19:53:13.000000 pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 19:53:13.000000 pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:53:13.000000 pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-15 19:53:14.220532 pyglotaran_extras-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.216531 pyglotaran_extras-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.204531 pyglotaran_extras-0.7.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.216531 pyglotaran_extras-0.7.0/tests/data/a_matrix/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/a_matrix_to_html_table_decimal_2.md
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/a_matrix_to_html_table_default.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/a_matrix_to_html_table_normalized.md
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_decimal_2.md
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_default.md
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_expanded_dataset_2.md
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_heading_offset_0.md
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_min_size_2.md
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_multiple_a_matrixes_in_dataset.md
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_normalized.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.216531 pyglotaran_extras-0.7.0/tests/deprecation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/deprecation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/deprecation/test_deprecation_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.216531 pyglotaran_extras-0.7.0/tests/inspect/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/inspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/inspect/test_a_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/inspect/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.220532 pyglotaran_extras-0.7.0/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/io/test_get_script_dir.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/io/test_load_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/io/test_setup_case_study.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:53:14.220532 pyglotaran_extras-0.7.0/tests/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-15 19:53:07.000000 pyglotaran_extras-0.7.0/tests/plotting/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.792002 pyglotaran_extras-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-27 22:24:03.792002 pyglotaran_extras-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.784001 pyglotaran_extras-0.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.780001 pyglotaran_extras-0.7.1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.788001 pyglotaran_extras-0.7.1/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/docs/_templates/autosummary/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/docs/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/docs/_templates/autosummary/method.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/docs/api_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.788001 pyglotaran_extras-0.7.1/pyglotaran_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.788001 pyglotaran_extras-0.7.1/pyglotaran_extras/deprecation/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/deprecation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/deprecation/deprecation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.788001 pyglotaran_extras-0.7.1/pyglotaran_extras/inspect/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/inspect/a_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/inspect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.788001 pyglotaran_extras-0.7.1/pyglotaran_extras/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/io/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/io/setup_case_study.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.792002 pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_coherent_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_concentrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_doas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_irf_dispersion_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11270 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24386 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyglotaran_extras/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.788001 pyglotaran_extras-0.7.1/pyglotaran_extras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-27 22:24:03.000000 pyglotaran_extras-0.7.1/pyglotaran_extras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-27 22:24:03.000000 pyglotaran_extras-0.7.1/pyglotaran_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:24:03.000000 pyglotaran_extras-0.7.1/pyglotaran_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 22:24:03.000000 pyglotaran_extras-0.7.1/pyglotaran_extras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 22:24:03.000000 pyglotaran_extras-0.7.1/pyglotaran_extras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:24:03.000000 pyglotaran_extras-0.7.1/pyglotaran_extras.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-27 22:24:03.792002 pyglotaran_extras-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.792002 pyglotaran_extras-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.784001 pyglotaran_extras-0.7.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.792002 pyglotaran_extras-0.7.1/tests/data/a_matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/data/a_matrix/a_matrix_to_html_table_decimal_2.md
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/data/a_matrix/a_matrix_to_html_table_default.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/data/a_matrix/a_matrix_to_html_table_normalized.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/data/a_matrix/show_a_matrixes_decimal_2.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/data/a_matrix/show_a_matrixes_default.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/data/a_matrix/show_a_matrixes_expanded_dataset_2.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/data/a_matrix/show_a_matrixes_heading_offset_0.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/data/a_matrix/show_a_matrixes_min_size_2.md
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/data/a_matrix/show_a_matrixes_multiple_a_matrixes_in_dataset.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/data/a_matrix/show_a_matrixes_normalized.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.792002 pyglotaran_extras-0.7.1/tests/deprecation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/deprecation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/deprecation/test_deprecation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.792002 pyglotaran_extras-0.7.1/tests/inspect/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/inspect/test_a_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/inspect/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.792002 pyglotaran_extras-0.7.1/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/io/test_get_script_dir.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/io/test_load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/io/test_setup_case_study.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:24:03.792002 pyglotaran_extras-0.7.1/tests/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-27 22:23:58.000000 pyglotaran_extras-0.7.1/tests/plotting/test_utils.py
```

### Comparing `pyglotaran_extras-0.7.0/CONTRIBUTING.rst` & `pyglotaran_extras-0.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/LICENSE` & `pyglotaran_extras-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/PKG-INFO` & `pyglotaran_extras-0.7.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,78 @@
 Metadata-Version: 2.1
 Name: pyglotaran_extras
-Version: 0.7.0
+Version: 0.7.1
 Summary: Supplementary package for pyglotaran with (example) plotting code.
 Home-page: https://github.com/glotaran/pyglotaran-extras
 Author: Joris Snellenburg
 Author-email: j.snellenburg@gmail.com
 License: MIT
 Project-URL: GloTarAn Ecosystem, https://glotaran.org
 Project-URL: Documentation, https://pyglotaran-extras.readthedocs.io
 Project-URL: Changelog, https://pyglotaran-extras.readthedocs.io/en/latest/changelog.html
 Project-URL: Source, https://github.com/glotaran/pyglotaran-extras
 Project-URL: Tracker, https://github.com/glotaran/pyglotaran-extras/issues
-Description: # pyglotaran-extras
-        
-        [![PyPI version](https://badge.fury.io/py/pyglotaran-extras.svg)](https://badge.fury.io/py/pyglotaran-extras)
-        [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pyglotaran-extras.svg)](https://anaconda.org/conda-forge/pyglotaran-extras)
-        [![Tests](https://github.com/glotaran/pyglotaran-extras/actions/workflows/test.yml/badge.svg)](https://github.com/glotaran/pyglotaran-extras/actions/workflows/test.yml)
-        [![Documentation Status](https://readthedocs.org/projects/pyglotaran-extras/badge/?version=latest)](https://pyglotaran-extras.readthedocs.io/en/latest/?badge=latest)
-        [![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/glotaran/pyglotaran-extras.git/main?urlpath=lab%2Ftree%2Fdocs%2Fsource%2Fnotebooks)
-        
-        [![codecov](https://codecov.io/gh/glotaran/pyglotaran-extras/branch/main/graph/badge.svg?token=I6F412Y390)](https://codecov.io/gh/glotaran/pyglotaran-extras)
-        [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/glotaran/pyglotaran-extras.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/glotaran/pyglotaran-extras/context:python)
-        [![Code style Python: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![Discord](https://img.shields.io/discord/883443835135475753.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/KfnEYRSTJx)
-        
-        Supplementary package for pyglotaran with (example) plotting code for use with the pyglotaran package.
-        Can be installed as a python package or from sources.
-        
-        ## Installation
-        
-        Prerequisites:
-        
-        - Python 3.8 or 3.9
-        - Python package `pyglotaran` v0.3.0 (or later)
-        
-        ### Stable Release
-        
-        To install pyglotaran-extras from [PyPI](https://pypi.org/), run this command in your terminal:
-        
-        ```console
-        pip install pyglotaran-extras
-        ```
-        
-        If you want to install it via conda, you can run the following command:
-        
-        ```console
-        conda install -c conda-forge pyglotaran-extras
-        ```
-        
-        ### From Source
-        
-        To install pyglotaran-extras from sources, either clone this repository or download the latest release, then run this command in your terminal:
-        
-        ```console
-        git clone https://github.com/glotaran/pyglotaran-extras.git
-        cd pyglotaran-extras
-        pip install -e .
-        ```
-        
-        or directly
-        
-        ```console
-        pip install git+https://github.com/glotaran/pyglotaran-extras.git
-        ```
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyglotaran-extras
+
+[![PyPI version](https://badge.fury.io/py/pyglotaran-extras.svg)](https://badge.fury.io/py/pyglotaran-extras)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/pyglotaran-extras.svg)](https://anaconda.org/conda-forge/pyglotaran-extras)
+[![Tests](https://github.com/glotaran/pyglotaran-extras/actions/workflows/test.yml/badge.svg)](https://github.com/glotaran/pyglotaran-extras/actions/workflows/test.yml)
+[![Documentation Status](https://readthedocs.org/projects/pyglotaran-extras/badge/?version=latest)](https://pyglotaran-extras.readthedocs.io/en/latest/?badge=latest)
+[![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/glotaran/pyglotaran-extras.git/main?urlpath=lab%2Ftree%2Fdocs%2Fsource%2Fnotebooks)
+
+[![codecov](https://codecov.io/gh/glotaran/pyglotaran-extras/branch/main/graph/badge.svg?token=I6F412Y390)](https://codecov.io/gh/glotaran/pyglotaran-extras)
+[![Code style Python: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Discord](https://img.shields.io/discord/883443835135475753.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/KfnEYRSTJx)
+
+Supplementary package for pyglotaran with (example) plotting code for use with the pyglotaran package.
+Can be installed as a python package or from sources.
+
+## Installation
+
+Prerequisites:
+
+- Python 3.8, 3.9 or 3.10
+- Python package `pyglotaran` v0.6.0 (or later)
+
+### Stable Release
+
+To install pyglotaran-extras from [PyPI](https://pypi.org/), run this command in your terminal:
+
+```console
+pip install pyglotaran-extras
+```
+
+If you want to install it via conda, you can run the following command:
+
+```console
+conda install -c conda-forge pyglotaran-extras
+```
+
+### From Source
+
+To install pyglotaran-extras from sources, either clone this repository or download the latest release, then run this command in your terminal:
+
+```console
+git clone https://github.com/glotaran/pyglotaran-extras.git
+cd pyglotaran-extras
+pip install -e .
+```
+
+or directly
+
+```console
+pip install git+https://github.com/glotaran/pyglotaran-extras.git
+```
```

### Comparing `pyglotaran_extras-0.7.0/README.md` & `pyglotaran_extras-0.7.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 [![PyPI version](https://badge.fury.io/py/pyglotaran-extras.svg)](https://badge.fury.io/py/pyglotaran-extras)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pyglotaran-extras.svg)](https://anaconda.org/conda-forge/pyglotaran-extras)
 [![Tests](https://github.com/glotaran/pyglotaran-extras/actions/workflows/test.yml/badge.svg)](https://github.com/glotaran/pyglotaran-extras/actions/workflows/test.yml)
 [![Documentation Status](https://readthedocs.org/projects/pyglotaran-extras/badge/?version=latest)](https://pyglotaran-extras.readthedocs.io/en/latest/?badge=latest)
 [![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/glotaran/pyglotaran-extras.git/main?urlpath=lab%2Ftree%2Fdocs%2Fsource%2Fnotebooks)
 
 [![codecov](https://codecov.io/gh/glotaran/pyglotaran-extras/branch/main/graph/badge.svg?token=I6F412Y390)](https://codecov.io/gh/glotaran/pyglotaran-extras)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/glotaran/pyglotaran-extras.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/glotaran/pyglotaran-extras/context:python)
 [![Code style Python: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Discord](https://img.shields.io/discord/883443835135475753.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/KfnEYRSTJx)
 
 Supplementary package for pyglotaran with (example) plotting code for use with the pyglotaran package.
 Can be installed as a python package or from sources.
 
 ## Installation
 
 Prerequisites:
 
-- Python 3.8 or 3.9
-- Python package `pyglotaran` v0.3.0 (or later)
+- Python 3.8, 3.9 or 3.10
+- Python package `pyglotaran` v0.6.0 (or later)
 
 ### Stable Release
 
 To install pyglotaran-extras from [PyPI](https://pypi.org/), run this command in your terminal:
 
 ```console
 pip install pyglotaran-extras
```

### Comparing `pyglotaran_extras-0.7.0/docs/Makefile` & `pyglotaran_extras-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/docs/_templates/autosummary/class.rst` & `pyglotaran_extras-0.7.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/docs/_templates/autosummary/module.rst` & `pyglotaran_extras-0.7.1/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/docs/conf.py` & `pyglotaran_extras-0.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/docs/installation.rst` & `pyglotaran_extras-0.7.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/docs/make.bat` & `pyglotaran_extras-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/__init__.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 from pyglotaran_extras.plotting.plot_doas import plot_doas
 from pyglotaran_extras.plotting.plot_guidance import plot_guidance
 from pyglotaran_extras.plotting.plot_irf_dispersion_center import plot_irf_dispersion_center
 from pyglotaran_extras.plotting.plot_overview import plot_overview
 from pyglotaran_extras.plotting.plot_overview import plot_simple_overview
 from pyglotaran_extras.plotting.plot_traces import plot_fitted_traces
 from pyglotaran_extras.plotting.plot_traces import select_plot_wavelengths
+from pyglotaran_extras.plotting.utils import add_subplot_labels
 
 __all__ = [
     "load_data",
     "setup_case_study",
     "plot_coherent_artifact",
     "plot_data_overview",
     "plot_doas",
     "plot_guidance",
     "plot_irf_dispersion_center",
     "plot_overview",
     "plot_simple_overview",
     "plot_fitted_traces",
     "select_plot_wavelengths",
+    "add_subplot_labels",
 ]
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
```

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/deprecation/deprecation_utils.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/deprecation/deprecation_utils.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/inspect/a_matrix.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/inspect/a_matrix.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/inspect/utils.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/inspect/utils.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/io/load_data.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/io/load_data.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/io/setup_case_study.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/io/setup_case_study.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/io/utils.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/io/utils.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_coherent_artifact.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_coherent_artifact.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,18 @@
     irf_y_label = "amplitude"
     irfas_y_label = "ΔA"
 
     if normalize is True:
         norm_factor = scales.max()
         irf_y_label = f"normalized {irf_y_label}"
 
-    plot_slice_irf = (
-        irf_data.sel(spectral=spectral, method="nearest") / irf_max * scales / norm_factor
-    )
+    if "spectral" in irf_data.coords:
+        irf_data = irf_data.sel(spectral=spectral, method="nearest")
+
+    plot_slice_irf = irf_data / irf_max * scales / norm_factor
     irf_sel_kwargs = (
         {"time": slice(time_range[0], time_range[1])} if time_range is not None else {}
     )
     plot_slice_irf.sel(**irf_sel_kwargs).plot.line(x="time", ax=axes[0])
     axes[0].set_title("IRF Derivatives")
     axes[0].set_ylabel(f"{irf_y_label} (a.u.)")
```

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_concentrations.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_concentrations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module containing concentration plot functionality."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from pyglotaran_extras.plotting.style import PlotStyle
+from pyglotaran_extras.plotting.utils import MinorSymLogLocator
 from pyglotaran_extras.plotting.utils import add_cycler_if_not_none
 from pyglotaran_extras.plotting.utils import get_shifted_traces
 
 if TYPE_CHECKING:
     import xarray as xr
     from cycler import Cycler
     from matplotlib.axis import Axis
@@ -65,7 +66,8 @@
         traces.sel(spectral=center_λ, method="nearest").plot.line(x="time", ax=ax)
     else:
         traces.plot.line(x="time", ax=ax)
     ax.set_title(title)
 
     if linlog:
         ax.set_xscale("symlog", linthresh=linthresh, linscale=linscale)
+        ax.xaxis.set_minor_locator(MinorSymLogLocator(linthresh))
```

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_data.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from glotaran.io.prepare_dataset import add_svd_to_dataset
 from matplotlib.axis import Axis
 
 from pyglotaran_extras.io.load_data import load_data
 from pyglotaran_extras.plotting.plot_svd import plot_lsv_data
 from pyglotaran_extras.plotting.plot_svd import plot_rsv_data
 from pyglotaran_extras.plotting.plot_svd import plot_sv_data
+from pyglotaran_extras.plotting.utils import MinorSymLogLocator
 from pyglotaran_extras.plotting.utils import not_single_element_dims
 from pyglotaran_extras.plotting.utils import shift_time_axis_by_irf_location
 
 __all__ = ["plot_data_overview"]
 
 if TYPE_CHECKING:
     from typing import Hashable
@@ -105,14 +106,15 @@
     plot_rsv_data(dataset, rsv_ax, indices=range(nr_of_data_svd_vectors), show_legend=False)
     if show_data_svd_legend is True:
         rsv_ax.legend(title="singular value index", loc="lower right", bbox_to_anchor=(1.13, 1))
     fig.suptitle(title, fontsize=16)
 
     if linlog:
         data_ax.set_xscale("symlog", linthresh=linthresh)
+        data_ax.xaxis.set_minor_locator(MinorSymLogLocator(linthresh))
     return fig, (data_ax, lsv_ax, sv_ax, rsv_ax)
 
 
 def _plot_single_trace(
     data_array: xr.DataArray,
     x_dim: Hashable,
     *,
@@ -146,8 +148,9 @@
     """
     fig, ax = plt.subplots(1, 1, figsize=figsize)
     data_array.plot.line(x=x_dim, ax=ax)
     fig.suptitle(title, fontsize=16)
 
     if linlog:
         ax.set_xscale("symlog", linthresh=linthresh)
+        ax.xaxis.set_minor_locator(MinorSymLogLocator(linthresh))
     return fig, ax
```

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_doas.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_doas.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,19 +101,21 @@
     )
     osc_sel_kwargs = (
         {"damped_oscillation": damped_oscillation} if damped_oscillation is not None else {}
     )
 
     irf_location = extract_irf_location(dataset, spectral, main_irf_nr)
 
+    oscillations = dataset[f"damped_oscillation_{oscillation_type}"]
+
+    if "spectral" in oscillations.coords:
+        oscillations = oscillations.sel(spectral=spectral, method="nearest")
+
     oscillations = shift_time_axis_by_irf_location(
-        dataset[f"damped_oscillation_{oscillation_type}"]
-        .sel(spectral=spectral, method="nearest")
-        .sel(**osc_sel_kwargs),
-        irf_location,
+        oscillations.sel(**osc_sel_kwargs), irf_location
     )
     oscillations_spectra = dataset["damped_oscillation_associated_spectra"].sel(**osc_sel_kwargs)
 
     damped_oscillation_phase = dataset["damped_oscillation_phase"].sel(**osc_sel_kwargs)
 
     osc_max = abs_max((oscillations - 1), result_dims="damped_oscillation")
     spectra_max = abs_max(oscillations_spectra, result_dims="damped_oscillation")
```

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_guidance.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_guidance.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_irf_dispersion_center.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_irf_dispersion_center.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_overview.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_overview.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_residual.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_residual.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from pyglotaran_extras.plotting.plot_irf_dispersion_center import _plot_irf_dispersion_center
 from pyglotaran_extras.plotting.style import PlotStyle
+from pyglotaran_extras.plotting.utils import MinorSymLogLocator
 from pyglotaran_extras.plotting.utils import add_cycler_if_not_none
 from pyglotaran_extras.plotting.utils import shift_time_axis_by_irf_location
 
 if TYPE_CHECKING:
     import xarray as xr
     from cycler import Cycler
     from matplotlib.axis import Axis
@@ -79,8 +80,9 @@
         _plot_irf_dispersion_center(
             res, ax=ax, spectral_axis="y", cycler=cycler, irf_location=irf_location
         )
         ax.set_xlabel("time")
         ax.legend()
     if linlog:
         ax.set_xscale("symlog", linthresh=linthresh)
+        ax.xaxis.set_minor_locator(MinorSymLogLocator(linthresh))
     ax.set_title(title)
```

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_spectra.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_spectra.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_svd.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_svd.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from glotaran.io.prepare_dataset import add_svd_to_dataset
 
 from pyglotaran_extras.plotting.style import PlotStyle
+from pyglotaran_extras.plotting.utils import MinorSymLogLocator
 from pyglotaran_extras.plotting.utils import add_cycler_if_not_none
 from pyglotaran_extras.plotting.utils import shift_time_axis_by_irf_location
 
 if TYPE_CHECKING:
     from typing import Sequence
 
     import xarray as xr
@@ -136,14 +137,15 @@
     add_cycler_if_not_none(ax, cycler)
     dLSV = res.data_left_singular_vectors
     dLSV = shift_time_axis_by_irf_location(dLSV, irf_location)
     _plot_svd_vectors(dLSV, indices, "left_singular_value_index", ax, show_legend)
     ax.set_title("data. LSV")
     if linlog:
         ax.set_xscale("symlog", linthresh=linthresh)
+        ax.xaxis.set_minor_locator(MinorSymLogLocator(linthresh))
 
 
 def plot_rsv_data(
     res: xr.Dataset,
     ax: Axis,
     indices: Sequence[int] = range(4),
     cycler: Cycler | None = PlotStyle().cycler,
@@ -236,14 +238,15 @@
     else:
         rLSV = res.residual_left_singular_vectors
     rLSV = shift_time_axis_by_irf_location(rLSV, irf_location)
     _plot_svd_vectors(rLSV, indices, "left_singular_value_index", ax, show_legend)
     ax.set_title("res. LSV")
     if linlog:
         ax.set_xscale("symlog", linthresh=linthresh)
+        ax.xaxis.set_minor_locator(MinorSymLogLocator(linthresh))
 
 
 def plot_rsv_residual(
     res: xr.Dataset,
     ax: Axis,
     indices: Sequence[int] = range(2),
     cycler: Cycler | None = PlotStyle().cycler,
```

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/plot_traces.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/plot_traces.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import TYPE_CHECKING
 from warnings import warn
 
 import matplotlib.pyplot as plt
 
 from pyglotaran_extras.io.utils import result_dataset_mapping
 from pyglotaran_extras.plotting.style import PlotStyle
+from pyglotaran_extras.plotting.utils import MinorSymLogLocator
 from pyglotaran_extras.plotting.utils import PlotDuplicationWarning
 from pyglotaran_extras.plotting.utils import add_cycler_if_not_none
 from pyglotaran_extras.plotting.utils import add_unique_figure_legend
 from pyglotaran_extras.plotting.utils import extract_dataset_scale
 from pyglotaran_extras.plotting.utils import extract_irf_location
 from pyglotaran_extras.plotting.utils import select_plot_wavelengths
 
@@ -93,14 +94,15 @@
             result_data = result_data.assign_coords(time=result_data.coords["time"] - irf_loc)
             (result_data.data / scale).plot(x="time", ax=axis, label=f"{dataset_name}_data")
             (result_data.fitted_data / scale).plot(x="time", ax=axis, label=f"{dataset_name}_fit")
         else:
             [next(axis._get_lines.prop_cycler) for _ in range(2)]
     if linlog:
         axis.set_xscale("symlog", linthresh=linthresh)
+        axis.xaxis.set_minor_locator(MinorSymLogLocator(linthresh))
     if show_zero_line is True:
         axis.axhline(0, color="k", linewidth=1)
     axis.set_ylabel(y_label)
     if per_axis_legend is True:
         axis.legend()
```

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/style.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/style.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras/plotting/utils.py` & `pyglotaran_extras-0.7.1/pyglotaran_extras/plotting/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 """Module containing plotting utility functionality."""
 from __future__ import annotations
 
+from math import ceil
+from math import log
+from types import MappingProxyType
 from typing import TYPE_CHECKING
 from typing import Iterable
 from warnings import warn
 
 import numpy as np
 import xarray as xr
+from matplotlib.ticker import Locator
 
 from pyglotaran_extras.inspect.utils import pretty_format_numerical_iterable
 from pyglotaran_extras.io.utils import result_dataset_mapping
 
 if TYPE_CHECKING:
+    from typing import Callable
     from typing import Hashable
+    from typing import Literal
+    from typing import Mapping
 
     from cycler import Cycler
     from matplotlib.axis import Axis
     from matplotlib.figure import Figure
     from matplotlib.pyplot import Axes
 
+    from pyglotaran_extras.types import BuiltinSubPlotLabelFormatFunctionKey
     from pyglotaran_extras.types import ResultLike
+    from pyglotaran_extras.types import SubPlotLabelCoord
 
 
 class PlotDuplicationWarning(UserWarning):
     """Warning given when there are more subplots than datapoints."""
 
 
 def select_irf_dispersion_center_by_index(
@@ -360,14 +369,33 @@
     else:
         raise ValueError(f"No concentrations in result:\n{res}")
 
     irf_location = extract_irf_location(res, center_λ, main_irf_nr)
     return shift_time_axis_by_irf_location(traces, irf_location)
 
 
+def ensure_axes_array(axes: Axis | Axes) -> Axes:
+    """Ensure that axes have flatten method even if it is a single axis.
+
+    Parameters
+    ----------
+    axes: Axis | Axes
+        Axis or Axes to convert for API consistency.
+
+    Returns
+    -------
+    Axes
+        Numpy ndarray of axes.
+    """
+    # We can't use `Axis` in isinstance so we check for the np.ndarray attribute of `Axes`
+    if hasattr(axes, "flatten") is False:
+        axes = np.array([axes])
+    return axes
+
+
 def add_cycler_if_not_none(axis: Axis | Axes, cycler: Cycler | None) -> None:
     """Add cycler to and axis if it is not None.
 
     This is a convenience function that allow to opt out of using
     a cycler, which is needed to run a plotting function in a loop
     where the cycler is controlled from the outside.
 
@@ -376,17 +404,15 @@
     ----------
     axis: Axis | Axes
         Axis to plot on.
     cycler: Cycler | None
         Plot style cycler to use.
     """
     if cycler is not None:
-        # We can't use `Axis` in isinstance so we check for the np.ndarray attribute of `Axes`
-        if hasattr(axis, "flatten") is False:
-            axis = np.array([axis])
+        axis = ensure_axes_array(axis)
         for ax in axis.flatten():
             ax.set_prop_cycle(cycler)
 
 
 def abs_max(
     data: xr.DataArray, *, result_dims: Hashable | Iterable[Hashable] = ()
 ) -> xr.DataArray:
@@ -470,15 +496,244 @@
 
     This helper function is for example used to determine if a data only have a single trace,
     since this requires different plotting code (e.g. ``data_array.plot.line(x="time")``).
 
     Parameters
     ----------
     data_array: xr.DataArray
-        _description_
+        DataArray to check if it has only a single dimension.
 
     Returns
     -------
     list[Hashable]
         Names of dimensions in ``data`` which don't have a size equal to one.
     """
     return [dim for dim, values in data_array.coords.items() if values.size != 1]
+
+
+class MinorSymLogLocator(Locator):
+    """Dynamically find minor tick positions based on major ticks for a symlog scaling.
+
+    Ref.: https://stackoverflow.com/a/45696768
+    """
+
+    def __init__(self, linthresh: float, nints: int = 10) -> None:
+        """Ticks will be placed between the major ticks.
+
+        The placement is linear for x between -linthresh and linthresh,
+        otherwise its logarithmically. nints gives the number of
+        intervals that will be bounded by the minor ticks.
+
+        Parameters
+        ----------
+        linthresh : float
+            A single float which defines the range (-x, x), within which the plot is linear.
+        nints : int
+            Number of minor tick between major ticks. Defaults to 10
+        """
+        self.linthresh = linthresh
+        self.nintervals = nints
+
+    def __call__(self) -> list[float]:
+        """Return the locations of the ticks.
+
+        Returns
+        -------
+        list[float]
+            Minor ticks position.
+        """
+        # Return the locations of the ticks
+        majorlocs = self.axis.get_majorticklocs()
+
+        if len(majorlocs) == 1:
+            return self.raise_if_exceeds(np.array([]))
+
+        # add temporary major tick locs at either end of the current range
+        # to fill in minor tick gaps
+        dmlower = majorlocs[1] - majorlocs[0]  # major tick difference at lower end
+        dmupper = majorlocs[-1] - majorlocs[-2]  # major tick difference at upper end
+
+        # add temporary major tick location at the lower end
+        if majorlocs[0] != 0.0 and (
+            (majorlocs[0] != self.linthresh and dmlower > self.linthresh)
+            or (dmlower == self.linthresh and majorlocs[0] < 0)
+        ):
+            majorlocs = np.insert(majorlocs, 0, majorlocs[0] * 10.0)
+        else:
+            majorlocs = np.insert(majorlocs, 0, majorlocs[0] - self.linthresh)
+
+        # add temporary major tick location at the upper end
+        if majorlocs[-1] != 0.0 and (
+            (np.abs(majorlocs[-1]) != self.linthresh and dmupper > self.linthresh)
+            or (dmupper == self.linthresh and majorlocs[-1] > 0)
+        ):
+            majorlocs = np.append(majorlocs, majorlocs[-1] * 10.0)
+        else:
+            majorlocs = np.append(majorlocs, majorlocs[-1] + self.linthresh)
+
+        # iterate through minor locs
+        minorlocs: list[float] = []
+
+        # handle the lowest part
+        for i in range(1, len(majorlocs)):
+            majorstep = majorlocs[i] - majorlocs[i - 1]
+            if abs(majorlocs[i - 1] + majorstep / 2) < self.linthresh:
+                ndivs = self.nintervals
+            else:
+                ndivs = self.nintervals - 1
+
+            minorstep = majorstep / ndivs
+            locs = np.arange(majorlocs[i - 1], majorlocs[i], minorstep)[1:]
+            minorlocs.extend(locs)
+
+        return self.raise_if_exceeds(np.array(minorlocs))
+
+    def tick_values(self, vmin: float, vmax: float) -> None:
+        """Return the values of the located ticks given **vmin** and **vmax** (not implemented).
+
+        Parameters
+        ----------
+        vmin : float
+            Minimum value.
+        vmax : float
+            Maximum value.
+
+        Raises
+        ------
+        NotImplementedError
+            Not used
+        """
+        raise NotImplementedError(f"Cannot get tick locations for a {type(self)} type.")
+
+
+def format_sub_plot_number_upper_case_letter(sub_plot_number: int, size: None | int = None) -> str:
+    """Format ``sub_plot_number`` into an upper case letter, that can be used as label.
+
+    Parameters
+    ----------
+    sub_plot_number : int
+        Number of the subplot starting at One.
+    size : None | int
+        Size of the axes array (number of plots). Defaults to None
+
+    Returns
+    -------
+    str
+        Upper case label for a sub plot.
+
+    Examples
+    --------
+    >>> print(format_sub_plot_number_upper_case_letter(1))
+    A
+
+    >>> print(format_sub_plot_number_upper_case_letter(26))
+    Z
+
+    >>> print(format_sub_plot_number_upper_case_letter(27))
+    AA
+
+    >>> print(format_sub_plot_number_upper_case_letter(1, 26))
+    AA
+
+    >>> print(format_sub_plot_number_upper_case_letter(2, 26))
+    AB
+
+    >>> print(format_sub_plot_number_upper_case_letter(26, 26))
+    AZ
+
+    >>> print(format_sub_plot_number_upper_case_letter(27, 50))
+    BA
+
+    See Also
+    --------
+    BuiltinLabelFormatFunctions
+    add_subplot_labels
+    """
+    sub_plot_number -= 1
+    if size is not None and size > 26:
+        return "".join(
+            format_sub_plot_number_upper_case_letter(((sub_plot_number // (26**i)) % 26) + 1)
+            for i in reversed(range(1, ceil(log(size, 26))))
+        ) + format_sub_plot_number_upper_case_letter((sub_plot_number % 26) + 1)
+    if sub_plot_number < 26:
+        return chr(ord("A") + sub_plot_number)
+    return format_sub_plot_number_upper_case_letter(
+        sub_plot_number // 26
+    ) + format_sub_plot_number_upper_case_letter((sub_plot_number % 26) + 1)
+
+
+BuiltinSubPlotLabelFormatFunctions: Mapping[
+    str, Callable[[int, int | None], str]
+] = MappingProxyType(
+    {
+        "number": lambda x, y: f"{x}",
+        "upper_case_letter": format_sub_plot_number_upper_case_letter,
+        "lower_case_letter": lambda x, y: format_sub_plot_number_upper_case_letter(x, y).lower(),
+    }
+)
+
+
+def get_subplot_label_format_function(
+    format_function: BuiltinSubPlotLabelFormatFunctionKey | Callable[[int, int | None], str]
+) -> Callable[[int, int | None], str]:
+    """Get subplot label function from ``BuiltinSubPlotLabelFormatFunctions`` if it is a key.
+
+    This function is mainly needed for typing reasons.
+
+    Parameters
+    ----------
+    format_function : BuiltinSubPlotLabelFormatFunctionKey | Callable[[int, int  |  None], str]
+        Key ``BuiltinSubPlotLabelFormatFunctions`` to retrieve builtin function or user defined
+        format function.
+
+    Returns
+    -------
+    Callable[[int, int | None], str]
+        Function to format subplot label.
+    """
+    if isinstance(format_function, str) and format_function in BuiltinSubPlotLabelFormatFunctions:
+        return BuiltinSubPlotLabelFormatFunctions[format_function]
+    return format_function  # type:ignore[return-value]
+
+
+def add_subplot_labels(
+    axes: Axis | Axes,
+    *,
+    label_position: tuple[float, float] = (-0.05, 1.05),
+    label_coords: SubPlotLabelCoord = "axes fraction",
+    direction: Literal["row", "column"] = "row",
+    label_format_template: str = "{}",
+    label_format_function: BuiltinSubPlotLabelFormatFunctionKey
+    | Callable[[int, int | None], str] = "number",
+    fontsize: int = 16,
+) -> None:
+    """Add labels to all subplots in ``axes`` in a consistent manner.
+
+    Parameters
+    ----------
+    axes : Axis | Axes
+        Axes (subplots) on which the labels should be added.
+    label_position : tuple[float, float]
+        Position of the label in ``label_coords`` coordinates.
+    label_coords : SubPlotLabelCoord
+        Coordinate system used for ``label_position``. Defaults to "axes fraction"
+    direction : Literal["row", "column"]
+        Direct in which the axes should be iterated in. Defaults to "row"
+    label_format_template : str
+        Template string to inject the return value of ``label_format_function`` into.
+        Defaults to "{}"
+    label_format_function : BuiltinSubPlotLabelFormatFunctionKey | Callable[[int, int | None], str]
+        Function to calculate the label for the axis index and ``axes`` size. Defaults to "number"
+    fontsize : int
+        Font size used for the label. Defaults to 16
+    """
+    axes = ensure_axes_array(axes)
+    format_function = get_subplot_label_format_function(label_format_function)
+    if direction == "column":
+        axes = axes.T
+    for i, ax in enumerate(axes.flatten(), start=1):
+        ax.annotate(
+            label_format_template.format(format_function(i, axes.size)),
+            xy=label_position,
+            xycoords=label_coords,
+            fontsize=fontsize,
+        )
```

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/PKG-INFO` & `pyglotaran_extras-0.7.1/pyglotaran_extras.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,78 @@
 Metadata-Version: 2.1
 Name: pyglotaran-extras
-Version: 0.7.0
+Version: 0.7.1
 Summary: Supplementary package for pyglotaran with (example) plotting code.
 Home-page: https://github.com/glotaran/pyglotaran-extras
 Author: Joris Snellenburg
 Author-email: j.snellenburg@gmail.com
 License: MIT
 Project-URL: GloTarAn Ecosystem, https://glotaran.org
 Project-URL: Documentation, https://pyglotaran-extras.readthedocs.io
 Project-URL: Changelog, https://pyglotaran-extras.readthedocs.io/en/latest/changelog.html
 Project-URL: Source, https://github.com/glotaran/pyglotaran-extras
 Project-URL: Tracker, https://github.com/glotaran/pyglotaran-extras/issues
-Description: # pyglotaran-extras
-        
-        [![PyPI version](https://badge.fury.io/py/pyglotaran-extras.svg)](https://badge.fury.io/py/pyglotaran-extras)
-        [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pyglotaran-extras.svg)](https://anaconda.org/conda-forge/pyglotaran-extras)
-        [![Tests](https://github.com/glotaran/pyglotaran-extras/actions/workflows/test.yml/badge.svg)](https://github.com/glotaran/pyglotaran-extras/actions/workflows/test.yml)
-        [![Documentation Status](https://readthedocs.org/projects/pyglotaran-extras/badge/?version=latest)](https://pyglotaran-extras.readthedocs.io/en/latest/?badge=latest)
-        [![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/glotaran/pyglotaran-extras.git/main?urlpath=lab%2Ftree%2Fdocs%2Fsource%2Fnotebooks)
-        
-        [![codecov](https://codecov.io/gh/glotaran/pyglotaran-extras/branch/main/graph/badge.svg?token=I6F412Y390)](https://codecov.io/gh/glotaran/pyglotaran-extras)
-        [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/glotaran/pyglotaran-extras.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/glotaran/pyglotaran-extras/context:python)
-        [![Code style Python: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![Discord](https://img.shields.io/discord/883443835135475753.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/KfnEYRSTJx)
-        
-        Supplementary package for pyglotaran with (example) plotting code for use with the pyglotaran package.
-        Can be installed as a python package or from sources.
-        
-        ## Installation
-        
-        Prerequisites:
-        
-        - Python 3.8 or 3.9
-        - Python package `pyglotaran` v0.3.0 (or later)
-        
-        ### Stable Release
-        
-        To install pyglotaran-extras from [PyPI](https://pypi.org/), run this command in your terminal:
-        
-        ```console
-        pip install pyglotaran-extras
-        ```
-        
-        If you want to install it via conda, you can run the following command:
-        
-        ```console
-        conda install -c conda-forge pyglotaran-extras
-        ```
-        
-        ### From Source
-        
-        To install pyglotaran-extras from sources, either clone this repository or download the latest release, then run this command in your terminal:
-        
-        ```console
-        git clone https://github.com/glotaran/pyglotaran-extras.git
-        cd pyglotaran-extras
-        pip install -e .
-        ```
-        
-        or directly
-        
-        ```console
-        pip install git+https://github.com/glotaran/pyglotaran-extras.git
-        ```
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyglotaran-extras
+
+[![PyPI version](https://badge.fury.io/py/pyglotaran-extras.svg)](https://badge.fury.io/py/pyglotaran-extras)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/pyglotaran-extras.svg)](https://anaconda.org/conda-forge/pyglotaran-extras)
+[![Tests](https://github.com/glotaran/pyglotaran-extras/actions/workflows/test.yml/badge.svg)](https://github.com/glotaran/pyglotaran-extras/actions/workflows/test.yml)
+[![Documentation Status](https://readthedocs.org/projects/pyglotaran-extras/badge/?version=latest)](https://pyglotaran-extras.readthedocs.io/en/latest/?badge=latest)
+[![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/glotaran/pyglotaran-extras.git/main?urlpath=lab%2Ftree%2Fdocs%2Fsource%2Fnotebooks)
+
+[![codecov](https://codecov.io/gh/glotaran/pyglotaran-extras/branch/main/graph/badge.svg?token=I6F412Y390)](https://codecov.io/gh/glotaran/pyglotaran-extras)
+[![Code style Python: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Discord](https://img.shields.io/discord/883443835135475753.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/KfnEYRSTJx)
+
+Supplementary package for pyglotaran with (example) plotting code for use with the pyglotaran package.
+Can be installed as a python package or from sources.
+
+## Installation
+
+Prerequisites:
+
+- Python 3.8, 3.9 or 3.10
+- Python package `pyglotaran` v0.6.0 (or later)
+
+### Stable Release
+
+To install pyglotaran-extras from [PyPI](https://pypi.org/), run this command in your terminal:
+
+```console
+pip install pyglotaran-extras
+```
+
+If you want to install it via conda, you can run the following command:
+
+```console
+conda install -c conda-forge pyglotaran-extras
+```
+
+### From Source
+
+To install pyglotaran-extras from sources, either clone this repository or download the latest release, then run this command in your terminal:
+
+```console
+git clone https://github.com/glotaran/pyglotaran-extras.git
+cd pyglotaran-extras
+pip install -e .
+```
+
+or directly
+
+```console
+pip install git+https://github.com/glotaran/pyglotaran-extras.git
+```
```

### Comparing `pyglotaran_extras-0.7.0/pyglotaran_extras.egg-info/SOURCES.txt` & `pyglotaran_extras-0.7.1/pyglotaran_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/pyproject.toml` & `pyglotaran_extras-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/setup.cfg` & `pyglotaran_extras-0.7.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -4,25 +4,23 @@
 description = Supplementary package for pyglotaran with (example) plotting code.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/glotaran/pyglotaran-extras
 author = Joris Snellenburg
 author_email = j.snellenburg@gmail.com
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3 :: Only
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Chemistry
 	Topic :: Scientific/Engineering :: Physics
 project_urls = 
 	GloTarAn Ecosystem=https://glotaran.org
 	Documentation=https://pyglotaran-extras.readthedocs.io
 	Changelog=https://pyglotaran-extras.readthedocs.io/en/latest/changelog.html
@@ -34,15 +32,15 @@
 install_requires = 
 	cycler>=0.10
 	matplotlib>=3.3.0
 	numpy>=1.21.2,<1.24
 	pyglotaran>=0.6
 	tabulate>=0.8.9
 	xarray>=2022.3.0
-python_requires = >=3.8,<3.11
+python_requires = >=3.8
 zip_safe = True
 
 [options.packages.find]
 include = 
 	pyglotaran_extras
 	pyglotaran_extras.*
```

### Comparing `pyglotaran_extras-0.7.0/tests/conftest.py` & `pyglotaran_extras-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/data/a_matrix/a_matrix_to_html_table_decimal_2.md` & `pyglotaran_extras-0.7.1/tests/data/a_matrix/a_matrix_to_html_table_decimal_2.md`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/data/a_matrix/a_matrix_to_html_table_default.md` & `pyglotaran_extras-0.7.1/tests/data/a_matrix/a_matrix_to_html_table_default.md`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/data/a_matrix/a_matrix_to_html_table_normalized.md` & `pyglotaran_extras-0.7.1/tests/data/a_matrix/a_matrix_to_html_table_normalized.md`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_decimal_2.md` & `pyglotaran_extras-0.7.1/tests/data/a_matrix/show_a_matrixes_decimal_2.md`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_default.md` & `pyglotaran_extras-0.7.1/tests/data/a_matrix/show_a_matrixes_default.md`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_expanded_dataset_2.md` & `pyglotaran_extras-0.7.1/tests/data/a_matrix/show_a_matrixes_expanded_dataset_2.md`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_heading_offset_0.md` & `pyglotaran_extras-0.7.1/tests/data/a_matrix/show_a_matrixes_heading_offset_0.md`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_min_size_2.md` & `pyglotaran_extras-0.7.1/tests/data/a_matrix/show_a_matrixes_min_size_2.md`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_multiple_a_matrixes_in_dataset.md` & `pyglotaran_extras-0.7.1/tests/data/a_matrix/show_a_matrixes_multiple_a_matrixes_in_dataset.md`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/data/a_matrix/show_a_matrixes_normalized.md` & `pyglotaran_extras-0.7.1/tests/data/a_matrix/show_a_matrixes_normalized.md`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/deprecation/test_deprecation_utils.py` & `pyglotaran_extras-0.7.1/tests/deprecation/test_deprecation_utils.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/inspect/test_a_matrix.py` & `pyglotaran_extras-0.7.1/tests/inspect/test_a_matrix.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/inspect/test_utils.py` & `pyglotaran_extras-0.7.1/tests/inspect/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/io/test_get_script_dir.ipynb` & `pyglotaran_extras-0.7.1/tests/io/test_get_script_dir.ipynb`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/io/test_load_data.py` & `pyglotaran_extras-0.7.1/tests/io/test_load_data.py`

 * *Files identical despite different names*

### Comparing `pyglotaran_extras-0.7.0/tests/io/test_setup_case_study.py` & `pyglotaran_extras-0.7.1/tests/io/test_setup_case_study.py`

 * *Files identical despite different names*

