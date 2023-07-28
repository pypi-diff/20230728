# Comparing `tmp/HOGBEN-1.1.2.2023.5.19.tar.gz` & `tmp/HOGBEN-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HOGBEN-1.1.2.2023.5.19.tar", last modified: Fri May 19 13:25:17 2023, max compression
+gzip compressed data, was "HOGBEN-1.2.1.tar", last modified: Fri Jul 28 09:09:52 2023, max compression
```

## Comparing `HOGBEN-1.1.2.2023.5.19.tar` & `HOGBEN-1.2.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.076039 HOGBEN-1.1.2.2023.5.19/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.076039 HOGBEN-1.1.2.2023.5.19/HOGBEN.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-19 13:25:17.000000 HOGBEN-1.1.2.2023.5.19/HOGBEN.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-19 13:25:17.000000 HOGBEN-1.1.2.2023.5.19/HOGBEN.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-19 13:24:58.000000 HOGBEN-1.1.2.2023.5.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-19 13:24:58.000000 HOGBEN-1.1.2.2023.5.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-19 13:25:17.076039 HOGBEN-1.1.2.2023.5.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-19 13:24:58.000000 HOGBEN-1.1.2.2023.5.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.068039 HOGBEN-1.1.2.2023.5.19/figures/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-19 13:24:58.000000 HOGBEN-1.1.2.2023.5.19/figures/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.068039 HOGBEN-1.1.2.2023.5.19/hogben/
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/angles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/contrasts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.068039 HOGBEN-1.1.2.2023.5.19/hogben/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.072039 HOGBEN-1.1.2.2023.5.19/hogben/data/DMPC_bilayer/
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DMPC_bilayer/Si-D2O.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DMPC_bilayer/Si-DMPC-D2O.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DMPC_bilayer/Si-DMPC-H2O.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.072039 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPC_RaLPS_bilayer/
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-D2O.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-H2O.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-SMW.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.072039 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPG_monolayer/
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPG_monolayer/dDPPG-NRW.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPG_monolayer/hDPPG-D2O.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPG_monolayer/hDPPG-NRW.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.072039 HOGBEN-1.1.2.2023.5.19/hogben/data/YIG_sample/
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/YIG_sample/YIG_down.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/YIG_sample/YIG_up.dat
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.072039 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/
--rw-r--r--   0 runner    (1001) docker     (123)    63893 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/INTER_non_polarised.dat
--rw-r--r--   0 runner    (1001) docker     (123)    51658 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_Polarised.dat
--rw-r--r--   0 runner    (1001) docker     (123)    53135 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_non_polarised.dat
--rw-r--r--   0 runner    (1001) docker     (123)    49407 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_non_polarised_old.dat
--rw-r--r--   0 runner    (1001) docker     (123)    49407 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_polarised_old.dat
--rw-r--r--   0 runner    (1001) docker     (123)    56140 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/POLREF_non_polarised.dat
--rw-r--r--   0 runner    (1001) docker     (123)    69362 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/POLREF_polarised.dat
--rw-r--r--   0 runner    (1001) docker     (123)    24527 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/SURF_non_polarised.dat
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/make_beam_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/kinetics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/magnetism.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.072039 HOGBEN-1.1.2.2023.5.19/hogben/models/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/bilayers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/magnetic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/monolayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/optimise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.076039 HOGBEN-1.1.2.2023.5.19/hogben/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/underlayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/visualise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.076039 HOGBEN-1.1.2.2023.5.19/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-19 13:25:17.076039 HOGBEN-1.1.2.2023.5.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:52.447979 HOGBEN-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:52.447979 HOGBEN-1.2.1/HOGBEN.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-28 09:09:52.000000 HOGBEN-1.2.1/HOGBEN.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-28 09:09:52.000000 HOGBEN-1.2.1/HOGBEN.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-28 09:09:37.000000 HOGBEN-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 09:09:37.000000 HOGBEN-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-28 09:09:52.447979 HOGBEN-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-28 09:09:37.000000 HOGBEN-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:52.431979 HOGBEN-1.2.1/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-28 09:09:37.000000 HOGBEN-1.2.1/figures/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:52.435979 HOGBEN-1.2.1/hogben/
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/contrasts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:52.435979 HOGBEN-1.2.1/hogben/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:52.439979 HOGBEN-1.2.1/hogben/data/DMPC_bilayer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/DMPC_bilayer/Si-D2O.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/DMPC_bilayer/Si-DMPC-D2O.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/DMPC_bilayer/Si-DMPC-H2O.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:52.439979 HOGBEN-1.2.1/hogben/data/DPPC_RaLPS_bilayer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-D2O.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-H2O.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-SMW.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:52.439979 HOGBEN-1.2.1/hogben/data/DPPG_monolayer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/DPPG_monolayer/dDPPG-NRW.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/DPPG_monolayer/hDPPG-D2O.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/DPPG_monolayer/hDPPG-NRW.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:52.439979 HOGBEN-1.2.1/hogben/data/YIG_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/YIG_sample/YIG_down.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/YIG_sample/YIG_up.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:52.443979 HOGBEN-1.2.1/hogben/data/directbeams/
+-rw-r--r--   0 runner    (1001) docker     (123)    63893 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/directbeams/INTER_non_polarised.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    51658 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/directbeams/OFFSPEC_Polarised.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    53135 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/directbeams/OFFSPEC_non_polarised.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    49407 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/directbeams/OFFSPEC_non_polarised_old.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    49407 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/directbeams/OFFSPEC_polarised_old.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    56140 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/directbeams/POLREF_non_polarised.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    69362 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/directbeams/POLREF_polarised.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    24527 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/directbeams/SURF_non_polarised.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/directbeams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/data/directbeams/make_beam_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/magnetism.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:52.447979 HOGBEN-1.2.1/hogben/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/models/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/models/bilayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/models/magnetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/models/monolayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/models/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/models/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/optimise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:52.447979 HOGBEN-1.2.1/hogben/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/underlayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/hogben/visualise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:52.447979 HOGBEN-1.2.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 09:09:52.447979 HOGBEN-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 09:09:38.000000 HOGBEN-1.2.1/setup.py
```

### Comparing `HOGBEN-1.1.2.2023.5.19/HOGBEN.egg-info/PKG-INFO` & `HOGBEN-1.2.1/HOGBEN.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HOGBEN
-Version: 1.1.2.2023.5.19
+Version: 1.2.1
 Summary: Holistic Optimization for Generating Better Experimental Neutrons - a package for optimzing neutron experiments using the Fisher information
 Home-page: https://github.com/jfkcooper/HOGBEN
 Author: Joshaniel Cooper
 Author-email: Jos.Cooper@stfc.ac.uk
 Project-URL: Bug Tracker, https://github.com/jfkcooper/HOGBEN/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `HOGBEN-1.1.2.2023.5.19/HOGBEN.egg-info/SOURCES.txt` & `HOGBEN-1.2.1/HOGBEN.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/LICENSE` & `HOGBEN-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/PKG-INFO` & `HOGBEN-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HOGBEN
