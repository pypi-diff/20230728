# Comparing `tmp/CASCADe-spectroscopy-1.2.3.tar.gz` & `tmp/CASCADe-spectroscopy-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CASCADe-spectroscopy-1.2.3.tar", last modified: Sun Jul 16 10:35:58 2023, max compression
+gzip compressed data, was "CASCADe-spectroscopy-1.2.4.tar", last modified: Fri Jul 28 13:51:23 2023, max compression
```

## Comparing `CASCADe-spectroscopy-1.2.3.tar` & `CASCADe-spectroscopy-1.2.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.835157 CASCADe-spectroscopy-1.2.3/
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.819157 CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/
--rw-r--r--   0 bouwman  (10420) users      (100)    21158 2023-07-16 10:35:58.000000 CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/PKG-INFO
--rw-r--r--   0 bouwman  (10420) users      (100)     1604 2023-07-16 10:35:58.000000 CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/SOURCES.txt
--rw-r--r--   0 bouwman  (10420) users      (100)        1 2023-07-16 10:35:58.000000 CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/dependency_links.txt
--rw-r--r--   0 bouwman  (10420) users      (100)      241 2023-07-16 10:35:58.000000 CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/requires.txt
--rw-r--r--   0 bouwman  (10420) users      (100)       14 2023-07-16 10:35:58.000000 CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/top_level.txt
--rw-r--r--   0 bouwman  (10420) users      (100)    35149 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/LICENSE.txt
--rw-rw-r--   0 bouwman  (10420) users      (100)      146 2022-01-29 13:05:24.000000 CASCADe-spectroscopy-1.2.3/MANIFEST.in
--rw-r--r--   0 bouwman  (10420) users      (100)    21158 2023-07-16 10:35:58.835157 CASCADe-spectroscopy-1.2.3/PKG-INFO
--rw-r--r--   0 bouwman  (10420) users      (100)    20448 2022-05-04 13:20:33.000000 CASCADe-spectroscopy-1.2.3/README.md
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.819157 CASCADe-spectroscopy-1.2.3/cascade/
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.819157 CASCADe-spectroscopy-1.2.3/cascade/TSO/
--rw-r--r--   0 bouwman  (10420) users      (100)   111340 2023-02-01 18:11:59.000000 CASCADe-spectroscopy-1.2.3/cascade/TSO/TSO.py
--rw-r--r--   0 bouwman  (10420) users      (100)      118 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/cascade/TSO/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)      534 2023-07-16 10:27:24.000000 CASCADe-spectroscopy-1.2.3/cascade/__init__.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.819157 CASCADe-spectroscopy-1.2.3/cascade/build_archive/
--rw-r--r--   0 bouwman  (10420) users      (100)      150 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.3/cascade/build_archive/__init__.py
--rwxr-xr-x   0 bouwman  (10420) users      (100)    26971 2023-01-19 10:42:28.000000 CASCADe-spectroscopy-1.2.3/cascade/build_archive/build_archive.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.823157 CASCADe-spectroscopy-1.2.3/cascade/cpm_model/
--rw-r--r--   0 bouwman  (10420) users      (100)      138 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/cascade/cpm_model/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)   143269 2023-02-09 20:42:11.000000 CASCADe-spectroscopy-1.2.3/cascade/cpm_model/cpm_model.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.823157 CASCADe-spectroscopy-1.2.3/cascade/data_model/
--rw-r--r--   0 bouwman  (10420) users      (100)      139 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/cascade/data_model/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)    33058 2022-12-13 22:35:41.000000 CASCADe-spectroscopy-1.2.3/cascade/data_model/data_model.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.823157 CASCADe-spectroscopy-1.2.3/cascade/exoplanet_tools/
--rw-r--r--   0 bouwman  (10420) users      (100)      157 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/cascade/exoplanet_tools/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)   106303 2023-07-16 10:10:15.000000 CASCADe-spectroscopy-1.2.3/cascade/exoplanet_tools/exoplanet_tools.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.823157 CASCADe-spectroscopy-1.2.3/cascade/initialize/
--rw-r--r--   0 bouwman  (10420) users      (100)      142 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/cascade/initialize/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)    33472 2023-01-23 08:17:03.000000 CASCADe-spectroscopy-1.2.3/cascade/initialize/initialize.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.827157 CASCADe-spectroscopy-1.2.3/cascade/instruments/
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.827157 CASCADe-spectroscopy-1.2.3/cascade/instruments/Generic/
--rw-r--r--   0 bouwman  (10420) users      (100)    16487 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/Generic/Generic.py
--rw-r--r--   0 bouwman  (10420) users      (100)       67 2019-07-02 16:36:37.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/Generic/__init__.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.827157 CASCADe-spectroscopy-1.2.3/cascade/instruments/HST/
--rw-r--r--   0 bouwman  (10420) users      (100)    97326 2023-01-23 08:09:03.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/HST/HST.py
--rw-r--r--   0 bouwman  (10420) users      (100)      123 2019-07-01 18:06:29.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/HST/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)     2577 2019-07-02 16:05:13.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/InstrumentsBaseClasses.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.831157 CASCADe-spectroscopy-1.2.3/cascade/instruments/JWST/
--rw-r--r--   0 bouwman  (10420) users      (100)    61037 2022-12-13 19:34:07.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/JWST/JWST.py
--rw-r--r--   0 bouwman  (10420) users      (100)       68 2019-07-02 16:14:39.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/JWST/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)     5048 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/ObservationGenerator.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.831157 CASCADe-spectroscopy-1.2.3/cascade/instruments/Spitzer/
--rw-r--r--   0 bouwman  (10420) users      (100)    46648 2022-01-30 23:14:50.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/Spitzer/Spitzer.py
--rw-r--r--   0 bouwman  (10420) users      (100)      135 2019-07-01 18:06:42.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/Spitzer/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)      614 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/__init__.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.831157 CASCADe-spectroscopy-1.2.3/cascade/spectral_extraction/
--rw-r--r--   0 bouwman  (10420) users      (100)      169 2019-07-23 14:55:38.000000 CASCADe-spectroscopy-1.2.3/cascade/spectral_extraction/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)   108152 2022-07-25 12:36:07.000000 CASCADe-spectroscopy-1.2.3/cascade/spectral_extraction/spectral_extraction.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.831157 CASCADe-spectroscopy-1.2.3/cascade/utilities/
--rw-r--r--   0 bouwman  (10420) users      (100)      139 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/cascade/utilities/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)    10685 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.3/cascade/utilities/readwrite_spectra.py
--rw-r--r--   0 bouwman  (10420) users      (100)    27545 2022-07-25 12:33:13.000000 CASCADe-spectroscopy-1.2.3/cascade/utilities/utilities.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.831157 CASCADe-spectroscopy-1.2.3/cascade/verbose/
--rw-r--r--   0 bouwman  (10420) users      (100)      132 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.3/cascade/verbose/__init__.py
--rwxr-xr-x   0 bouwman  (10420) users      (100)    40342 2022-07-23 06:59:01.000000 CASCADe-spectroscopy-1.2.3/cascade/verbose/verbose.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.835157 CASCADe-spectroscopy-1.2.3/scripts/
--rwxr-xr-x   0 bouwman  (10420) users      (100)    23962 2022-01-30 20:40:13.000000 CASCADe-spectroscopy-1.2.3/scripts/build_local_hst_archive.py
--rwxr-xr-x   0 bouwman  (10420) users      (100)     7757 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.3/scripts/run_cascade.py
--rwxr-xr-x   0 bouwman  (10420) users      (100)    12362 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.3/scripts/run_cascade.sh
--rwxr-xr-x   0 bouwman  (10420) users      (100)     4042 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.3/scripts/run_stats.sh
--rwxrwxr-x   0 bouwman  (10420) users      (100)     1927 2022-02-02 15:07:16.000000 CASCADe-spectroscopy-1.2.3/scripts/setup_cascade.py
--rw-r--r--   0 bouwman  (10420) users      (100)       38 2023-07-16 10:35:58.835157 CASCADe-spectroscopy-1.2.3/setup.cfg
--rw-r--r--   0 bouwman  (10420) users      (100)     2671 2023-07-16 10:27:24.000000 CASCADe-spectroscopy-1.2.3/setup.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.835157 CASCADe-spectroscopy-1.2.3/tests/
--rw-r--r--   0 bouwman  (10420) users      (100)        0 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/tests/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)      491 2019-02-17 14:49:38.000000 CASCADe-spectroscopy-1.2.3/tests/cascade_tests.py
--rw-r--r--   0 bouwman  (10420) users      (100)     1212 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.3/tests/cpm_model_tests.py
--rw-r--r--   0 bouwman  (10420) users      (100)     4940 2019-02-17 14:50:18.000000 CASCADe-spectroscopy-1.2.3/tests/data_model_tests.py
--rw-r--r--   0 bouwman  (10420) users      (100)     5889 2022-01-31 10:08:59.000000 CASCADe-spectroscopy-1.2.3/tests/exoplanet_tools_tests.py
--rw-r--r--   0 bouwman  (10420) users      (100)     2054 2022-01-25 23:52:24.000000 CASCADe-spectroscopy-1.2.3/tests/initialize_tests.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.891131 CASCADe-spectroscopy-1.2.4/
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.875131 CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/
+-rw-r--r--   0 bouwman  (10420) users      (100)    21158 2023-07-28 13:51:23.000000 CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/PKG-INFO
+-rw-r--r--   0 bouwman  (10420) users      (100)     1604 2023-07-28 13:51:23.000000 CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/SOURCES.txt
+-rw-r--r--   0 bouwman  (10420) users      (100)        1 2023-07-28 13:51:23.000000 CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/dependency_links.txt
+-rw-r--r--   0 bouwman  (10420) users      (100)      245 2023-07-28 13:51:23.000000 CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/requires.txt
+-rw-r--r--   0 bouwman  (10420) users      (100)       14 2023-07-28 13:51:23.000000 CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/top_level.txt
+-rw-r--r--   0 bouwman  (10420) users      (100)    35149 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/LICENSE.txt
+-rw-rw-r--   0 bouwman  (10420) users      (100)      146 2022-01-29 13:05:24.000000 CASCADe-spectroscopy-1.2.4/MANIFEST.in
+-rw-r--r--   0 bouwman  (10420) users      (100)    21158 2023-07-28 13:51:23.887131 CASCADe-spectroscopy-1.2.4/PKG-INFO
+-rw-r--r--   0 bouwman  (10420) users      (100)    20448 2022-05-04 13:20:33.000000 CASCADe-spectroscopy-1.2.4/README.md
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/TSO/
+-rw-r--r--   0 bouwman  (10420) users      (100)   111340 2023-02-01 18:11:59.000000 CASCADe-spectroscopy-1.2.4/cascade/TSO/TSO.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      118 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/cascade/TSO/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      534 2023-07-28 13:25:59.000000 CASCADe-spectroscopy-1.2.4/cascade/__init__.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/build_archive/
+-rw-r--r--   0 bouwman  (10420) users      (100)      150 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.4/cascade/build_archive/__init__.py
+-rwxr-xr-x   0 bouwman  (10420) users      (100)    26971 2023-01-19 10:42:28.000000 CASCADe-spectroscopy-1.2.4/cascade/build_archive/build_archive.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/cpm_model/
+-rw-r--r--   0 bouwman  (10420) users      (100)      138 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/cascade/cpm_model/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)   144192 2023-07-28 13:01:58.000000 CASCADe-spectroscopy-1.2.4/cascade/cpm_model/cpm_model.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/data_model/
+-rw-r--r--   0 bouwman  (10420) users      (100)      139 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/cascade/data_model/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)    33058 2022-12-13 22:35:41.000000 CASCADe-spectroscopy-1.2.4/cascade/data_model/data_model.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/exoplanet_tools/
+-rw-r--r--   0 bouwman  (10420) users      (100)      157 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/cascade/exoplanet_tools/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)   109672 2023-07-28 12:30:26.000000 CASCADe-spectroscopy-1.2.4/cascade/exoplanet_tools/exoplanet_tools.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/initialize/
+-rw-r--r--   0 bouwman  (10420) users      (100)      142 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/cascade/initialize/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)    33472 2023-01-23 08:17:03.000000 CASCADe-spectroscopy-1.2.4/cascade/initialize/initialize.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/instruments/
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.879131 CASCADe-spectroscopy-1.2.4/cascade/instruments/Generic/
+-rw-r--r--   0 bouwman  (10420) users      (100)    16487 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/Generic/Generic.py
+-rw-r--r--   0 bouwman  (10420) users      (100)       67 2019-07-02 16:36:37.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/Generic/__init__.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.883131 CASCADe-spectroscopy-1.2.4/cascade/instruments/HST/
+-rw-r--r--   0 bouwman  (10420) users      (100)    97326 2023-01-23 08:09:03.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/HST/HST.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      123 2019-07-01 18:06:29.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/HST/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     2577 2019-07-02 16:05:13.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/InstrumentsBaseClasses.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.883131 CASCADe-spectroscopy-1.2.4/cascade/instruments/JWST/
+-rw-r--r--   0 bouwman  (10420) users      (100)    61037 2022-12-13 19:34:07.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/JWST/JWST.py
+-rw-r--r--   0 bouwman  (10420) users      (100)       68 2019-07-02 16:14:39.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/JWST/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     5048 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/ObservationGenerator.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.883131 CASCADe-spectroscopy-1.2.4/cascade/instruments/Spitzer/
+-rw-r--r--   0 bouwman  (10420) users      (100)    46648 2022-01-30 23:14:50.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/Spitzer/Spitzer.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      135 2019-07-01 18:06:42.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/Spitzer/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      614 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.4/cascade/instruments/__init__.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.883131 CASCADe-spectroscopy-1.2.4/cascade/spectral_extraction/
+-rw-r--r--   0 bouwman  (10420) users      (100)      169 2019-07-23 14:55:38.000000 CASCADe-spectroscopy-1.2.4/cascade/spectral_extraction/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)   108152 2022-07-25 12:36:07.000000 CASCADe-spectroscopy-1.2.4/cascade/spectral_extraction/spectral_extraction.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.883131 CASCADe-spectroscopy-1.2.4/cascade/utilities/
+-rw-r--r--   0 bouwman  (10420) users      (100)      139 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/cascade/utilities/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)    10685 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.4/cascade/utilities/readwrite_spectra.py
+-rw-r--r--   0 bouwman  (10420) users      (100)    27545 2022-07-25 12:33:13.000000 CASCADe-spectroscopy-1.2.4/cascade/utilities/utilities.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.887131 CASCADe-spectroscopy-1.2.4/cascade/verbose/
+-rw-r--r--   0 bouwman  (10420) users      (100)      132 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.4/cascade/verbose/__init__.py
+-rwxr-xr-x   0 bouwman  (10420) users      (100)    40342 2022-07-23 06:59:01.000000 CASCADe-spectroscopy-1.2.4/cascade/verbose/verbose.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.887131 CASCADe-spectroscopy-1.2.4/scripts/
+-rwxr-xr-x   0 bouwman  (10420) users      (100)    23962 2022-01-30 20:40:13.000000 CASCADe-spectroscopy-1.2.4/scripts/build_local_hst_archive.py
+-rwxr-xr-x   0 bouwman  (10420) users      (100)     7757 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.4/scripts/run_cascade.py
+-rwxr-xr-x   0 bouwman  (10420) users      (100)    12362 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.4/scripts/run_cascade.sh
+-rwxr-xr-x   0 bouwman  (10420) users      (100)     4042 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.4/scripts/run_stats.sh
+-rwxrwxr-x   0 bouwman  (10420) users      (100)     1927 2022-02-02 15:07:16.000000 CASCADe-spectroscopy-1.2.4/scripts/setup_cascade.py
+-rw-r--r--   0 bouwman  (10420) users      (100)       38 2023-07-28 13:51:23.891131 CASCADe-spectroscopy-1.2.4/setup.cfg
+-rw-r--r--   0 bouwman  (10420) users      (100)     2678 2023-07-28 13:35:28.000000 CASCADe-spectroscopy-1.2.4/setup.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-28 13:51:23.887131 CASCADe-spectroscopy-1.2.4/tests/
+-rw-r--r--   0 bouwman  (10420) users      (100)        0 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.4/tests/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      491 2019-02-17 14:49:38.000000 CASCADe-spectroscopy-1.2.4/tests/cascade_tests.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     1212 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.4/tests/cpm_model_tests.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     4940 2019-02-17 14:50:18.000000 CASCADe-spectroscopy-1.2.4/tests/data_model_tests.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     5889 2022-01-31 10:08:59.000000 CASCADe-spectroscopy-1.2.4/tests/exoplanet_tools_tests.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     2054 2022-01-25 23:52:24.000000 CASCADe-spectroscopy-1.2.4/tests/initialize_tests.py
```

### Comparing `CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/PKG-INFO` & `CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CASCADe-spectroscopy
-Version: 1.2.3
+Version: 1.2.4
 Summary: CASCADe : Calibration of trAnsit Spectroscopy using CAusal Data
 Home-page: https://jbouwman.gitlab.io/CASCADe/
 Download-URL: https://gitlab.com/jbouwman/CASCADe
 Author: Jeroen Bouwman
 Author-email: bouwman@mpia.de
 License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/SOURCES.txt` & `CASCADe-spectroscopy-1.2.4/CASCADe_spectroscopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/LICENSE.txt` & `CASCADe-spectroscopy-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/PKG-INFO` & `CASCADe-spectroscopy-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CASCADe-spectroscopy
