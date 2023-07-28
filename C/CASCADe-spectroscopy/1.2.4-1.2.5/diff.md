# Comparing `tmp/CASCADe-spectroscopy-1.2.4.tar.gz` & `tmp/CASCADe-spectroscopy-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CASCADe-spectroscopy-1.2.4.tar", last modified: Fri Jul 28 13:51:23 2023, max compression
+gzip compressed data, was "CASCADe-spectroscopy-1.2.5.tar", last modified: Fri Jul 28 14:14:42 2023, max compression
```

## Comparing `CASCADe-spectroscopy-1.2.4.tar` & `CASCADe-spectroscopy-1.2.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.891131 CASCADe-spectroscopy-1.2.4/
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.875131 CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/
--rw-r--r--   0 bouwman  (10420) users      (100)    21158 2023-07-28 13:51:23.000000 CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/PKG-INFO
--rw-r--r--   0 bouwman  (10420) users      (100)     1604 2023-07-28 13:51:23.000000 CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/SOURCES.txt
--rw-r--r--   0 bouwman  (10420) users      (100)        1 2023-07-28 13:51:23.000000 CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/dependency_links.txt
--rw-r--r--   0 bouwman  (10420) users      (100)      245 2023-07-28 13:51:23.000000 CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/requires.txt
--rw-r--r--   0 bouwman  (10420) users      (100)       14 2023-07-28 13:51:23.000000 CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/top_level.txt
--rw-r--r--   0 bouwman  (10420) users      (100)    35149 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/LICENSE.txt
--rw-rw-r--   0 bouwman  (10420) users      (100)      146 2022-01-29 13:05:24.000000 CASCADe-spectroscopy-1.2.4/MANIFEST.in
--rw-r--r--   0 bouwman  (10420) users      (100)    21158 2023-07-28 13:51:23.887131 CASCADe-spectroscopy-1.2.4/PKG-INFO
--rw-r--r--   0 bouwman  (10420) users      (100)    20448 2022-05-04 13:20:33.000000 CASCADe-spectroscopy-1.2.4/README.md
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/TSO/
--rw-r--r--   0 bouwman  (10420) users      (100)   111340 2023-02-01 18:11:59.000000 CASCADe-spectroscopy-1.2.4/cascade/TSO/TSO.py
--rw-r--r--   0 bouwman  (10420) users      (100)      118 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/cascade/TSO/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)      534 2023-07-28 13:25:59.000000 CASCADe-spectroscopy-1.2.4/cascade/__init__.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/build_archive/
--rw-r--r--   0 bouwman  (10420) users      (100)      150 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.4/cascade/build_archive/__init__.py
--rwxr-xr-x   0 bouwman  (10420) users      (100)    26971 2023-01-19 10:42:28.000000 CASCADe-spectroscopy-1.2.4/cascade/build_archive/build_archive.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/cpm_model/
--rw-r--r--   0 bouwman  (10420) users      (100)      138 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/cascade/cpm_model/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)   144192 2023-07-28 13:01:58.000000 CASCADe-spectroscopy-1.2.4/cascade/cpm_model/cpm_model.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/data_model/
--rw-r--r--   0 bouwman  (10420) users      (100)      139 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/cascade/data_model/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)    33058 2022-12-13 22:35:41.000000 CASCADe-spectroscopy-1.2.4/cascade/data_model/data_model.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/exoplanet_tools/
--rw-r--r--   0 bouwman  (10420) users      (100)      157 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/cascade/exoplanet_tools/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)   109672 2023-07-28 12:30:26.000000 CASCADe-spectroscopy-1.2.4/cascade/exoplanet_tools/exoplanet_tools.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/initialize/
--rw-r--r--   0 bouwman  (10420) users      (100)      142 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/cascade/initialize/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)    33472 2023-01-23 08:17:03.000000 CASCADe-spectroscopy-1.2.4/cascade/initialize/initialize.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/instruments/
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/instruments/Generic/
--rw-r--r--   0 bouwman  (10420) users      (100)    16487 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/Generic/Generic.py
--rw-r--r--   0 bouwman  (10420) users      (100)       67 2019-07-02 16:36:37.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/Generic/__init__.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.883131 CASCADe-spectroscopy-1.2.4/cascade/instruments/HST/
--rw-r--r--   0 bouwman  (10420) users      (100)    97326 2023-01-23 08:09:03.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/HST/HST.py
--rw-r--r--   0 bouwman  (10420) users      (100)      123 2019-07-01 18:06:29.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/HST/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)     2577 2019-07-02 16:05:13.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/InstrumentsBaseClasses.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.883131 CASCADe-spectroscopy-1.2.4/cascade/instruments/JWST/
--rw-r--r--   0 bouwman  (10420) users      (100)    61037 2022-12-13 19:34:07.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/JWST/JWST.py
--rw-r--r--   0 bouwman  (10420) users      (100)       68 2019-07-02 16:14:39.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/JWST/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)     5048 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/ObservationGenerator.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.883131 CASCADe-spectroscopy-1.2.4/cascade/instruments/Spitzer/
--rw-r--r--   0 bouwman  (10420) users      (100)    46648 2022-01-30 23:14:50.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/Spitzer/Spitzer.py
--rw-r--r--   0 bouwman  (10420) users      (100)      135 2019-07-01 18:06:42.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/Spitzer/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)      614 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/__init__.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.883131 CASCADe-spectroscopy-1.2.4/cascade/spectral_extraction/
--rw-r--r--   0 bouwman  (10420) users      (100)      169 2019-07-23 14:55:38.000000 CASCADe-spectroscopy-1.2.4/cascade/spectral_extraction/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)   108152 2022-07-25 12:36:07.000000 CASCADe-spectroscopy-1.2.4/cascade/spectral_extraction/spectral_extraction.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.883131 CASCADe-spectroscopy-1.2.4/cascade/utilities/
--rw-r--r--   0 bouwman  (10420) users      (100)      139 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/cascade/utilities/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)    10685 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.4/cascade/utilities/readwrite_spectra.py
--rw-r--r--   0 bouwman  (10420) users      (100)    27545 2022-07-25 12:33:13.000000 CASCADe-spectroscopy-1.2.4/cascade/utilities/utilities.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.887131 CASCADe-spectroscopy-1.2.4/cascade/verbose/
--rw-r--r--   0 bouwman  (10420) users      (100)      132 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.4/cascade/verbose/__init__.py
--rwxr-xr-x   0 bouwman  (10420) users      (100)    40342 2022-07-23 06:59:01.000000 CASCADe-spectroscopy-1.2.4/cascade/verbose/verbose.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.887131 CASCADe-spectroscopy-1.2.4/scripts/
--rwxr-xr-x   0 bouwman  (10420) users      (100)    23962 2022-01-30 20:40:13.000000 CASCADe-spectroscopy-1.2.4/scripts/build_local_hst_archive.py
--rwxr-xr-x   0 bouwman  (10420) users      (100)     7757 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.4/scripts/run_cascade.py
--rwxr-xr-x   0 bouwman  (10420) users      (100)    12362 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.4/scripts/run_cascade.sh
--rwxr-xr-x   0 bouwman  (10420) users      (100)     4042 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.4/scripts/run_stats.sh
--rwxrwxr-x   0 bouwman  (10420) users      (100)     1927 2022-02-02 15:07:16.000000 CASCADe-spectroscopy-1.2.4/scripts/setup_cascade.py
--rw-r--r--   0 bouwman  (10420) users      (100)       38 2023-07-28 13:51:23.891131 CASCADe-spectroscopy-1.2.4/setup.cfg
--rw-r--r--   0 bouwman  (10420) users      (100)     2678 2023-07-28 13:35:28.000000 CASCADe-spectroscopy-1.2.4/setup.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.887131 CASCADe-spectroscopy-1.2.4/tests/
--rw-r--r--   0 bouwman  (10420) users      (100)        0 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/tests/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)      491 2019-02-17 14:49:38.000000 CASCADe-spectroscopy-1.2.4/tests/cascade_tests.py
--rw-r--r--   0 bouwman  (10420) users      (100)     1212 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.4/tests/cpm_model_tests.py
--rw-r--r--   0 bouwman  (10420) users      (100)     4940 2019-02-17 14:50:18.000000 CASCADe-spectroscopy-1.2.4/tests/data_model_tests.py
--rw-r--r--   0 bouwman  (10420) users      (100)     5889 2022-01-31 10:08:59.000000 CASCADe-spectroscopy-1.2.4/tests/exoplanet_tools_tests.py
--rw-r--r--   0 bouwman  (10420) users      (100)     2054 2022-01-25 23:52:24.000000 CASCADe-spectroscopy-1.2.4/tests/initialize_tests.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.388091 CASCADe-spectroscopy-1.2.5/
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.376091 CASCADe-spectroscopy-1.2.5/CASCADe_spectroscopy.egg-info/
+-rw-r--r--   0 bouwman  (10420) users      (100)    21158 2023-07-28 14:14:42.000000 CASCADe-spectroscopy-1.2.5/CASCADe_spectroscopy.egg-info/PKG-INFO
+-rw-r--r--   0 bouwman  (10420) users      (100)     1604 2023-07-28 14:14:42.000000 CASCADe-spectroscopy-1.2.5/CASCADe_spectroscopy.egg-info/SOURCES.txt
+-rw-r--r--   0 bouwman  (10420) users      (100)        1 2023-07-28 14:14:42.000000 CASCADe-spectroscopy-1.2.5/CASCADe_spectroscopy.egg-info/dependency_links.txt
+-rw-r--r--   0 bouwman  (10420) users      (100)      246 2023-07-28 14:14:42.000000 CASCADe-spectroscopy-1.2.5/CASCADe_spectroscopy.egg-info/requires.txt
+-rw-r--r--   0 bouwman  (10420) users      (100)       14 2023-07-28 14:14:42.000000 CASCADe-spectroscopy-1.2.5/CASCADe_spectroscopy.egg-info/top_level.txt
+-rw-r--r--   0 bouwman  (10420) users      (100)    35149 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.5/LICENSE.txt
+-rw-rw-r--   0 bouwman  (10420) users      (100)      146 2022-01-29 13:05:24.000000 CASCADe-spectroscopy-1.2.5/MANIFEST.in
+-rw-r--r--   0 bouwman  (10420) users      (100)    21158 2023-07-28 14:14:42.388091 CASCADe-spectroscopy-1.2.5/PKG-INFO
+-rw-r--r--   0 bouwman  (10420) users      (100)    20448 2022-05-04 13:20:33.000000 CASCADe-spectroscopy-1.2.5/README.md
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.376091 CASCADe-spectroscopy-1.2.5/cascade/
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.376091 CASCADe-spectroscopy-1.2.5/cascade/TSO/
+-rw-r--r--   0 bouwman  (10420) users      (100)   111340 2023-02-01 18:11:59.000000 CASCADe-spectroscopy-1.2.5/cascade/TSO/TSO.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      118 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.5/cascade/TSO/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      534 2023-07-28 14:13:55.000000 CASCADe-spectroscopy-1.2.5/cascade/__init__.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.376091 CASCADe-spectroscopy-1.2.5/cascade/build_archive/
+-rw-r--r--   0 bouwman  (10420) users      (100)      150 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.5/cascade/build_archive/__init__.py
+-rwxr-xr-x   0 bouwman  (10420) users      (100)    26971 2023-01-19 10:42:28.000000 CASCADe-spectroscopy-1.2.5/cascade/build_archive/build_archive.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.376091 CASCADe-spectroscopy-1.2.5/cascade/cpm_model/
+-rw-r--r--   0 bouwman  (10420) users      (100)      138 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.5/cascade/cpm_model/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)   144192 2023-07-28 13:01:58.000000 CASCADe-spectroscopy-1.2.5/cascade/cpm_model/cpm_model.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.376091 CASCADe-spectroscopy-1.2.5/cascade/data_model/
+-rw-r--r--   0 bouwman  (10420) users      (100)      139 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.5/cascade/data_model/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)    33058 2022-12-13 22:35:41.000000 CASCADe-spectroscopy-1.2.5/cascade/data_model/data_model.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.376091 CASCADe-spectroscopy-1.2.5/cascade/exoplanet_tools/
+-rw-r--r--   0 bouwman  (10420) users      (100)      157 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.5/cascade/exoplanet_tools/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)   109672 2023-07-28 12:30:26.000000 CASCADe-spectroscopy-1.2.5/cascade/exoplanet_tools/exoplanet_tools.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.376091 CASCADe-spectroscopy-1.2.5/cascade/initialize/
+-rw-r--r--   0 bouwman  (10420) users      (100)      142 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.5/cascade/initialize/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)    33472 2023-01-23 08:17:03.000000 CASCADe-spectroscopy-1.2.5/cascade/initialize/initialize.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.376091 CASCADe-spectroscopy-1.2.5/cascade/instruments/
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.376091 CASCADe-spectroscopy-1.2.5/cascade/instruments/Generic/
+-rw-r--r--   0 bouwman  (10420) users      (100)    16487 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.5/cascade/instruments/Generic/Generic.py
+-rw-r--r--   0 bouwman  (10420) users      (100)       67 2019-07-02 16:36:37.000000 CASCADe-spectroscopy-1.2.5/cascade/instruments/Generic/__init__.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.380091 CASCADe-spectroscopy-1.2.5/cascade/instruments/HST/
+-rw-r--r--   0 bouwman  (10420) users      (100)    97326 2023-01-23 08:09:03.000000 CASCADe-spectroscopy-1.2.5/cascade/instruments/HST/HST.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      123 2019-07-01 18:06:29.000000 CASCADe-spectroscopy-1.2.5/cascade/instruments/HST/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     2577 2019-07-02 16:05:13.000000 CASCADe-spectroscopy-1.2.5/cascade/instruments/InstrumentsBaseClasses.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.380091 CASCADe-spectroscopy-1.2.5/cascade/instruments/JWST/
+-rw-r--r--   0 bouwman  (10420) users      (100)    61037 2022-12-13 19:34:07.000000 CASCADe-spectroscopy-1.2.5/cascade/instruments/JWST/JWST.py
+-rw-r--r--   0 bouwman  (10420) users      (100)       68 2019-07-02 16:14:39.000000 CASCADe-spectroscopy-1.2.5/cascade/instruments/JWST/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     5048 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.5/cascade/instruments/ObservationGenerator.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.380091 CASCADe-spectroscopy-1.2.5/cascade/instruments/Spitzer/
+-rw-r--r--   0 bouwman  (10420) users      (100)    46648 2022-01-30 23:14:50.000000 CASCADe-spectroscopy-1.2.5/cascade/instruments/Spitzer/Spitzer.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      135 2019-07-01 18:06:42.000000 CASCADe-spectroscopy-1.2.5/cascade/instruments/Spitzer/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      614 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.5/cascade/instruments/__init__.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.384091 CASCADe-spectroscopy-1.2.5/cascade/spectral_extraction/
+-rw-r--r--   0 bouwman  (10420) users      (100)      169 2019-07-23 14:55:38.000000 CASCADe-spectroscopy-1.2.5/cascade/spectral_extraction/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)   108152 2022-07-25 12:36:07.000000 CASCADe-spectroscopy-1.2.5/cascade/spectral_extraction/spectral_extraction.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.384091 CASCADe-spectroscopy-1.2.5/cascade/utilities/
+-rw-r--r--   0 bouwman  (10420) users      (100)      139 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.5/cascade/utilities/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)    10685 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.5/cascade/utilities/readwrite_spectra.py
+-rw-r--r--   0 bouwman  (10420) users      (100)    27545 2022-07-25 12:33:13.000000 CASCADe-spectroscopy-1.2.5/cascade/utilities/utilities.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.384091 CASCADe-spectroscopy-1.2.5/cascade/verbose/
+-rw-r--r--   0 bouwman  (10420) users      (100)      132 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.5/cascade/verbose/__init__.py
+-rwxr-xr-x   0 bouwman  (10420) users      (100)    40342 2022-07-23 06:59:01.000000 CASCADe-spectroscopy-1.2.5/cascade/verbose/verbose.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.384091 CASCADe-spectroscopy-1.2.5/scripts/
+-rwxr-xr-x   0 bouwman  (10420) users      (100)    23962 2022-01-30 20:40:13.000000 CASCADe-spectroscopy-1.2.5/scripts/build_local_hst_archive.py
+-rwxr-xr-x   0 bouwman  (10420) users      (100)     7757 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.5/scripts/run_cascade.py
+-rwxr-xr-x   0 bouwman  (10420) users      (100)    12362 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.5/scripts/run_cascade.sh
+-rwxr-xr-x   0 bouwman  (10420) users      (100)     4042 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.5/scripts/run_stats.sh
+-rwxrwxr-x   0 bouwman  (10420) users      (100)     1927 2022-02-02 15:07:16.000000 CASCADe-spectroscopy-1.2.5/scripts/setup_cascade.py
+-rw-r--r--   0 bouwman  (10420) users      (100)       38 2023-07-28 14:14:42.388091 CASCADe-spectroscopy-1.2.5/setup.cfg
+-rw-r--r--   0 bouwman  (10420) users      (100)     2679 2023-07-28 14:13:46.000000 CASCADe-spectroscopy-1.2.5/setup.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 14:14:42.388091 CASCADe-spectroscopy-1.2.5/tests/
+-rw-r--r--   0 bouwman  (10420) users      (100)        0 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.5/tests/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      491 2019-02-17 14:49:38.000000 CASCADe-spectroscopy-1.2.5/tests/cascade_tests.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     1212 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.5/tests/cpm_model_tests.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     4940 2019-02-17 14:50:18.000000 CASCADe-spectroscopy-1.2.5/tests/data_model_tests.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     5889 2022-01-31 10:08:59.000000 CASCADe-spectroscopy-1.2.5/tests/exoplanet_tools_tests.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     2054 2022-01-25 23:52:24.000000 CASCADe-spectroscopy-1.2.5/tests/initialize_tests.py
```

### Comparing `CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/PKG-INFO` & `CASCADe-spectroscopy-1.2.5/CASCADe_spectroscopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CASCADe-spectroscopy
-Version: 1.2.4
+Version: 1.2.5
 Summary: CASCADe : Calibration of trAnsit Spectroscopy using CAusal Data
 Home-page: https://jbouwman.gitlab.io/CASCADe/
 Download-URL: https://gitlab.com/jbouwman/CASCADe
 Author: Jeroen Bouwman
 Author-email: bouwman@mpia.de
 License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/SOURCES.txt` & `CASCADe-spectroscopy-1.2.5/CASCADe_spectroscopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/LICENSE.txt` & `CASCADe-spectroscopy-1.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/PKG-INFO` & `CASCADe-spectroscopy-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CASCADe-spectroscopy
