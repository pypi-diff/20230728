# Comparing `tmp/pdstools-3.1.9.tar.gz` & `tmp/pdstools-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdstools-3.1.9.tar", last modified: Fri May 19 15:41:18 2023, max compression
+gzip compressed data, was "pdstools-3.2.tar", last modified: Fri Jul 28 14:48:21 2023, max compression
```

## Comparing `pdstools-3.1.9.tar` & `pdstools-3.2.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.858224 pdstools-3.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 15:41:09.000000 pdstools-3.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-19 15:41:18.858224 pdstools-3.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-19 15:41:09.000000 pdstools-3.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/pdstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-19 15:41:18.000000 pdstools-3.1.9/pdstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-19 15:41:18.000000 pdstools-3.1.9/pdstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:41:18.000000 pdstools-3.1.9/pdstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 15:41:18.000000 pdstools-3.1.9/pdstools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-19 15:41:18.000000 pdstools-3.1.9/pdstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 15:41:18.000000 pdstools-3.1.9/pdstools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-19 15:41:09.000000 pdstools-3.1.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.850224 pdstools-3.1.9/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/adm/
--rw-r--r--   0 runner    (1001) docker     (123)    56340 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/adm/ADMDatamart.py
--rw-r--r--   0 runner    (1001) docker     (123)    40060 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/adm/ADMTrees.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/adm/Tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/adm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/app/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/app/Home.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/app/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/app/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/app/pages/Health Check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/ih/
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/ih/IHAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/ih/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15083 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/ih/legacy_IH.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/pega_io/
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/pega_io/API.py
--rw-r--r--   0 runner    (1001) docker     (123)    14118 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/pega_io/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/pega_io/S3.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/pega_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50996 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/plots/plot_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/plots/plots_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.854224 pdstools-3.1.9/python/pdstools/reports/
--rw-r--r--   0 runner    (1001) docker     (123)    40080 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/reports/HealthCheck.qmd
--rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/reports/HealthCheckModel.qmd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.858224 pdstools-3.1.9/python/pdstools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21567 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/cdh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/hds_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/pega_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/polars_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/show_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/streamlit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/table_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:18.858224 pdstools-3.1.9/python/pdstools/valuefinder/
--rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/valuefinder/ValueFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:41:09.000000 pdstools-3.1.9/python/pdstools/valuefinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 15:41:18.858224 pdstools-3.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:21.546279 pdstools-3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 14:48:09.000000 pdstools-3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-07-28 14:48:21.546279 pdstools-3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-28 14:48:09.000000 pdstools-3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:21.538279 pdstools-3.2/pdstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-07-28 14:48:21.000000 pdstools-3.2/pdstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-28 14:48:21.000000 pdstools-3.2/pdstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:48:21.000000 pdstools-3.2/pdstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 14:48:21.000000 pdstools-3.2/pdstools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-28 14:48:21.000000 pdstools-3.2/pdstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 14:48:21.000000 pdstools-3.2/pdstools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-28 14:48:09.000000 pdstools-3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:21.538279 pdstools-3.2/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:21.538279 pdstools-3.2/python/pdstools/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:21.542279 pdstools-3.2/python/pdstools/adm/
+-rw-r--r--   0 runner    (1001) docker     (123)    56117 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/adm/ADMDatamart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40061 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/adm/ADMTrees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/adm/Tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/adm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:21.542279 pdstools-3.2/python/pdstools/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/app/Home.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/app/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:21.542279 pdstools-3.2/python/pdstools/app/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/app/pages/Health Check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:21.542279 pdstools-3.2/python/pdstools/ih/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/ih/IHAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/ih/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15083 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/ih/legacy_IH.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:21.542279 pdstools-3.2/python/pdstools/pega_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/pega_io/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14118 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/pega_io/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/pega_io/S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/pega_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:21.542279 pdstools-3.2/python/pdstools/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50978 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/plots/plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29750 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/plots/plots_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:21.542279 pdstools-3.2/python/pdstools/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/reports/HealthCheck.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)    29444 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/reports/HealthCheckModel.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:21.546279 pdstools-3.2/python/pdstools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21558 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/utils/cdh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18245 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/utils/hds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22413 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/utils/hds_utils_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/utils/pega_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/utils/polars_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/utils/show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/utils/streamlit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/utils/table_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:21.546279 pdstools-3.2/python/pdstools/valuefinder/
+-rw-r--r--   0 runner    (1001) docker     (123)    24603 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/valuefinder/ValueFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:09.000000 pdstools-3.2/python/pdstools/valuefinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 14:48:09.000000 pdstools-3.2/python/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 14:48:21.546279 pdstools-3.2/setup.cfg
```

### Comparing `pdstools-3.1.9/LICENSE` & `pdstools-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/PKG-INFO` & `pdstools-3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.1.9
+Version: 3.2
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.1.9 Summary: Open source
-tooling that helps Data Scientists to analyze Pega models and conduct impactful
+Metadata-Version: 2.1 Name: pdstools Version: 3.2 Summary: Open source tooling
+that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
 pega,pegasystems,pds,pdstools,cdhtools,datascientist,tools Classifier: License
```

### Comparing `pdstools-3.1.9/README.md` & `pdstools-3.2/README.md`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/pdstools.egg-info/PKG-INFO` & `pdstools-3.2/pdstools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.1.9
+Version: 3.2
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.1.9 Summary: Open source
-tooling that helps Data Scientists to analyze Pega models and conduct impactful
+Metadata-Version: 2.1 Name: pdstools Version: 3.2 Summary: Open source tooling
+that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
 pega,pegasystems,pds,pdstools,cdhtools,datascientist,tools Classifier: License
```

### Comparing `pdstools-3.1.9/pdstools.egg-info/SOURCES.txt` & `pdstools-3.2/pdstools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 pdstools.egg-info/PKG-INFO
 pdstools.egg-info/SOURCES.txt
 pdstools.egg-info/dependency_links.txt
 pdstools.egg-info/entry_points.txt
 pdstools.egg-info/requires.txt
 pdstools.egg-info/top_level.txt
+python/requirements.txt
 python/pdstools/__init__.py
 python/pdstools/adm/ADMDatamart.py
 python/pdstools/adm/ADMTrees.py
 python/pdstools/adm/Tables.py
 python/pdstools/adm/__init__.py
 python/pdstools/app/Home.py
 python/pdstools/app/__init__.py