-Version: 1.1.2.2023.5.19
+Version: 1.2.1
 Summary: Holistic Optimization for Generating Better Experimental Neutrons - a package for optimzing neutron experiments using the Fisher information
 Home-page: https://github.com/jfkcooper/HOGBEN
 Author: Joshaniel Cooper
 Author-email: Jos.Cooper@stfc.ac.uk
 Project-URL: Bug Tracker, https://github.com/jfkcooper/HOGBEN/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `HOGBEN-1.1.2.2023.5.19/README.md` & `HOGBEN-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/figures/README.md` & `HOGBEN-1.2.1/figures/README.md`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/README.md` & `HOGBEN-1.2.1/hogben/README.md`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/angles.py` & `HOGBEN-1.2.1/hogben/angles.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/contrasts.py` & `HOGBEN-1.2.1/hogben/contrasts.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/DMPC_bilayer/Si-D2O.dat` & `HOGBEN-1.2.1/hogben/data/DMPC_bilayer/Si-D2O.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/DMPC_bilayer/Si-DMPC-D2O.dat` & `HOGBEN-1.2.1/hogben/data/DMPC_bilayer/Si-DMPC-D2O.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/DMPC_bilayer/Si-DMPC-H2O.dat` & `HOGBEN-1.2.1/hogben/data/DMPC_bilayer/Si-DMPC-H2O.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-D2O.dat` & `HOGBEN-1.2.1/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-D2O.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-H2O.dat` & `HOGBEN-1.2.1/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-H2O.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-SMW.dat` & `HOGBEN-1.2.1/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-SMW.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/DPPG_monolayer/dDPPG-NRW.dat` & `HOGBEN-1.2.1/hogben/data/DPPG_monolayer/dDPPG-NRW.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/DPPG_monolayer/hDPPG-D2O.dat` & `HOGBEN-1.2.1/hogben/data/DPPG_monolayer/hDPPG-D2O.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/DPPG_monolayer/hDPPG-NRW.dat` & `HOGBEN-1.2.1/hogben/data/DPPG_monolayer/hDPPG-NRW.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/YIG_sample/YIG_down.dat` & `HOGBEN-1.2.1/hogben/data/YIG_sample/YIG_down.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/YIG_sample/YIG_up.dat` & `HOGBEN-1.2.1/hogben/data/YIG_sample/YIG_up.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/INTER_non_polarised.dat` & `HOGBEN-1.2.1/hogben/data/directbeams/INTER_non_polarised.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_Polarised.dat` & `HOGBEN-1.2.1/hogben/data/directbeams/OFFSPEC_Polarised.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_non_polarised.dat` & `HOGBEN-1.2.1/hogben/data/directbeams/OFFSPEC_non_polarised.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_non_polarised_old.dat` & `HOGBEN-1.2.1/hogben/data/directbeams/OFFSPEC_non_polarised_old.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_polarised_old.dat` & `HOGBEN-1.2.1/hogben/data/directbeams/OFFSPEC_polarised_old.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/POLREF_non_polarised.dat` & `HOGBEN-1.2.1/hogben/data/directbeams/POLREF_non_polarised.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/POLREF_polarised.dat` & `HOGBEN-1.2.1/hogben/data/directbeams/POLREF_polarised.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/SURF_non_polarised.dat` & `HOGBEN-1.2.1/hogben/data/directbeams/SURF_non_polarised.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/make_beam_spectra.py` & `HOGBEN-1.2.1/hogben/data/directbeams/make_beam_spectra.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/kinetics.py` & `HOGBEN-1.2.1/hogben/kinetics.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/magnetism.py` & `HOGBEN-1.2.1/hogben/magnetism.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/models/README.md` & `HOGBEN-1.2.1/hogben/models/README.md`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/models/base.py` & `HOGBEN-1.2.1/hogben/models/base.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/models/bilayers.py` & `HOGBEN-1.2.1/hogben/models/bilayers.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/models/magnetic.py` & `HOGBEN-1.2.1/hogben/models/magnetic.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/models/monolayers.py` & `HOGBEN-1.2.1/hogben/models/monolayers.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/models/parsing.py` & `HOGBEN-1.2.1/hogben/models/parsing.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/models/samples.py` & `HOGBEN-1.2.1/hogben/models/samples.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/optimise.py` & `HOGBEN-1.2.1/hogben/optimise.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/simulate.py` & `HOGBEN-1.2.1/hogben/simulate.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/tests/test_simulation.py` & `HOGBEN-1.2.1/hogben/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/underlayers.py` & `HOGBEN-1.2.1/hogben/underlayers.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/utils.py` & `HOGBEN-1.2.1/hogben/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