-Version: 1.2.4
+Version: 1.2.5
 Summary: CASCADe : Calibration of trAnsit Spectroscopy using CAusal Data
 Home-page: https://jbouwman.gitlab.io/CASCADe/
 Download-URL: https://gitlab.com/jbouwman/CASCADe
 Author: Jeroen Bouwman
 Author-email: bouwman@mpia.de
 License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CASCADe-spectroscopy-1.2.4/README.md` & `CASCADe-spectroscopy-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/TSO/TSO.py` & `CASCADe-spectroscopy-1.2.5/cascade/TSO/TSO.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/__init__.py` & `CASCADe-spectroscopy-1.2.5/cascade/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*
 """
 CASCADe init file.
 
 @author: Jeroen Bouwman
 """
 
-__version__ = "1.2.4"
+__version__ = "1.2.5"
 __all__ = ['data_model', 'TSO', 'instruments', 'cpm_model',
            'initialize', 'exoplanet_tools', 'utilities',
            'spectral_extraction', 'build_archive', 'verbose']
 
 from . import data_model
 from . import TSO
 from . import instruments
```

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/build_archive/build_archive.py` & `CASCADe-spectroscopy-1.2.5/cascade/build_archive/build_archive.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/cpm_model/cpm_model.py` & `CASCADe-spectroscopy-1.2.5/cascade/cpm_model/cpm_model.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/data_model/data_model.py` & `CASCADe-spectroscopy-1.2.5/cascade/data_model/data_model.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/exoplanet_tools/exoplanet_tools.py` & `CASCADe-spectroscopy-1.2.5/cascade/exoplanet_tools/exoplanet_tools.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/initialize/initialize.py` & `CASCADe-spectroscopy-1.2.5/cascade/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/instruments/Generic/Generic.py` & `CASCADe-spectroscopy-1.2.5/cascade/instruments/Generic/Generic.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/instruments/HST/HST.py` & `CASCADe-spectroscopy-1.2.5/cascade/instruments/HST/HST.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/instruments/InstrumentsBaseClasses.py` & `CASCADe-spectroscopy-1.2.5/cascade/instruments/InstrumentsBaseClasses.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/instruments/JWST/JWST.py` & `CASCADe-spectroscopy-1.2.5/cascade/instruments/JWST/JWST.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/instruments/ObservationGenerator.py` & `CASCADe-spectroscopy-1.2.5/cascade/instruments/ObservationGenerator.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/instruments/Spitzer/Spitzer.py` & `CASCADe-spectroscopy-1.2.5/cascade/instruments/Spitzer/Spitzer.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/instruments/__init__.py` & `CASCADe-spectroscopy-1.2.5/cascade/instruments/__init__.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/spectral_extraction/spectral_extraction.py` & `CASCADe-spectroscopy-1.2.5/cascade/spectral_extraction/spectral_extraction.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/utilities/readwrite_spectra.py` & `CASCADe-spectroscopy-1.2.5/cascade/utilities/readwrite_spectra.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/utilities/utilities.py` & `CASCADe-spectroscopy-1.2.5/cascade/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/cascade/verbose/verbose.py` & `CASCADe-spectroscopy-1.2.5/cascade/verbose/verbose.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/scripts/build_local_hst_archive.py` & `CASCADe-spectroscopy-1.2.5/scripts/build_local_hst_archive.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/scripts/run_cascade.py` & `CASCADe-spectroscopy-1.2.5/scripts/run_cascade.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/scripts/run_cascade.sh` & `CASCADe-spectroscopy-1.2.5/scripts/run_cascade.sh`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/scripts/run_stats.sh` & `CASCADe-spectroscopy-1.2.5/scripts/run_stats.sh`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/scripts/setup_cascade.py` & `CASCADe-spectroscopy-1.2.5/scripts/setup_cascade.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/setup.py` & `CASCADe-spectroscopy-1.2.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     'description': 'CASCADe : Calibration of trAnsit Spectroscopy using CAusal Data',
     'long_description': README,
     'long_description_content_type': "text/markdown",
     'author': 'Jeroen Bouwman',
     'url': 'https://jbouwman.gitlab.io/CASCADe/',
     'download_url': 'https://gitlab.com/jbouwman/CASCADe',
     'author_email': 'bouwman@mpia.de',
-    'version': '1.2.4',
+    'version': '1.2.5',
     'python_requires': '>=3.8, <3.10',
     'license': 'GNU General Public License v3 (GPLv3)',
     'classifiers': ["Programming Language :: Python :: 3",
                     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
                     "Operating System :: OS Independent",
                     'Intended Audience :: Science/Research',
                     'Topic :: Scientific/Engineering :: Astronomy',
@@ -49,15 +49,15 @@
     'package_data': {"": scripts},
     'install_requires': ['batman-package', 'astropy', 'jplephem', 'scipy',
                          'numpy', 'configparser', 'photutils', 'pandas',
                          'scikit-learn', 'matplotlib', 'tqdm', 'seaborn',
                          'pytest', 'scikit-image>=0.19', 'sphinx', 'alabaster',
                          'networkx', 'cython', 'astroquery', 'numba',
                          'ray[default]', 'pyfiglet', 'termcolor',
-                         'statsmodels', 'h5py'
+                         'statsmodels', 'h5py',
                          'exotethys'],
     'scripts': scripts,
     'data_files': [('', [(HERE / 'README.md').as_posix(),
                          (HERE / 'LICENSE.txt').as_posix()])]
 }
 
 setuptools.setup(**config)
```

### Comparing `CASCADe-spectroscopy-1.2.4/tests/cpm_model_tests.py` & `CASCADe-spectroscopy-1.2.5/tests/cpm_model_tests.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/tests/data_model_tests.py` & `CASCADe-spectroscopy-1.2.5/tests/data_model_tests.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/tests/exoplanet_tools_tests.py` & `CASCADe-spectroscopy-1.2.5/tests/exoplanet_tools_tests.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.4/tests/initialize_tests.py` & `CASCADe-spectroscopy-1.2.5/tests/initialize_tests.py`

 * *Files identical despite different names*

