# Comparing `tmp/cdflib-1.0.5.tar.gz` & `tmp/cdflib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdflib-1.0.5.tar", last modified: Mon Jun 19 08:00:11 2023, max compression
+gzip compressed data, was "cdflib-1.1.0.tar", last modified: Fri Jul 28 10:06:03 2023, max compression
```

## Comparing `cdflib-1.0.5.tar` & `cdflib-1.1.0.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.726974 cdflib-1.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.706974 cdflib-1.0.5/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-19 07:59:50.000000 cdflib-1.0.5/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-19 07:59:50.000000 cdflib-1.0.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.702974 cdflib-1.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.706974 cdflib-1.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-19 07:59:50.000000 cdflib-1.0.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-19 07:59:50.000000 cdflib-1.0.5/.github/workflows/pypi-build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-19 07:59:50.000000 cdflib-1.0.5/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-19 07:59:50.000000 cdflib-1.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-19 07:59:50.000000 cdflib-1.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-19 07:59:50.000000 cdflib-1.0.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 07:59:50.000000 cdflib-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-19 07:59:50.000000 cdflib-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-19 08:00:11.726974 cdflib-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-19 07:59:50.000000 cdflib-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.706974 cdflib-1.0.5/archive/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-19 07:59:50.000000 cdflib-1.0.5/archive/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-06-19 07:59:50.000000 cdflib-1.0.5/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.710974 cdflib-1.0.5/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:59:50.000000 cdflib-1.0.5/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-19 07:59:50.000000 cdflib-1.0.5/benchmarks/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.714974 cdflib-1.0.5/cdflib/
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/CDFLeapSeconds.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 08:00:11.000000 cdflib-1.0.5/cdflib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    84143 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/cdfread.py
--rw-r--r--   0 runner    (1001) docker     (123)   104416 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/cdfwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    65533 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/epochs_astropy.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.714974 cdflib-1.0.5/cdflib/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38117 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/xarray/cdf_to_xarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    32580 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/xarray/xarray_to_cdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.714974 cdflib-1.0.5/cdflib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-19 08:00:11.000000 cdflib-1.0.5/cdflib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-19 08:00:11.000000 cdflib-1.0.5/cdflib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:00:11.000000 cdflib-1.0.5/cdflib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-19 08:00:11.000000 cdflib-1.0.5/cdflib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 08:00:11.000000 cdflib-1.0.5/cdflib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 07:59:50.000000 cdflib-1.0.5/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.718974 cdflib-1.0.5/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.718974 cdflib-1.0.5/doc/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/modules/cdfepoch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/modules/cdfread.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/modules/cdfwrite.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/modules/dataclasses.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/modules/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/modules/xarray.rst
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-19 07:59:50.000000 cdflib-1.0.5/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-19 07:59:50.000000 cdflib-1.0.5/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-19 07:59:50.000000 cdflib-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-19 08:00:11.726974 cdflib-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.722974 cdflib-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/test_astropy_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/test_cdfread.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/test_cdfread_rle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16228 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/test_cdfwrite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9647 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/test_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17241 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/test_xarray_reader_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.722974 cdflib-1.0.5/tests/testfiles/
--rw-r--r--   0 runner    (1001) docker     (123)   125566 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf
--rw-r--r--   0 runner    (1001) docker     (123)    67164 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
--rw-r--r--   0 runner    (1001) docker     (123)    70003 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-19 07:59:50.000000 cdflib-1.0.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:06:03.325638 cdflib-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:06:03.321638 cdflib-1.1.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-28 10:05:48.000000 cdflib-1.1.0/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 10:05:48.000000 cdflib-1.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:06:03.317638 cdflib-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:06:03.321638 cdflib-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 10:05:48.000000 cdflib-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-28 10:05:48.000000 cdflib-1.1.0/.github/workflows/pypi-build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-28 10:05:48.000000 cdflib-1.1.0/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-28 10:05:48.000000 cdflib-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-28 10:05:48.000000 cdflib-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-28 10:05:48.000000 cdflib-1.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 10:05:48.000000 cdflib-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 10:05:48.000000 cdflib-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-28 10:06:03.325638 cdflib-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-28 10:05:48.000000 cdflib-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:06:03.321638 cdflib-1.1.0/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-28 10:05:48.000000 cdflib-1.1.0/archive/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-07-28 10:05:48.000000 cdflib-1.1.0/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:06:03.321638 cdflib-1.1.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:05:48.000000 cdflib-1.1.0/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-28 10:05:48.000000 cdflib-1.1.0/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:06:03.321638 cdflib-1.1.0/cdflib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-28 10:05:48.000000 cdflib-1.1.0/cdflib/CDFLeapSeconds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-28 10:05:48.000000 cdflib-1.1.0/cdflib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-28 10:05:48.000000 cdflib-1.1.0/cdflib/_gzip_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 10:06:03.000000 cdflib-1.1.0/cdflib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84221 2023-07-28 10:05:48.000000 cdflib-1.1.0/cdflib/cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104448 2023-07-28 10:05:48.000000 cdflib-1.1.0/cdflib/cdfwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-28 10:05:48.000000 cdflib-1.1.0/cdflib/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65533 2023-07-28 10:05:48.000000 cdflib-1.1.0/cdflib/epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-07-28 10:05:48.000000 cdflib-1.1.0/cdflib/epochs_astropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 10:05:48.000000 cdflib-1.1.0/cdflib/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-28 10:05:48.000000 cdflib-1.1.0/cdflib/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-28 10:05:48.000000 cdflib-1.1.0/cdflib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:06:03.325638 cdflib-1.1.0/cdflib/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-28 10:05:48.000000 cdflib-1.1.0/cdflib/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38117 2023-07-28 10:05:48.000000 cdflib-1.1.0/cdflib/xarray/cdf_to_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32580 2023-07-28 10:05:48.000000 cdflib-1.1.0/cdflib/xarray/xarray_to_cdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:06:03.321638 cdflib-1.1.0/cdflib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-28 10:06:03.000000 cdflib-1.1.0/cdflib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-28 10:06:03.000000 cdflib-1.1.0/cdflib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:06:03.000000 cdflib-1.1.0/cdflib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-28 10:06:03.000000 cdflib-1.1.0/cdflib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 10:06:03.000000 cdflib-1.1.0/cdflib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 10:05:48.000000 cdflib-1.1.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:06:03.325638 cdflib-1.1.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-28 10:05:48.000000 cdflib-1.1.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-07-28 10:05:48.000000 cdflib-1.1.0/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-28 10:05:48.000000 cdflib-1.1.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-28 10:05:48.000000 cdflib-1.1.0/doc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-28 10:05:48.000000 cdflib-1.1.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-28 10:05:48.000000 cdflib-1.1.0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:06:03.325638 cdflib-1.1.0/doc/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-28 10:05:48.000000 cdflib-1.1.0/doc/modules/cdfepoch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-28 10:05:48.000000 cdflib-1.1.0/doc/modules/cdfread.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-28 10:05:48.000000 cdflib-1.1.0/doc/modules/cdfwrite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-28 10:05:48.000000 cdflib-1.1.0/doc/modules/dataclasses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-28 10:05:48.000000 cdflib-1.1.0/doc/modules/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-28 10:05:48.000000 cdflib-1.1.0/doc/modules/xarray.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-28 10:05:48.000000 cdflib-1.1.0/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-28 10:05:48.000000 cdflib-1.1.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-28 10:05:48.000000 cdflib-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-28 10:06:03.325638 cdflib-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:06:03.325638 cdflib-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-28 10:05:48.000000 cdflib-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-28 10:05:48.000000 cdflib-1.1.0/tests/test_astropy_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-28 10:05:48.000000 cdflib-1.1.0/tests/test_cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-28 10:05:48.000000 cdflib-1.1.0/tests/test_cdfread_rle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16228 2023-07-28 10:05:48.000000 cdflib-1.1.0/tests/test_cdfwrite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9647 2023-07-28 10:05:48.000000 cdflib-1.1.0/tests/test_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17241 2023-07-28 10:05:48.000000 cdflib-1.1.0/tests/test_xarray_reader_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:06:03.325638 cdflib-1.1.0/tests/testfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)   125566 2023-07-28 10:05:48.000000 cdflib-1.1.0/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)    67164 2023-07-28 10:05:48.000000 cdflib-1.1.0/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)    70003 2023-07-28 10:05:48.000000 cdflib-1.1.0/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-28 10:05:48.000000 cdflib-1.1.0/tox.ini
```

### Comparing `cdflib-1.0.5/.circleci/config.yml` & `cdflib-1.1.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/.github/workflows/ci.yml` & `cdflib-1.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/.github/workflows/pypi-build.yaml` & `cdflib-1.1.0/.github/workflows/pypi-build.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/.pre-commit-config.yaml` & `cdflib-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/.readthedocs.yml` & `cdflib-1.1.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/LICENSE` & `cdflib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/PKG-INFO` & `cdflib-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdflib
-Version: 1.0.5
+Version: 1.1.0
 Summary: A python CDF reader toolkit
 Home-page: https://github.com/MAVENSDC/cdflib
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: CDF,maven,lasp,PDS,GSFC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cdflib-1.0.5/README.md` & `cdflib-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/asv.conf.json` & `cdflib-1.1.0/asv.conf.json`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/benchmarks/benchmarks.py` & `cdflib-1.1.0/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/cdflib/CDFLeapSeconds.txt` & `cdflib-1.1.0/cdflib/CDFLeapSeconds.txt`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/cdflib/cdfread.py` & `cdflib-1.1.0/cdflib/cdfread.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import gzip
 import hashlib
 import io
 import os
 import struct
 import sys
 import tempfile
 import urllib.request
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
 import cdflib.epochs as epoch