+from typing import Optional, Union
 
 import numpy as np
 
 from dynesty import NestedSampler, DynamicNestedSampler
 from dynesty import plotting as dyplot
 from dynesty import utils as dyfunc
 
+import refl1d.experiment
 import refnx.reflect
 import refnx.analysis
 import bumps.parameter
 import bumps.fitproblem
 
 from hogben.simulate import reflectivity
 
@@ -22,51 +24,53 @@
                    bumps.fitproblem.FitProblem): objective to sample.
         params (list): varying model parameters.
         ndim (int): number of varying model parameters.
         sampler_static (dynesty.NestedSampler): static nested sampler.
         sampler_dynamic (dynesty.DynamicNestedSampler): dynamic nested sampler.
 
     """
+
     def __init__(self, objective):
         self.objective = objective
 
         # Determine if the objective is from refnx or Refl1D.
         if isinstance(objective, refnx.analysis.BaseObjective):
-            # Use log-likelihood and prior transform methods of refnx objective.
+            # Use log-likelihood and prior transform methods of refnx objective
             self.params = objective.varying_parameters()
             logl = objective.logl
             prior_transform = objective.prior_transform
 
         elif isinstance(objective, bumps.fitproblem.BaseFitProblem):
-            # Use this class' custom log-likelihood and prior transform methods.
+            # Use this class' custom log-likelihood and prior transform methods
             self.params = self.objective._parameters
             logl = self.logl_refl1d
             prior_transform = self.prior_transform_refl1d
 
         # Otherwise the given objective must be invalid.
         else:
             raise RuntimeError('invalid objective/fitproblem given')
 
         self.ndim = len(self.params)
         self.sampler_static = NestedSampler(logl, prior_transform, self.ndim)
-        self.sampler_dynamic = DynamicNestedSampler(logl, prior_transform, self.ndim)
+        self.sampler_dynamic = DynamicNestedSampler(logl, prior_transform,
+                                                    self.ndim)
 
     def logl_refl1d(self, x):
         """Calculates the log-likelihood of given parameter values `x`
            for a Refl1D FitProblem.
 
         Args:
             x (numpy.ndarray): parameter values to calculate likelihood of.
 
         Returns:
             float: log-likelihood of parameter values `x`.
 
         """
-        self.objective.setp(x) # Set the parameter values.
-        return -self.objective.model_nllf() # Calculate the log-likelihood.
+        self.objective.setp(x)  # Set the parameter values.
+        return -self.objective.model_nllf()  # Calculate the log-likelihood.
 
     def prior_transform_refl1d(self, u):
         """Calculates the prior transform for a Refl1D FitProblem.
 
         Args:
             u (numpy.ndarray): values in interval [0,1] to be transformed.
 
