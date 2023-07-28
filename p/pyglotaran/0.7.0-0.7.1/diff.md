# Comparing `tmp/pyglotaran-0.7.0.tar.gz` & `tmp/pyglotaran-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglotaran-0.7.0.tar", last modified: Mon Mar 27 21:24:32 2023, max compression
+gzip compressed data, was "pyglotaran-0.7.1.tar", last modified: Fri Jul 28 13:23:36 2023, max compression
```

## Comparing `pyglotaran-0.7.0.tar` & `pyglotaran-0.7.1.tar`

### file list

```diff
@@ -1,306 +1,317 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.217454 pyglotaran-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14169 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-03-27 21:24:32.217454 pyglotaran-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.189454 pyglotaran-0.7.0/glotaran/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.189454 pyglotaran-0.7.0/glotaran/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.189454 pyglotaran-0.7.0/glotaran/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.189454 pyglotaran-0.7.0/glotaran/builtin/io/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.189454 pyglotaran-0.7.0/glotaran/builtin/io/ascii/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/ascii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.189454 pyglotaran-0.7.0/glotaran/builtin/io/ascii/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/ascii/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   443681 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/ascii/test/data.ascii
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/ascii/test/test_explicit_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/ascii/wavelength_time_explicit_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.189454 pyglotaran-0.7.0/glotaran/builtin/io/folder/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/folder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/folder/folder_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.189454 pyglotaran-0.7.0/glotaran/builtin/io/folder/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/folder/test/test_folder_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.189454 pyglotaran-0.7.0/glotaran/builtin/io/netCDF/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/netCDF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/netCDF/netCDF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.189454 pyglotaran-0.7.0/glotaran/builtin/io/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/pandas/csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.189454 pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.189454 pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/data/reference_parameters.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/data/reference_parameters.ods
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/data/reference_parameters.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/data/reference_parameters.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/data/reference_parameters.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/data/reference_parameters_alternative_notation.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/data/reference_parameters_alternative_notation.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/data/reference_parameters_subset.csv
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/data/reference_parameters_subset.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/test_pandas_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/pandas/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/pandas/xlsx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.189454 pyglotaran-0.7.0/glotaran/builtin/io/sdt/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/sdt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/sdt/sdt_file_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.189454 pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.193454 pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/data_files/
--rw-r--r--   0 runner    (1001) docker     (123)  2104831 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/data_files/FLIM.sdt
--rw-r--r--   0 runner    (1001) docker     (123)   149520 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/data_files/FLIM.sdt.ascii
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/data_files/FLIM_legacy_sum_map.ssv
--rw-r--r--   0 runner    (1001) docker     (123)   136421 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/data_files/FLIM_legacy_trace.ssv
--rw-r--r--   0 runner    (1001) docker     (123)    26315 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/data_files/temporal.sdt
--rw-r--r--   0 runner    (1001) docker     (123)    75350 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/data_files/temporal.sdt.kin
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/test_file_readers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.193454 pyglotaran-0.7.0/glotaran/builtin/io/yml/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/yml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.197454 pyglotaran-0.7.0/glotaran/builtin/io/yml/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/yml/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/yml/test/test_load_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/yml/test/test_model_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/yml/test/test_model_spec.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/yml/test/test_save_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/yml/test/test_save_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/yml/test/test_save_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/yml/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/io/yml/yml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.197454 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.197454 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/baseline/baseline_megacomplex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.197454 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/baseline/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/baseline/test/test_baseline_megacomplex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.197454 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/clp_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/clp_guide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/clp_guide/clp_guide_megacomplex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.197454 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/clp_guide/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/clp_guide/test/test_clp_guide_megacomplex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.197454 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/coherent_artifact/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/coherent_artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/coherent_artifact/coherent_artifact_megacomplex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.197454 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/coherent_artifact/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/coherent_artifact/test/test_coherent_artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.197454 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/damped_oscillation/
--rwxr-xr-x   0 runner    (1001) docker     (123)      131 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/damped_oscillation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/damped_oscillation/damped_oscillation_megacomplex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.197454 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/damped_oscillation/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11625 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/damped_oscillation/test/test_doas_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.197454 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/decay_matrix_gaussian_irf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/decay_megacomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/decay_parallel_megacomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/decay_sequential_megacomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/initial_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/irf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/k_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.197454 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/test/test_decay_megacomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/test/test_k_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/test/test_spectral_irf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.197454 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/spectral/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/spectral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/spectral/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/spectral/spectral_megacomplex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.197454 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/spectral/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/spectral/test/test_spectral_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.201454 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/test/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/test/test_spectral_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/test/test_spectral_decay_full_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/builtin/megacomplexes/test/test_spectral_penalties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.201454 pyglotaran-0.7.0/glotaran/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.201454 pyglotaran-0.7.0/glotaran/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/cli/commands/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/cli/commands/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/cli/commands/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/cli/commands/pluginlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/cli/commands/print.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.201454 pyglotaran-0.7.0/glotaran/cli/commands/test/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/cli/commands/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/cli/commands/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/cli/commands/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.201454 pyglotaran-0.7.0/glotaran/cli/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/cli/test/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.201454 pyglotaran-0.7.0/glotaran/deprecation/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26313 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/deprecation_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.201454 pyglotaran-0.7.0/glotaran/deprecation/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/modules/builtin_io_yml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.201454 pyglotaran-0.7.0/glotaran/deprecation/modules/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/modules/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/modules/examples/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.201454 pyglotaran-0.7.0/glotaran/deprecation/modules/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/modules/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/modules/test/test_builtin_io_yml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/modules/test/test_changed_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/modules/test/test_glotaran_root.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/modules/test/test_project_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/modules/test/test_project_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.201454 pyglotaran-0.7.0/glotaran/deprecation/test/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.201454 pyglotaran-0.7.0/glotaran/deprecation/test/dummy_package/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/test/dummy_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/test/dummy_package/deprecated_module_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/deprecation/test/test_deprecation_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.201454 pyglotaran-0.7.0/glotaran/io/
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/io/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/io/prepare_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.201454 pyglotaran-0.7.0/glotaran/io/preprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/io/preprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/io/preprocessor/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/io/preprocessor/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.205454 pyglotaran-0.7.0/glotaran/io/preprocessor/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/io/preprocessor/test/test_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.205454 pyglotaran-0.7.0/glotaran/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/clp_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/clp_penalties.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/clp_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/dataset_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/interval_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    16912 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/megacomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.205454 pyglotaran-0.7.0/glotaran/model/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/test/expected_model_markdown.md
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/test/test_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/test/test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/test/test_megacomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/model/weight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.205454 pyglotaran-0.7.0/glotaran/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    20231 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/estimation_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    27908 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/matrix_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/nnls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/optimization_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/optimization_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.209454 pyglotaran-0.7.0/glotaran/optimization/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/test/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/test/suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/test/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/test/test_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/test/test_estimation_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/test/test_matrix_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/test/test_multiple_goups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/test/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/test/test_optimization_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/test/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/test/test_penalties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/test/test_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/optimization/variable_projection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.209454 pyglotaran-0.7.0/glotaran/parameter/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14175 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/parameter/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/parameter/parameter_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/parameter/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.209454 pyglotaran-0.7.0/glotaran/parameter/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/parameter/test/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/parameter/test/test_parameter_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/parameter/test/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/parameter/test/test_parameters_rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.209454 pyglotaran-0.7.0/glotaran/plugin_system/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/plugin_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18390 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/plugin_system/base_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/plugin_system/data_io_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/plugin_system/io_plugin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/plugin_system/megacomplex_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/plugin_system/project_io_registration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.209454 pyglotaran-0.7.0/glotaran/plugin_system/test/
--rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/plugin_system/test/test_base_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/plugin_system/test/test_data_io_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/plugin_system/test/test_io_plugin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/plugin_system/test/test_megacomplex_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/plugin_system/test/test_project_io_registration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.213454 pyglotaran-0.7.0/glotaran/project/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/dataclass_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.213454 pyglotaran-0.7.0/glotaran/project/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.213454 pyglotaran-0.7.0/glotaran/project/generators/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/generators/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/generators/test/test_genenerate_decay_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23982 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/project_data_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/project_model_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/project_parameter_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/project_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/project_result_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.213454 pyglotaran-0.7.0/glotaran/project/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/test/test_dataclass_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30986 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/test/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/test/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/project/test/test_scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.213454 pyglotaran-0.7.0/glotaran/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/simulation/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.213454 pyglotaran-0.7.0/glotaran/simulation/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/simulation/test/test_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.213454 pyglotaran-0.7.0/glotaran/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/testing/plugin_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.213454 pyglotaran-0.7.0/glotaran/testing/simulated_data/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/testing/simulated_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/testing/simulated_data/parallel_spectral_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/testing/simulated_data/sequential_spectral_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/testing/simulated_data/shared_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.213454 pyglotaran-0.7.0/glotaran/testing/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/testing/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/testing/test/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/testing/test/test_plugin_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.213454 pyglotaran-0.7.0/glotaran/typing/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/typing/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/typing/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.213454 pyglotaran-0.7.0/glotaran/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/utils/attrs_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/utils/ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/utils/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/utils/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/utils/tee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.217454 pyglotaran-0.7.0/glotaran/utils/test/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/utils/test/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/utils/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/utils/test/test_ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/utils/test/test_sanitize.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/glotaran/utils/test/test_tee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:24:32.217454 pyglotaran-0.7.0/pyglotaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-03-27 21:24:32.000000 pyglotaran-0.7.0/pyglotaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-03-27 21:24:32.000000 pyglotaran-0.7.0/pyglotaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 21:24:32.000000 pyglotaran-0.7.0/pyglotaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-27 21:24:32.000000 pyglotaran-0.7.0/pyglotaran.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-27 21:24:32.000000 pyglotaran-0.7.0/pyglotaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-27 21:24:32.000000 pyglotaran-0.7.0/pyglotaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 21:24:32.000000 pyglotaran-0.7.0/pyglotaran.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-03-27 21:24:32.217454 pyglotaran-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 21:24:29.000000 pyglotaran-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.956417 pyglotaran-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-28 13:23:36.956417 pyglotaran-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.920416 pyglotaran-0.7.1/glotaran/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.920416 pyglotaran-0.7.1/glotaran/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.920416 pyglotaran-0.7.1/glotaran/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.920416 pyglotaran-0.7.1/glotaran/builtin/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.920416 pyglotaran-0.7.1/glotaran/builtin/io/ascii/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/ascii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.924416 pyglotaran-0.7.1/glotaran/builtin/io/ascii/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/ascii/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   443681 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/ascii/test/data.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/ascii/test/test_explicit_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/ascii/wavelength_time_explicit_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.924416 pyglotaran-0.7.1/glotaran/builtin/io/folder/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/folder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/folder/folder_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.924416 pyglotaran-0.7.1/glotaran/builtin/io/folder/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/folder/test/test_folder_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.924416 pyglotaran-0.7.1/glotaran/builtin/io/netCDF/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/netCDF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/netCDF/netCDF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.924416 pyglotaran-0.7.1/glotaran/builtin/io/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/pandas/csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.924416 pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.924416 pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/data/reference_parameters.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/data/reference_parameters.ods
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/data/reference_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/data/reference_parameters.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/data/reference_parameters.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/data/reference_parameters_alternative_notation.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/data/reference_parameters_alternative_notation.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/data/reference_parameters_subset.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/data/reference_parameters_subset.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/test_pandas_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/pandas/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/pandas/xlsx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.924416 pyglotaran-0.7.1/glotaran/builtin/io/sdt/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/sdt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/sdt/sdt_file_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.924416 pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.928416 pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/data_files/
+-rw-r--r--   0 runner    (1001) docker     (123)  2104831 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/data_files/FLIM.sdt
+-rw-r--r--   0 runner    (1001) docker     (123)   149520 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/data_files/FLIM.sdt.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/data_files/FLIM_legacy_sum_map.ssv
+-rw-r--r--   0 runner    (1001) docker     (123)   136421 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/data_files/FLIM_legacy_trace.ssv
+-rw-r--r--   0 runner    (1001) docker     (123)    26315 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/data_files/temporal.sdt
+-rw-r--r--   0 runner    (1001) docker     (123)    75350 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/data_files/temporal.sdt.kin
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/test_file_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.928416 pyglotaran-0.7.1/glotaran/builtin/io/yml/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/yml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.932417 pyglotaran-0.7.1/glotaran/builtin/io/yml/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/yml/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/yml/test/test_load_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/yml/test/test_model_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/yml/test/test_model_spec.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/yml/test/test_save_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/yml/test/test_save_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/yml/test/test_save_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/yml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/io/yml/yml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.932417 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.932417 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/baseline/baseline_megacomplex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.932417 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/baseline/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/baseline/test/test_baseline_megacomplex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.932417 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/clp_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/clp_guide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/clp_guide/clp_guide_megacomplex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.932417 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/clp_guide/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/clp_guide/test/test_clp_guide_megacomplex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.932417 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/coherent_artifact_megacomplex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.932417 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.932417 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/test/integration/test_two_coherent_artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.916416 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/test/integration/two_coherent_artifacts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.932417 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/test/integration/two_coherent_artifacts/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/test/integration/two_coherent_artifacts/data/CA670.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)    28764 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/test/integration/two_coherent_artifacts/data/CA700.ascii
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.932417 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/test/integration/two_coherent_artifacts/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/test/integration/two_coherent_artifacts/models/two_coherent_artifacts.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.932417 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/test/integration/two_coherent_artifacts/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/test/integration/two_coherent_artifacts/parameters/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/test/integration/two_coherent_artifacts/parameters/two_coherent_artifacts.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/test/test_coherent_artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.932417 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/damped_oscillation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      131 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/damped_oscillation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/damped_oscillation/damped_oscillation_megacomplex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.932417 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/damped_oscillation/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11625 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/damped_oscillation/test/test_doas_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.936416 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/decay_matrix_gaussian_irf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/decay_megacomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/decay_parallel_megacomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/decay_sequential_megacomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/initial_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/irf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/k_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.936416 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/test/test_decay_megacomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/test/test_k_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/test/test_spectral_irf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.936416 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/spectral/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/spectral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/spectral/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/spectral/spectral_megacomplex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.936416 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/spectral/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/spectral/test/test_spectral_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.936416 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/test/test_spectral_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/test/test_spectral_decay_full_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/builtin/megacomplexes/test/test_spectral_penalties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.936416 pyglotaran-0.7.1/glotaran/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.936416 pyglotaran-0.7.1/glotaran/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/cli/commands/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/cli/commands/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/cli/commands/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/cli/commands/pluginlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/cli/commands/print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.936416 pyglotaran-0.7.1/glotaran/cli/commands/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/cli/commands/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/cli/commands/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/cli/commands/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.936416 pyglotaran-0.7.1/glotaran/cli/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/cli/test/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.936416 pyglotaran-0.7.1/glotaran/deprecation/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26313 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/deprecation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.936416 pyglotaran-0.7.1/glotaran/deprecation/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/modules/builtin_io_yml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.936416 pyglotaran-0.7.1/glotaran/deprecation/modules/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/modules/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/modules/examples/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.940416 pyglotaran-0.7.1/glotaran/deprecation/modules/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/modules/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/modules/test/test_builtin_io_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/modules/test/test_changed_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/modules/test/test_glotaran_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/modules/test/test_project_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/modules/test/test_project_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.940416 pyglotaran-0.7.1/glotaran/deprecation/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.940416 pyglotaran-0.7.1/glotaran/deprecation/test/dummy_package/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/test/dummy_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/test/dummy_package/deprecated_module_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/deprecation/test/test_deprecation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.940416 pyglotaran-0.7.1/glotaran/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/io/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/io/prepare_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.940416 pyglotaran-0.7.1/glotaran/io/preprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/io/preprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/io/preprocessor/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/io/preprocessor/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.940416 pyglotaran-0.7.1/glotaran/io/preprocessor/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/io/preprocessor/test/test_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.940416 pyglotaran-0.7.1/glotaran/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/clp_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/clp_penalties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/clp_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/dataset_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/interval_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16912 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/megacomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.944417 pyglotaran-0.7.1/glotaran/model/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/test/expected_model_markdown.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/test/test_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/test/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/test/test_megacomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/model/weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.944417 pyglotaran-0.7.1/glotaran/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20231 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/estimation_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27908 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/matrix_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/nnls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/optimization_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/optimization_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.944417 pyglotaran-0.7.1/glotaran/optimization/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/test/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/test/suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/test/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/test/test_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/test/test_estimation_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/test/test_matrix_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/test/test_multiple_goups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/test/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/test/test_optimization_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/test/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/test/test_penalties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/test/test_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/optimization/variable_projection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.944417 pyglotaran-0.7.1/glotaran/parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14175 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/parameter/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/parameter/parameter_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/parameter/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.948417 pyglotaran-0.7.1/glotaran/parameter/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/parameter/test/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/parameter/test/test_parameter_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/parameter/test/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/parameter/test/test_parameters_rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.948417 pyglotaran-0.7.1/glotaran/plugin_system/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/plugin_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18390 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/plugin_system/base_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/plugin_system/data_io_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/plugin_system/io_plugin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/plugin_system/megacomplex_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/plugin_system/project_io_registration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.948417 pyglotaran-0.7.1/glotaran/plugin_system/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/plugin_system/test/test_base_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/plugin_system/test/test_data_io_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/plugin_system/test/test_io_plugin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/plugin_system/test/test_megacomplex_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/plugin_system/test/test_project_io_registration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.948417 pyglotaran-0.7.1/glotaran/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/dataclass_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.948417 pyglotaran-0.7.1/glotaran/project/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.948417 pyglotaran-0.7.1/glotaran/project/generators/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/generators/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/generators/test/test_genenerate_decay_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23982 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/project_data_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/project_model_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/project_parameter_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/project_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/project_result_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.952417 pyglotaran-0.7.1/glotaran/project/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/test/test_dataclass_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30986 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/test/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/test/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/project/test/test_scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.952417 pyglotaran-0.7.1/glotaran/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/simulation/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.952417 pyglotaran-0.7.1/glotaran/simulation/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/simulation/test/test_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.952417 pyglotaran-0.7.1/glotaran/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/testing/plugin_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.952417 pyglotaran-0.7.1/glotaran/testing/simulated_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/testing/simulated_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/testing/simulated_data/parallel_spectral_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/testing/simulated_data/sequential_spectral_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/testing/simulated_data/shared_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.952417 pyglotaran-0.7.1/glotaran/testing/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/testing/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/testing/test/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/testing/test/test_plugin_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.952417 pyglotaran-0.7.1/glotaran/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/typing/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/typing/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.952417 pyglotaran-0.7.1/glotaran/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/utils/attrs_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/utils/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/utils/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/utils/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/utils/tee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.956417 pyglotaran-0.7.1/glotaran/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/utils/test/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/utils/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/utils/test/test_ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/utils/test/test_sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/glotaran/utils/test/test_tee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:36.956417 pyglotaran-0.7.1/pyglotaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-28 13:23:36.000000 pyglotaran-0.7.1/pyglotaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-28 13:23:36.000000 pyglotaran-0.7.1/pyglotaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:23:36.000000 pyglotaran-0.7.1/pyglotaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-28 13:23:36.000000 pyglotaran-0.7.1/pyglotaran.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-28 13:23:36.000000 pyglotaran-0.7.1/pyglotaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 13:23:36.000000 pyglotaran-0.7.1/pyglotaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:23:36.000000 pyglotaran-0.7.1/pyglotaran.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-28 13:23:36.956417 pyglotaran-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:23:32.000000 pyglotaran-0.7.1/setup.py
```

### Comparing `pyglotaran-0.7.0/AUTHORS.rst` & `pyglotaran-0.7.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/CONTRIBUTING.rst` & `pyglotaran-0.7.1/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 -----------------------
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1.  The pull request should include tests.
 2.  If the pull request adds functionality, the docs should be updated. Put
     your new functionality into a function with a `docstring`_.