+from cdflib._gzip_wrapper import gzip_inflate
 from cdflib.dataclasses import (
     AEDR,
     VDR,
     ADRInfo,
     AttData,
     CDFInfo,
     CDRInfo,
@@ -507,14 +507,15 @@
                 entryData = aedr_info.entry
                 # This exists to get rid of extraneous numpy arrays
                 if isinstance(entryData, np.ndarray):
                     if len(entryData) == 1:
                         entryData = entryData[0]
 
                 entries.append(entryData)
+                aedr_byte_loc = aedr_info.next_aedr
 
             return_dict[adr_info.name] = entries
             byte_loc = adr_info.next_adr_loc
 
         return return_dict
 
     def varattsget(self, variable: Union[str, int]) -> Dict[str, Union[None, str, np.ndarray]]:
@@ -575,15 +576,15 @@
         if self.cdfversion == 3:
             data_start, data_size, cType, _ = self._read_ccr(8)
         else:
             data_start, data_size, cType, _ = self._read_ccr2(8)
 
         if cType == 5:
             self._f.seek(data_start)
-            decompressed_data = gzip.decompress(self._f.read(data_size))
+            decompressed_data = gzip_inflate(self._f.read(data_size))
         elif cType == 1:
             self._f.seek(data_start)
             decompressed_data = self._uncompress_rle(self._f.read(data_size))
         else:
             return
 
         self.temp_file = Path(tempfile.NamedTemporaryFile(suffix=".cdf").name)
@@ -1978,15 +1979,15 @@
         block_size = int.from_bytes(self._f.read(8), "big")
         block = self._f.read(block_size - 8)
 
         section_type = int.from_bytes(block[0:4], "big")
         if section_type == 13:
             # a CVVR
             compressed_size = int.from_bytes(block[8:16], "big")
-            return gzip.decompress(block[16 : 16 + compressed_size])
+            return gzip_inflate(block[16 : 16 + compressed_size])
         elif section_type == 7:
             # a VVR
             return block[4:]
         else:
             raise RuntimeError("Unexpected section type")
 
     def _read_vvr_block2(self, offset: int) -> bytes:
@@ -1997,15 +1998,15 @@
         block_size = int.from_bytes(self._f.read(4), "big")
         block = self._f.read(block_size - 4)
 
         section_type = int.from_bytes(block[0:4], "big")
         if section_type == 13:
             # a CVVR
             compressed_size = int.from_bytes(block[8:12], "big")
-            return gzip.decompress(block[12 : 12 + compressed_size])
+            return gzip_inflate(block[12 : 12 + compressed_size])
         elif section_type == 7:
             # a VVR
             return block[4:]
         else:
             raise RuntimeError("Unexpected section type")
 
     @staticmethod
```

### Comparing `cdflib-1.0.5/cdflib/cdfwrite.py` & `cdflib-1.1.0/cdflib/cdfwrite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import binascii
-import gzip
 import hashlib
 import io
 import logging
 import math
 import numbers
 import pathlib
 import platform as pf
@@ -13,14 +12,15 @@
 from numbers import Number
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
 import cdflib.epochs as cdfepoch
+from cdflib._gzip_wrapper import gzip_deflate
 from cdflib.logging import logger
 
 __all__ = ["CDF"]
 
 
 def is_open(func):
     @wraps(func)
@@ -1027,15 +1027,15 @@
                 if endrec > (recs - 1):
                     endrec = recs - 1
                 endloc = (endrec + 1) * numValues * dataTypeSize
                 if endloc > len(data):
                     endrec = recs - 1
                     endloc = len(data)
                 bdata = data[startloc:endloc]
-                cdata = gzip.compress(bdata, compression)
+                cdata = gzip_deflate(bdata, compression)
                 if len(cdata) < len(bdata):
                     n1offset = self._write_cvvr(f, cdata)
                 else:
                     n1offset = self._write_vvr(f, bdata)
                 if x == 0:
                     # Create a VXR
                     VXRoffset = self._write_vxr(f)
@@ -2061,15 +2061,15 @@
 
         """
         f.seek(8)
         data = f.read()
         uSize = len(data)
         section_type = self.CCR_
         rfuA = 0
-        cData = gzip.compress(data, level)
+        cData = gzip_deflate(data, level)
         block_size = self.CCR_BASE_SIZE64 + len(cData)
         cprOffset = 0
         ccr1 = bytearray(32)
         # ccr1[0:4] = binascii.unhexlify(CDF.V3magicNUMBER_1)
         # ccr1[4:8] = binascii.unhexlify(CDF.V3magicNUMBER_2c)
         ccr1[0:8] = struct.pack(">q", block_size)
         ccr1[8:12] = struct.pack(">i", section_type)
```

### Comparing `cdflib-1.0.5/cdflib/dataclasses.py` & `cdflib-1.1.0/cdflib/dataclasses.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/cdflib/epochs.py` & `cdflib-1.1.0/cdflib/epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/cdflib/epochs_astropy.py` & `cdflib-1.1.0/cdflib/epochs_astropy.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/cdflib/s3.py` & `cdflib-1.1.0/cdflib/s3.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/cdflib/xarray/cdf_to_xarray.py` & `cdflib-1.1.0/cdflib/xarray/cdf_to_xarray.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/cdflib/xarray/xarray_to_cdf.py` & `cdflib-1.1.0/cdflib/xarray/xarray_to_cdf.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/cdflib.egg-info/PKG-INFO` & `cdflib-1.1.0/cdflib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdflib
-Version: 1.0.5
+Version: 1.1.0
 Summary: A python CDF reader toolkit
 Home-page: https://github.com/MAVENSDC/cdflib
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: CDF,maven,lasp,PDS,GSFC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cdflib-1.0.5/cdflib.egg-info/SOURCES.txt` & `cdflib-1.1.0/cdflib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 .github/workflows/pypi-build.yaml
 .github/workflows/python-lint.yml
 archive/.appveyor.yml
 benchmarks/__init__.py
 benchmarks/benchmarks.py
 cdflib/CDFLeapSeconds.txt
 cdflib/__init__.py
+cdflib/_gzip_wrapper.py
 cdflib/_version.py
 cdflib/cdfread.py
 cdflib/cdfwrite.py
 cdflib/dataclasses.py
 cdflib/epochs.py
 cdflib/epochs_astropy.py
 cdflib/logging.py
```

### Comparing `cdflib-1.0.5/doc/Makefile` & `cdflib-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/doc/changelog.rst` & `cdflib-1.1.0/doc/changelog.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 Changelog
 =========
 
+1.1.0
+=====
+- If the `deflate <https://github.com/dcwatson/deflate>`_ library is installed
+  it is now used to decompress data, which can lead to around 2x speedups over
+  the native gzip Python library.
+- Fixed reading attributes with multiple entries when using `cdflib.cdfread.CDF.globalattsget`.
+
 1.0.5
 =====
 - Fixed the output of :meth:`cdflib.epochs.CDFepoch.compute_tt2000` to
   be squeezed if a single input is given.
 - Fixed warnings with numpy 1.25.
 
 1.0.4
```

### Comparing `cdflib-1.0.5/doc/conf.py` & `cdflib-1.1.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/doc/index.rst` & `cdflib-1.1.0/doc/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
    python3 -m pip install cdflib
 
 
 What is cdflib?
 ------------------
 
-cdflib is an effort to replicate the CDF libraries using a pure python implementation.  This means users do not need to install the `CDF NASA libraries <https://cdf.gsfc.nasa.gov/>`_.
+cdflib is an effort to replicate the CDF libraries using a pure python implementation.
+This means users do not need to install the `CDF NASA libraries <https://cdf.gsfc.nasa.gov/>`_.
 
 The only module you need to install is ``numpy``, but there are a few things you can do with ``astropy`` and ``xarray``.
 
 While this originally started as a way to read PDS-archive compliant CDF files, thanks to many contributors, it has grown to be able to handle every type of CDF file.
 
 What can cdflib do?
 -------------------
```

### Comparing `cdflib-1.0.5/doc/make.bat` & `cdflib-1.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/doc/modules/cdfepoch.rst` & `cdflib-1.1.0/doc/modules/cdfepoch.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/doc/modules/cdfread.rst` & `cdflib-1.1.0/doc/modules/cdfread.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/doc/modules/cdfwrite.rst` & `cdflib-1.1.0/doc/modules/cdfwrite.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/meta.yaml` & `cdflib-1.1.0/meta.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/mypy.ini` & `cdflib-1.1.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/setup.cfg` & `cdflib-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/tests/test_astropy_epochs.py` & `cdflib-1.1.0/tests/test_astropy_epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/tests/test_cdfwrite.py` & `cdflib-1.1.0/tests/test_cdfwrite.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/tests/test_epochs.py` & `cdflib-1.1.0/tests/test_epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/tests/test_xarray_reader_writer.py` & `cdflib-1.1.0/tests/test_xarray_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf` & `cdflib-1.1.0/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf` & `cdflib-1.1.0/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.5/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf` & `cdflib-1.1.0/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf`

 * *Files identical despite different names*