@@ -30,14 +31,15 @@
 python/pdstools/reports/HealthCheckModel.qmd
 python/pdstools/reports/__init__.py
 python/pdstools/utils/__init__.py
 python/pdstools/utils/cdh_utils.py
 python/pdstools/utils/datasets.py
 python/pdstools/utils/errors.py
 python/pdstools/utils/hds_utils.py
+python/pdstools/utils/hds_utils_experimental.py
 python/pdstools/utils/pega_template.py
 python/pdstools/utils/polars_ext.py
 python/pdstools/utils/show_versions.py
 python/pdstools/utils/streamlit_utils.py
 python/pdstools/utils/table_definitions.py
 python/pdstools/utils/types.py
 python/pdstools/valuefinder/ValueFinder.py
```

### Comparing `pdstools-3.1.9/pyproject.toml` & `pdstools-3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 exclude = ['/tests/*', '*.dist-info', '/docs/*']
 
 [tool.setuptools.package-data]
 "*" = ['*.qmd']
 
 [project]
 name = "pdstools"
-dynamic = ["version"]
+dynamic = ["version", "dependencies"]
 description = "Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses."
 readme = "README.md"
 authors = [ { name = "Stijn Kas", email = "stijn.kas@pega.com" } ] 
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Development Status :: 4 - Beta",
@@ -28,29 +28,19 @@
     "pegasystems",
     "pds",
     "pdstools",
     "cdhtools",
     "datascientist",
     "tools",
 ]
-dependencies = [
-        "pandas>=1.5.3",
-        "plotly>=5.14.1",
-        "requests",
-        "pydot",
-        "polars>=0.17.14",
-        "pyarrow",
-        "tqdm",
-        "pyyaml",
-        "aioboto3>=11.0"
-    ]
 requires-python = ">=3.8"
 
 [tool.setuptools.dynamic]
 version = {attr="pdstools.__version__"}
+dependencies = {file = ["python/requirements.txt"]}
 
 [project.optional-dependencies]
 docs = ['sphinx','furo','sphinx-autoapi','nbsphinx','sphinx-copybutton','myst-parser']
 app = ['streamlit>=1.20', 'quarto', 'papermill', 'itables', 'jinja2>=3.1', 'xlsxwriter>=3.0']
 
 [project.urls]
 "Homepage" = "https://github.com/pegasystems/pega-datascientist-tools"
```

### Comparing `pdstools-3.1.9/python/pdstools/__init__.py` & `pdstools-3.2/python/pdstools/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Python pdstools"""
 
-__version__ = "3.1.9"
+__version__ = "3.2"
 
 from polars import enable_string_cache
 
 enable_string_cache(True)
 
 import sys
 from pathlib import Path
```

### Comparing `pdstools-3.1.9/python/pdstools/adm/ADMDatamart.py` & `pdstools-3.2/python/pdstools/adm/ADMDatamart.py`

 * *Files 2% similar despite different names*

```diff
@@ -743,30 +743,33 @@
                     raise ValueError("query values must be list")
 
             for col, val in query.items():
                 df = df.filter(pl.col(col).is_in(val))
         return df
 
     def discover_modelTypes(
-        self, df: pl.LazyFrame, by: str = "Configuration"
+        self, df: pl.LazyFrame, by: str = "Configuration", allow_collect=False
     ) -> Dict:  # pragma: no cover
         """Discovers the type of model embedded in the pyModelData column.
 
         By default, we do a groupby Configuration, because a model rule can only
         contain one type of model. Then, for each configuration, we look into the
         pyModelData blob and find the _serialClass, returning it in a dict.
 
         Parameters
         ----------
         df: pl.LazyFrame
             The dataframe to search for model types
         by: str
             The column to look for types in. Configuration is recommended.
+        allow_collect: bool, default = False
+            Set to True to allow discovering modelTypes, even if in lazy strategy.
+            It will fetch one modelData string per configuration.
         """
-        if self.import_strategy != "eager":
+        if self.import_strategy != "eager" and allow_collect == False:
             raise NotEagerError("Discovering AGB models")
         if "Modeldata" not in df.columns:
             raise ValueError(
                 (
                     "Modeldata column not in the data. "
                     "Please make sure to include it by using the 'include_cols' "
                     "argument with your ADMDatamart call, or setting 'subset' to False."
@@ -781,14 +784,15 @@
                 line.split('"')[-2].split(".")[-1]
                 for line in zlib.decompress(base64.b64decode(val)).decode().split("\n")
                 if line.startswith('  "_serialClass"')
             )
 
         if isinstance(df, pl.DataFrame):
             df = df.lazy()
+
         types = (
             df.filter(pl.col("Modeldata").is_not_null())
             .groupby(by)
             .agg(pl.col("Modeldata").last())
             .collect()
             .with_columns(pl.col("Modeldata").apply(lambda v: _getType(v)))
             .to_dicts()
@@ -1042,16 +1046,16 @@
             )
             .fill_null(0.5)
             .fill_nan(0.5)
         )
         mod_order = (
             df.select(
                 pl.concat_list(pl.col(pl.Float64))
-                .arr.eval(pl.element().mean())
-                .arr.get(0)
+                .list.eval(pl.element().mean())
+                .list.get(0)
             )
             .select(pl.all().arg_sort(descending=True))
             .to_series()
         )
         pred_order = [by] + [
             df.columns[i + 1]
             for i in 0
@@ -1104,51 +1108,34 @@
         -------
         pl.LazyFrame
            DataFrame with PositivesBin column and model count statistics
         """
         if self.import_strategy == "lazy" and not allow_collect:
             raise NotEagerError("Models by positive df.")
 
