# Comparing `tmp/optim_esm_tools-1.0.3.tar.gz` & `tmp/optim_esm_tools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optim_esm_tools-1.0.3.tar", last modified: Mon Jul 24 17:24:20 2023, max compression
+gzip compressed data, was "optim_esm_tools-1.1.0.tar", last modified: Fri Jul 28 13:41:53 2023, max compression
```

## Comparing `optim_esm_tools-1.0.3.tar` & `optim_esm_tools-1.1.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.972620 optim_esm_tools-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-07-24 17:24:20.972620 optim_esm_tools-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.964620 optim_esm_tools-1.0.3/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/bin/oet_plot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.964620 optim_esm_tools-1.0.3/optim_esm_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/_test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.968620 optim_esm_tools-1.0.3/optim_esm_tools/analyze/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/cmip_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/pre_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    27787 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/tipping_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/xarray_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/optim_esm_conf.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.968620 optim_esm_tools-1.0.3/optim_esm_tools/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15918 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/plotting/map_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/plotting/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.968620 optim_esm_tools-1.0.3/optim_esm_tools/synda_files/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/synda_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/synda_files/synda_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.968620 optim_esm_tools-1.0.3/optim_esm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-07-24 17:24:20.000000 optim_esm_tools-1.0.3/optim_esm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-24 17:24:20.000000 optim_esm_tools-1.0.3/optim_esm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:24:20.000000 optim_esm_tools-1.0.3/optim_esm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:24:20.000000 optim_esm_tools-1.0.3/optim_esm_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 17:24:20.000000 optim_esm_tools-1.0.3/optim_esm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 17:24:20.000000 optim_esm_tools-1.0.3/optim_esm_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-24 17:24:20.972620 optim_esm_tools-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.972620 optim_esm_tools-1.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_pangeo_download.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:41:53.545358 optim_esm_tools-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-07-28 13:41:53.545358 optim_esm_tools-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:41:53.541358 optim_esm_tools-1.1.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/bin/oet_plot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:41:53.541358 optim_esm_tools-1.1.0/optim_esm_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/_test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:41:53.541358 optim_esm_tools-1.1.0/optim_esm_tools/analyze/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/analyze/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/analyze/cmip_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/analyze/find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/analyze/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/analyze/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/analyze/pre_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24707 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/analyze/region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/analyze/time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/analyze/tipping_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/analyze/xarray_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/optim_esm_conf.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:41:53.541358 optim_esm_tools-1.1.0/optim_esm_tools/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15903 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/plotting/map_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/plotting/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:41:53.545358 optim_esm_tools-1.1.0/optim_esm_tools/synda_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/synda_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/synda_files/synda_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/optim_esm_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:41:53.541358 optim_esm_tools-1.1.0/optim_esm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-07-28 13:41:53.000000 optim_esm_tools-1.1.0/optim_esm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-28 13:41:53.000000 optim_esm_tools-1.1.0/optim_esm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:41:53.000000 optim_esm_tools-1.1.0/optim_esm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:41:53.000000 optim_esm_tools-1.1.0/optim_esm_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:41:53.000000 optim_esm_tools-1.1.0/optim_esm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 13:41:53.000000 optim_esm_tools-1.1.0/optim_esm_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:41:53.545358 optim_esm_tools-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:41:53.545358 optim_esm_tools-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/test/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/test/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/test/test_find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/test/test_pangeo_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/test/test_region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/test/test_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/test/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/test/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-28 13:41:50.000000 optim_esm_tools-1.1.0/test/test_xarray_tools.py
```

### Comparing `optim_esm_tools-1.0.3/PKG-INFO` & `optim_esm_tools-1.1.0/optim_esm_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: optim_esm_tools
-Version: 1.0.3
+Name: optim-esm-tools
+Version: 1.1.0
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,14 +15,29 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
+        1.1.0 / 2023-07-28
+        ## What's Changed
+        *Minor change*
+        Add the required tools to analyze time series and their properties
+        * Statistical tools for time series by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/96
+        *Patch*
+        * Fix lon/lat for cluster plot and temp folder for preprocess by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/93
+        * Load intake store from intake by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/94
+        * Plotting flexibility by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/95
+        * Minor search tweak by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/97
+        
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v1.0.3...v1.1.0
+        
+        
         1.0.3 / 2023-07-24
         ------------------
         * Fix clustering fudge factor by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/91
         * Preprocessing running mean fix by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/92
         
         
         **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v1.0.2...v1.0.3