-Version: 1.2.3
+Version: 1.2.4
 Summary: CASCADe : Calibration of trAnsit Spectroscopy using CAusal Data
 Home-page: https://jbouwman.gitlab.io/CASCADe/
 Download-URL: https://gitlab.com/jbouwman/CASCADe
 Author: Jeroen Bouwman
 Author-email: bouwman@mpia.de
 License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CASCADe-spectroscopy-1.2.3/README.md` & `CASCADe-spectroscopy-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/TSO/TSO.py` & `CASCADe-spectroscopy-1.2.4/cascade/TSO/TSO.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/__init__.py` & `CASCADe-spectroscopy-1.2.4/cascade/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*
 """
 CASCADe init file.
 
 @author: Jeroen Bouwman
 """
 
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 __all__ = ['data_model', 'TSO', 'instruments', 'cpm_model',
            'initialize', 'exoplanet_tools', 'utilities',
            'spectral_extraction', 'build_archive', 'verbose']
 
 from . import data_model
 from . import TSO
 from . import instruments
```

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/build_archive/build_archive.py` & `CASCADe-spectroscopy-1.2.4/cascade/build_archive/build_archive.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/cpm_model/cpm_model.py` & `CASCADe-spectroscopy-1.2.4/cascade/cpm_model/cpm_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from scipy.linalg import solve_triangular
 from scipy.linalg import cholesky
 import astropy.units as u
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import StandardScaler
 
 from ..exoplanet_tools import lightcurve
+from ..exoplanet_tools import  spotprofile
 from ..data_model import SpectralData
 from ..data_model import SpectralDataTimeSeries
 from cascade import __version__
 
 __all__ = ['ols',
            'check_causality', 'select_regressors', 'return_design_matrix',
            'log_likelihood', 'modified_AIC', 'create_regularization_matrix',
@@ -671,32 +672,37 @@
 
         Returns
         -------
         None.
 
         """
         self.lightcurve_model = lightcurve(self.cascade_configuration)
+        self.spot_model = spotprofile(self.cascade_configuration)
         try:
             time_offset = \
                 ast.literal_eval(self.cascade_configuration.model_time_offset)
         except AttributeError:
             time_offset = 0.0
         fit_lightcurve_model, fit_ld_correcton, fit_dilution_correction = \
             self.lightcurve_model.interpolated_lc_model(
                 self.fit_dataset, time_offset=time_offset
                                                         )
         mid_transit_time = \
             self.lightcurve_model.return_mid_transit(
                 self.fit_dataset, time_offset=time_offset
                                                      )
+
+        fit_spot_model = self.spot_model.return_spot_profile(self.fit_dataset)
+
         self.fit_lightcurve_model = fit_lightcurve_model
         self.fit_ld_correcton = fit_ld_correcton
         self.fit_dilution_correction = fit_dilution_correction
         self.mid_transit_time = mid_transit_time
         self.fit_ld_coefficients = self.lightcurve_model.limbdarkning_model.ld
+        self.fit_spot_model = fit_spot_model
 
     def get_lightcurve_model(self):
         """
         Get the lightcurve model.
 
         Returns
         -------
@@ -908,14 +914,20 @@
         additional_regressors = []
         for regressor in self.regression_parameters.additional_regressor_list:
             additional_regressors.append(
                 self.select_data(getattr(self, 'regressor_'+regressor),
                                  selection,
                                  bootstrap_indici=bootstrap_indici)
                                         )
+        if self.fit_spot_model is not np.nan:
+             additional_regressors.append(
+                 self.select_data(self.fit_spot_model, selection,
+                                  bootstrap_indici=bootstrap_indici)
+                                         )
+
         n_additional = len(additional_regressors) + 2
         regression_matrix = \
             np.vstack(additional_regressors+[regression_matrix])
         regression_matrix = self.RS.fit_transform(regression_matrix.T).T
 
         lc = self.select_data(self.fit_lightcurve_model, selection,
                               bootstrap_indici=bootstrap_indici)
@@ -1188,16 +1200,27 @@
             self.cpm_parameters.add_fwhm_model_order = 1
         if self.cpm_parameters.add_fwhm:
             for power in range(1, self.cpm_parameters.add_fwhm_model_order+1):
                 additional_regressor_list.append('fwhm_{}'.format(power))
 
         self.cpm_parameters.additional_regressor_list = \
             additional_regressor_list
-        self.cpm_parameters.n_additional_regressors = \
-            2 + len(additional_regressor_list)
+
+        try:
+            self.cpm_parameters.add_spot_profile = \
+                ast.literal_eval(self.cascade_configuration.cpm_add_spot_profile)
+        except AttributeError:
+            self.cpm_parameters.add_spot_profile = False
+
+        if self.cpm_parameters.add_spot_profile:
+            self.cpm_parameters.n_additional_regressors = \
+                3 + len(additional_regressor_list)
+        else:
+            self.cpm_parameters.n_additional_regressors = \
+                2 + len(additional_regressor_list)
 
     def get_regression_parameters(self):
         """
         Get all parameters controling the regression analysis.
 
         Returns
         -------
```

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/data_model/data_model.py` & `CASCADe-spectroscopy-1.2.4/cascade/data_model/data_model.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/exoplanet_tools/exoplanet_tools.py` & `CASCADe-spectroscopy-1.2.4/cascade/exoplanet_tools/exoplanet_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,16 @@
            'surface_gravity', 'scale_height', 'transit_depth', 'planck',
            'equilibrium_temperature', 'get_calalog', 'parse_database',
            'convert_spectrum_to_brighness_temperature', 'combine_spectra',
            'extract_exoplanet_data', 'lightcurve', 'batman_model',
            'masked_array_input', 'eclipse_to_transit', 'transit_to_eclipse',
            'exotethys_model', 'limbdarkning', 'exotethys_stellar_model',
            'SpectralModel', 'rayLightcurve', 'rayLimbdarkning',