-        def orderedCut(
-            s, label="PositivesBin", bins=list(range(0, 210, 10))
-        ) -> pl.Series:
-            _arg_sort = pl.Series(name="_sort", values=s.arg_sort())
-            result = pl.cut(
-                s, bins=[bins + [float("inf")]][0], category_label="PositivesBin"
-            )
-            return (
-                result.select(
-                    [
-                        pl.col(label),
-                        _arg_sort,
-                    ]
-                )
-                .sort("_sort")
-                .drop("_sort")
-                .to_series()
-            )
-
         modelsByPositives = df.select([by, "Positives", "ModelID"]).collect()
         return (
-            modelsByPositives.hstack(
-                [
-                    orderedCut(
-                        modelsByPositives["Positives"],
-                    )
-                ]
+            modelsByPositives.join(
+                modelsByPositives["Positives"].cut(
+                    bins=list(range(0, 210, 10)),
+                    series=False,
+                    category_label="PositivesBin",
+                ),
+                on="Positives",
+                how="left",
             )
             .lazy()
-            .groupby([by, "PositivesBin"])
+            .groupby([by, "PositivesBin", "break_point"])
             .agg([pl.min("Positives"), pl.n_unique("ModelID").alias("ModelCount")])
             .with_columns(
                 (pl.col("ModelCount") / (pl.sum("ModelCount").over(by))).alias(
                     "cumModels"
                 )
             )
-            .sort("PositivesBin")
+            .sort("break_point")
         )
 
     def get_model_stats(self, last: bool = True) -> dict:
         """Returns a dictionary containing various statistics for the model data.
 
         Parameters
         ----------
@@ -1438,12 +1425,12 @@
         from xlsxwriter import Workbook
 
         tabs = {tab: getattr(self, tab) for tab in self.ApplicableTables}
         with Workbook(file) as wb:
             for tab, data in tabs.items():
                 data = data.with_columns(
                     pl.col(pl.List(pl.Categorical), pl.List(pl.Utf8))
-                    .arr.eval(pl.element().cast(pl.Utf8))
-                    .arr.join(", ")
+                    .list.eval(pl.element().cast(pl.Utf8))
+                    .list.join(", ")
                 )
                 data.write_excel(workbook=wb, worksheet=tab)
         return file
```

### Comparing `pdstools-3.1.9/python/pdstools/adm/ADMTrees.py` & `pdstools-3.2/python/pdstools/adm/ADMTrees.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,15 +494,15 @@
                     .apply(lambda x: self.parseSplitValues(x)[1])
                     .alias("sign"),
                     pl.first("split")
                     .apply(lambda x: self.parseSplitValues(x)[2])
                     .alias("values"),
                 ]
             )
-            .with_columns(n=pl.col("gains").arr.lengths())
+            .with_columns(n=pl.col("gains").list.lengths())
         )
 
     def getSplitsRecursively(
         self, tree: Dict, splits: List, gains: List
     ) -> Tuple[List, List]:
         """Recursively finds splits and their gains for each node.
```

### Comparing `pdstools-3.1.9/python/pdstools/adm/Tables.py` & `pdstools-3.2/python/pdstools/adm/Tables.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/python/pdstools/app/cli.py` & `pdstools-3.2/python/pdstools/app/cli.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/python/pdstools/app/pages/Health Check.py` & `pdstools-3.2/python/pdstools/app/pages/Health Check.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/python/pdstools/ih/IHAnalysis.py` & `pdstools-3.2/python/pdstools/ih/IHAnalysis.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/python/pdstools/ih/legacy_IH.py` & `pdstools-3.2/python/pdstools/ih/legacy_IH.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/python/pdstools/pega_io/API.py` & `pdstools-3.2/python/pdstools/pega_io/API.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/python/pdstools/pega_io/File.py` & `pdstools-3.2/python/pdstools/pega_io/File.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/python/pdstools/pega_io/S3.py` & `pdstools-3.2/python/pdstools/pega_io/S3.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/python/pdstools/plots/plot_base.py` & `pdstools-3.2/python/pdstools/plots/plot_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,24 +112,21 @@
         """
 
         if top_n < 1:
             return df
 
         if facets:
             df = df.join(
-                df.groupby(*facets, "PredictorName")
-                .agg(pl.median(to_plot))
-                .select(
-                    pl.col(*facets, "PredictorName")
-                    .sort_by(to_plot, "PredictorName")
-                    .tail(top_n)
-                    .list()
-                    .over(facets)
-                    .flatten()
-                ),
+                df.groupby(*facets)
+                .agg(
+                    pl.col("PredictorName")
+                    .sort_by("PerformanceBin", "PredictorName", descending=True)
+                    .head(20)
+                )
+                .explode("PredictorName"),
                 on=(*facets, "PredictorName"),
             )
 
         else:
             df = df.join(
                 df.filter(pl.col("PredictorName").cast(pl.Utf8) != "Classifier")
                 .groupby("PredictorName")
@@ -478,15 +475,15 @@
         if len(facets) > 0 and facets[0] is not None:
             groupby = groupby + facets
         if metric in ["Performance", "weighted_performance", "SuccessRate"]:
             df = (
                 df.groupby_dynamic("SnapshotTime", every=every, by=groupby)
                 .agg(
                     [
-                        (pl.sum("Positives") / pl.sum("ResponseCount")).alias(
+                        weighed_average_polars("SuccessRate", "ResponseCount").alias(
                             "SuccessRate"
                         ),
                         weighed_performance_polars().alias("weighted_performance"),
                     ]
                 )
                 .with_columns(pl.col("weighted_performance") * 100)
             ).sort(["SnapshotTime", by])
@@ -1344,25 +1341,26 @@
             print("Plot is only available in Plotly.")
 
         levels = kwargs.pop("levels", self.context_keys)
         mapping = {
             f"{by}_count": "Model count",
             "Percentage_without_responses": "Percentage without responses",
             "ResponseCount_sum": "Response Count sum",
-            "SuccessRate_mean": "Success Rate mean",
+            "SuccessRate_mean": "(%) Success Rate mean",
             "Performance_weighted": "Performance weighted mean",
             "Positives_sum": "Positives sum",
         }
         df = (
             self.model_summary(by=by, query=query, context_keys=levels)
             .select(pl.col(levels).cast(pl.Utf8), pl.col(list(mapping.keys())))
             .rename(mapping)
             .sort(levels)
             .fill_null("Missing")
             .with_columns(pl.col("Performance weighted mean") * 100)
+            .with_columns(pl.col("(%) Success Rate mean") * 100)
             .fill_nan(pl.lit(50))
             .fill_nan(0)
             .collect()
         )
 
         if "Issue" in df.columns and "OmniChannel" in df["Issue"].unique():
             print(
@@ -1416,15 +1414,15 @@
                 "Model count",
                 "Weighted mean performance, per context key combination",
                 False,
                 False,
                 None,
             ],
             "successrate": [
-                "Success Rate mean",
+                "(%) Success Rate mean",
                 "Model count",
                 "Success rate, per context key combination",
                 False,
                 False,
                 0.5,
             ],
         }
```

### Comparing `pdstools-3.1.9/python/pdstools/plots/plots_plotly.py` & `pdstools-3.2/python/pdstools/plots/plots_plotly.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                 mode="lines+markers",
             )
         )
         fig.update_layout(
             template="none", title=title, xaxis_title="Range", yaxis_title="Responses"
         )
         fig.update_yaxes(title_text="Propensity", secondary_y=True)
-        fig.layout.yaxis2.tickformat = ",.0%"
+        fig.layout.yaxis2.tickformat = ",.2%"
         fig.layout.yaxis2.zeroline = False
         fig.update_yaxes(showgrid=False)
 
         return fig
 
     @staticmethod
     def post_plot(
@@ -171,17 +171,17 @@
         Returns
         -------
         plt.figure
         """
 
         hide_legend = kwargs.pop("hide_legend", False)
         metric_hovers = {
-            "SuccessRate": ":.2%",
-            "Performance": ":.2f",
-            "weighted_performance": ":.2f",
+            "SuccessRate": ":.4%",
+            "Performance": ":.4f",
+            "weighted_performance": ":.4f",
             "Positives": ":.d",
             "ResponseCount": ":.d",
         }
         if metric in ["Performance", "weighted_performance", "SuccessRate"]:
             df = df.to_pandas(use_pyarrow_extension_array=False)
             x = "SnapshotTime"
             y = metric
@@ -211,15 +211,15 @@
             facet_col=facet,
             facet_col_wrap=kwargs.pop("facet_col_wrap", 5),
             template="pega",
         )
         if hide_legend:
             fig.update_layout(showlegend=False)
         if metric == "SuccessRate":
