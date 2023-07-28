# Comparing `tmp/seveno-pyutil-0.8.4.tar.gz` & `tmp/seveno-pyutil-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seveno-pyutil-0.8.4.tar", last modified: Wed Jul 26 13:07:08 2023, max compression
+gzip compressed data, was "seveno-pyutil-0.8.5.tar", last modified: Fri Jul 28 09:46:05 2023, max compression
```

## Comparing `seveno-pyutil-0.8.4.tar` & `seveno-pyutil-0.8.5.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.365502 seveno-pyutil-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-26 13:07:08.365502 seveno-pyutil-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.357502 seveno-pyutil-0.8.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.361502 seveno-pyutil-0.8.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.361502 seveno-pyutil-0.8.4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/examples_and_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:07:08.365502 seveno-pyutil-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.357502 seveno-pyutil-0.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.361502 seveno-pyutil-0.8.4/src/seveno_pyutil/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/benchmarking_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/collections_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/datetime_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/error_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/file_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.365502 seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/pretty_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/sql_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/metaprogramming_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/os_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/string_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.361502 seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-26 13:07:08.000000 seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-26 13:07:08.000000 seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:07:08.000000 seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:07:08.000000 seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-26 13:07:08.000000 seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 13:07:08.000000 seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.365502 seveno-pyutil-0.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/benchmarking_utilities_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/collections_utilities_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/datetime_utilities_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/error_utilities_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/file_utilities_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.365502 seveno-pyutil-0.8.4/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/metaprograming_helpers_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/string_utilities_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:46:05.810467 seveno-pyutil-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-28 09:46:05.810467 seveno-pyutil-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:46:05.802467 seveno-pyutil-0.8.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:46:05.802467 seveno-pyutil-0.8.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:46:05.802467 seveno-pyutil-0.8.5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/docs/examples_and_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:46:05.810467 seveno-pyutil-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:46:05.802467 seveno-pyutil-0.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:46:05.806467 seveno-pyutil-0.8.5/src/seveno_pyutil/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/src/seveno_pyutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/src/seveno_pyutil/benchmarking_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/src/seveno_pyutil/collections_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/src/seveno_pyutil/datetime_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/src/seveno_pyutil/error_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/src/seveno_pyutil/file_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:46:05.806467 seveno-pyutil-0.8.5/src/seveno_pyutil/logging_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/src/seveno_pyutil/logging_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/src/seveno_pyutil/logging_utilities/pretty_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15952 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/src/seveno_pyutil/logging_utilities/sql_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/src/seveno_pyutil/logging_utilities/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/src/seveno_pyutil/metaprogramming_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/src/seveno_pyutil/os_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/src/seveno_pyutil/string_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:46:05.806467 seveno-pyutil-0.8.5/src/seveno_pyutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-28 09:46:05.000000 seveno-pyutil-0.8.5/src/seveno_pyutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-28 09:46:05.000000 seveno-pyutil-0.8.5/src/seveno_pyutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:46:05.000000 seveno-pyutil-0.8.5/src/seveno_pyutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:46:05.000000 seveno-pyutil-0.8.5/src/seveno_pyutil.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-28 09:46:05.000000 seveno-pyutil-0.8.5/src/seveno_pyutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 09:46:05.000000 seveno-pyutil-0.8.5/src/seveno_pyutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:46:05.806467 seveno-pyutil-0.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/tests/benchmarking_utilities_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/tests/collections_utilities_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/tests/datetime_utilities_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/tests/error_utilities_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/tests/file_utilities_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:46:05.806467 seveno-pyutil-0.8.5/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/tests/metaprograming_helpers_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/tests/string_utilities_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-28 09:45:51.000000 seveno-pyutil-0.8.5/tests/test_helpers.py
```

### Comparing `seveno-pyutil-0.8.4/CHANGELOG.md` & `seveno-pyutil-0.8.5/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 0.8.4 (2023-07-28)
+
+- feat: removed SQL duration threshold warning
+- feat: support logging of compiled SQL statements on psycopg3
+
 ## 0.8.4 (2023-07-26)
 
 - fix: don't rely on json to be able to encode SQL parameters
 
 ## 0.8.3 (2023-06-26)
 
 - build: added GitHub action for publishing releases to PyPi