-3.  The pull request should work for Python 3.10
+3.  The pull request should work for Python 3.10 and 3.11
     Check your Github Actions ``https://github.com/<your_name_here>/pyglotaran/actions``
     and make sure that the tests pass for all supported Python versions.
 
 .. _docstring:
 
 Docstrings
 ----------
```

### Comparing `pyglotaran-0.7.0/LICENSE` & `pyglotaran-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/PKG-INFO` & `pyglotaran-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglotaran
-Version: 0.7.0
+Version: 0.7.1
 Summary: The Glotaran fitting engine.
 Home-page: https://github.com/glotaran/pyglotaran
 Author: Joern Weissenborn, Joris Snellenburg, Ivo van Stokkum
 Author-email: joern.weissenborn@gmail.com, j.snellenburg@gmail.com, i.h.m.van.stokkum@vu.nl
 License: LGPL-3.0
 Project-URL: Glotaran Ecosystem, https://glotaran.org
 Project-URL: Documentation, https://pyglotaran.readthedocs.io
@@ -18,15 +18,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: <3.11,>=3.10
+Requires-Python: <3.12,>=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: extras
 Provides-Extra: full
 License-File: LICENSE
 
 # pyglotaran
```

### Comparing `pyglotaran-0.7.0/README.md` & `pyglotaran-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/changelog.md` & `pyglotaran-0.7.1/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 # Changelog
 
