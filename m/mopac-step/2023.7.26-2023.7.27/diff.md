# Comparing `tmp/mopac_step-2023.7.26.tar.gz` & `tmp/mopac_step-2023.7.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mopac_step-2023.7.26.tar", last modified: Wed Jul 26 20:42:00 2023, max compression
+gzip compressed data, was "mopac_step-2023.7.27.tar", last modified: Fri Jul 28 00:52:50 2023, max compression
```

## Comparing `mopac_step-2023.7.26.tar` & `mopac_step-2023.7.27.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.725808 mopac_step-2023.7.26/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-26 20:42:00.725808 mopac_step-2023.7.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.717808 mopac_step-2023.7.26/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.717808 mopac_step-2023.7.26/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.717808 mopac_step-2023.7.26/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.721808 mopac_step-2023.7.26/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.721808 mopac_step-2023.7.26/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.721808 mopac_step-2023.7.26/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.729808 mopac_step-2023.7.26/mopac_step/
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-26 20:42:00.729808 mopac_step-2023.7.26/mopac_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.725808 mopac_step-2023.7.26/mopac_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/data/configuration.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24413 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/data/seamm-mopac.yml
--rw-r--r--   0 runner    (1001) docker     (123)    41932 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/forceconstants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/forceconstants_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/forceconstants_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/ir_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/ir_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/lewis_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/lewis_structure_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/lewis_structure_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    62438 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/mopac.py
--rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/mopac_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/mopac_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/optimization_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/thermodynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/thermodynamics_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/thermodynamics_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/tk_forceconstants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/tk_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/tk_lewis_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/tk_mopac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/tk_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/tk_thermodynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.725808 mopac_step-2023.7.26/mopac_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-26 20:42:00.000000 mopac_step-2023.7.26/mopac_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-26 20:42:00.000000 mopac_step-2023.7.26/mopac_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:42:00.000000 mopac_step-2023.7.26/mopac_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-26 20:42:00.000000 mopac_step-2023.7.26/mopac_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 20:42:00.000000 mopac_step-2023.7.26/mopac_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 20:42:00.000000 mopac_step-2023.7.26/mopac_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:41:40.000000 mopac_step-2023.7.26/mopac_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-26 20:42:00.725808 mopac_step-2023.7.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.725808 mopac_step-2023.7.26/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/tests/test_mopac_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:52:50.696977 mopac_step-2023.7.27/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-28 00:52:50.696977 mopac_step-2023.7.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:52:50.680976 mopac_step-2023.7.27/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:52:50.680976 mopac_step-2023.7.27/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:52:50.680976 mopac_step-2023.7.27/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:52:50.684976 mopac_step-2023.7.27/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:52:50.684976 mopac_step-2023.7.27/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:52:50.684976 mopac_step-2023.7.27/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:52:50.700977 mopac_step-2023.7.27/mopac_step/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-28 00:52:50.700977 mopac_step-2023.7.27/mopac_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:52:50.696977 mopac_step-2023.7.27/mopac_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/data/configuration.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24413 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/data/seamm-mopac.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    41936 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/forceconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/forceconstants_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/forceconstants_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/ir_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/ir_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/lewis_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/lewis_structure_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/lewis_structure_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62438 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/mopac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/mopac_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/mopac_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/optimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/thermodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/thermodynamics_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/thermodynamics_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/tk_forceconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/tk_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/tk_lewis_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/tk_mopac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/tk_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/mopac_step/tk_thermodynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:52:50.696977 mopac_step-2023.7.27/mopac_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-28 00:52:50.000000 mopac_step-2023.7.27/mopac_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-28 00:52:50.000000 mopac_step-2023.7.27/mopac_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 00:52:50.000000 mopac_step-2023.7.27/mopac_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-28 00:52:50.000000 mopac_step-2023.7.27/mopac_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 00:52:50.000000 mopac_step-2023.7.27/mopac_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 00:52:50.000000 mopac_step-2023.7.27/mopac_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 00:52:29.000000 mopac_step-2023.7.27/mopac_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-28 00:52:50.700977 mopac_step-2023.7.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:52:50.696977 mopac_step-2023.7.27/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/tests/test_mopac_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-28 00:52:21.000000 mopac_step-2023.7.27/versioneer.py
```

### Comparing `mopac_step-2023.7.26/CONTRIBUTING.rst` & `mopac_step-2023.7.27/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/HISTORY.rst` & `mopac_step-2023.7.27/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 =======
 History
 =======