```

### Comparing `seveno-pyutil-0.8.4/LICENSE` & `seveno-pyutil-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/PKG-INFO` & `seveno-pyutil-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seveno-pyutil
-Version: 0.8.4
+Version: 0.8.5
 Summary: Various unsorted Python utilities
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/seveno_pyutil
 Project-URL: Documentation, https://seveno-pyutil.readthedocs.io/en/latest/
 Keywords: utilities
 Platform: any
```

### Comparing `seveno-pyutil-0.8.4/README.md` & `seveno-pyutil-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/docs/CHANGELOG.md` & `seveno-pyutil-0.8.5/docs/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 0.8.4 (2023-07-28)
+
+- feat: removed SQL duration threshold warning
+- feat: support logging of compiled SQL statements on psycopg3
+
 ## 0.8.4 (2023-07-26)
 
 - fix: don't rely on json to be able to encode SQL parameters
 
 ## 0.8.3 (2023-06-26)
 
 - build: added GitHub action for publishing releases to PyPi
```

### Comparing `seveno-pyutil-0.8.4/docs/Makefile` & `seveno-pyutil-0.8.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/docs/api.rst` & `seveno-pyutil-0.8.5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/docs/conf.py` & `seveno-pyutil-0.8.5/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import datetime
 
 author = "tadams42"
 project = "seveno-pyutil"
 copyright = (
     ", ".join(str(y) for y in range(2017, datetime.now().year + 1)) + ", " + author
 )
-release = "0.8.4"
+release = "0.8.5"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
```

### Comparing `seveno-pyutil-0.8.4/docs/examples_and_usage.rst` & `seveno-pyutil-0.8.5/docs/examples_and_usage.rst`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/docs/make.bat` & `seveno-pyutil-0.8.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/pyproject.toml` & `seveno-pyutil-0.8.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "seveno-pyutil"
-version = "0.8.4"
+version = "0.8.5"
 description = "Various unsorted Python utilities"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"Intended Audience :: Developers",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `seveno-pyutil-0.8.4/src/seveno_pyutil/__init__.py` & `seveno-pyutil-0.8.5/src/seveno_pyutil/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.4"
+__version__ = "0.8.5"
 
 import logging
 
 from .benchmarking_utilities import Stopwatch
 from .collections_utilities import in_batches
 from .datetime_utilities import ensure_tzinfo, iter_year_month
 from .error_utilities import ExceptionsAsErrors, add_error_to
```

### Comparing `seveno-pyutil-0.8.4/src/seveno_pyutil/benchmarking_utilities.py` & `seveno-pyutil-0.8.5/src/seveno_pyutil/benchmarking_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/src/seveno_pyutil/collections_utilities.py` & `seveno-pyutil-0.8.5/src/seveno_pyutil/collections_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/src/seveno_pyutil/datetime_utilities.py` & `seveno-pyutil-0.8.5/src/seveno_pyutil/datetime_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/src/seveno_pyutil/error_utilities.py` & `seveno-pyutil-0.8.5/src/seveno_pyutil/error_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/src/seveno_pyutil/file_utilities.py` & `seveno-pyutil-0.8.5/src/seveno_pyutil/file_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/pretty_formatter.py` & `seveno-pyutil-0.8.5/src/seveno_pyutil/logging_utilities/pretty_formatter.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/sql_filter.py` & `seveno-pyutil-0.8.5/src/seveno_pyutil/logging_utilities/sql_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,46 +4,62 @@
 import json
 import logging
 import timeit
 from dataclasses import dataclass, field
 from datetime import date, datetime, timedelta
 from decimal import Decimal
 from pathlib import Path
-from typing import TYPE_CHECKING, Callable, ClassVar, Final
+from typing import TYPE_CHECKING
 from uuid import UUID
 
 import pygments
 import sqlparse
 
 # from pygments.formatters import TerminalTrueColorFormatter
 from pygments.formatters import Terminal256Formatter
 from pygments.lexers import SqlLexer
 
+HAS_PSYCOPG2 = False
+
+try:
+    import psycopg2
+
+    HAS_PSYCOPG2 = True
+except Exception:
+    pass
+
+HAS_PSYCOPG3 = False
+try:
+    import psycopg
+
+    HAS_PSYCOPG3 = True
+except Exception:
+    pass
+
 HAS_FLASK = False
 try:
     import flask
 
     HAS_FLASK = True
 except Exception:
     pass
 