-            fig.update_yaxes(tickformat=",.0%")
+            fig.update_yaxes(tickformat=".2%")
             fig.update_layout(yaxis={"rangemode": "tozero"})
 
         return self.post_plot(fig, name="Lines_over_time", title=title, **kwargs)
 
     def PropositionSuccessRates(
         self, df, metric="SuccessRate", by="Name", show_error=True, facet=None, **kwargs
     ):
@@ -608,15 +608,20 @@
             x="PositivesBin",
             y="cumModels",
             color=by,
             markers=True,
             title=title,
             labels={"cumModels": "Percentage of Models", "PositivesBin": "Positives"},
             template="pega",
-            category_orders={"PositivesBin": df["PositivesBin"].unique().to_list()},
+            category_orders={
+                "PositivesBin": df.select("PositivesBin", "break_point")
+                .unique()
+                .sort("break_point")["PositivesBin"]
+                .to_list()
+            },
         )
         fig.layout.yaxis.tickformat = ",.0%"
         fig = self.post_plot(fig, name="Models_by_positives", **kwargs)
         return fig
 
     def TreeMap(
         self,
@@ -706,15 +711,15 @@
                 (1, colorscale[2]),
             ]
 
         hover_data = {
             "Model count": ":.d",
             "Percentage without responses": ":.0%",
             "Response Count sum": ":.d",
-            "Success Rate mean": ":.2%",
+            "(%) Success Rate mean": ":.3f",
             "Performance weighted mean": ":.2f",
             "Positives sum": ":.d",
         }
 
         fig = px.treemap(
             df.to_pandas(use_pyarrow_extension_array=True),
             path=context_keys,
```

### Comparing `pdstools-3.1.9/python/pdstools/reports/HealthCheck.qmd` & `pdstools-3.2/python/pdstools/reports/HealthCheck.qmd`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,19 @@
 # Initialize the class after the parameters have been overwritten.
  
 if len(kwargs)>0: #override with keyword arguments
     datamart = ADMDatamart(**kwargs).fillMissing()
 else: #fall back to 'default'
     datamart = datasets.CDHSample()
 
+treatment = (
+    "Treatment" in datamart.modelData.columns
+    and datamart.modelData.schema["Treatment"] != pl.Null
+)
+    
 last_data = (
     datamart.last(strategy='lazy')
     .with_columns(pl.col(pl.Categorical).cast(pl.Utf8))
     .with_columns(
         [
             pl.col(pl.Utf8).fill_null("NA"),
             pl.col(pl.Null).fill_null("NA"),
@@ -98,15 +103,14 @@
     "Push_Click_Through_Rate",
     "Retail_Click_Through_Rate",
     "Retail_Click_Through_Rate_Outbound",
     "SMS_Click_Through_Rate",
     "Web_Click_Through_Rate",
 ]
 
-
 ```
 
 This document gives a generic and global overview of the Adaptive models 
 and predictors. It is generated from a Python markdown file in the [Pega Data Scientist Tools](https://github.com/pegasystems/pega-datascientist-tools). That repository
 of tools and scripts also contains a notebook to generate stand-alone
 model reports for individual models, please refer 
 to the [Wiki](https://github.com/pegasystems/pega-datascientist-tools/wiki).
@@ -125,15 +129,14 @@
 In the cell below, all data preprocessing is executed, such as importing the data and applying global filters. By default, the values are populated by environment variables supplied when running the file, but for customization purposes, you can edit this cell.
 
 # Overview of the Actions
 In a standard setup, the offers/conversations are presented as treatments for actions in a hierarchical structure setup in NBA Designer. The recommendation is to have multiple treatments for an action. Treatments are often channel specific and you would typically expect more unique treatments than there are actions.
 
 Adaptive Models are created per treatment (at least in the default setup) and the recommendation is to stick the default context keys of the models.
 ```{python}
-datamart.context_keys
 context_keys= {'Channels':'Channel/Direction', 'Issues':'Issue', 'Groups':'Group','Actions':'Name', 'Treatments':'Treatment'}
 value_keys = ['Actions', 'Treatments','Issues', 'Groups', 'Channels']
 counts, values = dict(), dict()
 
 for label, column in context_keys.items():
     if column in last_data.columns:
         if label in value_keys:
@@ -153,41 +156,40 @@
 
 ### Guidance
 - Look out for propositions that stand out, having a far higher success rate than the rest. Check with business if that is expected.
 
 - Variation in the set of offered propositions across customers is also an important metric but not one that can be derived from the Adaptive Model data - this requires analysis of the actual interactions.
 ```{python}
 facet = "Channel/Direction"
-hover_columns = ["Issue", "Group", "Name"]
-df = last_data.lazy().with_columns(pl.concat_str(facet.split("/"), separator="/").alias(facet)).with_columns(pl.col(pl.Categorical).cast(pl.Utf8))
+hover_columns = [col for col in  ["Issue", "Group", "Name"] if col in datamart_all_columns]
+if treatment:
+    hover_columns += ["Treatment"]
 df = (
-    df
-    .filter(pl.col("ResponseCount") > 100)
-    .groupby(hover_columns + ["ModelID","Channel/Direction"])
-    .agg(
-        cdh_utils.weighed_average_polars("SuccessRate", "ResponseCount").alias(
-            "SuccessRate"
-        )
-    )
+    last_data.lazy()
+    .with_columns(pl.concat_str(facet.split("/"), separator="/").alias(facet))
+    .with_columns(pl.col(pl.Categorical).cast(pl.Utf8))
+)
+df = (
+    df.filter(pl.col("ResponseCount") > 100)
+    .select(hover_columns + ["ModelID", "Channel/Direction","SuccessRate"])
     .with_columns(pl.col("SuccessRate").round(4))
     .sort(["Channel/Direction", "SuccessRate"], descending=True)
     .groupby(["Channel/Direction"])
     .head(20)
     .collect()
 ).to_pandas(use_pyarrow_extension_array=True)
 
 hover_data = {
     "SuccessRate": ":.2%",
-    "Issue": ":.d",
-    "Group": ":.d",
-    "Name": ":.d",
 }
+for col in hover_columns:
+    hover_data[col] = ":.d"
 
 
-facet= "Channel/Direction"
+facet = "Channel/Direction"
 facet_col_wrap = 3
 fig = px.bar(
     df.sort_values(["Channel/Direction", "SuccessRate"]),
     x="SuccessRate",
     y="ModelID",
     color="SuccessRate",
     facet_col=facet,
@@ -202,45 +204,54 @@
     matches=None,
 ).update_traces(textposition="inside")
 fig.for_each_annotation(
     lambda a: a.update(text=a.text.replace("Channel/Direction=", ""))
 )
 fig.update(layout_coloraxis_showscale=False)
 
-unique_count = datamart.last(strategy='lazy').with_columns(pl.concat_str(facet.split("/"), separator="/").alias(facet)).select(facet).collect().to_series().n_unique()
+unique_count = (
+    datamart.last(strategy="lazy")
+    .with_columns(pl.concat_str(facet.split("/"), separator="/").alias(facet))
+    .select(facet)
+    .collect()
+    .to_series()
+    .n_unique()
+)
 
-height = 200 + (math.ceil( unique_count / facet_col_wrap) * 250)
+height = 200 + (math.ceil(unique_count / facet_col_wrap) * 250)
 
 fig.update_layout(autosize=True, height=height)
 
 display(fig)
 ```
 
 ## All Success Rates
 Interactive chart with all success rates.
 
 ```{python}
+levels = [col for col in ["Configuration",'Channel', 'Direction', 'Issue', 'Group', "Name", "Treatment"] if col in datamart_all_columns]
 fig = datamart.plotTreeMap(color_var="SuccessRate",
-                     groupby_col= None,
-                     levels=['Channel', 'Direction', 'Issue', 'Group', "Name"], 
-                     colorscale=pega_template.success)
+                     groupby_col=None,
+                     levels=levels, 
+                     colorscale=pega_template.success,
+                     query=pl.col("ResponseCount")>100,)
 fig
 ```
 
 ## Success Rates over Time
 Showing how the overall channel success rates evolved over the time that the data export covers. Split by Channel and model configuration. Usually there are separate model configurations for different channels but sometimes there are also additional model configurations for different outcomes (e.g. conversion) or different customers (e.g. anonymous).
 
 ### Guidance
 - There shouldn’t be too sudden changes over time
 ```{python}
 by = "Channel/Direction"
 facet = "Configuration"
 fig = datamart.plotOverTime('SuccessRate', by=by, facets=facet, facet_col_wrap=2, query=pl.col("ResponseCount") > 100)
 fig.update_yaxes(matches=None)
-fig.for_each_yaxis(lambda yaxis: yaxis.update(showticklabels=True, rangemode="tozero"))
+fig.for_each_yaxis(lambda yaxis: yaxis.update(showticklabels=True))
 unique_count = datamart.modelData.with_columns(pl.concat_str(facet.split("/"), separator="/").alias(facet)).select(facet).collect().unique().shape[0]
 height = 200 + (math.ceil( unique_count / 2) * 250)
 fig.update_layout(autosize=True, height=height)
 fig.for_each_annotation(
     lambda a: a.update(text=a.text.replace(f"{facet}=", ""))
 )
 fig.for_each_xaxis(lambda xaxis: xaxis.update(showticklabels=True))
@@ -327,37 +338,38 @@
 
 ### Model performance of all the actions (interactive Treemap)
 Using an interactive treemap to visualize the performance. Lighter is better, darker is low performance.
 
 It can be interesting to see which issues, groups or channels can be better predicted than others. Identifying categories of items for which the predictions are poor can help to drive the search for better predictors, for example.
 
 ```{python}
-fig = datamart.plotTreeMap(color_var="performance_weighted", groupby_col= None, levels=['Channel', 'Direction', 'Issue', 'Group', "Name"])
+fig = datamart.plotTreeMap(color_var="performance_weighted", groupby_col= None, levels=levels)
 
 fig.show()
 ```
 
 ### Response counts for all the actions
 Using an interactive treemap to visualize the response counts.
 Different channels will have very different numbers but within one channel the relative differences in response counts give an indication how skewed the distribution is.
 
 Warning : Currently treemap calculates mean response count moving upwards in the hierarchy. 
 ```{python}
-fig = datamart.plotTreeMap(color_var="responsecount", levels=['Channel', 'Direction', 'Issue', 'Group', "Name"], colorscale=pega_template.negative_positive)
+fig = datamart.plotTreeMap(color_var="responsecount", levels=levels, colorscale=pega_template.negative_positive)
 fig
 
 ```
 # Analysis of Predictors
 This analysis focuses on finding which are top predictors that are driving the models.
 
 The predictors are categorized (by color) by the “source”. By default this takes just the first part before the dot, so this typically distinguishes between Customer, Account, IH and parameterized (Param.) predictors. You can customize this to add patterns to identify for example external scores.
 
 ## Number of Predictors per model configuration 
 
 ```{python}
+#| error: true
 if include_tables:
     predictors_per_configuration = datamart.predictors_per_configuration.to_pandas(use_pyarrow_extension_array=False)
     show(predictors_per_configuration)
 else:
     print('Please refer to the `predictors_per_configuration` tab in the included Excel file.')
 ```
 
@@ -368,14 +380,15 @@
 ### Guidance
 - Number of predictors per model 200 - 700
 - There should be IH* predictors
 - There should not be > 100 IH predictors
 - No more than a few dozen Param predictors
 
 ```{python}
+#| error: true
 if datamart.predictorData is not None:
     figs = datamart.plotPredictorPerformance(top_n=20, facets='Configuration',separate=True, active_only=True)
     if not isinstance(figs, list):
         figs = [figs]
     for fig in figs:
         fig.update_traces(width=0.3)
         fig.update_layout(font=dict(size=10))
@@ -388,17 +401,18 @@
 
 ## Importance by Predictor Category 
 Aggregating up to the category of the predictors. This gives a view at a glance of how well e.g. interaction history, external model scores or contextual data are doing overall.
 
 ### Predictor Category performance per Channel/Direction/Issue 
 
 ```{python}
+#| error: true
 facets = 'Configuration/Channel/Direction'
 facet_col_wrap = 3
-fig = datamart.plotPredictorCategoryPerformance(facets='Configuration/Channel/Direction', facet_col_wrap=facet_col_wrap)
+fig = datamart.plotPredictorCategoryPerformance(facets=facets, facet_col_wrap=facet_col_wrap)
 
 fig.update_layout(font=dict(size=10))
 fig.for_each_annotation(
     lambda a: a.update(text=a.text.replace(f"{facets}=", ""))
 )
 fig.for_each_annotation(lambda a: a.update(text=" <br> ".join(a.text.split("/"))))
 
@@ -736,97 +750,97 @@
 cdh_utils.legend_color_order(only_positives).show()
 ```
 
 ## Models with largest number of responses (positive or negative)
 Zooming in into the models that drive most of the responses, here we list the top 20 models with the highest number of responses.
 
 ```{python}
-facet= "Configuration/Issue/Group/Name/Channel/Direction"
+subset = ['Configuration', 'Issue', 'Group', 'Name', 'Channel', 'Direction']
+facet = '/'.join([col for col in subset if col in datamart_all_columns])
+
 for split_facet in facet.split("/"):
     last_data = last_data.with_columns(
         pl.col(split_facet).cast(pl.Utf8).fill_null("NA")
     )
 last_data = last_data.with_columns(pl.concat_str(facet.split("/"), separator="/").alias(facet))
 response_counts = last_data.groupby([facet] + facet.split("/")).agg(
     [
         pl.sum("ResponseCount").alias("all_responses"),
         pl.sum("Positives").alias("positive_sum")
         ]
     )
 
 all_responses = response_counts.sort("all_responses", descending=False).tail(20)
 hover_data = {
-    "Configuration": ":.d",
-    "Issue": ":.d",
-    "Group": ":.d",
-    "Name": ":.d",
-    "Channel": ":.d",
-    "Direction": ":.d",
     facet: False
 }
-fig = px.bar(all_responses.to_pandas(use_pyarrow_extension_array=True), x ="all_responses", y=facet, color="Channel", title="Top 20 Highest Responses", template="pega", text=facet, hover_data=hover_data)
+for col in facet.split("/"):
+    hover_data[col] = ":.d"
+
+possible_color_vars = ['Channel', 'Issue', 'Name']
+color = next((col for col in possible_color_vars if col in datamart_all_columns), None)
+
+fig = px.bar(all_responses.to_pandas(use_pyarrow_extension_array=True), x ="all_responses", y=facet, color=color, title="Top 20 Highest Responses", template="pega", text=facet, hover_data=hover_data)
 fig.update_yaxes(matches=None, showticklabels=False, visible=False).update_traces(textposition="inside")
 fig.for_each_annotation(
     lambda a: a.update(text=a.text.replace(facet, ""))
 )
-    
+fig.update_layout(yaxis={'categoryorder':'total ascending'})    
 cdh_utils.legend_color_order(fig).show()
 ```
 
 ## Models with largest number of positive responses. 
 And these are the 20 models with the largest number of positives.
 
 ```{python}
 positives = response_counts.sort("positive_sum", descending=True).head(20)
-fig = px.bar(positives.to_pandas(use_pyarrow_extension_array=True), x ="positive_sum", y=facet, color="Channel", title="Top 20 Highest Positives", template="pega", text=facet, hover_data=hover_data)
+fig = px.bar(positives.to_pandas(use_pyarrow_extension_array=True), x ="positive_sum", y=facet, color=color, title="Top 20 Highest Positives", template="pega", text=facet, hover_data=hover_data)
 fig.update_yaxes(matches=None, showticklabels=False, visible=False).update_xaxes(matches=None).update_traces(textposition='inside')
 fig.for_each_annotation(
     lambda a: a.update(text=a.text.replace(facet, ""))
 )
 fig.update_layout(yaxis={'categoryorder':'total ascending'})
-fig.data[0]
 
 cdh_utils.legend_color_order(fig).show()
 ```
 
 ## Analysis of Performance vs Volume
 Is most volume driven by models that have a good predictive performance? Ideally yes, so the targeting of the customers is optimal. If a lot of volume is driven by models that are not very predictive, this could be a reason to look into the available predictor data.
 
 The plot below shows this relation. Horizontally the model performance (the AUC, ranging from 50 to 100 as Pega usually scales this), descretized into a number of ranges, and vertically the percentage of responses.
 
 A lot of volume on the first bins, where the performance is minimal, means that a lot of immature models are used. This is sub-optimal in terms of targeting. Ideally there is a smooth curve with a peak in the 60-80 range of AUC. Much higher AUC’s are possibly indicative of immature models or even outcome leakers (although that is effectively prevented by the standard delayed learning pattern). AUC’s below 60 are not uncommon but should be investigated - consider different predictors or outcomes.
 ```{python}
+#| error: true
 to_plot = "Performance"
 df = (
-    datamart.combinedData.with_columns(pl.col(to_plot) * 100)
+    datamart.modelData.with_columns(pl.col(to_plot) * 100)
     .groupby([to_plot, "Channel", "Direction"])
-    .agg(pl.sum("BinResponseCount"))
+    .agg(pl.sum("ResponseCount"))
     .with_columns(pl.col(to_plot).round(2))
     .collect()
 )
 
 cut_off_value = [percentile for percentile in range(50, 100, 3)]
-
 df_pl = df.get_column(to_plot).fill_null(0).fill_nan(0).cut(bins=cut_off_value, category_label="PerformanceBin").lazy()
 join = df.lazy().join(
     df_pl.select([to_plot, "PerformanceBin"]).unique(), on=to_plot, how="left"
 )
-grouped = join.groupby(["Channel", "PerformanceBin"]).agg(pl.sum("BinResponseCount"))
-
+grouped = join.groupby(["Channel", "PerformanceBin"]).agg(pl.sum("ResponseCount"))
 out = (
     grouped.sort(["Channel", "PerformanceBin"])
     .select(
         [
-            "Channel",
+            pl.col("Channel").cast(pl.Utf8),
             "PerformanceBin",
-            "BinResponseCount",
-            pl.col("BinResponseCount").sum().over("Channel").alias("sum"),
+            "ResponseCount",
+            pl.col("ResponseCount").sum().over("Channel").alias("sum"),
         ]
     )
-    .with_columns([(pl.col("BinResponseCount") / pl.col("sum")).alias("Volume")])
+    .with_columns([(pl.col("ResponseCount") / pl.col("sum")).alias("Volume")])
 )
 
 out = out.sort(["Channel", "PerformanceBin"]).collect().to_pandas()
 fig = px.bar(
     out,
     x="PerformanceBin",
     y="Volume",
@@ -836,21 +850,21 @@
 )
 for bar in fig.data:
   bar.visible = "legendonly"
 
 channels = out["Channel"].unique()
 for channel_num, channel in enumerate(channels):
     channel_df = out[out["Channel"] == channel]
-    fig.add_traces(go.Scatter(x = channel_df.PerformanceBin, y=channel_df.Volume, line_shape = 'spline', marker_color = fig.data[channel_num].marker.color, name=channel))
+    fig.add_traces(go.Scatter(x = channel_df["PerformanceBin"], y=channel_df.Volume, line_shape = 'spline', marker_color = fig.data[channel_num].marker.color, name=channel))
 
 
 fig.update_yaxes(tickformat=",.0%")
 fig.update_xaxes(categoryorder='array', categoryarray = out.sort_values("PerformanceBin")["PerformanceBin"].unique())
 
-fig.show()
+cdh_utils.legend_color_order(fig).show()
 
 ```
 
 ## Positives vs. Number of Models
 Ideally, all models have received plenty of responses which will make them “mature” and makes sure they are as predictive as possible. \n
 Often we see that there is a significant percentage of models that are still relatively new and have not received much feedback (yet). Below graph shows the percentages of models that have fewer than 200 positives. \n
 Having many on the left-hand side (with very low or perhaps no positives) may or not be a problem. The models may still be there in the datamart but might represent actions/treatments that are not active. 
@@ -874,14 +888,15 @@
 Often however, multiple factors are included in the prioritization, changing this picture.
 
 Note that the propensity bins are not of equal width. Propensities are typically very low so with an equal width distribution, almost all volume would be in the first bins. The binning here is based on (roughly) equal volume across all data.
 
 So when one of the graphs shows more volume on the left, that is to be interpreted as relative to the other graphs.
 
 ```{python}
+#| error: true
 to_plot = "Propensity"
 if to_plot == "Propensity" and to_plot not in datamart.predictorData.columns:
     to_plot = "BinPropensity"
 df = datamart.combinedData.filter(pl.col("PredictorName")!="Classifier").groupby([to_plot, "Channel", "Direction"]).agg(pl.sum("BinResponseCount")).with_columns(pl.col(to_plot).round(4).cast(pl.Float64)).collect()
 color_col = "Channel"
 smallest_bin = 0
```

### Comparing `pdstools-3.1.9/python/pdstools/utils/cdh_utils.py` & `pdstools-3.2/python/pdstools/utils/cdh_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
         The column to parse
 
     """
     if isinstance(x, str):
         x = pl.col(x)
     x = x.cast(pl.Utf8) if not isinstance(x, pl.Utf8) else x
     return (
-        pl.when(x.str.split(".").arr.lengths() > 1)
-        .then(x.str.split(".").arr.get(0))
+        pl.when(x.str.split(".").list.lengths() > 1)
+        .then(x.str.split(".").list.get(0))
         .otherwise(pl.lit("Primary"))
     ).alias("PredictorCategory")
 
 
 def _extract_keys(
     df: any_frame,
     col="Name",
@@ -290,22 +290,23 @@
         The AUC as a value between 0.5 and 1.
 
     Examples:
         >>> auc_from_bincounts([3,1,0], [2,0,1])
     """
     pos = np.asarray(pos)
     neg = np.asarray(neg)
-    if probs is None:
-        o = np.argsort(-(pos / (pos + neg)))
-    else:
-        o = np.argsort(-np.asarray(probs))
-    FPR = np.flip(np.cumsum(neg[o]) / np.sum(neg), axis=0)
-    TPR = np.flip(np.cumsum(pos[o]) / np.sum(pos), axis=0)
-    Area = (FPR - np.append(FPR[1:], 0)) * (TPR + np.append(TPR[1:], 0)) / 2
-    return safe_range_auc(np.sum(Area))
+    if probs is None:  
+        probs = pos / (pos + neg)  
+  
+    binorder = np.argsort(probs)[::-1]  
+    FPR = np.cumsum(neg[binorder]) / np.sum(neg)  
+    TPR = np.cumsum(pos[binorder]) / np.sum(pos)  
+      
+    Area = (np.diff(FPR, prepend=0)) * (TPR + np.insert(np.roll(TPR, 1)[1:], 0,0)) / 2  
+    return safe_range_auc(np.sum(Area))  
 
 
 def aucpr_from_probs(
     groundtruth: List[int], probs: List[float]
 ) -> List[float]:  # pragma: no cover
     """Calculates PR AUC (precision-recall) from an array of truth values and predictions.
     Calculates the area under the PR curve from an array of truth values and
```

### Comparing `pdstools-3.1.9/python/pdstools/utils/datasets.py` & `pdstools-3.2/python/pdstools/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/python/pdstools/utils/hds_utils.py` & `pdstools-3.2/python/pdstools/utils/hds_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,21 +217,23 @@
                 for filename in (
                     df.select(pl.col("filename").unique())
                     .collect()
                     .to_series()
                     .to_list()
                 ):
                     newName = Path(out_filename) / Path(filename).name
+                    if not os.path.exists(newName.parent):
+                        os.mkdir(newName.parent)
                     df.filter(pl.col("filename") == filename).drop(
                         "filename"
                     ).collect().write_ndjson(newName)
 
         if mode == "optimized":
             if "filename" in df.columns:
-                df = df.drop(pl.col("filename"))
+                df = df.drop("filename")
             df = df.collect()
             if out_format == "ndjson":
                 df.write_ndjson(f"{out_filename}.json")
             elif out_format == "parquet":
                 df.write_parquet(f"{out_filename}.parquet")
             elif out_format == "arrow":
                 df.write_ipc(f"{out_filename}.arrow")
@@ -402,15 +404,15 @@
                 else:
                     numeric_predictors_to_mask.append(val)
             ih_predictors[val] = (
                 f"IH_PREDICTOR_{idx}" if self.config.mask_ih_names else val
             )
 
         for idx, val in enumerate(predictors_t):
-            if self.config.mask_predictor_values:
+            if self.config.mask_predictor_values and val != "filename":
                 if self.predictors_by_type[val] == "symbolic":
                     symbolic_predictors_to_mask.append(val)
                 else:
                     numeric_predictors_to_mask.append(val)
             predictors[val] = (
                 f"PREDICTOR_{idx}" if self.config.mask_predictor_names else val
             )
@@ -426,18 +428,17 @@
         column_mapping = {
             **predictors,
             **context_keys,
             **ih_predictors,
             **special_predictors,
             **outcome_column,
         }
-        if "filename" in symbolic_predictors_to_mask:
-            symbolic_predictors_to_mask.remove("filename")
-        if "filename" in column_mapping:
-            _ = column_mapping.pop("filename", None)
+
+        if "filename" in predictors_t:
+            column_mapping["filename"] = "filename"
 
         return symbolic_predictors_to_mask, numeric_predictors_to_mask, column_mapping
 
     def getHasher(
         self,
         cols,
         algorithm="xxhash",
```

### Comparing `pdstools-3.1.9/python/pdstools/utils/pega_template.py` & `pdstools-3.2/python/pdstools/utils/pega_template.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/python/pdstools/utils/polars_ext.py` & `pdstools-3.2/python/pdstools/utils/polars_ext.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/python/pdstools/utils/show_versions.py` & `pdstools-3.2/python/pdstools/utils/show_versions.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/python/pdstools/utils/streamlit_utils.py` & `pdstools-3.2/python/pdstools/utils/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/python/pdstools/utils/table_definitions.py` & `pdstools-3.2/python/pdstools/utils/table_definitions.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.9/python/pdstools/valuefinder/ValueFinder.py` & `pdstools-3.2/python/pdstools/valuefinder/ValueFinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,21 @@
         self.ncust = self.df.select(
             (pl.lit(10) ** pl.col("CustomerID").n_unique().log10().ceil())
             .cast(pl.UInt32)
             .alias("ncust")
         )
 
         self.NBADStages = ["Eligibility", "Applicability", "Suitability", "Arbitration"]
+        self.StageOrder = (
+            pl.DataFrame(
+                {"pyStage": self.NBADStages}, schema={"pyStage": pl.Categorical}
+            )
+            .select(pl.col("pyStage").cat.set_ordering("physical"))
+            .lazy()
+        )  # This pre-fills the stringcache to make the ordering of stages correct
         self.maxPropPerCustomer = self.df.groupby(["CustomerID", "pyStage"]).agg(
             pl.max("pyModelPropensity").alias("MaxModelPropensity")
         )
 
         if import_strategy == "eager":
             self.df = self.df.collect().lazy()
             self.th = self.th.collect().lazy()
@@ -321,15 +328,15 @@
         """
         i = 0
         figs = make_subplots(
             rows=len(self.NBADStages), cols=1, shared_xaxes=True, vertical_spacing=0.005
         )
         for stage in self.NBADStages:
             data = self.df.filter(pl.col("pyStage") == stage)
-            data = data.pdstools.sample(sampledN).collect()
+            data = data.pdstools.sample(sampledN).drop_nulls().collect()
             temp = ff.create_distplot(
                 [data["pyModelPropensity"].to_list()],
                 ["pyModelPropensity"],
                 show_rug=False,
                 show_hist=False,
             )
             tempdf = pd.DataFrame(
@@ -658,24 +665,19 @@
         elif level.casefold() in {"issue", "pyissue"}:
             level, cat = "pyIssue", "Issues"
         elif level.casefold() in {"group", "pygroup"}:
             level, cat = "pyGroup", "Groups"
 
         df = self.df if query is None else self.df.filter(query)
         df = (
-            pl.LazyFrame(
-                {"pyStage": self.NBADStages}, schema={"pyStage": pl.Categorical}
-            )
-            .join(
-                df.groupby("pyStage")
-                .agg(pl.col(level).cast(pl.Utf8).value_counts().sort())
-                .explode(level)
-                .unnest(level),
-                on="pyStage",
-            )
+            df.groupby("pyStage")
+            .agg(pl.col(level).cast(pl.Utf8).value_counts(sort=True))
+            .explode(level)
+            .unnest(level)
+            .sort("pyStage")
             .rename({level: "Name", "counts": "Count", "pyStage": "Stage"})
             .collect()
         )
         if return_df:
             return df
 
         fig = px.funnel(
@@ -685,8 +687,10 @@
             color="Name",
             text="Name",
             title=f"Distribution of {cat.casefold()} over the stages",
             template="none",
         )
         fig.update_xaxes(categoryorder="array", categoryarray=self.NBADStages)
         fig.update_layout(legend_title_text=cat)
+        if return_df == "both":
+            return fig, df
         return fig
```