+2023.7.27 -- Bugfix: printing bond order info
+  * If the bond orders were printed but not used on the system, the code crashed.
+    
 2023.7.26 -- Added output of bond orders
   * Also added capability to use the bond orders to put bond multiplicities on the
     structure.
     
 2023.7.24 -- Bugfix in Lewis structure with bond orders
   * Major issue in getting the bonds from the Lewis structure where the atoms and bond
     orders were mixed up.
```

### Comparing `mopac_step-2023.7.26/LICENSE` & `mopac_step-2023.7.27/LICENSE`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/PKG-INFO` & `mopac_step-2023.7.27/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mopac_step
-Version: 2023.7.26
+Version: 2023.7.27
 Summary: A SEAMM plug-in to setup, run and analyze semiempirical calculations with MOPAC
 Home-page: https://github.com/molssi-seam/mopac_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,MOPAC,semiempirical,orbitals
 Platform: Linux
@@ -89,14 +89,17 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.7.27 -- Bugfix: printing bond order info
+  * If the bond orders were printed but not used on the system, the code crashed.
+    
 2023.7.26 -- Added output of bond orders
   * Also added capability to use the bond orders to put bond multiplicities on the
     structure.
     
 2023.7.24 -- Bugfix in Lewis structure with bond orders
   * Major issue in getting the bonds from the Lewis structure where the atoms and bond
     orders were mixed up.
```

### Comparing `mopac_step-2023.7.26/README.rst` & `mopac_step-2023.7.27/README.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/docs/Makefile` & `mopac_step-2023.7.27/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/docs/_static/SEAMM inverted.png` & `mopac_step-2023.7.27/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/docs/_static/SEAMM logo.png` & `mopac_step-2023.7.27/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/docs/_static/molssi_main_logo.png` & `mopac_step-2023.7.27/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/docs/_static/molssi_main_logo_inverted_white.png` & `mopac_step-2023.7.27/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/docs/_static/molssi_square.png` & `mopac_step-2023.7.27/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/docs/_static/nsf.png` & `mopac_step-2023.7.27/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/docs/conf.py` & `mopac_step-2023.7.27/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/docs/developer_guide/installation.rst` & `mopac_step-2023.7.27/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/docs/getting_started/index.rst` & `mopac_step-2023.7.27/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/docs/index.rst` & `mopac_step-2023.7.27/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/docs/make.bat` & `mopac_step-2023.7.27/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/__init__.py` & `mopac_step-2023.7.27/mopac_step/__init__.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/data/configuration.txt` & `mopac_step-2023.7.27/mopac_step/data/configuration.txt`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/data/properties.csv` & `mopac_step-2023.7.27/mopac_step/data/properties.csv`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/data/references.bib` & `mopac_step-2023.7.27/mopac_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/energy.py` & `mopac_step-2023.7.27/mopac_step/energy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1092,10 +1092,10 @@
             configuration.bonds.delete()
             configuration.bonds.append(i=iatoms, j=jatoms, bondorder=bond_order)
             text2 = (
                 "\nReplaced the bonds in the configuration with those from the "
                 "calculated bond orders.\n"
             )
 
-        text += str(__(text2, indent=self.indent + 4 * " "))
+            text += str(__(text2, indent=self.indent + 4 * " "))
 
         return text