-if TYPE_CHECKING:
-    from sqlalchemy.engine import Connection, Engine
-
 
 class SQLFilter(logging.Filter):
     """
     Filter for SQLAlchemy SQL loggers. Optionally reformats and colorizes queries.
 
-    To use it with SQLAlchemy:
+    To use it with Flask and SQLAlchemy:
 
-    - add it to ``sqlalchemy.engine`` logger and call
-      `:meth:register_sqlalchemy_logging_events`
+    - configure Flask app
+    - configure SQLAlchemy engine events (call `:meth:register_sqlalchemy_logging_events`)
+    - configure logging
 
-    Supports following logging placeholders:
+    All three steps are presented in example below. After it has been configured,
+    provides following logging placeholders:
 
     +-------------------+----------------------------------------------+
     | placeholder       | description                                  |
     +-------------------+----------------------------------------------+
     | %(sql)s           | Formatted SQL statement that was executed    |
     +-------------------+----------------------------------------------+
     | %(sql_duration)s  | Formatted duration of SQL execution          |
@@ -58,118 +74,106 @@
             pain and should be avoided.
 
     Example::
 
         import logging
         from logging.config import dictConfig
 
-        from seveno_pyutil import SQLFilter
+        import flask
+        from seveno_pyutil import FlaskSQLStats, SQLFilter
 
-        try:
-            import sqlalchemy
-            SQLFilter.register_sqlalchemy_logging_events('myapp.db')
-        except ImportError:
-            pass
-
-        dictConfig({
-            'version': 1,
-            'disable_existing_loggers': False,
-            'formatters': {
-                'sqlalchemy_sql': {'format': '(%(sql_duration)s) %(sql)s %(message)s'}
-            },
-            'filters': {
-                'colored_sql': {
-                    '()': 'seveno_pyutil.SQLFilter'
-                    'colorize_queries': True,
-                    'multiline_queries': True,
-                }
-            },
-            'handlers': {
-                'console_sqlalchemy': {
-                    'class': 'logging.StreamHandler',
-                    'level': 'DEBUG',
-                    'formatter': 'sqlalchemy_sql',
-                    'filters': ['colored_sql'],
-                    'stream': 'ext://sys.stdout'
-                }
-            },
-            'loggers': {
-                'myapp.db': {
-                    'level': 'DEBUG',
-                    'propagate': False,
-                    'handlers': ['console_sqlalchemy']
-                }
+        dictConfig(
+            {
+                "version": 1,
+                "disable_existing_loggers": False,
+                "formatters": {
+                    "app": {"format": "lvl=%(levelname)s msg=%(message)s"},
+                    "app.db": {
+                        "format": "lvl=%(levelname)s, sqld=%(sql_duration)s sql=%(sql)s msg=%(message)s"
+                    },
+                },
+                "filters": {
+                    "colored_sql": {
+                        "()": "seveno_pyutil.SQLFilter",
+                        "colorize_queries": True,
+                        "multiline_queries": True,
+                    }
+                },
+                "handlers": {
+                    "console": {
+                        "class": "logging.StreamHandler",
+                        "level": "DEBUG",
+                        "formatter": "app",
+                        "stream": "ext://sys.stdout",
+                    },
+                    "console_sqlalchemy": {
+                        "class": "logging.StreamHandler",
+                        "level": "DEBUG",
+                        "formatter": "db",
+                        "filters": ["colored_sql"],
+                        "stream": "ext://sys.stdout",
+                    },
+                },
+                "loggers": {
+                    "myapp": {
+                        "level": "INFO",
+                        "propagate": False,
+                        "handlers": ["console"],
+                    },
+                    "myapp.db": {
+                        "level": "DEBUG",
+                        "propagate": False,
+                        "handlers": ["console_sqlalchemy"],
+                    },
+                },
             }
-        })
+        )
 
+
+        class RequestLoggingMiddleware:
+            def __init__(self, sql_logger_name, app=None):
+                self.sql_logger_name = sql_logger_name
+                if app:
+                    self.init_app(app)
+
+            def init_app(self, app: flask.Flask):
+                SQLFilter.register_sqlalchemy_logging_events(self.sql_logger_name)
+
+                @app.before_request
+                def log_current_request():
+                    FlaskSQLStats.open()
+
+                    @flask.after_this_request
+                    def log_current_response(response):
+                        logger.info("Some HTTP request was processed :)")
+                        FlaskSQLStats.close()
+                        return response
+
+
+        logger = logging.getLogger(__name__)
+        app = flask.Flask(__name__)
+        RequestLoggingMiddleware("myapp.db").init_app(app)
     """
 
     @classmethod