-           'DilutionCorrection', 'rayDilutionCorrection']
+           'DilutionCorrection', 'rayDilutionCorrection', 'spotprofile',
+           'raySpotprofile']
 
 
 # enable cds to be able to use certain quantities defined in this system
 # cds_enable = cds.enable()
 
 ###########################################################################
 # astropy does not have V and K band magnitudes, we define it here ourself
@@ -1862,14 +1863,114 @@
 class rayLimbdarkning(limbdarkning):
     """Ray wrapper regressionDataServer class."""
 
     def __init__(self, cascade_configuration):
         super().__init__(cascade_configuration)
 
 
+class spotprofile:
+    """
+    Class defining the profile of a spot crossing
+
+    This class defines the light curve of a spot crossing. It implemets a
+    flattened Gaussian function suggested y Fraine et al 2014 to simulated
+    the planet crossing a star spot.
+
+    Attributes
+    ----------
+    lc : 'array_like'
+        The lightcurve model
+    par : 'ordered_dict'
+        The lightcurve parameters
+
+    """
+
+    def __init__(self, cascade_configuration):
+        self.cascade_configuration = cascade_configuration
+        # check if cascade is initialized
+        if self.cascade_configuration.isInitialized:
+            self.par = self.get_spot_parameters(self.cascade_configuration)
+        else:
+            raise ValueError("CASCADe not initialized, \
+                              aborting creation of lightcurve")
+
+    @staticmethod
+    def get_spot_parameters(cascade_configuration):
+        """
+        Get the relevant parameters for the spot profile.
+
+        Parameters
+        ----------
+        cascade_configuration : 'cascade.configuration'
+            The cascade configuration.
+
+        Returns
+        -------
+        par : 'collections.OrderedDict'
+            configuration parameters for spot profile.
+
+        """
+        try:
+            add_spot_profile = \
+                ast.literal_eval(cascade_configuration.cpm_add_spot_profile)
+        except AttributeError:
+            warnings.warn("Warning: starspot parameters not defined.")
+            add_spot_profile = False
+        try:
+            spot_offset = ast.literal_eval(cascade_configuration.cpm_spot_offset)
+            spot_width = ast.literal_eval(cascade_configuration.cpm_spot_width)
+            profile_power = \
+                ast.literal_eval(cascade_configuration.cpm_spot_profile_power)
+        except AttributeError:
+            warnings.warn("Warning: starspot parameters not defined.")
+            spot_offset = 0.0
+            spot_width = 0.001
+            profile_power = 2.0
+
+        par = collections.OrderedDict(asp=add_spot_profile,
+                                      offset=spot_offset,
+                                      width=spot_width,
+                                      power=profile_power)
+        return par
+
+    def return_spot_profile(self, dataset):
+        """
+        Spot profile function.
+
+        Parameters
+        ----------
+        dataset : : 'cascade.data_model.SpectralDataTimeSeries'
+            Input dataset.
+
+        Returns
+        -------
+        spot_lc : 'ndarray'
+             Normalized spot lightcuve model.
+
+        """
+        if  self.par['asp']:
+            spot_lc = np.exp(
+                -1*np.abs(
+                    (dataset.time.data.value - self.par['offset']) /
+                    self.par['width'])**self.par['power']
+                )
+            spot_lc = spot_lc/np.max(spot_lc)
+        else:
+            warnings.warn('Spot profile not set to active.')
+            spot_lc = np.nan
+        return spot_lc
+
+@ray.remote
+class raySpotprofile(spotprofile):
+    """Ray wrapper spotprofile class."""
+
+    def __init__(self, cascade_configuration):
+        super().__init__(cascade_configuration)
+
+
 class lightcurve:
     """
     Class defining lightcurve model.
 
     This class defines the light curve model used to model the observed
     transit/eclipse observations.
     Current valid lightcurve models: batman
@@ -2110,15 +2211,17 @@
 
         model_wavelengths, model_fluxes = \
             boats.get_model_spectrum(InputParameter['stellar_models_grids'],
                                      params=params,
                                      star_database_interpolation='seq_linear')
 
         # bug fix for poor wavelength resolution of stellar model at mid-IR
-        if InputParameter['stellar_models_grids'] == 'Atlas_2000':
+        if InputParameter['stellar_models_grids'] in  ['Atlas_2000',
+                                                       'MPS_Atlas_set1_2023',
+                                                       'MPS_Atlas_set2_2023']:
             grid_step = 5*u.Angstrom
             grid_max = (40.0*u.micron).to(u.Angstrom)
             ngrid = int((grid_max - model_wavelengths[0])/grid_step)
             grid_wavelenths = np.linspace(model_wavelengths[0], grid_max, ngrid)
             f = interpolate.interp1d(np.log(model_wavelengths.value),
                                      np.log(model_fluxes.value), kind='linear')
             grid_fluxes = \
```

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/initialize/initialize.py` & `CASCADe-spectroscopy-1.2.4/cascade/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/instruments/Generic/Generic.py` & `CASCADe-spectroscopy-1.2.4/cascade/instruments/Generic/Generic.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/instruments/HST/HST.py` & `CASCADe-spectroscopy-1.2.4/cascade/instruments/HST/HST.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/instruments/InstrumentsBaseClasses.py` & `CASCADe-spectroscopy-1.2.4/cascade/instruments/InstrumentsBaseClasses.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/instruments/JWST/JWST.py` & `CASCADe-spectroscopy-1.2.4/cascade/instruments/JWST/JWST.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/instruments/ObservationGenerator.py` & `CASCADe-spectroscopy-1.2.4/cascade/instruments/ObservationGenerator.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/instruments/Spitzer/Spitzer.py` & `CASCADe-spectroscopy-1.2.4/cascade/instruments/Spitzer/Spitzer.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/instruments/__init__.py` & `CASCADe-spectroscopy-1.2.4/cascade/instruments/__init__.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/spectral_extraction/spectral_extraction.py` & `CASCADe-spectroscopy-1.2.4/cascade/spectral_extraction/spectral_extraction.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/utilities/readwrite_spectra.py` & `CASCADe-spectroscopy-1.2.4/cascade/utilities/readwrite_spectra.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/utilities/utilities.py` & `CASCADe-spectroscopy-1.2.4/cascade/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/cascade/verbose/verbose.py` & `CASCADe-spectroscopy-1.2.4/cascade/verbose/verbose.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/scripts/build_local_hst_archive.py` & `CASCADe-spectroscopy-1.2.4/scripts/build_local_hst_archive.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/scripts/run_cascade.py` & `CASCADe-spectroscopy-1.2.4/scripts/run_cascade.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/scripts/run_cascade.sh` & `CASCADe-spectroscopy-1.2.4/scripts/run_cascade.sh`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/scripts/run_stats.sh` & `CASCADe-spectroscopy-1.2.4/scripts/run_stats.sh`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/scripts/setup_cascade.py` & `CASCADe-spectroscopy-1.2.4/scripts/setup_cascade.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/setup.py` & `CASCADe-spectroscopy-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     'description': 'CASCADe : Calibration of trAnsit Spectroscopy using CAusal Data',
     'long_description': README,
     'long_description_content_type': "text/markdown",
     'author': 'Jeroen Bouwman',
     'url': 'https://jbouwman.gitlab.io/CASCADe/',
     'download_url': 'https://gitlab.com/jbouwman/CASCADe',
     'author_email': 'bouwman@mpia.de',
-    'version': '1.2.3',
+    'version': '1.2.4',
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
-                         'statsmodels',
+                         'statsmodels', 'h5py'
                          'exotethys'],
     'scripts': scripts,
     'data_files': [('', [(HERE / 'README.md').as_posix(),
                          (HERE / 'LICENSE.txt').as_posix()])]
 }
 
 setuptools.setup(**config)
```

### Comparing `CASCADe-spectroscopy-1.2.3/tests/cpm_model_tests.py` & `CASCADe-spectroscopy-1.2.4/tests/cpm_model_tests.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/tests/data_model_tests.py` & `CASCADe-spectroscopy-1.2.4/tests/data_model_tests.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/tests/exoplanet_tools_tests.py` & `CASCADe-spectroscopy-1.2.4/tests/exoplanet_tools_tests.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.3/tests/initialize_tests.py` & `CASCADe-spectroscopy-1.2.4/tests/initialize_tests.py`

 * *Files identical despite different names*