@@ -126,64 +130,80 @@
                                    truths=np.zeros(self.ndim),
                                    truth_color='black')
 
         # Label the axes with parameter labels.
         axes = np.reshape(np.array(fig.get_axes()), (self.ndim, self.ndim))
         for i in range(1, self.ndim):
             for j in range(self.ndim):
-                if i == self.ndim-1:
-                    axes[i,j].set_xlabel(self.params[j].name)
+                if i == self.ndim - 1:
+                    axes[i, j].set_xlabel(self.params[j].name)
                 if j == 0:
-                    axes[i,j].set_ylabel(self.params[i].name)
+                    axes[i, j].set_ylabel(self.params[i].name)
 
-        axes[self.ndim-1, self.ndim-1].set_xlabel(self.params[-1].name)
+        axes[self.ndim - 1, self.ndim - 1].set_xlabel(self.params[-1].name)
         return fig
 
-def fisher(qs, xi, counts, models, step=0.005):
+
+def fisher(qs: list[list],
+           xi: list[Union['refnx.analysis.Parameter',
+                          'bumps.parameter.Parameter']],
+           counts: list[int],
+           models: list[Union['refnx.reflect.ReflectModel',
+                              'refl1d.experiment.Experiment']],
+           step: float = 0.005) -> np.ndarray:
     """Calculates the Fisher information matrix for multiple `models`
-       containing parameters `xi`.
+    containing parameters `xi`. The model describes the experiment,
+    including the sample, and is defined using `refnx` or `refl1d`. The
+    lower and upper bounds of each parameter in the model are transformed
+    into a standardized range from 0 to 1, which is used to calculate the
+    Fisher information matrix. Each parameter in the Fisher information
+    matrix is scaled using an importance parameter. By default,
+    the importance parameter is set to 1 for all parameters, and can be set
+    by changing the `importance` attribute of the parameter when setting up
+    the model. For example the relative importance of the thickness in
+    "layer1" can be set to 2 using `layer1.thickness.importance = 2` or
+    `layer1.thick.importance = 2` in `refnx` and `refl1d` respectively.
 
     Args:
-        qs (list): Q points for each model.
-        xi (list): varying model parameters.
-        counts (list): incident neutron counts corresponding to each Q value.
-        models (list): models to calculate gradients with.
-        step (float): step size to take when calculating gradient.
-
+        qs: The Q points for each model.
+        xi: The varying model parameters.
+        counts: incident neutron counts corresponding to each Q value.
+        models: models to calculate gradients with.
+        step: step size to take when calculating gradient.
     Returns:
         numpy.ndarray: Fisher information matrix for given models and data.
 
     """