-    def register_sqlalchemy_logging_events(
-        cls,
-        logger: str | logging.Logger,
-        duration_threshold_ms: int | float | timedelta | None = None,
-    ):
-        """
-        Must be called when logging SQLAlchemy statements and durations.
-
-        Arguments:
-            logger: name of logger or logging.Logger instance that will be used to log
-                SQL messages.
-            duration_threshold_ms: If given, only queries lasting longer than this
-                threshold will be logged.
-            statistics_ctx_get: callable that returns mutable dict. If given, then each
-                time SQL query is executes, this dict will be updated.
-
-                It can be used for example in Flask to track SQL execution statistics
-                during one HTTP request::
-
-                    import flask
-                    from seveno_pyutil import FlaskSQLStats, SQLFilter
-
-                    SQLFilter.register_sqlalchemy_logging_events(
-                        "may_app_sql_logger", 100
-                    )
-
-                    app = flask.Flask()
-
-                    @app.before_request
-                    def log_current_request():
-                        FlaskSQLStats.open()
-
-                        @flask.after_this_request
-                        def log_current_response(response):
-                            FlaskSQLStats.close()
-                            return response
-        """
-
+    def register_sqlalchemy_logging_events(cls, logger: str | logging.Logger):
         from sqlalchemy import event
         from sqlalchemy.engine import Engine
 
-        connection_enricher = ConnectionEnricher(logger, duration_threshold_ms)
+        connection_enricher = ConnectionEnricher(logger)
 
         @event.listens_for(Engine, "before_cursor_execute")
         def before_cursor_execute(
-            conn: Connection,
-            cursor: "DBAPICursor",
-            statement: str,
-            parameters: dict,
-            context: "ExecutionContext",
-            executemany: bool,
+            conn, cursor, statement: str, parameters: dict, context, executemany: bool
         ):
             connection_enricher.start(conn)
 
         @event.listens_for(Engine, "after_cursor_execute")
         def after_cursor_execute(
-            conn: Connection,
-            cursor: "DBAPICursor",
-            statement: str,
-            parameters: dict,
-            context: "ExecutionContext",
-            executemany: bool,
+            conn, cursor, statement: str, parameters: dict, context, executemany: bool
         ):
             connection_enricher.end(conn, cursor, statement, parameters)
 
         @event.listens_for(Engine, "handle_error")
         def receive_handle_error(exception_context):
             connection_enricher.error(exception_context)
 
@@ -190,82 +194,46 @@
         self.enricher.add_attributes(record)
         return super().filter(record)
 
 
 class ConnectionEnricher:
     _ATTR_START_TIME = "query_start_time"
 
-    def __init__(
-        self,
-        lgr: str | logging.Logger,
-        duration_threshold: int | float | timedelta | None,
-    ):
+    def __init__(self, lgr: str | logging.Logger):
         self.lgr: logging.Logger
         if isinstance(lgr, str):
             self.lgr = logging.getLogger(lgr)
         else:
             self.lgr = lgr
 
-        self.duration_threshold: timedelta | None = None
-        if duration_threshold is not None:
-            if isinstance(duration_threshold, timedelta):
-                self.duration_threshold = duration_threshold
-            else:
-                self.duration_threshold = timedelta(milliseconds=duration_threshold)
-
     def start(self, conn: Connection | None):
         if conn:
             conn.info.setdefault(self._ATTR_START_TIME, []).append(
                 timeit.default_timer()
             )
 
     def end(
         self, conn: Connection, cursor: "DBAPICursor", statement: str, parameters: dict
     ):
         statement_duration = self._execution_duration(conn)
         FlaskSQLStats.incr_stats(self.lgr, statement_duration)
 
-        compiled = None
-        try:
-            compiled = cursor.mogrify(statement, parameters).decode()
-        except Exception:
-            compiled = None
-
-        warned = False
-        if (
-            self.duration_threshold is not None
-            and statement_duration >= self.duration_threshold
-        ):
-            self.lgr.warning(
-                "Detected SQL query running longer than {:.2f} ms! ".format(
-                    self.duration_threshold.total_seconds() * 1000
-                ),
-                extra={
-                    RecordEnricher.ATTR_DATA: SQLRecordedQuery(
-                        statement=str(statement),
-                        parameters=parameters,
-                        duration=statement_duration,
-                        compiled=compiled,
-                    )
-                },
-            )
-            warned = True
+        compiled = self._compiled_sql(conn, cursor, statement, parameters)
 