```

### Comparing `optim_esm_tools-1.0.3/README.md` & `optim_esm_tools-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.3/bin/oet_plot` & `optim_esm_tools-1.1.0/bin/oet_plot`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools/_test_utils.py` & `optim_esm_tools-1.1.0/optim_esm_tools/_test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 # -*- coding: utf-8 -*-
 import os
 
 EXMPLE_DATA_SET = 'CMIP6/ScenarioMIP/CCCma/CanESM5/ssp585/r3i1p2f1/Amon/tas/gn/v20190429/tas_Amon_CanESM5_ssp585_r3i1p2f1_gn_201501-210012.nc'
 
 
+def cmip_store():
+    import intake
+
+    return intake.open_esm_datastore(
+        'https://storage.googleapis.com/cmip6/pangeo-cmip6.json'
+    )
+
+
 def get_file_from_pangeo(experiment_id='ssp585', refresh=True):
     dest_folder = os.path.split(
         get_example_data_loc().replace('ssp585', experiment_id)
     )[0]
     if experiment_id in ['piControl', 'historical']:
         dest_folder = dest_folder.replace('ScenarioMIP', 'CMIP')
     write_to = os.path.join(dest_folder, 'test.nc')
     if os.path.exists(write_to) and not refresh:
         print(f'already file at {write_to}')
         return write_to
 
-    from xmip.utils import google_cmip_col
-
-    col = google_cmip_col()
+    col = cmip_store()
     query = dict(
         source_id='CanESM5',
         variable_id='tas',
         table_id='Amon',
         experiment_id=experiment_id,
     )
     if experiment_id in ['historical', 'ssp585']:
@@ -82,14 +88,22 @@
 def synda_test_available():
     """Check if we can run a synda-dependent test"""
     return os.environ.get('ST_HOME') is not None and os.path.exists(
         get_example_data_loc()
     )
 
 
+def get_path_for_ds(data_name, refresh=True):
+    path = get_file_from_pangeo(data_name, refresh=refresh)
+    year_path = year_means(path, refresh=refresh)
+    assert year_path
+    assert os.path.exists(year_path)
+    return year_path
+
+
 def minimal_xr_ds(len_x=513, len_y=181, len_time=10, add_nans=True):
     import numpy as np
     import xarray as xr
 
     lon = np.linspace(0, 360, len_x)[:-1]
     lat = np.linspace(-90, 90, len_y)[:-1]
     time = np.arange(len_time)
```

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools/analyze/clustering.py` & `optim_esm_tools-1.1.0/optim_esm_tools/analyze/clustering.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools/analyze/cmip_handler.py` & `optim_esm_tools-1.1.0/optim_esm_tools/analyze/cmip_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -140,45 +140,35 @@
     if not os.path.exists(data_path):
         message = f'No dataset at {data_path}'
         if strict:
             raise FileNotFoundError(message)
         warn(message)
         return None
 
-    temp_file = os.path.join(base, 'temp_final.nc')
     if pre_process:
-        data_path = oet.analyze.pre_process.pre_process(
+        data_set = oet.analyze.pre_process.get_preprocessed_ds(
             source=data_path,
             max_time=max_time,
             min_time=min_time,
-            save_as=temp_file,
             _ma_window=_ma_window,
             variable_id=variable_of_interest,
         )
     else:
-        log.warning(
-            f'Not preprocessing file is dangerous, dimensions may differ wildly!'
-        )
-    # At this point, if load is None, change it to true, we will have to load it anyway to do the
-    # transforms
-    load = load if load is not None else True
-    data_set = oet.analyze.io.load_glob(data_path, load=load)
-
-    if os.path.exists(temp_file):
-        # Maybe we can make this optional, but, for now, let's prevent double caching of
-        # res_file and temp_file
-        os.remove(temp_file)
+        message = 'Not preprocessing file is dangerous, dimensions may differ wildly!'
+        log.warning(message)
+        data_set = oet.analyze.io.load_glob(data_path, load=load)
 
     if apply_transform:
-        data_set = add_conditions_to_ds(
-            data_set,
-            variable_of_interest=variable_of_interest,
-            _ma_window=_ma_window,
-            **kwargs,
+        kwargs.update(
+            dict(
+                variable_of_interest=variable_of_interest,
+                _ma_window=_ma_window,
+            )
         )
+        data_set = add_conditions_to_ds(data_set, **kwargs)
 
     folders = base.split(os.sep)
 
     # start with -1 (for i==0)
     metadata = {k: folders[-i - 1] for i, k in enumerate(_FOLDER_FMT[::-1])}
     metadata.update(dict(path=base, file=res_file, running_mean_period=_ma_window))
```

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools/analyze/find_matches.py` & `optim_esm_tools-1.1.0/optim_esm_tools/analyze/find_matches.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from optim_esm_tools.config import config, get_logger
 from collections import defaultdict
 
 
 @timed
 @check_accepts(
     accepts=dict(
-        activity_id=('ScenarioMIP', 'CMIP', '*'),
+        activity_id=('AerChemMIP', 'ScenarioMIP', 'CMIP', '*'),
         experiment_id=(
             'piControl',
             'historical',
             'ssp119',
             'ssp126',
             'ssp245',
             'ssp370',
@@ -179,7 +179,58 @@
     path = _get_head(path)
     return os.path.join(
         os.sep,
         *path.split(os.sep)[
             : -len(config['CMIP_files']['folder_fmt'].split()) - look_back_extra
         ],
     )
+
+
+def associate_historical(
+    data_set=None,
+    path=None,
+    match_to='piControl',
+    activity_id='CMIP',
+    look_back_extra=0,
+    query_updates=None,
+    search_kw=None,
+    strict=True,
+):
+    if data_set is None and path is None:
+        raise ValueError(
+            'No dataset, no path, can\'t match if I don\'t know what I\'m looking for'
+        )
+    log = get_logger()
+    path = path or data_set.attrs['path']
+    base = base_from_path(path, look_back_extra=look_back_extra)
+    search = folder_to_dict(path)
+    search['activity_id'] = activity_id
+    if search['experiment_id'] == match_to:
+        message = f'Cannot match {match_to} to itself!'
+        if strict:
+            raise NotImplementedError(message)
+        log.warning(message)
+    search['experiment_id'] = match_to
+    if search_kw:
+        search.update(search_kw)
+        print(search)
+    if query_updates is None:
+        query_updates = [
+            dict(),
+            dict(variant_label='*'),
+            dict(version='*'),
+            # can lead to funny behavior as grid differences may cause breaking compares
+            dict(grid_label='*'),
+        ]
+
+    for try_n, update_query in enumerate(query_updates):
+        if try_n:
+            message = f'No results after {try_n} try, retying with {update_query}'
+            log.info(message)
+        search.update(update_query)
+        this_try = find_matches(base, **search)
+        if this_try:
+            return this_try
+    message = f'Looked for {search}, in {base} found nothing'
+    if strict:
+        raise RuntimeError(message)
+    log.warning(message)
```

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools/analyze/io.py` & `optim_esm_tools-1.1.0/optim_esm_tools/analyze/io.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools/analyze/pre_process.py` & `optim_esm_tools-1.1.0/optim_esm_tools/analyze/pre_process.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,49 @@
 from optim_esm_tools.config import config, get_logger
 from optim_esm_tools.analyze.xarray_tools import _native_date_fmt
 from optim_esm_tools.analyze.io import load_glob
 from optim_esm_tools.analyze.globals import _DEFAULT_MAX_TIME
 import numpy as np
 import os
 import typing as ty
+import tempfile
+
+
+def get_preprocessed_ds(source, **kw):
+    """Create a temporary working directory for pre-process and delete all intermediate files"""
+    if 'working_dir' in kw:
+        message = (
+            f'Calling get_preprocessed_ds with working_dir={kw.get("working_dir")} is not '
+            'intended, as this function is meant to open a temporary directory, load the '
+            'dataset, and remove all local files.'
+        )
+        get_logger().warning(message)
+    with tempfile.TemporaryDirectory() as temp_dir:
+        defaults = dict(
+            source=source, working_dir=temp_dir, clean_up=False, save_as=None
+        )
+        for k, v in defaults.items():
+            kw.setdefault(k, v)
+        intermediate_file = pre_process(**kw)
+        # After with close this "with", we lose the file, so load it just to be sure we have all we need
+        ds = load_glob(intermediate_file).load()
+    return ds
 
 
 @timed
 def pre_process(
     source: str,
     target_grid: str = None,
     max_time: ty.Optional[ty.Tuple[int, int, int]] = _DEFAULT_MAX_TIME,
     min_time: ty.Optional[ty.Tuple[int, int, int]] = None,
     save_as: str = None,
     clean_up: bool = True,
     _ma_window: int = None,
     variable_id: str = None,
+    working_dir: str = None,
 ) -> str:
     """Apply several preprocessing steps to the file located at <source>:
       - Slice the data to desired time range
       - regrid to simple grid
       - calculate corresponding area
       - calculate running mean, detrended and not-detrended
       - merge all files into one
@@ -53,43 +76,43 @@
     min_time = min_time or (0, 1, 1)  # unreasonably long ago
     target_grid = target_grid or config['analyze']['regrid_to']
     _ma_window = _ma_window or config['analyze']['moving_average_years']
     _check_time_range(source, max_time, min_time, _ma_window)
 
     cdo_int = cdo.Cdo()
     head, _ = os.path.split(source)
+    working_dir = working_dir or head
 
     # Several intermediate_files
-    f_time = os.path.join(head, 'time_sel.nc')
-    f_det = os.path.join(head, 'detrend.nc')
-    f_det_rm = os.path.join(head, f'detrend_rm_{_ma_window}.nc')
-    f_rm = os.path.join(head, f'rm_{_ma_window}.nc')
-    f_tmp = os.path.join(head, 'tmp.nc')
-    f_regrid = os.path.join(head, 'regrid.nc')
-    f_area = os.path.join(head, 'area.nc')
+    f_time = os.path.join(working_dir, 'time_sel.nc')
+    f_det = os.path.join(working_dir, 'detrend.nc')
+    f_det_rm = os.path.join(working_dir, f'detrend_rm_{_ma_window}.nc')
+    f_rm = os.path.join(working_dir, f'rm_{_ma_window}.nc')
+    f_tmp = os.path.join(working_dir, 'tmp.nc')
+    f_regrid = os.path.join(working_dir, 'regrid.nc')
+    f_area = os.path.join(working_dir, 'area.nc')
     files = [f_time, f_det, f_det_rm, f_rm, f_tmp, f_regrid, f_area]
 
-    save_as = save_as or os.path.join(head, 'result.nc')
+    save_as = save_as or os.path.join(working_dir, 'result.nc')
 
     # Several names:
     var = variable_id
     var_det = f'{var}_detrend'
     var_rm = f'{var}_run_mean_{_ma_window}'
     var_det_rm = f'{var_det}_run_mean_{_ma_window}'
 
     for p in files + [save_as]:
         if p == source:
             raise ValueError(f'source equals other path {p}')
         if os.path.exists(p):
             get_logger().warning(f'Removing {p}!')
             os.remove(p)
 
-    cdo_int.seldate(
-        f'{_fmt_date(min_time)},{_fmt_date(max_time)}', input=source, output=f_time
-    )
+    time_range = f'{_fmt_date(min_time)},{_fmt_date(max_time)}'
+    cdo_int.seldate(time_range, input=source, output=f_time)
 
     cdo_int.remapbil(target_grid, input=f_time, output=f_regrid)
     cdo_int.gridarea(input=f_regrid, output=f_area)
 
     cdo_int.detrend(input=f_regrid, output=f_tmp)
     cdo_int.chname(f'{var},{var_det}', input=f_tmp, output=f_det)
     os.remove(f_tmp)
@@ -104,17 +127,17 @@
         var_rm_name=var_rm,
     )
     os.remove(f_tmp)
 
     cdo_int.detrend(input=f_rm, output=f_tmp)
     cdo_int.chname(f'{var_rm},{var_det_rm}', input=f_tmp, output=f_det_rm)
     # remove in cleanup
-    cdo_int.merge(
-        input=' '.join([f_regrid, f_det, f_det_rm, f_rm, f_area]), output=save_as
-    )
+
+    input_files = ' '.join([f_regrid, f_det, f_det_rm, f_rm, f_area])
+    cdo_int.merge(input=input_files, output=save_as)
 
     if clean_up:
         for p in files:
             os.remove(p)
     return save_as
```

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools/analyze/region_finding.py` & `optim_esm_tools-1.1.0/optim_esm_tools/analyze/region_finding.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import optim_esm_tools as oet
 from optim_esm_tools.plotting.map_maker import MapMaker, HistoricalMapMaker
 from optim_esm_tools.analyze import tipping_criteria
+from optim_esm_tools.analyze.globals import _CMIP_HANDLER_VERSION
 from optim_esm_tools.analyze.cmip_handler import read_ds
-from optim_esm_tools.analyze.clustering import (
-    build_cluster_mask,
-    build_weighted_cluster,
-)
+from optim_esm_tools.analyze.clustering import build_cluster_mask
+from optim_esm_tools.analyze.clustering import build_weighted_cluster
+from optim_esm_tools.analyze.xarray_tools import mask_xr_ds, mask_to_reduced_dataset
 from optim_esm_tools.plotting.plot import setup_map, _show
-from optim_esm_tools.analyze.tipping_criteria import rank2d
-from optim_esm_tools.analyze.find_matches import base_from_path
-from .globals import _CMIP_HANDLER_VERSION
 
 import numpy as np
 import matplotlib.pyplot as plt
 import logging
 import xarray as xr
 
 import typing as ty
@@ -28,65 +25,14 @@
 # >>> scipy.stats.norm.cdf(3)
 # 0.9986501019683699
 # >> scipy.stats.norm.cdf(2)
 # 0.9772498680518208
 _two_sigma_percent = 97.72498680518208
 
 
-def mask_xr_ds(data_set, da_mask, masked_dims=None, drop=False):
-    # Modify the ds in place - make a copy!
-    data_set = data_set.copy()
-    if masked_dims is None:
-        masked_dims = oet.config.config['analyze']['lon_lat_dim'].split(',')
-
-    ds_start = data_set.copy()
-    func_by_drop = {True: _drop_by_mask, False: _mask_xr_ds}[drop]
-    data_set = func_by_drop(data_set, masked_dims, ds_start, da_mask)
-    data_set = data_set.assign_attrs(ds_start.attrs)
-    return data_set
-
-
-def _drop_by_mask(data_set, masked_dims, ds_start, da_mask):
-    """Drop values with masked_dims dimensions.
-    Unfortunately, data_set.where(da_mask, drop=True) sometimes leads to bad results,
-    for example for time_bnds (time, bnds) being dropped by (lon, lat). So we have to do
-    some funny bookkeeping of which data vars we can drop with data_set.where.
-    """
-
-    dropped = []
-    for k, data_array in data_set.data_vars.items():
-        if not all(dim in list(data_array.dims) for dim in masked_dims):
-            dropped += [k]
-
-    data_set = data_set.drop_vars(dropped)
-
-    data_set = data_set.where(da_mask, drop=True)
-
-    # Restore ignored variables and attributes
-    for k in dropped:
-        data_set[k] = ds_start[k]
-    return data_set
-
-
-def _mask_xr_ds(data_set, masked_dims, ds_start, da_mask):
-    """Rebuild data_set for each variable that has all masked_dims"""
-    for k, data_array in data_set.data_vars.items():
-        if all(dim in list(data_array.dims) for dim in masked_dims):
-            # First dim is time?
-            if (
-                'time' == data_array.dims[0] and data_array.shape[1:] == da_mask.T.shape
-            ) or data_array.shape == da_mask.T.shape:
-                raise ValueError(f'Please make "{k}" lat, lon, now "{data_array.dims}"')
-            da = data_set[k].where(da_mask, drop=False)
-            da = da.assign_attrs(ds_start[k].attrs)
-            data_set[k] = da
-
-    return data_set
-
-
 def plt_show(*a):
     """Wrapper to disable class methods to follow up with show"""
 
     def somedec_outer(fn):
         @wraps(fn)
         def plt_func(*args, **kwargs):
             res = fn(*args, **kwargs)
@@ -241,30 +187,26 @@
         self.log.info(f'Keeping {len(ret_m)}/{len(masks_and_clusters[0])} of masks')
         return ret_m, ret_c
 
     @plt_show
     def summarize_mask(self, mask, m_i):
         self._summarize_mask(mask)
         plt.suptitle(self.title + f' cluster {m_i}')
-        self.save(f'{self.title_label}_cluster_{m_i}')
+        self.save(f'{self.title_label}_cluster-{m_i}')
 
         self.store_mask(mask, m_i)
 
     @apply_options
     def store_mask(self, mask, m_i, store_masks=True):
         if not store_masks:
             return
         save_in = self.save_kw['save_in']
         store_in_dir = os.path.join(save_in, 'masks')
         os.makedirs(store_in_dir, exist_ok=True)
-        # Mask twice, "mask" is a np.ndarray, whereas ds.where needs a xr.DataArray.
-        # While we could make this more efficient (and only use the second step), the first step
-        # does only take ~10 ms
-        ds_masked = mask_xr_ds(self.data_set.copy(), mask)
-        ds_masked = mask_xr_ds(ds_masked, ~ds_masked['cell_area'].isnull(), drop=True)
+        ds_masked = mask_to_reduced_dataset(self.data_set, mask)
         ds_masked.to_netcdf(
             os.path.join(
                 store_in_dir,
                 f'{self.title_label}_cluster-{m_i}_v{_CMIP_HANDLER_VERSION}.nc',
             )
         )
 
@@ -417,15 +359,15 @@
         lon_lat_dim=('lon', 'lat'),
     ):
         labels = [crit.short_description for crit in self.criteria]
 
         sums = []
         for lab in labels:
             vals = self.data_set[lab].values
-            vals = rank2d(vals)
+            vals = tipping_criteria.rank2d(vals)
             vals[np.isnan(vals)] = 0
             sums.append(vals)
 
         tot_sum = np.zeros_like(sums[0])
         for s in sums:
             tot_sum += s
         tot_sum /= len(sums)
@@ -513,17 +455,16 @@
 
         ds_dummy['area_square'].plot(cbar_kwargs=mask_cbar_kw, vmin=0, extend='neither')
         plt.title('')
         if scatter_medians:
             if cluster_kw is None:
                 cluster_kw = dict()
             for m_i, cluster in enumerate(clusters):
-                ax.scatter(
-                    *np.median(cluster, axis=0), label=f'cluster {m_i}', **cluster_kw
-                )
+                lat, lon = np.median(cluster, axis=0)
+                ax.scatter(lon, lat, label=f'cluster {m_i}', **cluster_kw)
             if legend:
                 plt.legend(**oet.utils.legend_kw())
         plt.suptitle(f'Clusters {self.title}', y=0.97 if len(masks) < 4 else 0.99)
         return ax
 
     def _plot_basic_map(self):
         mm = MapMaker(self.data_set)
@@ -574,20 +515,20 @@
             )
         _ma_window = _ma_window or oet.config.config['analyze']['moving_average_years']
         masks, clusters = masks_and_clusters
         legend_kw = oet.utils.legend_kw(
             loc='upper left', bbox_to_anchor=None, mode=None, ncol=4
         )
         for m_i, (mask, cluster) in enumerate(zip(masks, clusters)):
-            x, y = np.median(cluster, axis=0)
+            lat, lon = np.median(cluster, axis=0)
             plot_labels = {
-                f'{self.variable}': f'Cluster {m_i} near ~{x:.1f}:{y:.1f}',
-                f'{self.variable}_detrend': f'Cluster {m_i} near ~{x:.1f}:{y:.1f}',
-                f'{self.variable}_detrend_run_mean_{_ma_window}': f'Cluster {m_i} $RM_{{{_ma_window}}}$ near ~{x:.1f}:{y:.1f}',
-                f'{self.variable}_run_mean_{_ma_window}': f'Cluster {m_i} $RM_{{{_ma_window}}}$ near ~{x:.1f}:{y:.1f}',
+                f'{self.variable}': f'Cluster {m_i} near ~{lat:.1f}:{lon:.1f}',
+                f'{self.variable}_detrend': f'Cluster {m_i} near ~{lat:.1f}:{lon:.1f}',
+                f'{self.variable}_detrend_run_mean_{_ma_window}': f'Cluster {m_i} $RM_{{{_ma_window}}}$ near ~{lat:.1f}:{lon:.1f}',
+                f'{self.variable}_run_mean_{_ma_window}': f'Cluster {m_i} $RM_{{{_ma_window}}}$ near ~{lat:.1f}:{lon:.1f}',
             }
             ds_sel = mask_xr_ds(self.data_set.copy(), mask)
             mm_sel = MapMaker(ds_sel)
             axes = mm_sel.time_series(
                 variable=self.variable,
                 show_std=True,
                 labels=plot_labels,
@@ -648,45 +589,24 @@
     def find_historical(
         self,
         match_to='piControl',
         look_back_extra=0,
         query_updates=None,
         search_kw=None,
     ):
-        base = base_from_path(
-            self.data_set.attrs['path'], look_back_extra=look_back_extra
+        path = self.data_set.attrs['path']
+        return oet.analyze.find_matches.associate_historical(
+            path=path,
+            data_set=None,
+            match_to=match_to,
+            look_back_extra=look_back_extra,
+            query_updates=query_updates,
+            search_kw=search_kw,
         )
 
-        search = oet.analyze.find_matches.folder_to_dict(self.data_set.attrs['path'])
-        search['activity_id'] = 'CMIP'
-        if search['experiment_id'] == match_to:
-            raise NotImplementedError(f'Cannot match {match_to} to itself!')
-        search['experiment_id'] = match_to
-        if search_kw:
-            search.update(search_kw)
-        if query_updates is None:
-            query_updates = [
-                dict(),
-                dict(variant_label='*'),
-                dict(version='*'),
-                # can lead to funny behavior as grid differences may cause breaking compares
-                dict(grid_label='*'),
-            ]
-
-        for try_n, update_query in enumerate(query_updates):
-            if try_n:
-                self.log.info(
-                    f'No results after {try_n} try, retying with {update_query}'
-                )
-            search.update(update_query)
-            this_try = oet.analyze.find_matches.find_matches(base, **search)
-            if this_try:
-                return this_try
-        raise RuntimeError(f'Looked for {search}, in {base} found nothing')
-
     @apply_options
     def get_historical_ds(self, read_ds_kw=None, **kw):
         read_ds_kw = read_ds_kw or dict()
         for k, v in dict(min_time=None, max_time=None).items():
             read_ds_kw.setdefault(k, v)
         historical_path = self.find_historical(**kw)[0]
         return read_ds(historical_path, **read_ds_kw)
@@ -714,15 +634,15 @@
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
         ds = self.data_set.copy()
         combined_score = np.ones_like(ds[labels[0]].values)
 
         for label in labels:
-            combined_score *= rank2d(ds[label].values)
+            combined_score *= tipping_criteria.rank2d(ds[label].values)
         self.check_shape(combined_score)
         masks, clusters = build_weighted_cluster(
             weights=combined_score,
             lon_coord=self.data_set[lon_lat_dim[0]].values,
             lat_coord=self.data_set[lon_lat_dim[1]].values,
             threshold=min_weight,
         )
@@ -735,15 +655,15 @@
         """Get mask for max of ii and iii and a box around that"""
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
         ds = self.data_set.copy()
         combined_score = np.ones_like(ds[labels[0]].values)
         for label in labels:
-            combined_score *= rank2d(ds[label].values)
+            combined_score *= tipping_criteria.rank2d(ds[label].values)
 
         # Combined score is fraction, not percent!
         all_mask = combined_score > (product_percentiles / 100)
 
         self.check_shape(all_mask)
 
         masks, clusters = build_cluster_mask(
```

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools/analyze/tipping_criteria.py` & `optim_esm_tools-1.1.0/optim_esm_tools/analyze/tipping_criteria.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools/config.py` & `optim_esm_tools-1.1.0/optim_esm_tools/config.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools/optim_esm_conf.ini` & `optim_esm_tools-1.1.0/optim_esm_tools/optim_esm_conf.ini`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 [constants]
 # 365.25 * 24 * 3600
 seconds_to_year = 31557600
 
 
 [versions]
-cmip_handler = 0.4.4
+cmip_handler = 0.4.5
 
 
 [display]
 progress_bar = True
 
 
 [analyze]
 regrid_to = n90
 moving_average_years = 10
 lon_lat_dim = lon,lat
 
 # If any of these names are in the dataset, remove them as they break pre-processing and are calculated for the regridded file anyway
 remove_vars = area cell_area GEOLON GEOLAT
-cartopy_projection = PlateCarree
+cartopy_projection = Robinson
 
 # In the clustering method, assume points closer than clustering_fudge_factor * max_distance belong
 # to the same cluster. See analyze.clustering._infer_max_step_size for more information
 clustering_fudge_factor = 1.1
 clustering_min_neighbors = 8
 
 # Split data sets on this year for nominal analyses
@@ -33,63 +33,67 @@
 
 [CMIP_files]
 folder_fmt = activity_id institution_id source_id experiment_id variant_label domain variable_id grid_label version
 base_name = merged.nc
 temp_file_name = temp_pre.nc
 
 excluded =
-        ; # This one only has a dataset which is 5 years long, rendering it quite useless for 10yr running means
+        # This one only has a dataset which is 5 years long, rendering it quite useless for 10yr running means
         E3SM-Project       E3SM-1-1-ECA     piControl   r1i1p1f1  *        *  gr  v20201204
         E3SM-Project       E3SM-1-1-ECA     piControl   r1i1p1f1  *        *  *   v20201203
 
-        ; # Bad data https://errata.es-doc.org/static/index.html?experiment=ssp585&institute=thu&project=cmip6&source=ciesm
-        ; THU                CIESM            ssp585      r1i1p1f1  *        *  *   v20200417
+        # Bad data https://errata.es-doc.org/static/index.html?experiment=ssp585&institute=thu&project=cmip6&source=ciesm
+        THU                CIESM            ssp585      r1i1p1f1  *        *  *   v20200417
 
-        ; ### Too short datasets ###
-        ; BCC_BCC            ESM1             ssp370      r3i1p1f1  tas      *  *   v20190702
-        ; HAMMOZ-Consortium  MPI-ESM-1-2-HAM  ssp370      r3i1p1f1  tas      *  *   v20191218
+        ### Too short datasets ###
         NCC                NorESM2-LM       ssp245      r1i1p1f2  tas      *  *   v20210908
         E3SM-Project       E3SM-1-1         ssp245      r1i1p1f1  *        *  gr  v20201109
         CNRM-CERFACS       CNRM-CM6-1       ssp245      *         *        *  *   v20200212
+        BCC_BCC            ESM1             ssp370      *         *        *  *   *
 
-        ; # These sets have data in the 1e20 range:
+        ; unstructured source grid non conformal indexing for lat/lon (one iterator i for x and y)
+        MPI-M              ICON-ESM-LR      *           *         *       *   gn  v20210215
+        MPI-M              ICON-ESM-LR      *           *         *       *   gn  v20220111
+        AWI                AWI-ESM-1-1-LR   *           r1i1p1f1  *       *   gn  v20200212
+        AWI                AWI-CM-1-1-MR    *           *         Oyear   *   gn  v20181218
+
+        # This dataset contains overlapping time stamps
+        NCC                NorESM2-MM       historical r3i1p1f1   *       *   gn  v20200702
+
+        ## Short datasets
+        ; HAMMOZ-Consortium  MPI-ESM-1-2-HAM  ssp370      r3i1p1f1  tas      *  *   v20191218
+        # These sets have data in the 1e20 range:
         ; AS-RCEC            TaiESM1          *           r1i1p1f1  siconc   *  gn  v20201124
         ; AS-RCEC            TaiESM1          *           r1i1p1f1  tos      *  gn  v20210416
         ; AS-RCEC            TaiESM1          *           r1i1p1f1  sithick  *  gn  v20210416
 
         ; #  --- TODO ---
         ; #  Verify if this exclusions are correct
         ; # Something wrong happened with the lon/lat coords.
         ; NCAR               CESM2            ssp370      r4i1p1f1  siconc   *  gn  v20200528
 
         ; # Projection fails
         ; DKRZ               MPI-ESM1-2-LR    ssp119      r1i1p1f1  siconc   *  *   v20210901
 
-
-        ; unstructured source grid non conformal indexing for lat/lon (one iterator i for x and y)
-        MPI-M              ICON-ESM-LR      *           *         *       *   gn  v20210215
-        MPI-M              ICON-ESM-LR      *           *         *       *   gn  v20220111
-        AWI                AWI-ESM-1-1-LR   *           r1i1p1f1  *       *   gn  v20200212
-        AWI                AWI-CM-1-1-MR    *           *         Oyear   *   gn  v20181218
-
 [log]
 logging_level = WARNING
 
 
 # For the wrapper that monitors real time of functions (@timed)
 [time_tool]
 min_seconds = 10
 reporter = warning
 
 
 [variable_label]
 # Labels
 tas = T
 siconc = S.I.C.
-
+tos = T
+sos = Salinity
 
 [variable_range]
 # Ranges of variables to set. Defaults to None,None
 # Ranges set by current ax always precedes these defaults!
 tas=None,None
 tas_detrend=-6,6
 siconc=-5,105
```

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools/plotting/map_maker.py` & `optim_esm_tools-1.1.0/optim_esm_tools/plotting/map_maker.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 
 import matplotlib.pyplot as plt
 
 from immutabledict import immutabledict
 from .plot import *
 from matplotlib.colors import LogNorm
 
-# import xrft
-
 from optim_esm_tools.analyze.globals import _SECONDS_TO_YEAR
 from optim_esm_tools.analyze import tipping_criteria
 
 
 class MapMaker(object):
     data_set: xr.Dataset
     labels = tuple('i ii iii iv v vi vii viii ix x'.split())
```

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools/plotting/plot.py` & `optim_esm_tools-1.1.0/optim_esm_tools/plotting/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 import matplotlib.pyplot as plt
 import optim_esm_tools as oet
 from optim_esm_tools.config import config
 
 
-def setup_map():
-    plt.gcf().add_subplot(projection=get_cartopy_projection())
+def setup_map(
+    projection=None, coastlines=True, add_features=False, **projection_kwargs
+):
+    plt.gcf().add_subplot(
+        projection=get_cartopy_projection(projection, **projection_kwargs)
+    )
     ax = plt.gca()
-    ax.coastlines()
+    if coastlines:
+        ax.coastlines()
+    if add_features:
+        import cartopy.feature as cfeature
+
+        allowed = 'LAND OCEAN COASTLINE BORDERS LAKES RIVERS'.split()
+        for feat in oet.utils.to_str_tuple(add_features):
+            assert feat.upper() in allowed, f'{feat} not in {allowed}'
+            ax.add_feature(getattr(cfeature, feat.upper()))
+
     gl = ax.gridlines(draw_labels=True)
     gl.top_labels = False
 
 
 def _show(show):
     if show:
         plt.show()
@@ -47,14 +60,14 @@
     )
 
 
 def get_unit(ds, var):
     return ds[var].attrs.get('units', '?').replace('%', '\%')
 
 
-def get_cartopy_projection():
+def get_cartopy_projection(projection=None, **projection_kwargs):
     import cartopy.crs as ccrs
 
-    projection = config['analyze']['cartopy_projection']
+    projection = projection or config['analyze']['cartopy_projection']
     if not hasattr(ccrs, projection):
         raise ValueError(f'Invalid projection {projection}')
-    return getattr(ccrs, projection)()
+    return getattr(ccrs, projection)(**projection_kwargs)
```

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools/synda_files/synda_files.py` & `optim_esm_tools-1.1.0/optim_esm_tools/synda_files/synda_files.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools/utils.py` & `optim_esm_tools-1.1.0/optim_esm_tools/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -241,14 +241,34 @@
         borderaxespad=0.0,
         frameon=True,
     )
     options.update(kw)
     return options
 
 
+def filter_keyword_arguments(
+    kw: ty.Mapping, func: type, allow_varkw: bool = False
+) -> dict:
+    """Only pass accepted keyword arguments (from kw) into function "func"
+
+    Args:
+        kw (ty.Mapping): kwargs that could go into function func
+        func (type): a function
+        allow_varkw (bool, optional): If True and the function take kwargs, just return the <kw>
+            argument. Defaults to False.
+
+    Returns:
+        dict: Filtered keyword arguments
+    """
+    spec = inspect.getfullargspec(func)
+    if allow_varkw and spec.varkw is not None:
+        return kw
+    return {k: v for k, v in kw.items() if k in spec.args}
+
+
 def check_accepts(
     accepts: ty.Mapping[str, ty.Iterable] = immutabledict(unit=('absolute', 'std')),
     do_raise: bool = True,
 ):
     """Wrapper for function if certain kwargs are from a defined list of variables.
 
     Example:
```

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools.egg-info/PKG-INFO` & `optim_esm_tools-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: optim-esm-tools
-Version: 1.0.3
+Name: optim_esm_tools
+Version: 1.1.0
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,14 +15,29 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
+        1.1.0 / 2023-07-28
+        ## What's Changed
+        *Minor change*
+        Add the required tools to analyze time series and their properties
+        * Statistical tools for time series by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/96
+        *Patch*
+        * Fix lon/lat for cluster plot and temp folder for preprocess by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/93
+        * Load intake store from intake by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/94
+        * Plotting flexibility by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/95
+        * Minor search tweak by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/97
+        
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v1.0.3...v1.1.0
+        
+        
         1.0.3 / 2023-07-24
         ------------------
         * Fix clustering fudge factor by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/91
         * Preprocessing running mean fix by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/92
         
         
         **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v1.0.2...v1.0.3
```

### Comparing `optim_esm_tools-1.0.3/optim_esm_tools.egg-info/SOURCES.txt` & `optim_esm_tools-1.1.0/optim_esm_tools.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 optim_esm_tools/analyze/clustering.py
 optim_esm_tools/analyze/cmip_handler.py
 optim_esm_tools/analyze/find_matches.py
 optim_esm_tools/analyze/globals.py
 optim_esm_tools/analyze/io.py
 optim_esm_tools/analyze/pre_process.py
 optim_esm_tools/analyze/region_finding.py
+optim_esm_tools/analyze/time_statistics.py
 optim_esm_tools/analyze/tipping_criteria.py
 optim_esm_tools/analyze/xarray_tools.py
 optim_esm_tools/plotting/__init__.py
 optim_esm_tools/plotting/map_maker.py
 optim_esm_tools/plotting/plot.py
 optim_esm_tools/synda_files/__init__.py
 optim_esm_tools/synda_files/synda_files.py
 test/test_basics.py
 test/test_clustering.py
 test/test_find_matches.py
 test/test_pangeo_download.py
 test/test_plotting.py
 test/test_region_finding.py
+test/test_time_statistics.py
 test/test_utils.py
 test/test_viewer.py
 test/test_workflow.py
 test/test_xarray_tools.py
```

### Comparing `optim_esm_tools-1.0.3/setup.py` & `optim_esm_tools-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 readme = open('README.md').read()
 history = open('HISTORY.md').read()
 requirements = open_requirements('requirements.txt')
 
 setuptools.setup(
     name='optim_esm_tools',
-    version='1.0.3',
+    version='1.1.0',
     description='Tools for OptimESM',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author='Joran R. Angevaare',
     url='https://github.com/JoranAngevaare/optim_esm_tools',
     packages=setuptools.find_packages(),
     package_dir={
```

### Comparing `optim_esm_tools-1.0.3/test/test_clustering.py` & `optim_esm_tools-1.1.0/test/test_clustering.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.3/test/test_find_matches.py` & `optim_esm_tools-1.1.0/test/test_find_matches.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.3/test/test_region_finding.py` & `optim_esm_tools-1.1.0/test/test_region_finding.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,31 +5,25 @@
 from optim_esm_tools.analyze.cmip_handler import read_ds
 import tempfile
 import os
 
 
 class Work(unittest.TestCase):
     """
-    Note of caution! cache=True can lead to funky behavoir!
+    Note of caution! _CACHE_TRUE=True can lead to funky behavior!
     """
 
     @classmethod
     def setUpClass(cls):
         for data_name in ['ssp585', 'piControl']:
             cls.get_path(data_name)
 
     @staticmethod
     def get_path(data_name, refresh=True):
-        path = optim_esm_tools._test_utils.get_file_from_pangeo(
-            data_name, refresh=refresh
-        )
-        year_path = optim_esm_tools._test_utils.year_means(path, refresh=refresh)
-        assert year_path
-        assert os.path.exists(year_path)
-        return year_path
+        return optim_esm_tools._test_utils.get_path_for_ds(data_name, refresh=refresh)
 
     def test_max_region(self, make='MaxRegion', new_opt=None, skip_save=True):
         cls = getattr(region_finding, make)
         file_path = self.get_path('ssp585', refresh=False)
 
         head, tail = os.path.split(file_path)
         extra_opt = dict(
```

### Comparing `optim_esm_tools-1.0.3/test/test_utils.py` & `optim_esm_tools-1.1.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.3/test/test_viewer.py` & `optim_esm_tools-1.1.0/test/test_viewer.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.3/test/test_workflow.py` & `optim_esm_tools-1.1.0/test/test_workflow.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.3/test/test_xarray_tools.py` & `optim_esm_tools-1.1.0/test/test_xarray_tools.py`

 * *Files identical despite different names*