+(changes-0_7_1)=
+
+## 🚀 0.7.1 (2023-07-28)
+
+### ✨ Features
+
+- ✨ Python 3.11 support (#1161)
+
+### 🩹 Bug fixes
+
+- 🩹 Fix coherent artifact clp label duplication (#1292)
+
 (changes-0_7_0)=
 
-## 🚀 0.7.0 (2023-03-27)
+## 🚀 0.7.0 (Unreleased)
 
 ### 💥 BREAKING CHANGE
 
 - 💥🚧 Dropped support for Python 3.8 and 3.9 and only support 3.10 (#1135)
 
 ### ✨ Features
 
@@ -22,14 +34,15 @@
 - ✨ Integrate plugin system into Project (#1229)
 - 👌 Make yaml the default plugin when passing a folder to save_result and load_result (#1230)
 - ✨ Allow usage of subfolders in project API for parameters, models and data (#1232)
 - ✨ Allow import of xarray objects in project API import_data (#1235)
 - 🩹 Add number_of_clps to result and correct degrees_of_freedom calculation (#1249)
 - 👌 Improve Project API data handling (#1257)
 - 🗑️ Deprecate Result.number_of_parameters in favor of Result.number_of_free_parameters (#1262)
+- 👌Improve reporting of standard error in case of non_negative constraint in the parameter (#1320)
 
 ### 🩹 Bug fixes
 
 - 🩹 Fix result data overwritten when using multiple dataset_groups (#1147)
 - 🩹 Fix for normalization issue described in #1157 (multi-gaussian irfs and multiple time ranges (streak))
 - 🩹 Fix for crash described in #1183 when doing an optimization using more than 30 datasets (#1184)
 - 🩹 Fix pretty_format_numerical for negative values (#1192)
```

### Comparing `pyglotaran-0.7.0/glotaran/analysis/__init__.py` & `pyglotaran-0.7.1/glotaran/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/ascii/test/data.ascii` & `pyglotaran-0.7.1/glotaran/builtin/io/ascii/test/data.ascii`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/ascii/test/test_explicit_file_reader.py` & `pyglotaran-0.7.1/glotaran/builtin/io/ascii/test/test_explicit_file_reader.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/ascii/wavelength_time_explicit_file.py` & `pyglotaran-0.7.1/glotaran/builtin/io/ascii/wavelength_time_explicit_file.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/folder/folder_plugin.py` & `pyglotaran-0.7.1/glotaran/builtin/io/folder/folder_plugin.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/folder/test/test_folder_plugin.py` & `pyglotaran-0.7.1/glotaran/builtin/io/folder/test/test_folder_plugin.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/netCDF/netCDF.py` & `pyglotaran-0.7.1/glotaran/builtin/io/netCDF/netCDF.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/pandas/csv.py` & `pyglotaran-0.7.1/glotaran/builtin/io/pandas/csv.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/data/reference_parameters.ods` & `pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/data/reference_parameters.ods`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/data/reference_parameters.xlsx` & `pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/data/reference_parameters.xlsx`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/data/reference_parameters_alternative_notation.xlsx` & `pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/data/reference_parameters_alternative_notation.xlsx`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/pandas/test/test_pandas_parameters.py` & `pyglotaran-0.7.1/glotaran/builtin/io/pandas/test/test_pandas_parameters.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/pandas/tsv.py` & `pyglotaran-0.7.1/glotaran/builtin/io/pandas/tsv.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/pandas/xlsx.py` & `pyglotaran-0.7.1/glotaran/builtin/io/pandas/xlsx.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/sdt/sdt_file_reader.py` & `pyglotaran-0.7.1/glotaran/builtin/io/sdt/sdt_file_reader.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/__init__.py` & `pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/data_files/FLIM.sdt` & `pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/data_files/FLIM.sdt`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/data_files/FLIM.sdt.ascii` & `pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/data_files/FLIM.sdt.ascii`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/data_files/FLIM_legacy_sum_map.ssv` & `pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/data_files/FLIM_legacy_sum_map.ssv`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/data_files/FLIM_legacy_trace.ssv` & `pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/data_files/FLIM_legacy_trace.ssv`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/data_files/temporal.sdt` & `pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/data_files/temporal.sdt`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/data_files/temporal.sdt.kin` & `pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/data_files/temporal.sdt.kin`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/sdt/test/test_file_readers.py` & `pyglotaran-0.7.1/glotaran/builtin/io/sdt/test/test_file_readers.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/yml/test/test_load_parameters.py` & `pyglotaran-0.7.1/glotaran/builtin/io/yml/test/test_load_parameters.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/yml/test/test_model_parser.py` & `pyglotaran-0.7.1/glotaran/builtin/io/yml/test/test_model_parser.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/yml/test/test_model_spec.yml` & `pyglotaran-0.7.1/glotaran/builtin/io/yml/test/test_model_spec.yml`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/yml/test/test_save_model.py` & `pyglotaran-0.7.1/glotaran/builtin/io/yml/test/test_save_model.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/yml/test/test_save_result.py` & `pyglotaran-0.7.1/glotaran/builtin/io/yml/test/test_save_result.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/yml/test/test_save_scheme.py` & `pyglotaran-0.7.1/glotaran/builtin/io/yml/test/test_save_scheme.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/yml/utils.py` & `pyglotaran-0.7.1/glotaran/builtin/io/yml/utils.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/io/yml/yml.py` & `pyglotaran-0.7.1/glotaran/builtin/io/yml/yml.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/baseline/baseline_megacomplex.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/baseline/baseline_megacomplex.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/baseline/test/test_baseline_megacomplex.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/baseline/test/test_baseline_megacomplex.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/clp_guide/clp_guide_megacomplex.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/clp_guide/clp_guide_megacomplex.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/clp_guide/test/test_clp_guide_megacomplex.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/clp_guide/test/test_clp_guide_megacomplex.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/coherent_artifact/coherent_artifact_megacomplex.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/coherent_artifact/coherent_artifact_megacomplex.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     ) -> tuple[float, float]:
         center, width, _, shift, _, _ = irf.parameter(global_index, global_axis)
         center = center[0] - shift
         width = self.width.value if self.width is not None else width[0]
         return center, width
 
     def compartments(self):
-        return [f"coherent_artifact_{i}" for i in range(1, self.order + 1)]
+        return [f"coherent_artifact_{i}_{self.label}" for i in range(1, self.order + 1)]
 
     def finalize_data(
         self,
         dataset_model: DatasetModel,
         dataset: xr.Dataset,
         is_full_model: bool = False,
         as_global: bool = False,
```

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/damped_oscillation/damped_oscillation_megacomplex.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/damped_oscillation/damped_oscillation_megacomplex.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/damped_oscillation/test/test_doas_model.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/damped_oscillation/test/test_doas_model.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/decay_matrix_gaussian_irf.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/decay_matrix_gaussian_irf.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/decay_megacomplex.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/decay_megacomplex.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/decay_parallel_megacomplex.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/decay_parallel_megacomplex.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/decay_sequential_megacomplex.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/decay_sequential_megacomplex.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/initial_concentration.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/initial_concentration.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/irf.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/irf.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/k_matrix.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/k_matrix.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/test/test_decay_megacomplex.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/test/test_decay_megacomplex.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/test/test_k_matrix.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/test/test_k_matrix.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/test/test_spectral_irf.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/test/test_spectral_irf.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/decay/util.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/decay/util.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/spectral/shape.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/spectral/shape.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/spectral/spectral_megacomplex.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/spectral/spectral_megacomplex.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/spectral/test/test_spectral_model.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/spectral/test/test_spectral_model.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/test/test_spectral_decay.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/test/test_spectral_decay.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/test/test_spectral_decay_full_model.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/test/test_spectral_decay_full_model.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/builtin/megacomplexes/test/test_spectral_penalties.py` & `pyglotaran-0.7.1/glotaran/builtin/megacomplexes/test/test_spectral_penalties.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/cli/commands/explore.py` & `pyglotaran-0.7.1/glotaran/cli/commands/explore.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/cli/commands/optimize.py` & `pyglotaran-0.7.1/glotaran/cli/commands/optimize.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/cli/commands/pluginlist.py` & `pyglotaran-0.7.1/glotaran/cli/commands/pluginlist.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/cli/commands/print.py` & `pyglotaran-0.7.1/glotaran/cli/commands/print.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/cli/commands/util.py` & `pyglotaran-0.7.1/glotaran/cli/commands/util.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/cli/commands/validate.py` & `pyglotaran-0.7.1/glotaran/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/cli/main.py` & `pyglotaran-0.7.1/glotaran/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/cli/test/test_cli.py` & `pyglotaran-0.7.1/glotaran/cli/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/deprecation/__init__.py` & `pyglotaran-0.7.1/glotaran/deprecation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/deprecation/deprecation_utils.py` & `pyglotaran-0.7.1/glotaran/deprecation/deprecation_utils.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/deprecation/modules/builtin_io_yml.py` & `pyglotaran-0.7.1/glotaran/deprecation/modules/builtin_io_yml.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/deprecation/modules/examples/sequential.py` & `pyglotaran-0.7.1/glotaran/deprecation/modules/examples/sequential.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/deprecation/modules/test/__init__.py` & `pyglotaran-0.7.1/glotaran/deprecation/modules/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/deprecation/modules/test/test_builtin_io_yml.py` & `pyglotaran-0.7.1/glotaran/deprecation/modules/test/test_builtin_io_yml.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/deprecation/modules/test/test_changed_imports.py` & `pyglotaran-0.7.1/glotaran/deprecation/modules/test/test_changed_imports.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/deprecation/modules/test/test_glotaran_root.py` & `pyglotaran-0.7.1/glotaran/deprecation/modules/test/test_glotaran_root.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/deprecation/modules/test/test_project_project.py` & `pyglotaran-0.7.1/glotaran/deprecation/modules/test/test_project_project.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/deprecation/modules/test/test_project_result.py` & `pyglotaran-0.7.1/glotaran/deprecation/modules/test/test_project_result.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/deprecation/test/dummy_package/__init__.py` & `pyglotaran-0.7.1/glotaran/deprecation/test/dummy_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/deprecation/test/dummy_package/deprecated_module_attribute.py` & `pyglotaran-0.7.1/glotaran/deprecation/test/dummy_package/deprecated_module_attribute.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/deprecation/test/test_deprecation_utils.py` & `pyglotaran-0.7.1/glotaran/deprecation/test/test_deprecation_utils.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/io/__init__.py` & `pyglotaran-0.7.1/glotaran/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/io/interface.py` & `pyglotaran-0.7.1/glotaran/io/interface.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/io/prepare_dataset.py` & `pyglotaran-0.7.1/glotaran/io/prepare_dataset.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/io/preprocessor/pipeline.py` & `pyglotaran-0.7.1/glotaran/io/preprocessor/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/io/preprocessor/preprocessor.py` & `pyglotaran-0.7.1/glotaran/io/preprocessor/preprocessor.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/io/preprocessor/test/test_preprocessor.py` & `pyglotaran-0.7.1/glotaran/io/preprocessor/test/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/model/__init__.py` & `pyglotaran-0.7.1/glotaran/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/model/clp_constraint.py` & `pyglotaran-0.7.1/glotaran/model/clp_constraint.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/model/clp_penalties.py` & `pyglotaran-0.7.1/glotaran/model/clp_penalties.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/model/dataset_group.py` & `pyglotaran-0.7.1/glotaran/model/dataset_group.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/model/dataset_model.py` & `pyglotaran-0.7.1/glotaran/model/dataset_model.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/model/interval_item.py` & `pyglotaran-0.7.1/glotaran/model/interval_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,12 +36,12 @@
         if self.interval is None or index is None:
             return True
 
         def applies(interval: tuple[float, float]):
             lower, upper = interval[0], interval[1]
             if lower > upper:
                 lower, upper = upper, lower
-            return lower <= index <= upper  # type:ignore[operator]
+            return lower <= index <= upper
 
         if isinstance(self.interval, tuple):
             return applies(self.interval)
         return any(applies(i) for i in self.interval)
```

### Comparing `pyglotaran-0.7.0/glotaran/model/item.py` & `pyglotaran-0.7.1/glotaran/model/item.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/model/megacomplex.py` & `pyglotaran-0.7.1/glotaran/model/megacomplex.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/model/model.py` & `pyglotaran-0.7.1/glotaran/model/model.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/model/test/expected_model_markdown.md` & `pyglotaran-0.7.1/glotaran/model/test/expected_model_markdown.md`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/model/test/test_dataset_model.py` & `pyglotaran-0.7.1/glotaran/model/test/test_dataset_model.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/model/test/test_item.py` & `pyglotaran-0.7.1/glotaran/model/test/test_item.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/model/test/test_megacomplex.py` & `pyglotaran-0.7.1/glotaran/model/test/test_megacomplex.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/model/test/test_model.py` & `pyglotaran-0.7.1/glotaran/model/test/test_model.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/data_provider.py` & `pyglotaran-0.7.1/glotaran/optimization/data_provider.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/estimation_provider.py` & `pyglotaran-0.7.1/glotaran/optimization/estimation_provider.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/matrix_provider.py` & `pyglotaran-0.7.1/glotaran/optimization/matrix_provider.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/nnls.py` & `pyglotaran-0.7.1/glotaran/optimization/nnls.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/optimization_group.py` & `pyglotaran-0.7.1/glotaran/optimization/optimization_group.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/optimization_history.py` & `pyglotaran-0.7.1/glotaran/optimization/optimization_history.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/optimize.py` & `pyglotaran-0.7.1/glotaran/optimization/optimize.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/optimizer.py` & `pyglotaran-0.7.1/glotaran/optimization/optimizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from scipy.optimize import OptimizeResult
 from scipy.optimize import least_squares
 
 from glotaran import __version__ as glotaran_version
 from glotaran.optimization.optimization_group import OptimizationGroup
 from glotaran.optimization.optimization_history import OptimizationHistory
 from glotaran.parameter import ParameterHistory
+from glotaran.parameter.parameter import _log_value
 from glotaran.project import Result
 from glotaran.project import Scheme
 from glotaran.utils.regex import RegexPattern
 from glotaran.utils.tee import TeeContext
 
 if TYPE_CHECKING:
     from glotaran.typing.types import ArrayLike
@@ -295,15 +296,22 @@
         # See PR #706: More robust covariance matrix calculation
         _, jacobian_sv, jacobian_rsv = np.linalg.svd(jacobian, full_matrices=False)
         jacobian_sv_square = jacobian_sv**2
         mask = jacobian_sv_square > np.finfo(float).eps
         covariance_matrix = (jacobian_rsv[mask].T / jacobian_sv_square[mask]) @ jacobian_rsv[mask]
         standard_errors = root_mean_square_error * np.sqrt(np.diag(covariance_matrix))
         for label, error in zip(self._free_parameter_labels, standard_errors):
-            self._parameters.get(label).standard_error = error
+            parameter = self._parameters.get(label)
+            if parameter.non_negative:
+                if error < np.abs(_log_value(parameter.value)):
+                    parameter.standard_error = parameter.value * (np.exp(error) - 1.0)
+                else:
+                    parameter.standard_error = np.abs(parameter.value)
+            else:
+                self._parameters.get(label).standard_error = error
         return covariance_matrix
 
     @staticmethod
     def get_current_optimization_iteration(optimize_stdout: str) -> int:
         """Extract current iteration from ``optimize_stdout``.
 
         Parameters
```

### Comparing `pyglotaran-0.7.0/glotaran/optimization/test/models.py` & `pyglotaran-0.7.1/glotaran/optimization/test/models.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/test/suites.py` & `pyglotaran-0.7.1/glotaran/optimization/test/suites.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/test/test_constraints.py` & `pyglotaran-0.7.1/glotaran/optimization/test/test_constraints.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/test/test_data_provider.py` & `pyglotaran-0.7.1/glotaran/optimization/test/test_data_provider.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/test/test_estimation_provider.py` & `pyglotaran-0.7.1/glotaran/optimization/test/test_estimation_provider.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/test/test_matrix_provider.py` & `pyglotaran-0.7.1/glotaran/optimization/test/test_matrix_provider.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/test/test_multiple_goups.py` & `pyglotaran-0.7.1/glotaran/optimization/test/test_multiple_goups.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/test/test_optimization.py` & `pyglotaran-0.7.1/glotaran/optimization/test/test_optimization.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/test/test_optimization_history.py` & `pyglotaran-0.7.1/glotaran/optimization/test/test_optimization_history.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/test/test_optimizer.py` & `pyglotaran-0.7.1/glotaran/optimization/test/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/test/test_penalties.py` & `pyglotaran-0.7.1/glotaran/optimization/test/test_penalties.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/test/test_relations.py` & `pyglotaran-0.7.1/glotaran/optimization/test/test_relations.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/optimization/variable_projection.py` & `pyglotaran-0.7.1/glotaran/optimization/variable_projection.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/parameter/__init__.py` & `pyglotaran-0.7.1/glotaran/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/parameter/parameter.py` & `pyglotaran-0.7.1/glotaran/parameter/parameter.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/parameter/parameter_history.py` & `pyglotaran-0.7.1/glotaran/parameter/parameter_history.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/parameter/parameters.py` & `pyglotaran-0.7.1/glotaran/parameter/parameters.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/parameter/test/test_parameter.py` & `pyglotaran-0.7.1/glotaran/parameter/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/parameter/test/test_parameter_history.py` & `pyglotaran-0.7.1/glotaran/parameter/test/test_parameter_history.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/parameter/test/test_parameters.py` & `pyglotaran-0.7.1/glotaran/parameter/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/parameter/test/test_parameters_rendering.py` & `pyglotaran-0.7.1/glotaran/parameter/test/test_parameters_rendering.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/plugin_system/base_registry.py` & `pyglotaran-0.7.1/glotaran/plugin_system/base_registry.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/plugin_system/data_io_registration.py` & `pyglotaran-0.7.1/glotaran/plugin_system/data_io_registration.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/plugin_system/io_plugin_utils.py` & `pyglotaran-0.7.1/glotaran/plugin_system/io_plugin_utils.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/plugin_system/megacomplex_registration.py` & `pyglotaran-0.7.1/glotaran/plugin_system/megacomplex_registration.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/plugin_system/project_io_registration.py` & `pyglotaran-0.7.1/glotaran/plugin_system/project_io_registration.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/plugin_system/test/test_base_registry.py` & `pyglotaran-0.7.1/glotaran/plugin_system/test/test_base_registry.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/plugin_system/test/test_data_io_registration.py` & `pyglotaran-0.7.1/glotaran/plugin_system/test/test_data_io_registration.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/plugin_system/test/test_io_plugin_utils.py` & `pyglotaran-0.7.1/glotaran/plugin_system/test/test_io_plugin_utils.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/plugin_system/test/test_megacomplex_registration.py` & `pyglotaran-0.7.1/glotaran/plugin_system/test/test_megacomplex_registration.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/plugin_system/test/test_project_io_registration.py` & `pyglotaran-0.7.1/glotaran/plugin_system/test/test_project_io_registration.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/project/dataclass_helpers.py` & `pyglotaran-0.7.1/glotaran/project/dataclass_helpers.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/project/generators/generator.py` & `pyglotaran-0.7.1/glotaran/project/generators/generator.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/project/generators/test/test_genenerate_decay_model.py` & `pyglotaran-0.7.1/glotaran/project/generators/test/test_genenerate_decay_model.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/project/project.py` & `pyglotaran-0.7.1/glotaran/project/project.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/project/project_data_registry.py` & `pyglotaran-0.7.1/glotaran/project/project_data_registry.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/project/project_model_registry.py` & `pyglotaran-0.7.1/glotaran/project/project_model_registry.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/project/project_parameter_registry.py` & `pyglotaran-0.7.1/glotaran/project/project_parameter_registry.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/project/project_registry.py` & `pyglotaran-0.7.1/glotaran/project/project_registry.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/project/project_result_registry.py` & `pyglotaran-0.7.1/glotaran/project/project_result_registry.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/project/result.py` & `pyglotaran-0.7.1/glotaran/project/result.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/project/scheme.py` & `pyglotaran-0.7.1/glotaran/project/scheme.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/project/test/test_dataclass_helpers.py` & `pyglotaran-0.7.1/glotaran/project/test/test_dataclass_helpers.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/project/test/test_project.py` & `pyglotaran-0.7.1/glotaran/project/test/test_project.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/project/test/test_result.py` & `pyglotaran-0.7.1/glotaran/project/test/test_result.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/project/test/test_scheme.py` & `pyglotaran-0.7.1/glotaran/project/test/test_scheme.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/simulation/simulation.py` & `pyglotaran-0.7.1/glotaran/simulation/simulation.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/simulation/test/test_simulation.py` & `pyglotaran-0.7.1/glotaran/simulation/test/test_simulation.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/testing/plugin_system.py` & `pyglotaran-0.7.1/glotaran/testing/plugin_system.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/testing/simulated_data/parallel_spectral_decay.py` & `pyglotaran-0.7.1/glotaran/testing/simulated_data/parallel_spectral_decay.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/testing/simulated_data/sequential_spectral_decay.py` & `pyglotaran-0.7.1/glotaran/testing/simulated_data/sequential_spectral_decay.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/testing/simulated_data/shared_decay.py` & `pyglotaran-0.7.1/glotaran/testing/simulated_data/shared_decay.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/testing/test/test_plugin_system.py` & `pyglotaran-0.7.1/glotaran/testing/test/test_plugin_system.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/typing/protocols.py` & `pyglotaran-0.7.1/glotaran/typing/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/typing/types.py` & `pyglotaran-0.7.1/glotaran/typing/types.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/utils/attrs_helper.py` & `pyglotaran-0.7.1/glotaran/utils/attrs_helper.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/utils/helpers.py` & `pyglotaran-0.7.1/glotaran/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/utils/io.py` & `pyglotaran-0.7.1/glotaran/utils/io.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/utils/ipython.py` & `pyglotaran-0.7.1/glotaran/utils/ipython.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/utils/regex.py` & `pyglotaran-0.7.1/glotaran/utils/regex.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/utils/sanitize.py` & `pyglotaran-0.7.1/glotaran/utils/sanitize.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/utils/tee.py` & `pyglotaran-0.7.1/glotaran/utils/tee.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/utils/test/test_helpers.py` & `pyglotaran-0.7.1/glotaran/utils/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/utils/test/test_io.py` & `pyglotaran-0.7.1/glotaran/utils/test/test_io.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/utils/test/test_ipython.py` & `pyglotaran-0.7.1/glotaran/utils/test/test_ipython.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/utils/test/test_sanitize.py` & `pyglotaran-0.7.1/glotaran/utils/test/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/glotaran/utils/test/test_tee.py` & `pyglotaran-0.7.1/glotaran/utils/test/test_tee.py`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/pyglotaran.egg-info/PKG-INFO` & `pyglotaran-0.7.1/pyglotaran.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglotaran
-Version: 0.7.0
+Version: 0.7.1
 Summary: The Glotaran fitting engine.
 Home-page: https://github.com/glotaran/pyglotaran
 Author: Joern Weissenborn, Joris Snellenburg, Ivo van Stokkum
 Author-email: joern.weissenborn@gmail.com, j.snellenburg@gmail.com, i.h.m.van.stokkum@vu.nl
 License: LGPL-3.0
 Project-URL: Glotaran Ecosystem, https://glotaran.org
 Project-URL: Documentation, https://pyglotaran.readthedocs.io
@@ -18,15 +18,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: <3.11,>=3.10
+Requires-Python: <3.12,>=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: extras
 Provides-Extra: full
 License-File: LICENSE
 
 # pyglotaran
```

### Comparing `pyglotaran-0.7.0/pyglotaran.egg-info/SOURCES.txt` & `pyglotaran-0.7.1/pyglotaran.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,20 @@
 glotaran/builtin/megacomplexes/baseline/test/test_baseline_megacomplex.py
 glotaran/builtin/megacomplexes/clp_guide/__init__.py
 glotaran/builtin/megacomplexes/clp_guide/clp_guide_megacomplex.py
 glotaran/builtin/megacomplexes/clp_guide/test/test_clp_guide_megacomplex.py
 glotaran/builtin/megacomplexes/coherent_artifact/__init__.py
 glotaran/builtin/megacomplexes/coherent_artifact/coherent_artifact_megacomplex.py
 glotaran/builtin/megacomplexes/coherent_artifact/test/test_coherent_artifact.py
+glotaran/builtin/megacomplexes/coherent_artifact/test/integration/test_two_coherent_artifacts.py
+glotaran/builtin/megacomplexes/coherent_artifact/test/integration/two_coherent_artifacts/data/CA670.ascii
+glotaran/builtin/megacomplexes/coherent_artifact/test/integration/two_coherent_artifacts/data/CA700.ascii
+glotaran/builtin/megacomplexes/coherent_artifact/test/integration/two_coherent_artifacts/models/two_coherent_artifacts.yml
+glotaran/builtin/megacomplexes/coherent_artifact/test/integration/two_coherent_artifacts/parameters/expected.csv
+glotaran/builtin/megacomplexes/coherent_artifact/test/integration/two_coherent_artifacts/parameters/two_coherent_artifacts.csv
 glotaran/builtin/megacomplexes/damped_oscillation/__init__.py
 glotaran/builtin/megacomplexes/damped_oscillation/damped_oscillation_megacomplex.py
 glotaran/builtin/megacomplexes/damped_oscillation/test/test_doas_model.py
 glotaran/builtin/megacomplexes/decay/__init__.py
 glotaran/builtin/megacomplexes/decay/decay_matrix_gaussian_irf.py
 glotaran/builtin/megacomplexes/decay/decay_megacomplex.py
 glotaran/builtin/megacomplexes/decay/decay_parallel_megacomplex.py
```

### Comparing `pyglotaran-0.7.0/pyglotaran.egg-info/entry_points.txt` & `pyglotaran-0.7.1/pyglotaran.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/pyproject.toml` & `pyglotaran-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyglotaran-0.7.0/setup.cfg` & `pyglotaran-0.7.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 description = The Glotaran fitting engine.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/glotaran/pyglotaran
 author = Joern Weissenborn, Joris Snellenburg, Ivo van Stokkum
 author_email = joern.weissenborn@gmail.com, j.snellenburg@gmail.com, i.h.m.van.stokkum@vu.nl
 license = LGPL-3.0
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Education
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 	Natural Language :: English
 	Operating System :: OS Independent
@@ -32,26 +32,26 @@
 packages = find:
 install_requires = 
 	asteval!=0.9.28,>=0.9.22
 	attrs>=22.1.0
 	click>=8.1.3
 	netCDF4>=1.5.7
 	numba>=0.55.0
-	numpy>=1.21.2,<1.24
+	numpy>=1.21.2,<1.25
 	odfpy>=1.4.1
 	openpyxl>=3.0.10
 	pandas>=1.3.4
 	pydantic>=1.10.2
 	rich>=10.9.0
 	ruamel.yaml>=0.17.17
 	scipy>=1.7.2
 	sdtfile>=2020.8.3
 	tabulate>=0.8.9
 	xarray>=2022.3.0
-python_requires = >=3.10, <3.11
+python_requires = >=3.10, <3.12
 tests_require = pytest
 zip_safe = True
 
 [options.entry_points]
 console_scripts = 
 	glotaran=glotaran.cli.main:main
 glotaran.plugins.data_io =
```