-        if not warned and statement_duration is not None:
-            self.lgr.debug(
-                "",
-                extra={
-                    RecordEnricher.ATTR_DATA: SQLRecordedQuery(
-                        statement=str(statement),
-                        parameters=parameters,
-                        duration=statement_duration,
-                        compiled=compiled,
-                    )
-                },
-            )
+        self.lgr.debug(
+            "",
+            extra={
+                RecordEnricher.ATTR_DATA: SQLRecordedQuery(
+                    statement=str(statement),
+                    parameters=parameters,
+                    duration=statement_duration,
+                    compiled=compiled,
+                )
+            },
+        )
 
     def error(self, exception_context):
         msg = "SQL engine exception detected."
 
         try:
             msg = msg + " " + str(exception_context.original_exception).strip()
         except Exception:
@@ -279,14 +247,40 @@
                     parameters=exception_context.parameters,
                     duration=self._execution_duration(exception_context.connection),
                 )
             },
         )
 
     @classmethod
+    def _compiled_sql(cls, conn, cursor, statement, parameters):
+        compiled = None
+
+        if HAS_PSYCOPG2:
+            try:
+                compiled = cursor.mogrify(statement, parameters).decode()
+            except Exception:
+                pass
+
+        elif HAS_PSYCOPG3:
+            try:
+                cc = psycopg.ClientCursor(connection=conn.connection.dbapi_connection)
+                compiled = cc.mogrify(statement, parameters)
+            except Exception:
+                pass
+
+        # Other drivers would need their own implementation. Since we are not using
+        # them, we don't provide one. Returning None here means SQL will be logged
+        # separately from it's parameters, ie.
+        #   sql=SELECT id, foo FROM foos where foo = %(bar)s; with params {"bar": baz}
+        # instead of
+        #   sql=SELECT id, foo FROM foos where foo = 'baz'
+
+        return compiled
+
+    @classmethod
     def _execution_duration(cls, conn: Connection | None) -> timedelta:
         data: list[float] = getattr(conn, "info", dict()).get(cls._ATTR_START_TIME, [])
         started_at = data.pop(-1) if data else 0
         return timedelta(milliseconds=(timeit.default_timer() - started_at) * 1000.0)
 
 
 @dataclass
```

### Comparing `seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py` & `seveno-pyutil-0.8.5/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/utilities.py` & `seveno-pyutil-0.8.5/src/seveno_pyutil/logging_utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/src/seveno_pyutil/metaprogramming_helpers.py` & `seveno-pyutil-0.8.5/src/seveno_pyutil/metaprogramming_helpers.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/src/seveno_pyutil/os_utilities.py` & `seveno-pyutil-0.8.5/src/seveno_pyutil/os_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/PKG-INFO` & `seveno-pyutil-0.8.5/src/seveno_pyutil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seveno-pyutil
-Version: 0.8.4
+Version: 0.8.5
 Summary: Various unsorted Python utilities
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/seveno_pyutil
 Project-URL: Documentation, https://seveno-pyutil.readthedocs.io/en/latest/
 Keywords: utilities
 Platform: any
```

### Comparing `seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/SOURCES.txt` & `seveno-pyutil-0.8.5/src/seveno_pyutil.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .bumpversion.cfg
+.pre-commit-config.yaml
 .readthedocs.yml
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
```

### Comparing `seveno-pyutil-0.8.4/tests/collections_utilities_spec.py` & `seveno-pyutil-0.8.5/tests/collections_utilities_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/tests/datetime_utilities_spec.py` & `seveno-pyutil-0.8.5/tests/datetime_utilities_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/tests/error_utilities_spec.py` & `seveno-pyutil-0.8.5/tests/error_utilities_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/tests/metaprograming_helpers_spec.py` & `seveno-pyutil-0.8.5/tests/metaprograming_helpers_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.4/tests/string_utilities_spec.py` & `seveno-pyutil-0.8.5/tests/string_utilities_spec.py`

 * *Files identical despite different names*