```

### Comparing `mopac_step-2023.7.26/mopac_step/energy_parameters.py` & `mopac_step-2023.7.27/mopac_step/energy_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/energy_step.py` & `mopac_step-2023.7.27/mopac_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/forceconstants.py` & `mopac_step-2023.7.27/mopac_step/forceconstants.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/forceconstants_parameters.py` & `mopac_step-2023.7.27/mopac_step/forceconstants_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/forceconstants_step.py` & `mopac_step-2023.7.27/mopac_step/forceconstants_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/installer.py` & `mopac_step-2023.7.27/mopac_step/installer.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/ir.py` & `mopac_step-2023.7.27/mopac_step/ir.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/ir_parameters.py` & `mopac_step-2023.7.27/mopac_step/ir_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/ir_step.py` & `mopac_step-2023.7.27/mopac_step/ir_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/lewis_structure.py` & `mopac_step-2023.7.27/mopac_step/lewis_structure.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/lewis_structure_parameters.py` & `mopac_step-2023.7.27/mopac_step/lewis_structure_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/lewis_structure_step.py` & `mopac_step-2023.7.27/mopac_step/lewis_structure_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/metadata.py` & `mopac_step-2023.7.27/mopac_step/metadata.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/mopac.py` & `mopac_step-2023.7.27/mopac_step/mopac.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/mopac_base.py` & `mopac_step-2023.7.27/mopac_step/mopac_base.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/mopac_step.py` & `mopac_step-2023.7.27/mopac_step/mopac_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/optimization.py` & `mopac_step-2023.7.27/mopac_step/optimization.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/optimization_parameters.py` & `mopac_step-2023.7.27/mopac_step/optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/optimization_step.py` & `mopac_step-2023.7.27/mopac_step/optimization_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/thermodynamics.py` & `mopac_step-2023.7.27/mopac_step/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/thermodynamics_parameters.py` & `mopac_step-2023.7.27/mopac_step/thermodynamics_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/thermodynamics_step.py` & `mopac_step-2023.7.27/mopac_step/thermodynamics_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/tk_energy.py` & `mopac_step-2023.7.27/mopac_step/tk_energy.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/tk_forceconstants.py` & `mopac_step-2023.7.27/mopac_step/tk_forceconstants.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/tk_ir.py` & `mopac_step-2023.7.27/mopac_step/tk_ir.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/tk_lewis_structure.py` & `mopac_step-2023.7.27/mopac_step/tk_lewis_structure.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/tk_mopac.py` & `mopac_step-2023.7.27/mopac_step/tk_mopac.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/tk_optimization.py` & `mopac_step-2023.7.27/mopac_step/tk_optimization.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step/tk_thermodynamics.py` & `mopac_step-2023.7.27/mopac_step/tk_thermodynamics.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step.egg-info/PKG-INFO` & `mopac_step-2023.7.27/mopac_step.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mopac-step
-Version: 2023.7.26
+Version: 2023.7.27
 Summary: A SEAMM plug-in to setup, run and analyze semiempirical calculations with MOPAC
 Home-page: https://github.com/molssi-seam/mopac_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,MOPAC,semiempirical,orbitals
 Platform: Linux
@@ -89,14 +89,17 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.7.27 -- Bugfix: printing bond order info
+  * If the bond orders were printed but not used on the system, the code crashed.
+    
 2023.7.26 -- Added output of bond orders
   * Also added capability to use the bond orders to put bond multiplicities on the
     structure.
     
 2023.7.24 -- Bugfix in Lewis structure with bond orders
   * Major issue in getting the bonds from the Lewis structure where the atoms and bond
     orders were mixed up.
```

### Comparing `mopac_step-2023.7.26/mopac_step.egg-info/SOURCES.txt` & `mopac_step-2023.7.27/mopac_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/mopac_step.egg-info/entry_points.txt` & `mopac_step-2023.7.27/mopac_step.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/setup.py` & `mopac_step-2023.7.27/setup.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/tests/test_mopac_step.py` & `mopac_step-2023.7.27/tests/test_mopac_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.26/versioneer.py` & `mopac_step-2023.7.27/versioneer.py`

 * *Files identical despite different names*