-    n = sum(len(q) for q in qs) # Number of data points.
-    m = len(xi) # Number of parameters.
+    n = sum(len(q) for q in qs)  # Number of data points.
+    m = len(xi)  # Number of parameters.
     J = np.zeros((n, m))
 
     # There is no information if there is no data.
     if n == 0:
         return np.zeros((m, m))
 
     # Calculate the gradient of model reflectivity with every model parameter
     # for every model data point.
     for i in range(m):
         parameter = xi[i]
         old = parameter.value
 
         # Calculate reflectance for each model for first part of gradient.
-        x1 = parameter.value = old*(1-step)
+        x1 = parameter.value = old * (1 - step)
         y1 = np.concatenate([reflectivity(q, model)
                              for q, model in list(zip(qs, models))])
 
         # Calculate reflectance for each model for second part of gradient.
-        x2 = parameter.value = old*(1+step)
+        x2 = parameter.value = old * (1 + step)
         y2 = np.concatenate([reflectivity(q, model)
                              for q, model in list(zip(qs, models))])
 
-        parameter.value = old # Reset the parameter.
+        parameter.value = old  # Reset the parameter.
 
-        J[:,i] = (y2-y1) / (x2-x1) # Calculate the gradient.
+        J[:, i] = (y2 - y1) / (x2 - x1)  # Calculate the gradient.
 
     # Calculate the reflectance for each model for the given Q values.
     r = np.concatenate([reflectivity(q, model)
                         for q, model in list(zip(qs, models))])
 
     # Calculate the Fisher information matrix using equations from the paper.
     M = np.diag(np.concatenate(counts) / r, k=0)
@@ -196,29 +216,39 @@
             lb = np.array([param.bounds.lb for param in xi])
             ub = np.array([param.bounds.ub for param in xi])
 
         elif isinstance(xi[0], bumps.parameter.Parameter):
             lb = np.array([param.bounds.limits[0] for param in xi])
             ub = np.array([param.bounds.limits[1] for param in xi])
 
-        # Using the equations from the paper for the coordinate transform.
-        H = np.diag(1/(ub-lb))
-        g = np.dot(np.dot(H.T, g), H)
+        # Scale each parameter with their specified importance,
+        # scale with one if no importance was specified.
+        importance_array = []
+        for param in xi:
+            if hasattr(param, "importance"):
+                importance_array.append(param.importance)
+            else:
+                importance_array.append(1)
+        importance = np.diag(importance_array)
+        H = np.diag(1 / (ub - lb))  # Get unit scaling Jacobian.
+        g = np.dot(np.dot(H.T, g), H) # Perform unit scaling.
+        g = np.dot(g, importance) # Perform importance scaling.
 
-    # Return the Fisher information matrix.
+        # Return the Fisher information matrix.
     return g
 
+
 def save_plot(fig, save_path, filename):
     """Saves a figure to a given directory.
 
     Args:
         fig (matplotlib.pyplot.Figure): figure to save.
         save_path (str): path to directory to save figure to.
         filename (str): name of file to save plot as.
 
     """
     # Create the directory if not present.
     if not os.path.exists(save_path):
         os.makedirs(save_path)
 
-    file_path = os.path.join(save_path, filename+'.png')
+    file_path = os.path.join(save_path, filename + '.png')
     fig.savefig(file_path, dpi=600)
```

### Comparing `HOGBEN-1.1.2.2023.5.19/hogben/visualise.py` & `HOGBEN-1.2.1/hogben/visualise.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/notebooks/README.md` & `HOGBEN-1.2.1/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.5.19/setup.cfg` & `HOGBEN-1.2.1/setup.cfg`

 * *Files identical despite different names*

