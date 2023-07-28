# Comparing `tmp/arcesetc-0.1.tar.gz` & `tmp/arcesetc-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arcesetc-0.1.tar", last modified: Wed Dec 12 04:00:54 2018, max compression
+gzip compressed data, was "arcesetc-0.3.tar", last modified: Fri Jul 28 18:57:25 2023, max compression
```

## Comparing `arcesetc-0.1.tar` & `arcesetc-0.3.tar`

### file list

```diff
@@ -1,148 +1,91 @@
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/
--rw-r--r--   0 bmmorris   (501) staff       (20)    35654 2018-12-03 03:00:30.000000 arcesetc-0.1/ah_bootstrap.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/arcesetc/
--rw-r--r--   0 bmmorris   (501) staff       (20)      899 2018-12-03 15:02:32.000000 arcesetc-0.1/arcesetc/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     2023 2018-12-03 03:00:28.000000 arcesetc-0.1/arcesetc/_astropy_init.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     2513 2018-12-03 03:00:28.000000 arcesetc-0.1/arcesetc/conftest.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/arcesetc/data/
--rw-r--r--   0 bmmorris   (501) staff       (20)   969324 2018-12-11 16:13:21.000000 arcesetc-0.1/arcesetc/data/archive.hdf5
--rw-r--r--   0 bmmorris   (501) staff       (20)   737280 2018-12-11 16:39:52.000000 arcesetc-0.1/arcesetc/data/BD28_4211.0026.wfrmcpc.fits
--rw-r--r--   0 bmmorris   (501) staff       (20)   737280 2018-12-02 20:24:34.000000 arcesetc-0.1/arcesetc/data/HIP107864.0003.wfrmcpc.fits
--rw-r--r--   0 bmmorris   (501) staff       (20)   737280 2018-12-11 16:11:03.000000 arcesetc-0.1/arcesetc/data/HR5191.0002.wfrmcpc.fits
--rw-r--r--   0 bmmorris   (501) staff       (20)      246 2018-12-03 03:00:28.000000 arcesetc-0.1/arcesetc/data/README.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1661 2018-12-11 16:13:21.000000 arcesetc-0.1/arcesetc/data/sptype_dict.json
--rw-r--r--   0 bmmorris   (501) staff       (20)     1152 2018-12-11 16:34:40.000000 arcesetc-0.1/arcesetc/data/sptype_to_temp.json
--rw-r--r--   0 bmmorris   (501) staff       (20)     6729 2018-12-03 16:13:19.000000 arcesetc-0.1/arcesetc/plots.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/arcesetc/tests/
--rw-r--r--   0 bmmorris   (501) staff       (20)      108 2018-12-03 03:00:28.000000 arcesetc-0.1/arcesetc/tests/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)      768 2018-12-03 03:00:28.000000 arcesetc-0.1/arcesetc/tests/coveragerc
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/arcesetc/tests/legacy_specutils/
--rw-r--r--   0 bmmorris   (501) staff       (20)        0 2018-12-03 22:20:49.000000 arcesetc-0.1/arcesetc/tests/legacy_specutils/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     4097 2018-12-03 22:17:17.000000 arcesetc-0.1/arcesetc/tests/legacy_specutils/indexer.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    21548 2018-12-03 22:27:34.000000 arcesetc-0.1/arcesetc/tests/legacy_specutils/readspec.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    14892 2018-12-03 22:21:18.000000 arcesetc-0.1/arcesetc/tests/legacy_specutils/spectrum1d.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    23832 2018-12-03 22:21:17.000000 arcesetc-0.1/arcesetc/tests/legacy_specutils/specwcs.py
--rw-r--r--   0 bmmorris   (501) staff       (20)      289 2018-12-03 03:00:28.000000 arcesetc-0.1/arcesetc/tests/setup_package.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     4097 2018-12-12 03:43:41.000000 arcesetc-0.1/arcesetc/tests/test_utils.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     8959 2018-12-10 22:30:26.000000 arcesetc-0.1/arcesetc/util.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     7344 2018-12-12 03:58:11.000000 arcesetc-0.1/arcesetc/version.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/
--rw-r--r--   0 bmmorris   (501) staff       (20)    35654 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/ah_bootstrap.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/
--rw-r--r--   0 bmmorris   (501) staff       (20)     1738 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/__init__.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/commands/
--rw-r--r--   0 bmmorris   (501) staff       (20)        0 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/commands/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     2738 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/commands/_dummy.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    19715 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/commands/build_ext.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    10319 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/commands/build_sphinx.py
--rw-r--r--   0 bmmorris   (501) staff       (20)      120 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/commands/setup_package.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/commands/src/
--rw-r--r--   0 bmmorris   (501) staff       (20)     3033 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/commands/src/compiler.c
--rw-r--r--   0 bmmorris   (501) staff       (20)     1283 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/commands/test.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     1930 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/conftest.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     7922 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/distutils_helpers.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/
--rw-r--r--   0 bmmorris   (501) staff       (20)      589 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/__init__.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/automodapi/
--rw-r--r--   0 bmmorris   (501) staff       (20)       20 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/automodapi/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     5316 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/automodapi/autodoc_enhancements.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    15785 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/automodapi/automodapi.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    26520 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/automodapi/automodsumm.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     3711 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/automodapi/smart_resolver.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/automodapi/templates/
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/automodapi/templates/autosummary_core/
--rw-r--r--   0 bmmorris   (501) staff       (20)      170 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/automodapi/templates/autosummary_core/base.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1161 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/automodapi/templates/autosummary_core/class.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      703 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/automodapi/templates/autosummary_core/module.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     7140 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/automodapi/utils.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/numpydoc/
--rw-r--r--   0 bmmorris   (501) staff       (20)      117 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/numpydoc/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    18769 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    10822 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape_sphinx.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     9563 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/numpydoc/numpydoc.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/numpydoc/templates/
--rw-r--r--   0 bmmorris   (501) staff       (20)      214 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/numpydoc/templates/numpydoc_docstring.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      189 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/extern/setup_package.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     6465 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/git_helpers.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     3141 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/openmp_helpers.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    26278 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/setup_helpers.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/
--rw-r--r--   0 bmmorris   (501) staff       (20)      437 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    11549 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/conf.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/ext/
--rw-r--r--   0 bmmorris   (501) staff       (20)       66 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/ext/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     2915 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/ext/changelog_links.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     1953 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/ext/doctest.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     5940 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/ext/edit_on_github.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/ext/tests/
--rw-r--r--   0 bmmorris   (501) staff       (20)        0 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/ext/tests/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)      760 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/ext/tocdepthfix.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/local/
--rw-r--r--   0 bmmorris   (501) staff       (20)      658 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.inv
--rw-r--r--   0 bmmorris   (501) staff       (20)     2820 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.txt
--rw-r--r--   0 bmmorris   (501) staff       (20)      292 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/setup_package.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/
--rw-r--r--   0 bmmorris   (501) staff       (20)       73 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/globaltoc.html
--rw-r--r--   0 bmmorris   (501) staff       (20)     3433 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/layout.html
--rw-r--r--   0 bmmorris   (501) staff       (20)       34 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/localtoc.html
--rw-r--r--   0 bmmorris   (501) staff       (20)      272 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/searchbox.html
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/
--rw-r--r--   0 bmmorris   (501) staff       (20)     5201 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout.svg
--rw-r--r--   0 bmmorris   (501) staff       (20)     1725 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout_20.png
--rw-r--r--   0 bmmorris   (501) staff       (20)    32988 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.ico
--rw-r--r--   0 bmmorris   (501) staff       (20)     4634 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.svg
--rw-r--r--   0 bmmorris   (501) staff       (20)     1884 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo_32.png
--rw-r--r--   0 bmmorris   (501) staff       (20)    12067 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/bootstrap-astropy.css
--rw-r--r--   0 bmmorris   (501) staff       (20)     2769 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/copybutton.js
--rw-r--r--   0 bmmorris   (501) staff       (20)     4971 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/sidebar.js
--rw-r--r--   0 bmmorris   (501) staff       (20)      192 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/theme.conf
--rw-r--r--   0 bmmorris   (501) staff       (20)      515 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/test_helpers.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    25574 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/utils.py
--rw-r--r--   0 bmmorris   (501) staff       (20)      566 2018-12-03 03:20:31.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/version.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     9686 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/astropy_helpers/version_helpers.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/astropy_helpers.egg-info/
--rw-r--r--   0 bmmorris   (501) staff       (20)        1 2018-12-03 03:20:31.000000 arcesetc-0.1/astropy_helpers/astropy_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 bmmorris   (501) staff       (20)        1 2018-12-03 03:20:31.000000 arcesetc-0.1/astropy_helpers/astropy_helpers.egg-info/not-zip-safe
--rw-r--r--   0 bmmorris   (501) staff       (20)     4505 2018-12-03 03:20:31.000000 arcesetc-0.1/astropy_helpers/astropy_helpers.egg-info/PKG-INFO
--rw-r--r--   0 bmmorris   (501) staff       (20)     3086 2018-12-03 03:20:31.000000 arcesetc-0.1/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 bmmorris   (501) staff       (20)       16 2018-12-03 03:20:31.000000 arcesetc-0.1/astropy_helpers/astropy_helpers.egg-info/top_level.txt
--rw-r--r--   0 bmmorris   (501) staff       (20)    17822 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/CHANGES.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1491 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/LICENSE.rst
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/astropy_helpers/licenses/
--rw-r--r--   0 bmmorris   (501) staff       (20)     1644 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/licenses/LICENSE_ASTROSCRAPPY.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     2505 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/licenses/LICENSE_COPYBUTTON.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     5959 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/licenses/LICENSE_NUMPYDOC.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     3010 2018-12-03 03:00:29.000000 arcesetc-0.1/astropy_helpers/README.rst
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/docs/
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/docs/.ipynb_checkpoints/
--rw-r--r--   0 bmmorris   (501) staff       (20)     2371 2018-12-09 22:04:02.000000 arcesetc-0.1/docs/.ipynb_checkpoints/paper-checkpoint.md
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/docs/_templates/
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/docs/_templates/autosummary/
--rw-r--r--   0 bmmorris   (501) staff       (20)      250 2018-12-03 02:58:11.000000 arcesetc-0.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      251 2018-12-03 02:58:11.000000 arcesetc-0.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      252 2018-12-03 02:58:11.000000 arcesetc-0.1/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/docs/arcesetc/
--rw-r--r--   0 bmmorris   (501) staff       (20)    56442 2018-12-12 00:49:20.000000 arcesetc-0.1/docs/arcesetc/cmd.png
--rw-r--r--   0 bmmorris   (501) staff       (20)     3631 2018-12-12 03:40:28.000000 arcesetc-0.1/docs/arcesetc/gettingstarted.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      165 2018-12-03 03:00:28.000000 arcesetc-0.1/docs/arcesetc/index.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      494 2018-12-10 16:26:22.000000 arcesetc-0.1/docs/arcesetc/installation.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1987 2018-12-12 03:37:48.000000 arcesetc-0.1/docs/arcesetc/nextsteps.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     7390 2018-12-03 04:28:23.000000 arcesetc-0.1/docs/conf.py
--rw-r--r--   0 bmmorris   (501) staff       (20)      607 2018-12-08 15:41:03.000000 arcesetc-0.1/docs/index.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     4513 2018-12-03 03:00:28.000000 arcesetc-0.1/docs/make.bat
--rw-r--r--   0 bmmorris   (501) staff       (20)     4581 2018-12-03 03:00:28.000000 arcesetc-0.1/docs/Makefile
--rw-r--r--   0 bmmorris   (501) staff       (20)     3671 2018-12-03 15:38:37.000000 arcesetc-0.1/docs/paper.bib
--rw-r--r--   0 bmmorris   (501) staff       (20)     2820 2018-12-11 16:47:24.000000 arcesetc-0.1/docs/paper.md
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2018-12-12 04:00:54.000000 arcesetc-0.1/licenses/
--rw-r--r--   0 bmmorris   (501) staff       (20)     9745 2018-12-03 03:00:28.000000 arcesetc-0.1/licenses/APACHE2.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1305 2018-12-03 03:00:28.000000 arcesetc-0.1/licenses/BSD2.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1510 2018-12-03 03:00:28.000000 arcesetc-0.1/licenses/BSD3.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)    37593 2018-12-03 03:00:28.000000 arcesetc-0.1/licenses/GPLv3.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1054 2018-12-03 05:38:09.000000 arcesetc-0.1/licenses/MIT.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      372 2018-12-03 03:00:28.000000 arcesetc-0.1/licenses/README.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1659 2018-12-03 03:00:28.000000 arcesetc-0.1/licenses/TEMPLATE_LICENCE.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      486 2018-12-12 04:00:54.000000 arcesetc-0.1/PKG-INFO
--rw-r--r--   0 bmmorris   (501) staff       (20)     2675 2018-12-11 00:16:47.000000 arcesetc-0.1/README.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1318 2018-12-12 04:00:44.000000 arcesetc-0.1/setup.cfg
--rwxr-xr-x   0 bmmorris   (501) staff       (20)     5339 2018-12-03 03:00:28.000000 arcesetc-0.1/setup.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.926827 arcesetc-0.3/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.902302 arcesetc-0.3/.github/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.906566 arcesetc-0.3/.github/workflows/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      412 2023-07-28 18:34:36.000000 arcesetc-0.3/.github/workflows/ci.yml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1902 2023-07-28 15:20:05.000000 arcesetc-0.3/.gitignore
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      606 2023-07-28 18:38:07.000000 arcesetc-0.3/.readthedocs.yml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1072 2023-07-28 15:20:05.000000 arcesetc-0.3/LICENSE
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4759 2023-07-28 18:57:25.926637 arcesetc-0.3/PKG-INFO
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3140 2023-07-28 18:56:40.000000 arcesetc-0.3/README.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.907978 arcesetc-0.3/arcesetc/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      453 2023-07-28 18:34:36.000000 arcesetc-0.3/arcesetc/__init__.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      878 2023-07-28 18:34:36.000000 arcesetc-0.3/arcesetc/conftest.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.917116 arcesetc-0.3/arcesetc/data/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   737280 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/data/BD28_4211.0026.wfrmcpc.fits
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   737280 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/data/HIP107864.0003.wfrmcpc.fits
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   737280 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/data/HR5191.0002.wfrmcpc.fits
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      246 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/data/README.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   987636 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/data/archive.hdf5
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2025 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/data/sptype_dict.json
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1152 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/data/sptype_to_temp.json
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     6732 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/plots.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.917594 arcesetc-0.3/arcesetc/tests/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      108 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/tests/__init__.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4099 2023-07-28 18:34:36.000000 arcesetc-0.3/arcesetc/tests/test_utils.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     9169 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/util.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      155 2023-07-28 18:57:25.000000 arcesetc-0.3/arcesetc/version.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.909116 arcesetc-0.3/arcesetc.egg-info/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4759 2023-07-28 18:57:25.000000 arcesetc-0.3/arcesetc.egg-info/PKG-INFO
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2112 2023-07-28 18:57:25.000000 arcesetc-0.3/arcesetc.egg-info/SOURCES.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2023-07-28 18:57:25.000000 arcesetc-0.3/arcesetc.egg-info/dependency_links.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2023-07-28 15:33:13.000000 arcesetc-0.3/arcesetc.egg-info/not-zip-safe
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      248 2023-07-28 18:57:25.000000 arcesetc-0.3/arcesetc.egg-info/requires.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       44 2023-07-28 18:57:25.000000 arcesetc-0.3/arcesetc.egg-info/top_level.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1853 2023-07-28 15:20:05.000000 arcesetc-0.3/contributing.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.919161 arcesetc-0.3/docs/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       98 2023-07-28 18:37:19.000000 arcesetc-0.3/docs/.rtd_environment.yaml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2719 2023-07-28 18:34:36.000000 arcesetc-0.3/docs/Makefile
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.902947 arcesetc-0.3/docs/_build/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.903823 arcesetc-0.3/docs/_build/html/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.903732 arcesetc-0.3/docs/_build/html/_downloads/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.919363 arcesetc-0.3/docs/_build/html/_downloads/1285442fc69ec296739193a5bb01cfd3/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      271 2023-07-28 18:25:45.000000 arcesetc-0.3/docs/_build/html/_downloads/1285442fc69ec296739193a5bb01cfd3/gettingstarted-4.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.919628 arcesetc-0.3/docs/_build/html/_downloads/134ab96a9d43a359afd7287f2aa43fe5/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      271 2023-07-28 18:32:03.000000 arcesetc-0.3/docs/_build/html/_downloads/134ab96a9d43a359afd7287f2aa43fe5/gettingstarted-4.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.919888 arcesetc-0.3/docs/_build/html/_downloads/841caadd042d58ca8a1c4363a8e368a7/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      276 2023-07-28 18:25:45.000000 arcesetc-0.3/docs/_build/html/_downloads/841caadd042d58ca8a1c4363a8e368a7/gettingstarted-2.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.920165 arcesetc-0.3/docs/_build/html/_downloads/b66b1a2ed9b3ca7d529871c1355618c7/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      280 2023-07-28 18:25:45.000000 arcesetc-0.3/docs/_build/html/_downloads/b66b1a2ed9b3ca7d529871c1355618c7/gettingstarted-1.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.920460 arcesetc-0.3/docs/_build/html/_downloads/c5ac9a86f2a29263110f45bf565f7bd4/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      270 2023-07-28 18:25:45.000000 arcesetc-0.3/docs/_build/html/_downloads/c5ac9a86f2a29263110f45bf565f7bd4/gettingstarted-3.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.920739 arcesetc-0.3/docs/_build/html/_downloads/d90ff9160e5ef651bae7944605ca23d4/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      280 2023-07-28 18:32:02.000000 arcesetc-0.3/docs/_build/html/_downloads/d90ff9160e5ef651bae7944605ca23d4/gettingstarted-1.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.921011 arcesetc-0.3/docs/_build/html/_downloads/d97ef3d967eb2cc595a6a4c3ad1454e7/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      276 2023-07-28 18:32:02.000000 arcesetc-0.3/docs/_build/html/_downloads/d97ef3d967eb2cc595a6a4c3ad1454e7/gettingstarted-2.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.921305 arcesetc-0.3/docs/_build/html/_downloads/da6f961d2f854338ba956b87cf0e425a/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      270 2023-07-28 18:32:03.000000 arcesetc-0.3/docs/_build/html/_downloads/da6f961d2f854338ba956b87cf0e425a/gettingstarted-3.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.903886 arcesetc-0.3/docs/_build/html/plot_directive/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.922361 arcesetc-0.3/docs/_build/html/plot_directive/arcesetc/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      280 2023-07-28 18:32:02.000000 arcesetc-0.3/docs/_build/html/plot_directive/arcesetc/gettingstarted-1.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      276 2023-07-28 18:32:02.000000 arcesetc-0.3/docs/_build/html/plot_directive/arcesetc/gettingstarted-2.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      270 2023-07-28 18:32:03.000000 arcesetc-0.3/docs/_build/html/plot_directive/arcesetc/gettingstarted-3.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      271 2023-07-28 18:32:03.000000 arcesetc-0.3/docs/_build/html/plot_directive/arcesetc/gettingstarted-4.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.904040 arcesetc-0.3/docs/_templates/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.923092 arcesetc-0.3/docs/_templates/autosummary/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      250 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      251 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      252 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.924119 arcesetc-0.3/docs/arcesetc/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    59283 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/arcesetc/cmd.png
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3768 2023-07-28 18:34:36.000000 arcesetc-0.3/docs/arcesetc/gettingstarted.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      165 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/arcesetc/index.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      485 2023-07-28 18:34:36.000000 arcesetc-0.3/docs/arcesetc/installation.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2003 2023-07-28 18:34:36.000000 arcesetc-0.3/docs/arcesetc/nextsteps.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     5913 2023-07-28 18:34:36.000000 arcesetc-0.3/docs/conf.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      780 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/index.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3426 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/paper.bib
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3131 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/paper.md
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.925734 arcesetc-0.3/licenses/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     9745 2023-07-28 15:20:05.000000 arcesetc-0.3/licenses/APACHE2.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1305 2023-07-28 15:20:05.000000 arcesetc-0.3/licenses/BSD2.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1510 2023-07-28 15:20:05.000000 arcesetc-0.3/licenses/BSD3.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    37593 2023-07-28 15:20:05.000000 arcesetc-0.3/licenses/GPLv3.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1054 2023-07-28 15:20:05.000000 arcesetc-0.3/licenses/MIT.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      372 2023-07-28 15:20:05.000000 arcesetc-0.3/licenses/README.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1659 2023-07-28 15:20:05.000000 arcesetc-0.3/licenses/TEMPLATE_LICENCE.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.925909 arcesetc-0.3/notebooks/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   241099 2023-07-28 15:20:05.000000 arcesetc-0.3/notebooks/example.ipynb
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2128 2023-07-28 18:34:36.000000 arcesetc-0.3/pyproject.toml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       38 2023-07-28 18:57:25.926878 arcesetc-0.3/setup.cfg
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       61 2023-07-28 18:34:36.000000 arcesetc-0.3/setup.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1763 2023-07-28 18:34:36.000000 arcesetc-0.3/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `arcesetc-0.1/arcesetc/data/archive.hdf5` & `arcesetc-0.3/arcesetc/data/archive.hdf5`

 * *Files 2% similar despite different names*

#### h5dump {}

```diff
@@ -1,8 +1,8 @@
-HDF5 "/tmp/diffoscope_pxq7bwr5_/tmpdib3iks4_TarContainer/0/7.hdf5" {
+HDF5 "/tmp/diffoscope_pxq7bwr5_/tmppc5odkc8_TarContainer/0/17.hdf5" {
 GROUP "/" {
    DATASET "51 Peg" {
       DATATYPE  H5T_IEEE_F32LE
       DATASPACE  SIMPLE { ( 107, 19 ) / ( 107, 19 ) }
       DATA {
       (0,0): 3545.35, 0.0456983, 1651, -1.53743e-21, 1.54843e-20,
       (0,5): 8.21569e-18, -9.34073e-17, -1.75794e-14, 2.24079e-13,
@@ -25884,14 +25884,571 @@
          DATATYPE  H5T_IEEE_F32LE
          DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
          DATA {
          (0): 9.745
          }
       }
    }
+   DATASET "HD 289002" {
+      DATATYPE  H5T_IEEE_F32LE
+      DATASPACE  SIMPLE { ( 107, 19 ) / ( 107, 19 ) }
+      DATA {
+      (0,0): 3545.05, 0.0455988, 1651, -6.80284e-23, -1.09063e-20,
+      (0,5): 1.78783e-19, 5.08807e-17, -1.0669e-17, -9.29655e-14,
+      (0,9): -3.63376e-13, 8.41508e-11, 4.10729e-10, -3.9406e-08,
+      (0,13): -1.75546e-07, 9.24447e-06, 2.95825e-05, -0.00111606,
+      (0,17): -0.00157938, 0.115188,
+      (1,0): 3567.33, 0.0458901, 1651, 1.54114e-22, 4.94524e-21,
+      (1,5): -1.17014e-18, -2.49723e-17, 3.30159e-15, 4.685e-14,
+      (1,9): -4.46297e-12, -4.09809e-11, 3.04813e-09, 1.70868e-08,
+      (1,13): -1.00808e-06, -2.8159e-06, 0.000138033, -0.000129879,
+      (1,17): -0.00487154, 0.110819,
+      (2,0): 3589.9, 0.046185, 1651, 1.47821e-22, -7.85322e-21, -8.5872e-19,
+      (2,6): 3.77312e-17, 1.9063e-15, -7.08705e-14, -2.06012e-12,
+      (2,10): 6.52745e-11, 1.14722e-09, -3.02375e-08, -3.25511e-07,
+      (2,14): 6.61531e-06, 4.23547e-05, -0.000765562, -0.00103607, 0.136717,
+      (3,0): 3612.74, 0.0464836, 1651, -3.79766e-22, -1.4958e-20,
+      (3,5): 1.71478e-18, 6.73538e-17, -3.01891e-15, -1.1686e-13,
+      (3,9): 2.63027e-12, 9.7911e-11, -1.18787e-09, -4.05601e-08, 2.6412e-07,
+      (3,14): 7.74823e-06, -2.46671e-05, -0.00081194, 0.000964546, 0.152882,
+      (4,0): 3635.89, 0.046786, 1651, -9.51842e-22, -1.78324e-20,
+      (4,5): 4.96941e-18, 8.82281e-17, -1.01863e-14, -1.68871e-13,
+      (4,9): 1.03791e-11, 1.56514e-10, -5.50491e-09, -7.21041e-08,
+      (4,13): 1.46395e-06, 1.56253e-05, -0.000172851, -0.00163715,
+      (4,17): 0.00684721, 0.183991,
+      (5,0): 3659.33, 0.0470922, 1651, -2.4134e-22, 2.47469e-22, 1.38004e-18,
+      (5,6): -3.28207e-18, -3.11984e-15, 1.05587e-14, 3.54342e-12,
+      (5,10): -1.42078e-11, -2.12741e-09, 8.84617e-09, 6.52353e-07,
+      (5,14): -2.09917e-06, -9.15473e-05, -0.000259556, 0.00496087, 0.204468,
+      (6,0): 3683.08, 0.0474023, 1651, 1.70095e-22, -2.43674e-21,
+      (6,5): -9.53433e-19, 1.28732e-17, 2.13604e-15, -2.64883e-14,
+      (6,9): -2.44474e-12, 2.68672e-11, 1.51424e-09, -1.41413e-08,
+      (6,13): -4.92042e-07, 4.01109e-06, 7.25983e-05, -0.000898078,
+      (6,17): -0.00287062, 0.22482,
+      (7,0): 3707.13, 0.0477164, 1651, -2.46448e-23, 3.81018e-21,
+      (7,5): 1.81676e-19, -2.07872e-17, -5.19981e-16, 4.4475e-14,
+      (7,9): 7.48095e-13, -4.70877e-11, -5.77007e-10, 2.53931e-08,
+      (7,13): 2.33408e-07, -6.07731e-06, -4.47885e-05, 4.35078e-05,
+      (7,17): 0.00318821, 0.230929,
+      (8,0): 3731.51, 0.0480345, 1651, 2.29139e-22, -1.50368e-22,
+      (8,5): -1.38392e-18, 1.43134e-18, 3.35463e-15, -3.8588e-15,
+      (8,9): -4.1582e-12, 4.16332e-12, 2.77467e-09, -1.90933e-09,
+      (8,13): -9.55266e-07, 7.6129e-07, 0.000143784, -0.000683415,
+      (8,17): -0.0054966, 0.278474,
+      (9,0): 3756.2, 0.0483568, 1651, -1.60837e-22, 2.438e-22, 1.0522e-18,
+      (9,6): -1.3084e-18, -2.78438e-15, 2.77639e-15, 3.81834e-12,
+      (9,10): -2.81175e-12, -2.88386e-09, 9.98392e-10, 1.17257e-06,
+      (9,14): 6.80884e-07, -0.000229695, -0.000875064, 0.015772, 0.314552,
+      (10,0): 3781.23, 0.0486832, 1651, 6.43268e-23, -1.2098e-21,
+      (10,5): -3.81712e-19, 8.02186e-18, 8.75303e-16, -2.14668e-14,
+      (10,9): -9.46395e-13, 2.96924e-11, 4.3707e-10, -2.26756e-08,
+      (10,13): -5.15268e-09, 9.68762e-06, -5.34613e-05, -0.00245931,
+      (10,17): 0.00991847, 0.428713,
+      (11,0): 3806.59, 0.049014, 1651, -1.08802e-22, -2.74396e-21,
+      (11,5): 7.37356e-19, 1.66731e-17, -2.03937e-15, -4.03759e-14,
+      (11,9): 2.95491e-12, 4.9476e-11, -2.39488e-09, -3.22377e-08,
+      (11,13): 1.07287e-06, 1.10407e-05, -0.000243762, -0.00223301,
+      (11,17): 0.0215619, 0.426562,
+      (12,0): 3832.3, 0.0493492, 1651, 2.9624e-22, 2.43162e-21, -1.90848e-18,
+      (12,6): -1.32502e-17, 4.98299e-15, 2.85735e-14, -6.74638e-12,
+      (12,10): -3.11055e-11, 5.02133e-09, 1.80024e-08, -1.99741e-06,
+      (12,14): -4.98162e-06, 0.000374049, -4.76046e-05, -0.0226439, 0.394299,
+      (13,0): 3858.36, 0.0496889, 1651, -4.83286e-23, 6.38452e-23,
+      (13,5): 3.10109e-19, -8.35065e-19, -7.83851e-16, 3.12778e-15,
+      (13,9): 9.76879e-13, -4.94383e-12, -6.06941e-10, 3.10364e-09,
+      (13,13): 1.62124e-07, 3.47547e-07, -1.16781e-05, -0.00141582,
+      (13,17): 0.00144197, 0.578335,
+      (14,0): 3884.77, 0.0500332, 1651, 1.62742e-22, -1.28221e-22,
+      (14,5): -1.10158e-18, 1.7377e-18, 3.04828e-15, -6.1957e-15,
+      (14,9): -4.42964e-12, 9.27063e-12, 3.60528e-09, -6.37265e-09,
+      (14,13): -1.61161e-06, 2.23872e-06, 0.000352882, -0.00101546,
+      (14,17): -0.0266017, 0.50061,
+      (15,0): 3911.55, 0.0503821, 1651, -5.40555e-23, 4.43988e-23,
+      (15,5): 3.54428e-19, -1.08436e-18, -9.28596e-16, 4.75734e-15,
+      (15,9): 1.22904e-12, -8.25707e-12, -8.49757e-10, 5.86761e-09,
+      (15,13): 2.83049e-07, -3.29664e-07, -3.72995e-05, -0.00164045,
+      (15,17): 0.00288838, 0.687513,
+      (16,0): 3938.7, 0.0507358, 1651, 2.14478e-23, 5.34879e-22,
+      (16,5): -1.20877e-19, -2.91061e-18, 2.59712e-16, 6.01243e-15,
+      (16,9): -2.56391e-13, -5.61514e-12, 9.46549e-11, 1.63301e-09,
+      (16,13): 2.5774e-08, 1.42039e-06, -3.26453e-05, -0.00174939,
+      (16,17): 0.00773731, 0.714659,
+      (17,0): 3966.23, 0.0510944, 1651, 1.67527e-22, 1.9138e-21,
+      (17,5): -1.17191e-18, -1.1962e-17, 3.3356e-15, 3.00231e-14,
+      (17,9): -4.95438e-12, -3.87077e-11, 4.08777e-09, 2.70297e-08,
+      (17,13): -1.8345e-06, -9.36753e-06, 0.00040066, 0.000552665,
+      (17,17): -0.0310453, 0.563622,
+      (18,0): 3994.15, 0.0514579, 1651, -4.19011e-23, 7.61936e-22,
+      (18,5): 3.15702e-19, -5.27053e-18, -9.55191e-16, 1.44177e-14,
+      (18,9): 1.47373e-12, -1.95414e-11, -1.21007e-09, 1.29942e-08,
+      (18,13): 4.9781e-07, -2.66721e-06, -8.63213e-05, -0.00144343,
+      (18,17): 0.00574461, 0.79755,
+      (19,0): 4022.46, 0.0518266, 1651, 1.22944e-22, 1.05654e-21,
+      (19,5): -8.78734e-19, -6.45797e-18, 2.54157e-15, 1.55253e-14,
+      (19,9): -3.80268e-12, -1.84709e-11, 3.11448e-09, 1.09306e-08,
+      (19,13): -1.34937e-06, -2.08641e-06, 0.000265558, -0.00122656,
+      (19,17): -0.0139198, 0.790107,
+      (20,0): 4051.18, 0.0522004, 1651, 1.44707e-23, 6.77544e-23,
+      (20,5): -1.00664e-19, -4.61944e-19, 2.79678e-16, 1.31794e-15,
+      (20,9): -3.95174e-13, -1.81594e-12, 2.98075e-10, 6.89626e-10,
+      (20,13): -1.11086e-07, 1.34973e-06, 1.126e-05, -0.00197141, 0.00306206,
+      (20,18): 0.897854,
+      (21,0): 4080.32, 0.0525796, 1651, 1.31618e-23, 6.56692e-22,
+      (21,5): -9.63682e-20, -4.74325e-18, 2.73642e-16, 1.35475e-14,
+      (21,9): -3.68039e-13, -1.91315e-11, 2.14782e-10, 1.31904e-08,
+      (21,13): -1.11262e-08, -2.8146e-06, -3.18066e-05, -0.00151298,
+      (21,17): 0.00554068, 0.89739,
+      (22,0): 4109.87, 0.0529641, 1651, -8.83611e-23, -2.15836e-21,
+      (22,5): 6.52395e-19, 1.40644e-17, -1.97401e-15, -3.6223e-14,
+      (22,9): 3.1478e-12, 4.66731e-11, -2.82845e-09, -3.14244e-08,
+      (22,13): 1.4169e-06, 1.09214e-05, -0.000365696, -0.00257146, 0.0390002,
+      (22,18): 0.813445,
+      (23,0): 4139.86, 0.0533542, 1651, 4.58978e-23, 7.90589e-22,
+      (23,5): -3.36768e-19, -5.19189e-18, 1.00295e-15, 1.34984e-14,
+      (23,9): -1.55443e-12, -1.75349e-11, 1.33224e-09, 1.15285e-08,
+      (23,13): -6.12466e-07, -2.68377e-06, 0.000128714, -0.00125993,
+      (23,17): -0.0063025, 0.942995,
+      (24,0): 4170.29, 0.05375, 1651, 4.13964e-24, 3.82295e-23, -2.72246e-20,
+      (24,6): -2.52222e-19, 6.81742e-17, 7.69166e-16, -7.82001e-14,
+      (24,10): -1.33459e-12, 3.42839e-11, 9.95456e-10, 8.54854e-09,
+      (24,14): 6.58735e-07, -1.56375e-05, -0.00180075, 0.00560276, 1.03315,
+      (25,0): 4201.17, 0.0541515, 1651, -3.2096e-24, -1.29414e-22,
+      (25,5): 2.04767e-20, 9.01903e-19, -5.17571e-17, -2.49081e-15,
+      (25,9): 6.81913e-14, 3.49935e-12, -5.56126e-11, -2.94501e-09,
+      (25,13): 3.63286e-08, 2.30517e-06, -2.05554e-05, -0.00209461,
+      (25,17): 0.00585541, 1.07682,
+      (26,0): 4232.51, 0.054559, 1651, -2.13821e-24, -2.88502e-22,
+      (26,5): 9.37259e-21, 1.93624e-18, -5.11127e-18, -5.03194e-15,
+      (26,9): -3.33252e-14, 6.4259e-12, 6.70208e-11, -4.51902e-09,
+      (26,13): -4.56653e-08, 2.62677e-06, 7.20905e-06, -0.00211093,
+      (26,17): 0.00261832, 1.10276,
+      (27,0): 4264.32, 0.0549725, 1651, -3.22244e-24, -9.86532e-23,
+      (27,5): 1.91949e-20, 5.76556e-19, -3.96215e-17, -1.23685e-15,
+      (27,9): 2.61058e-14, 1.24278e-12, 1.50757e-11, -9.70799e-10,
+      (27,13): -2.40314e-08, 1.51784e-06, 3.34382e-06, -0.00200306,
+      (27,17): 0.00281611, 1.1257,
+      (28,0): 4296.61, 0.0553922, 1651, 9.08242e-24, 1.51698e-22,
+      (28,5): -6.98987e-20, -1.19027e-18, 2.1393e-16, 3.71666e-15,
+      (28,9): -3.29926e-13, -5.78556e-12, 2.64859e-10, 4.35623e-09,
+      (28,13): -9.6863e-08, -5.60516e-07, 3.6049e-06, -0.00167456,
+      (28,17): 0.00501446, 1.15033,
+      (29,0): 4329.4, 0.0558183, 1651, -3.55354e-23, -1.34533e-21,
+      (29,5): 2.77935e-19, 1.01553e-17, -8.71977e-16, -3.06935e-14,
+      (29,9): 1.38986e-12, 4.73459e-11, -1.16324e-09, -3.93811e-08,
+      (29,13): 4.59655e-07, 1.74922e-05, -4.94003e-05, -0.00456691,
+      (29,17): -0.00790575, 1.16157,
+      (30,0): 4362.69, 0.0562508, 1651, -9.10558e-24, 2.23122e-22,
+      (30,5): 6.54803e-20, -2.07638e-18, -1.73583e-16, 7.52433e-15,
+      (30,9): 1.91647e-13, -1.32978e-11, -4.14036e-11, 1.13563e-08,
+      (30,13): -6.70969e-08, -3.11476e-06, 2.88245e-05, -0.00163298,
+      (30,17): 0.00488738, 1.21419,
+      (31,0): 4396.5, 0.05669, 1651, -1.19297e-23, -3.63151e-22, 1.02354e-19,
+      (31,6): 2.70556e-18, -3.6294e-16, -7.91589e-15, 6.85304e-13,
+      (31,10): 1.1531e-11, -7.37916e-10, -8.92877e-09, 4.49668e-07,
+      (31,14): 4.25336e-06, -0.00014493, -0.00232339, 0.0202913, 1.24472,
+      (32,0): 4430.84, 0.0571359, 1651, 7.86025e-24, 1.32133e-22,
+      (32,5): -6.23324e-20, -1.00051e-18, 1.96649e-16, 3.07009e-15,
+      (32,9): -3.11809e-13, -4.8536e-12, 2.54721e-10, 3.96141e-09,
+      (32,13): -9.08278e-08, -8.69224e-07, -1.41081e-06, -0.00144814,
+      (32,17): 0.00720929, 1.23748,
+      (33,0): 4465.72, 0.0575888, 1651, 2.42416e-23, -1.88171e-22,
+      (33,5): -2.17447e-19, 1.67755e-18, 7.89829e-16, -5.81679e-15,
+      (33,9): -1.48686e-12, 9.90039e-12, 1.53943e-09, -8.66787e-09,
+      (33,13): -8.53393e-07, 4.22374e-06, 0.000221906, -0.00218109,
+      (33,17): -0.017136, 1.28343,
+      (34,0): 4501.15, 0.0580488, 1651, -1.30775e-25, -2.1309e-22,
+      (34,5): 1.51242e-21, 1.67471e-18, -9.90298e-18, -5.08619e-15,
+      (34,9): 3.28762e-14, 7.44758e-12, -5.4339e-11, -5.51325e-09,
+      (34,13): 4.63912e-08, 2.69423e-06, -2.42221e-05, -0.00216797,
+      (34,17): 0.00850147, 1.40712,
+      (35,0): 4537.15, 0.0585162, 1651, -4.64434e-24, -9.607e-23,
+      (35,5): 4.29446e-20, 7.8367e-19, -1.62183e-16, -2.52141e-15,
+      (35,9): 3.21355e-13, 4.09961e-12, -3.56776e-10, -3.76379e-09,
+      (35,13): 2.21182e-07, 2.63892e-06, -7.48254e-05, -0.00231678,
+      (35,17): 0.0130034, 1.46461,
+      (36,0): 4573.73, 0.0589909, 1651, 2.54847e-24, 6.81497e-23,
+      (36,5): -2.24481e-20, -5.94557e-19, 8.0597e-17, 2.08734e-15,
+      (36,9): -1.49734e-13, -3.69526e-12, 1.47651e-10, 3.19864e-09,
+      (36,13): -6.50777e-08, -4.56978e-07, -7.37549e-07, -0.00176727,
+      (36,17): 0.00726348, 1.48057,
+      (37,0): 4610.91, 0.0594734, 1651, 7.6052e-25, 1.35619e-23,
+      (37,5): -7.01325e-21, -2.10985e-20, 2.68927e-17, -2.70483e-16,
+      (37,9): -5.35076e-14, 1.09623e-12, 5.40508e-11, -1.76e-09, -1.7404e-08,
+      (37,14): 1.90978e-06, -1.23263e-05, -0.00214633, 0.00836845, 1.52363,
+      (38,0): 4648.69, 0.0599636, 1651, 1.08092e-24, 8.97047e-24,
+      (38,5): -8.64402e-21, -7.66738e-20, 2.61012e-17, 3.12567e-16,
+      (38,9): -3.45173e-14, -7.3174e-13, 1.11313e-11, 7.99024e-10,
+      (38,13): 2.07605e-08, 2.86534e-07, -2.50625e-05, -0.00177841,
+      (38,17): 0.00938013, 1.55139,
+      (39,0): 4687.1, 0.0604619, 1651, -7.72369e-26, -1.29381e-22,
+      (39,5): -4.40747e-22, 1.16208e-18, 5.09567e-18, -4.12649e-15,
+      (39,9): -1.19438e-14, 7.37371e-12, 3.07204e-12, -7.12758e-09,
+      (39,13): 2.15135e-08, 4.25622e-06, -2.79468e-05, -0.00265061,
+      (39,17): 0.0107685, 1.62889,
+      (40,0): 4726.15, 0.0609684, 1651, 3.58329e-25, -1.95783e-23,
+      (40,5): -5.59943e-21, 1.75387e-19, 3.01386e-17, -6.38193e-16,
+      (40,9): -7.48682e-14, 1.21527e-12, 8.8149e-11, -1.41547e-09,
+      (40,13): -3.6316e-08, 1.54231e-06, -1.28255e-05, -0.00205791,
+      (40,17): 0.0108646, 1.62641,
+      (41,0): 4765.86, 0.0614834, 1651, -9.11018e-25, 1.93566e-23,
+      (41,5): 7.99185e-21, -1.85573e-19, -2.63005e-17, 7.39351e-16,
+      (41,9): 3.94264e-14, -1.55738e-12, -2.57379e-11, 1.67694e-09,
+      (41,13): 8.72012e-09, -2.5345e-07, -1.06289e-05, -0.00164105,
+      (41,17): 0.00734624, 1.65492,
+      (42,0): 4806.24, 0.062007, 1651, 4.64379e-25, -1.10583e-23,
+      (42,5): -4.64322e-21, 8.74829e-20, 1.7795e-17, -2.53067e-16,
+      (42,9): -3.17349e-14, 3.38511e-13, 2.24499e-11, -3.76839e-10,
+      (42,13): 6.94296e-09, 9.75455e-07, -2.11612e-05, -0.00199523,
+      (42,17): 0.0102907, 1.71501,
+      (43,0): 4847.31, 0.0625395, 1651, -1.45231e-23, -3.2926e-22, 1.468e-19,
+      (43,6): 3.15291e-18, -5.96157e-16, -1.21566e-14, 1.23699e-12,
+      (43,10): 2.41022e-11, -1.37243e-09, -2.60077e-08, 7.66035e-07,
+      (43,14): 1.50901e-05, -0.000169767, -0.00509575, 0.00338457, 1.75211,
+      (44,0): 4889.08, 0.0630811, 1651, -5.83344e-24, -6.78062e-23,
+      (44,5): 6.00797e-20, 5.47907e-19, -2.45998e-16, -1.59135e-15,
+      (44,9): 5.05558e-13, 1.89127e-12, -5.39608e-10, -7.29996e-10,
+      (44,13): 2.80331e-07, 5.9357e-07, -6.74894e-05, -0.00192665, 0.0149871,
+      (44,18): 1.7293,
+      (45,0): 4931.59, 0.063632, 1651, -4.98918e-24, -1.70856e-22,
+      (45,5): 5.15692e-20, 1.61435e-18, -2.17294e-16, -6.01485e-15,
+      (45,9): 4.80547e-13, 1.11735e-11, -5.98781e-10, -1.08331e-08,
+      (45,13): 4.20832e-07, 5.63658e-06, -0.000160065, -0.00262968,
+      (45,17): 0.0293899, 1.7808,
+      (46,0): 4974.84, 0.0641926, 1651, -2.72043e-25, 1.06829e-24,
+      (46,5): 2.83024e-21, -1.2016e-20, -1.22673e-17, 4.66971e-17,
+      (46,9): 2.88811e-14, -7.08162e-14, -4.12844e-11, -8.55354e-11,
+      (46,13): 4.03619e-08, 7.67261e-07, -3.01741e-05, -0.00188497,
+      (46,17): 0.0128975, 1.83695,
+      (47,0): 5018.86, 0.064763, 1651, -8.29183e-25, -1.75683e-23,
+      (47,5): 9.31522e-21, 1.66176e-19, -4.2202e-17, -5.93799e-16,
+      (47,9): 9.98102e-14, 9.82435e-13, -1.3528e-10, -7.99977e-10,
+      (47,13): 1.12209e-07, 7.55876e-07, -6.13209e-05, -0.00166066,
+      (47,17): 0.0193274, 1.79541,
+      (48,0): 5063.66, 0.0653435, 1651, 5.59637e-25, 2.99785e-24,
+      (48,5): -6.03802e-21, -1.37762e-20, 2.66132e-17, -1.29685e-17,
+      (48,9): -6.07893e-14, 1.83327e-13, 7.34214e-11, -4.96887e-10,
+      (48,13): -3.74266e-08, 1.01026e-06, -7.1517e-06, -0.00185361,
+      (48,17): 0.0122889, 1.84251,
+      (49,0): 5109.27, 0.0659344, 1651, 3.29944e-25, 2.2442e-23,
+      (49,5): -3.58363e-21, -2.38059e-19, 1.61228e-17, 1.00219e-15,
+      (49,9): -3.79905e-14, -2.09932e-12, 4.6976e-11, 2.16009e-09,
+      (49,13): -2.18613e-08, -5.09644e-07, -1.10666e-05, -0.00148914,
+      (49,17): 0.012741, 1.85444,
+      (50,0): 5155.71, 0.066536, 1651, -2.60312e-25, -6.87816e-24,
+      (50,5): 3.03887e-21, 8.28491e-20, -1.43918e-17, -3.8452e-16,
+      (50,9): 3.58514e-14, 8.65753e-13, -5.19855e-11, -1.03905e-09,
+      (50,13): 4.86693e-08, 1.0276e-06, -3.46414e-05, -0.00167069, 0.0161601,
+      (50,18): 1.83725,
+      (51,0): 5203, 0.0671485, 1651, -2.50932e-25, -1.60755e-23, 2.63752e-21,
+      (51,6): 1.58659e-19, -1.13308e-17, -6.0474e-16, 2.59719e-14,
+      (51,10): 1.10673e-12, -3.59943e-11, -1.02869e-09, 3.58018e-08,
+      (51,14): 8.16874e-07, -3.08606e-05, -0.00150131, 0.0168921, 1.77971,
+      (52,0): 5251.17, 0.0677723, 1651, 1.10326e-25, -1.56768e-23,
+      (52,5): -1.5214e-21, 1.79987e-19, 7.94152e-18, -8.18945e-16,
+      (52,9): -1.93405e-14, 1.8729e-12, 1.95827e-11, -2.3012e-09,
+      (52,13): 3.77914e-09, 1.7868e-06, -2.56287e-05, -0.00175383, 0.0183272,
+      (52,18): 1.7812,
+      (53,0): 5300.24, 0.0684077, 1651, -2.40806e-25, -5.94928e-24,
+      (53,5): 2.53895e-21, 6.31256e-20, -1.00733e-17, -2.65885e-16,
+      (53,9): 1.85446e-14, 5.70887e-13, -1.70817e-11, -7.13332e-10,
+      (53,13): 1.48016e-08, 8.14361e-07, -2.33866e-05, -0.00142785,
+      (53,17): 0.0191817, 1.6852,
+      (54,0): 5350.23, 0.0690551, 1651, -5.4365e-26, -9.78797e-24,
+      (54,5): 8.92363e-22, 1.24043e-19, -5.56073e-18, -6.08852e-16,
+      (54,9): 1.78233e-14, 1.4704e-12, -3.35324e-11, -1.86367e-09,
+      (54,13): 4.14316e-08, 1.4613e-06, -3.79363e-05, -0.0015213, 0.0221811,
+      (54,18): 1.68379,
+      (55,0): 5401.18, 0.0697147, 1651, 4.91381e-25, -3.86883e-24,
+      (55,5): -6.26228e-21, 5.61695e-20, 3.20563e-17, -3.07793e-16,
+      (55,9): -8.35011e-14, 8.16822e-13, 1.14304e-10, -1.14755e-09,
+      (55,13): -7.17695e-08, 1.10977e-06, 1.87338e-06, -0.00148552,
+      (55,17): 0.0183446, 1.71815,
+      (56,0): 5453.11, 0.0703868, 1651, 1.62963e-25, 1.03702e-23,
+      (56,5): -2.17675e-21, -1.27894e-19, 1.19733e-17, 6.37077e-16,
+      (56,9): -3.42562e-14, -1.61643e-12, 5.1872e-11, 2.11571e-09,
+      (56,13): -3.31029e-08, -1.03664e-06, -9.20343e-06, -0.00089535,
+      (56,17): 0.0207174, 1.70669,
+      (57,0): 5506.04, 0.071072, 1651, 3.40781e-25, -3.56493e-24,
+      (57,5): -4.50529e-21, 4.01053e-20, 2.3966e-17, -1.68448e-16,
+      (57,9): -6.50365e-14, 3.29746e-13, 9.29104e-11, -3.52014e-10,
+      (57,13): -6.03386e-08, 5.12171e-07, -4.4243e-07, -0.00132627, 0.019215,
+      (57,18): 1.80611,
+      (58,0): 5560.01, 0.0717706, 1651, 4.68362e-25, 1.04352e-23,
+      (58,5): -6.30373e-21, -1.24227e-19, 3.41598e-17, 5.76336e-16,
+      (58,9): -9.46722e-14, -1.30208e-12, 1.39448e-10, 1.41481e-09,
+      (58,13): -9.78713e-08, -3.50631e-07, 1.19694e-05, -0.00118636,
+      (58,17): 0.0188265, 1.86781,
+      (59,0): 5615.06, 0.0724829, 1651, -4.13078e-26, -1.15477e-23,
+      (59,5): 3.03375e-22, 1.35769e-19, -4.81819e-19, -6.2225e-16,
+      (59,9): -5.21711e-16, 1.40682e-12, -1.34353e-12, -1.67494e-09,
+      (59,13): 1.40796e-08, 1.27801e-06, -2.79118e-05, -0.00148765,
+      (59,17): 0.0218799, 1.915,
+      (60,0): 5671.2, 0.0732094, 1651, 7.16176e-26, -5.22283e-24,
+      (60,5): -1.14889e-21, 5.69373e-20, 7.2e-18, -2.27694e-16, -2.24544e-14,
+      (60,10): 3.86608e-13, 3.5877e-11, -2.11302e-10, -2.40259e-08,
+      (60,14): 1.14877e-07, -6.10459e-06, -0.00101712, 0.016206, 1.87104,
+      (61,0): 5728.48, 0.0739504, 1651, -8.35622e-26, -6.15055e-24,
+      (61,5): 9.35444e-22, 7.3503e-20, -3.77762e-18, -3.42336e-16,
+      (61,9): 6.1158e-15, 7.81835e-13, -2.07711e-12, -9.16915e-10,
+      (61,13): 1.11843e-10, 6.98773e-07, -1.33575e-05, -0.00112811,
+      (61,17): 0.0187882, 1.80898,
+      (62,0): 5786.92, 0.0747066, 1651, 1.47654e-25, 6.56308e-24,
+      (62,5): -1.94561e-21, -8.72571e-20, 1.00719e-17, 4.62215e-16,
+      (62,9): -2.55029e-14, -1.23727e-12, 3.0663e-11, 1.73452e-09,
+      (62,13): -8.59716e-09, -1.0471e-06, -1.91538e-05, -0.000560967,
+      (62,17): 0.0215597, 1.68136,
+      (63,0): 5846.57, 0.0754783, 1651, 3.86964e-25, 1.30311e-23,
+      (63,5): -5.49071e-21, -1.74477e-19, 3.11545e-17, 9.24598e-16,
+      (63,9): -8.97935e-14, -2.45856e-12, 1.36905e-10, 3.40391e-09,
+      (63,13): -1.00243e-07, -2.11497e-06, 1.59392e-05, -0.000392125,
+      (63,17): 0.018126, 1.73439,
+      (64,0): 5907.47, 0.0762659, 1651, -1.43006e-25, -1.22678e-23,
+      (64,5): 2.03498e-21, 1.67203e-19, -1.18546e-17, -8.98513e-16,
+      (64,9): 3.68135e-14, 2.40859e-12, -6.7072e-11, -3.37071e-09,
+      (64,13): 7.59424e-08, 2.48471e-06, -5.85515e-05, -0.00154626,
+      (64,17): 0.0319621, 1.73838,
+      (65,0): 5969.64, 0.0770701, 1651, -9.01433e-27, 1.38808e-24,
+      (65,5): 1.09328e-22, -2.45638e-20, -4.5529e-19, 1.69177e-16,
+      (65,9): 8.18803e-16, -5.76851e-13, -1.68215e-12, 1.00254e-09,
+      (65,13): 7.72418e-09, -6.84265e-07, -2.05379e-05, -0.000609579,
+      (65,17): 0.023191, 1.69265,
+      (66,0): 6033.14, 0.0778913, 1651, 1.93216e-26, -6.40086e-25,
+      (66,5): -2.94586e-22, 8.18982e-21, 1.82108e-18, -3.86408e-17,
+      (66,9): -5.7476e-15, 7.84291e-14, 8.99839e-12, -6.28032e-11,
+      (66,13): -2.6839e-09, 1.43336e-07, -1.44644e-05, -0.000849429,
+      (66,17): 0.0217006, 1.73637,
+      (67,0): 6098.01, 0.0787302, 1651, 7.44407e-26, 2.8731e-24,
+      (67,5): -1.18042e-21, -4.35994e-20, 7.50191e-18, 2.63173e-16,
+      (67,9): -2.4138e-14, -8.00898e-13, 4.02057e-11, 1.26921e-09,
+      (67,13): -2.86482e-08, -8.49592e-07, -5.63768e-06, -0.000532378,
+      (67,17): 0.0209153, 1.74096,
+      (68,0): 6164.28, 0.0795872, 1651, 8.57529e-27, -2.50439e-24,
+      (68,5): -1.90407e-22, 3.62414e-20, 1.63857e-18, -2.02284e-16,
+      (68,9): -6.93823e-15, 5.40769e-13, 1.46121e-11, -6.99858e-10,
+      (68,13): -1.12903e-08, 4.95516e-07, -9.24476e-06, -0.000842845,
+      (68,17): 0.0206654, 1.74291,
+      (69,0): 6232.02, 0.0804629, 1651, 6.02195e-26, 4.9127e-25,
+      (69,5): -9.29576e-22, -5.63236e-21, 5.6527e-18, 2.25991e-17,
+      (69,9): -1.69856e-14, -3.51427e-14, 2.52084e-11, 4.39759e-12,
+      (69,13): -1.25111e-08, 1.38914e-07, -1.34594e-05, -0.000786557,
+      (69,17): 0.022244, 1.73823,
+      (70,0): 6301.25, 0.0813581, 1651, 4.23305e-26, -2.73685e-24,
+      (70,5): -7.88101e-22, 4.63616e-20, 5.8159e-18, -3.11171e-16,
+      (70,9): -2.14134e-14, 1.04689e-12, 4.00166e-11, -1.84045e-09,
+      (70,13): -3.11471e-08, 1.67222e-06, -6.0384e-06, -0.00121401,
+      (70,17): 0.0232764, 1.70112,
+      (71,0): 6372.04, 0.0822733, 1651, 6.80606e-27, 9.91134e-25,
+      (71,5): -9.74195e-23, -1.67223e-20, 5.34842e-19, 1.1322e-16,
+      (71,9): -1.34391e-15, -3.9087e-13, 9.39552e-13, 7.12219e-10,
+      (71,13): 3.94967e-09, -5.44489e-07, -1.49911e-05, -0.000488901,
+      (71,17): 0.0215097, 1.74248,
+      (72,0): 6444.45, 0.0832092, 1651, -1.2026e-26, 7.00434e-26, 1.9847e-22,
+      (72,6): -2.24138e-21, -1.28367e-18, 2.24129e-17, 4.22207e-15,
+      (72,10): -1.01815e-13, -8.23819e-12, 2.20653e-10, 1.27238e-08,
+      (72,14): -1.1646e-07, -2.00663e-05, -0.000648858, 0.0226576, 1.77879,
+      (73,0): 6518.51, 0.0841666, 1651, -5.29061e-26, -2.25254e-24,
+      (73,5): 9.53306e-22, 3.93336e-20, -6.74553e-18, -2.68448e-16,
+      (73,9): 2.36386e-14, 8.9227e-13, -4.28669e-11, -1.45584e-09,
+      (73,13): 4.0755e-08, 1.09221e-06, -2.79492e-05, -0.000858914,
+      (73,17): 0.0224933, 1.69818,
+      (74,0): 6594.3, 0.0851461, 1651, -2.58642e-26, 1.53887e-24,
+      (74,5): 4.56819e-22, -2.93178e-20, -3.12859e-18, 2.16728e-16,
+      (74,9): 1.02295e-14, -7.79667e-13, -1.55935e-11, 1.37277e-09,
+      (74,13): 9.76147e-09, -9.04414e-07, -1.05119e-05, -0.000559355,
+      (74,17): 0.0231621, 1.75152,
+      (75,0): 6671.87, 0.0861487, 1651, 3.50225e-26, 4.66179e-25,
+      (75,5): -6.85585e-22, -8.14235e-21, 5.44227e-18, 5.81074e-17,
+      (75,9): -2.2354e-14, -2.20551e-13, 4.99479e-11, 4.7965e-10,
+      (75,13): -5.69394e-08, -5.24409e-07, 2.14128e-05, -0.000231022,
+      (75,17): 0.0146228, 1.6472,
+      (76,0): 6751.29, 0.0871751, 1651, -5.3196e-28, 3.58835e-25,
+      (76,5): 3.46967e-24, -6.35374e-21, 1.44166e-20, 4.46069e-17,
+      (76,9): -2.6723e-17, -1.60257e-13, -1.19911e-12, 3.13567e-10,
+      (76,13): 6.90251e-09, -2.54451e-07, -1.69229e-05, -0.000468373,
+      (76,17): 0.0222656, 1.76413,
+      (77,0): 6832.62, 0.0882261, 1651, 1.43499e-26, -8.64637e-25,
+      (77,5): -3.72897e-22, 1.24654e-20, 3.70503e-18, -5.83015e-17,
+      (77,9): -1.8052e-14, 5.7388e-14, 4.4818e-11, 2.72517e-10, -5.05577e-08,
+      (77,14): -6.11177e-07, 1.08786e-05, -0.000222495, 0.0180739, 1.67962,
+      (78,0): 6915.94, 0.0893027, 1651, -1.39168e-27, -8.97326e-25,
+      (78,5): 4.35418e-23, 1.66427e-20, -5.91844e-19, -1.19953e-16,
+      (78,9): 4.15111e-15, 4.19329e-13, -1.55888e-11, -7.24711e-10,
+      (78,13): 3.11797e-08, 6.18978e-07, -3.47221e-05, -0.000679907,
+      (78,17): 0.0274333, 1.63161,
+      (79,0): 7001.31, 0.0904058, 1651, 2.02707e-27, -1.40543e-26,
+      (79,5): -3.84102e-23, 3.03313e-22, 2.78964e-19, -2.08582e-18,
+      (79,9): -8.62775e-16, 4.96657e-15, 2.46784e-13, 4.85019e-13,
+      (79,13): 5.52721e-09, 2.68573e-08, -1.58912e-05, -0.000461353,
+      (79,17): 0.0209301, 1.64306,
+      (80,0): 7088.82, 0.0915364, 1651, 9.24559e-27, -4.42781e-26,
+      (80,5): -2.02884e-22, 1.19641e-21, 1.78929e-18, -1.21579e-17,
+      (80,9): -8.04111e-15, 6.04428e-14, 1.9088e-11, -1.59308e-10,
+      (80,13): -2.13487e-08, 2.62867e-07, 2.80782e-06, -0.000595759,
+      (80,17): 0.0169636, 1.60678,
+      (81,0): 7178.54, 0.0926956, 1651, -1.93951e-27, -3.15658e-25,
+      (81,5): 4.12668e-23, 6.222e-21, -3.58609e-19, -4.81973e-17,
+      (81,9): 1.60198e-15, 1.82975e-13, -3.76791e-12, -3.38618e-10,
+      (81,13): 4.58009e-09, 2.67586e-07, -5.88353e-06, -0.000347461,
+      (81,17): 0.0135033, 1.39389,
+      (82,0): 7270.56, 0.0938844, 1651, 1.24798e-28, -1.93158e-25,
+      (82,5): -1.6538e-23, 3.69723e-21, 2.99695e-19, -2.73969e-17,
+      (82,9): -2.25343e-15, 9.8316e-14, 8.3406e-12, -1.75344e-10,
+      (82,13): -1.45903e-08, 1.74644e-07, 6.47064e-06, -0.000405318,
+      (82,17): 0.0119813, 1.38957,
+      (83,0): 7364.98, 0.0951041, 1651, 2.55524e-27, -4.92829e-26,
+      (83,5): -5.82137e-23, 9.00671e-22, 5.1828e-19, -5.8554e-18,
+      (83,9): -2.24379e-15, 1.45125e-14, 4.62476e-12, -1.17197e-12,
+      (83,13): -2.64139e-09, -1.40419e-08, -6.64864e-06, -0.000310781,
+      (83,17): 0.0155416, 1.38362,
+      (84,0): 7461.88, 0.0963558, 1651, 2.83883e-27, -6.33354e-26,
+      (84,5): -6.52542e-23, 1.70334e-21, 6.00421e-19, -1.7839e-17,
+      (84,9): -2.808e-15, 9.22047e-14, 6.92028e-12, -2.44568e-10,
+      (84,13): -7.81136e-09, 3.34185e-07, -9.15304e-07, -0.000466696,
+      (84,17): 0.0129845, 1.3431,
+      (85,0): 7561.36, 0.0976408, 1651, 1.18668e-26, -4.3856e-25,
+      (85,5): -3.39217e-22, 7.0566e-21, 3.80989e-18, -3.09347e-17,
+      (85,9): -2.13647e-14, -4.4372e-14, 6.20573e-11, 6.36443e-10,
+      (85,13): -8.50629e-08, -1.3781e-06, 3.65823e-05, 0.000455025, 0.006294,
+      (85,18): 1.22154,
+      (86,0): 7663.53, 0.0989604, 1651, 6.41768e-27, 2.4099e-25,
+      (86,5): -1.67877e-22, -4.93513e-21, 1.77279e-18, 3.74935e-17,
+      (86,9): -9.56595e-15, -1.26369e-13, 2.73107e-11, 1.62711e-10,
+      (86,13): -3.74924e-08, 3.81868e-08, 1.37106e-05, -0.000371249,
+      (86,17): 0.0173143, 0.977753,
+      (87,0): 7768.5, 0.100316, 1651, 1.72691e-28, 1.98468e-26, -4.96526e-24,
+      (87,6): -6.61527e-22, 6.17633e-20, 8.36669e-18, -4.28003e-16,
+      (87,10): -5.19783e-14, 1.69828e-12, 1.67078e-10, -3.29603e-09,
+      (87,14): -2.4583e-07, 1.75062e-07, -7.07603e-05, 0.00953056, 1.06282,
+      (88,0): 7876.38, 0.10171, 1651, -1.06846e-27, -8.20172e-26,
+      (88,5): 2.49016e-23, 1.87931e-21, -2.25379e-19, -1.66338e-17,
+      (88,9): 9.96749e-16, 7.03492e-14, -2.25743e-12, -1.39996e-10,
+      (88,13): 2.85776e-09, 1.16304e-07, -4.28421e-06, -0.000206417,
+      (88,17): 0.00943694, 1.00875,
+      (89,0): 7987.3, 0.103142, 1651, 1.74513e-27, -7.21456e-27,
+      (89,5): -4.58582e-23, 2.72126e-22, 4.78528e-19, -3.51385e-18,
+      (89,9): -2.50885e-15, 2.02711e-14, 6.83022e-12, -5.31625e-11,
+      (89,13): -8.58421e-09, 6.51086e-08, 1.28549e-06, -0.000195782,
+      (89,17): 0.00858076, 0.951316,
+      (90,0): 8101.4, 0.104615, 1651, 3.02912e-28, 3.46545e-26, -7.39023e-24,
+      (90,6): -9.25519e-22, 7.03637e-20, 9.69719e-18, -3.25204e-16,
+      (90,10): -5.01904e-14, 6.81068e-13, 1.31904e-10, 2.38383e-11,
+      (90,14): -1.48741e-07, -3.44721e-06, -0.000108102, 0.00789407,
+      (90,18): 0.875473,
+      (91,0): 8218.8, 0.106132, 1651, 1.99743e-27, 1.84403e-26, -5.91214e-23,
+      (91,6): -3.85588e-22, 7.11525e-19, 2.96271e-18, -4.45844e-15,
+      (91,10): -1.06196e-14, 1.53978e-11, 2.18114e-11, -2.81517e-08,
+      (91,14): -3.25979e-08, 2.20889e-05, -8.28611e-05, 0.000592894, 0.75471,
+      (92,0): 8339.65, 0.107692, 1651, -1.82449e-28, -1.16715e-26,
+      (92,5): 5.22074e-24, 3.07037e-22, -6.13404e-20, -3.06584e-18,
+      (92,9): 3.87678e-16, 1.38838e-14, -1.47236e-12, -2.47036e-11,
+      (92,13): 3.66012e-09, 6.43144e-09, -6.67292e-06, -9.89457e-05,
+      (92,17): 0.00920509, 0.725283,
+      (93,0): 8464.11, 0.109299, 1651, -1.60817e-28, 6.88819e-27, 6.8124e-24,
+      (93,6): -1.71652e-22, -1.11599e-19, 1.67252e-18, 9.23068e-16,
+      (93,10): -7.96095e-15, -4.14765e-12, 1.75857e-11, 1.00624e-08,
+      (93,14): -5.12653e-12, -1.27267e-05, -0.000144459, 0.00959225,
+      (93,18): 0.695308,
+      (94,0): 8592.34, 0.110955, 1651, -7.40567e-29, 3.38253e-27,
+      (94,5): 1.99191e-24, -1.22865e-22, -2.01208e-20, 1.69875e-18,
+      (94,9): 9.14837e-17, -1.14535e-14, -1.68025e-13, 3.98385e-11,
+      (94,13): 1.31867e-10, -6.35979e-08, -1.13041e-06, -5.48623e-05,
+      (94,17): 0.00487517, 0.652469,
+      (95,0): 8724.51, 0.112662, 1651, -3.80445e-28, -2.22932e-26,
+      (95,5): 1.24798e-23, 6.54321e-22, -1.65011e-19, -7.55927e-18,
+      (95,9): 1.12354e-15, 4.35331e-14, -4.15708e-12, -1.31093e-10,
+      (95,13): 8.01021e-09, 2.06281e-07, -7.1126e-06, -0.000241423,
+      (95,17): 0.00446982, 0.657911,
+      (96,0): 8860.82, 0.114421, 1651, 4.83548e-29, 9.59349e-27,
+      (96,5): -1.93984e-24, -3.46301e-22, 3.14152e-20, 4.92912e-18,
+      (96,9): -2.62207e-16, -3.53136e-14, 1.18429e-12, 1.34332e-10,
+      (96,13): -2.7133e-09, -2.57869e-07, 2.04949e-06, 0.000143961,
+      (96,17): 0.00299791, 0.542228,
+      (97,0): 9001.45, 0.116237, 1651, 4.70341e-29, -1.21011e-26,
+      (97,5): -2.24105e-24, 3.85658e-22, 4.19895e-20, -4.90776e-18,
+      (97,9): -4.06258e-16, 3.15005e-14, 2.18661e-12, -1.04206e-10,
+      (97,13): -6.39424e-09, 1.54726e-07, 8.5616e-06, -9.66876e-05,
+      (97,17): -0.00147894, 0.465276,
+      (98,0): 9146.62, 0.118111, 1651, -7.35187e-29, 3.48592e-27,
+      (98,5): 2.85226e-24, -1.29716e-22, -4.54001e-20, 1.88123e-18,
+      (98,9): 3.79538e-16, -1.36408e-14, -1.76419e-12, 5.31742e-11,
+      (98,13): 4.45151e-09, -1.09517e-07, -5.90371e-06, 4.90338e-05,
+      (98,17): 0.00519504, 0.478934,
+      (99,0): 9296.55, 0.120047, 1651, 5.21005e-29, -3.96155e-27,
+      (99,5): -1.97262e-24, 1.21574e-22, 2.85747e-20, -1.48622e-18,
+      (99,9): -1.9587e-16, 9.3405e-15, 6.19697e-13, -3.28753e-11,
+      (99,13): -6.50059e-10, 7.15817e-08, -2.68111e-07, -0.000142954,
+      (99,17): 0.000210327, 0.428638,
+      (100,0): 9451.48, 0.122047, 1651, -9.05085e-30, 8.16131e-27,
+      (100,5): 5.82176e-25, -2.84831e-22, -1.26776e-20, 3.94387e-18,
+      (100,9): 1.32224e-16, -2.75428e-14, -7.39792e-13, 1.01819e-10,
+      (100,13): 2.29664e-09, -1.88321e-07, -3.89753e-06, 0.000111533,
+      (100,17): 0.00334833, 0.263298,
+      (101,0): 9611.65, 0.124115, 1651, -2.17921e-29, -8.07301e-27,
+      (101,5): 5.75846e-25, 2.76148e-22, -5.10262e-21, -3.68027e-18,
+      (101,9): 1.30654e-17, 2.39836e-14, 4.5416e-14, -7.8157e-11,
+      (101,13): -2.57126e-10, 1.16247e-07, 4.9702e-08, -8.54038e-05,
+      (101,17): 0.00148879, 0.250039,
+      (102,0): 9777.36, 0.126254, 1651, -1.24414e-29, -1.26574e-27,
+      (102,5): 4.19361e-25, 4.56834e-23, -4.94686e-21, -6.40745e-19,
+      (102,9): 2.02459e-17, 4.35127e-15, 3.25544e-14, -1.43135e-11,
+      (102,13): -4.33671e-10, 1.96293e-08, 7.67463e-07, -2.47268e-05,
+      (102,17): 0.000268535, 0.21962,
+      (103,0): 9948.87, 0.128468, 1651, -8.69702e-30, 3.17561e-28,
+      (103,5): 4.0404e-25, -1.12431e-23, -7.55448e-21, 1.50796e-19,
+      (103,9): 7.20502e-17, -9.53017e-16, -3.66105e-13, 2.77018e-12,
+      (103,13): 9.43417e-10, -1.94027e-09, -1.10133e-06, -1.69311e-05,
+      (103,17): 0.000513689, 0.155266,
+      (104,0): 10126.5, 0.130761, 1651, 9.18028e-31, 8.6631e-28,
+      (104,5): -7.74298e-26, -3.1753e-23, 2.41513e-21, 4.45138e-19,
+      (104,9): -3.58961e-17, -3.00823e-15, 2.723e-13, 1.04076e-11,
+      (104,13): -1.02801e-09, -1.90261e-08, 1.70102e-06, 1.17288e-05,
+      (104,17): -0.00093605, 0.0742655,
+      (105,0): 10310.6, 0.133137, 1651, -9.25668e-30, -7.17603e-28,
+      (105,5): 4.02603e-25, 2.8564e-23, -6.90349e-21, -4.40296e-19,
+      (105,9): 5.89012e-17, 3.29401e-15, -2.58449e-13, -1.21859e-11,
+      (105,13): 5.33448e-10, 1.98035e-08, -3.57129e-07, -1.10568e-05,
+      (105,17): -0.000110375, 0.0260702,
+      (106,0): 10501.5, 0.135602, 1651, 3.21035e-28, -1.12092e-26,
+      (106,5): -1.38013e-23, 4.6239e-22, 2.34334e-19, -7.33685e-18,
+      (106,9): -1.99911e-15, 5.6425e-14, 9.00736e-12, -2.17127e-10,
+      (106,13): -2.05758e-08, 3.87203e-07, 2.06126e-05, -0.000256239,
+      (106,17): -0.00593036, 0.0309743
+      }
+      ATTRIBUTE "NAME" {
+         DATATYPE  H5T_STRING {
+            STRSIZE H5T_VARIABLE;
+            STRPAD H5T_STR_NULLTERM;
+            CSET H5T_CSET_UTF8;
+            CTYPE H5T_C_S1;
+         }
+         DATASPACE  SCALAR
+         DATA {
+         (0): "HD 289002"
+         }
+      }
+      ATTRIBUTE "SP_TYPE" {
+         DATATYPE  H5T_STRING {
+            STRSIZE H5T_VARIABLE;
+            STRPAD H5T_STR_NULLTERM;
+            CSET H5T_CSET_UTF8;
+            CTYPE H5T_C_S1;
+         }
+         DATASPACE  SCALAR
+         DATA {
+         (0): "B1V"
+         }
+      }
+      ATTRIBUTE "V" {
+         DATATYPE  H5T_IEEE_F32LE
+         DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
+         DATA {
+         (0): 10.44
+         }
+      }
+   }
    DATASET "HD 35601" {
       DATATYPE  H5T_IEEE_F32LE
       DATASPACE  SIMPLE { ( 107, 19 ) / ( 107, 19 ) }
       DATA {
       (0,0): 3511.02, 0.0444457, 1913, -5.80215e-25, 4.04167e-24,
       (0,5): 4.36491e-21, -2.24534e-20, -1.30633e-17, 5.08111e-17,
       (0,9): 1.9793e-14, -6.17834e-14, -1.59345e-11, 4.54526e-11, 6.4933e-09,
@@ -60386,25 +60943,511 @@
             STRSIZE H5T_VARIABLE;
             STRPAD H5T_STR_NULLTERM;
             CSET H5T_CSET_UTF8;
             CTYPE H5T_C_S1;
          }
          DATASPACE  SCALAR
          DATA {
-         (0): "G5"
+         (0): "G5V"
          }
       }
       ATTRIBUTE "V" {
          DATATYPE  H5T_IEEE_F32LE
          DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
          DATA {
          (0): 12.02
          }
       }
    }
+   DATASET "Sirius" {
+      DATATYPE  H5T_IEEE_F32LE
+      DATASPACE  SIMPLE { ( 107, 19 ) / ( 107, 19 ) }
+      DATA {
+      (0,0): 3545.05, 0.0455988, 1651, -1.94848e-19, -6.47531e-18,
+      (0,5): 9.22412e-16, 3.23853e-14, -1.59083e-12, -6.55983e-11,
+      (0,9): 1.06092e-09, 6.99698e-08, 5.12042e-08, -4.32172e-05,
+      (0,13): -0.000370061, 0.0163978, 0.13016, -4.24224, -9.16326, 794.499,
+      (1,0): 3567.33, 0.0458901, 1651, 1.96469e-19, 3.37073e-18,
+      (1,5): -1.09723e-15, -1.89569e-14, 2.48751e-12, 4.23612e-11,
+      (1,9): -2.94599e-09, -4.73002e-08, 1.94294e-06, 2.62647e-05,
+      (1,13): -0.000688559, -0.00466451, 0.107248, -1.94208, -1.84021,
+      (1,18): 903.873,
+      (2,0): 3589.9, 0.046185, 1651, 4.76541e-19, 1.79354e-18, -2.72554e-15,
+      (2,6): -9.21261e-15, 6.41606e-12, 1.90055e-11, -8.02753e-09,
+      (2,10): -1.8811e-08, 5.71949e-06, 6.82165e-06, -0.00226358, 0.00307567,
+      (2,15): 0.424898, -3.83728, -21.0823, 1202.25,
+      (3,0): 3612.74, 0.0464836, 1651, -4.04875e-19, -6.80846e-18,
+      (3,5): 2.06904e-15, 2.10212e-14, -4.40643e-12, -1.13279e-11,
+      (3,9): 5.08655e-09, -2.41691e-08, -3.4226e-06, 3.32156e-05, 0.00132526,
+      (3,14): -0.0118166, -0.273798, -1.42618, 25.9552, 1317.47,
+      (4,0): 3635.89, 0.046786, 1651, -9.38685e-19, -3.12348e-17,
+      (4,5): 4.76911e-15, 1.5976e-13, -9.41793e-12, -3.22166e-10,
+      (4,9): 9.06848e-09, 3.25888e-07, -4.38063e-06, -0.000176103,
+      (4,13): 0.00100606, 0.0527184, -0.117767, -10.5548, 15.3021, 1838.57,
+      (5,0): 3659.33, 0.0470922, 1651, 5.03647e-19, 4.79805e-18,
+      (5,5): -2.99289e-15, -2.5363e-14, 7.22053e-12, 5.42291e-11,
+      (5,9): -9.06256e-09, -5.92487e-08, 6.28771e-06, 3.25476e-05,
+      (5,13): -0.00234376, -0.00434776, 0.404269, -4.63305, -17.6144,
+      (5,18): 2060.89,
+      (6,0): 3683.08, 0.0474023, 1651, 2.55374e-20, 6.52202e-18,
+      (6,5): -1.63842e-16, -3.50351e-14, 4.73989e-13, 7.36509e-11,
+      (6,9): -8.18393e-10, -7.51696e-08, 8.89632e-07, 3.49778e-05,
+      (6,13): -0.000563876, -0.000738925, 0.17046, -6.608, -13.9943, 2449.25,
+      (7,0): 3707.13, 0.0477164, 1651, 2.03132e-19, 1.48285e-17,
+      (7,5): -9.05677e-16, -7.75715e-14, 1.4595e-12, 1.57973e-10,
+      (7,9): -1.01968e-09, -1.5587e-07, 3.48958e-07, 7.24035e-05,
+      (7,13): -0.000166365, -0.00730014, 0.0896548, -7.36575, -10.9107,
+      (7,18): 2935.02,
+      (8,0): 3731.51, 0.0480345, 1651, 4.26379e-18, 4.95382e-17,
+      (8,5): -2.53212e-14, -2.72592e-13, 6.03938e-11, 6.00864e-10,
+      (8,9): -7.36978e-08, -6.74192e-07, 4.84093e-05, 0.000399745, -0.016399,
+      (8,14): -0.111566, 2.44343, 5.18116, -96.7883, 3109.47,
+      (9,0): 3756.2, 0.0483568, 1651, -4.99192e-18, -3.58819e-17,
+      (9,5): 3.18349e-14, 1.92522e-13, -8.26279e-11, -4.12279e-10,
+      (9,9): 1.11703e-07, 4.52555e-07, -8.33324e-05, -0.000275157, 0.0332575,
+      (9,14): 0.0976801, -6.21678, -23.8652, 375.062, 4593.71,
+      (10,0): 3781.23, 0.0486832, 1651, 6.01981e-19, -4.05187e-17,
+      (10,5): -2.6429e-15, 2.71635e-13, 2.57982e-12, -7.36447e-10,
+      (10,9): 4.58127e-09, 1.03342e-06, -1.20043e-05, -0.000797196,
+      (10,13): 0.00987608, 0.333298, -3.35485, -72.7345, 362.883, 8750.8,
+      (11,0): 3806.59, 0.049014, 1651, -9.66312e-19, -7.51809e-17,
+      (11,5): 6.30243e-15, 4.44822e-13, -1.77211e-11, -1.0451e-09,
+      (11,9): 2.82002e-08, 1.23379e-06, -2.75986e-05, -0.000763141, 0.016476,
+      (11,14): 0.240884, -5.39946, -44.9765, 706.039, 9180.34,
+      (12,0): 3832.3, 0.0493492, 1651, 4.00539e-18, 7.03338e-17,
+      (12,5): -2.62055e-14, -4.26556e-13, 7.00406e-11, 1.053e-09,
+      (12,9): -9.82672e-08, -1.36277e-06, 7.73491e-05, 0.000987365,
+      (12,13): -0.0337737, -0.383788, 7.50488, 56.6893, -650.983, 5961.1,
+      (13,0): 3858.36, 0.0496889, 1651, 8.10771e-20, 1.83122e-17,
+      (13,5): -6.39347e-16, -1.22441e-13, 2.26698e-12, 3.26846e-10,
+      (13,9): -4.47024e-09, -4.33367e-07, 4.94335e-06, 0.000274874,
+      (13,13): -0.00272364, -0.0394397, 0.442602, -41.2827, 93.455, 16837.6,
+      (14,0): 3884.77, 0.0500332, 1651, 4.17345e-18, 4.83286e-17,
+      (14,5): -2.83978e-14, -3.01014e-13, 7.90078e-11, 7.66666e-10,
+      (14,9): -1.15581e-07, -1.03193e-06, 9.51495e-05, 0.000787874,
+      (14,13): -0.0436994, -0.327485, 10.36, 49.4104, -1017.51, 9004.34,
+      (15,0): 3911.55, 0.0503821, 1651, -8.97212e-20, -5.73542e-18,
+      (15,5): -7.14731e-17, 1.55192e-14, 2.40772e-12, 1.46018e-11,
+      (15,9): -7.27983e-09, -7.74539e-08, 9.36779e-06, 5.61311e-05,
+      (15,13): -0.00546537, 0.0367031, 0.936254, -61.344, 195.413, 22678.7,
+      (16,0): 3938.7, 0.0507358, 1651, -2.37942e-18, -2.02711e-17,
+      (16,5): 1.60021e-14, 1.08371e-13, -4.35067e-11, -2.17842e-10,
+      (16,9): 6.12566e-08, 2.01999e-07, -4.75929e-05, -9.46286e-05, 0.020126,
+      (16,14): 0.0542236, -4.16729, -56.1991, 237.743, 25473.3,
+      (17,0): 3966.23, 0.0510944, 1651, 4.41596e-18, 7.20564e-17,
+      (17,5): -3.10998e-14, -4.62952e-13, 8.9597e-11, 1.20609e-09,
+      (17,9): -1.35719e-07, -1.641e-06, 0.00011551, 0.00125001, -0.0545598,
+      (17,14): -0.517337, 13.1307, 83.2528, -1285.49, 11606.4,
+      (18,0): 3994.15, 0.0514579, 1651, -5.8132e-19, -6.80772e-18,
+      (18,5): 3.92631e-15, 3.22935e-14, -1.03474e-11, -5.1868e-11,
+      (18,9): 1.30215e-08, 3.72121e-08, -7.32405e-06, -4.43675e-05,
+      (18,13): 0.000975787, 0.0889232, 0.10889, -85.0228, 221.515, 31428.6,
+      (19,0): 4022.46, 0.0518266, 1651, 6.98593e-19, 6.07474e-18,
+      (19,5): -5.16331e-15, -4.08686e-14, 1.55994e-11, 1.10003e-10,
+      (19,9): -2.46736e-08, -1.46661e-07, 2.16096e-05, 8.57545e-05,
+      (19,13): -0.0100411, 0.0202659, 2.06727, -67.9701, -113.208, 36181.4,
+      (20,0): 4051.18, 0.0522004, 1651, -5.15557e-20, 1.02026e-17,
+      (20,5): 5.39548e-16, -7.14436e-14, -2.04357e-12, 1.99533e-10,
+      (20,9): 3.75249e-09, -2.77836e-07, -3.66532e-06, 0.000185183,
+      (20,13): 0.00197977, -0.0147895, -0.583532, -65.573, 41.1832, 37985.8,
+      (21,0): 4080.32, 0.0525796, 1651, 1.23173e-18, 3.84552e-17,
+      (21,5): -8.30753e-15, -2.59383e-13, 2.18608e-11, 6.87839e-10,
+      (21,9): -2.77536e-08, -8.88693e-07, 1.65301e-05, 0.000536278,
+      (21,13): -0.00332913, -0.0678326, 0.0912672, -80.4776, -362.056,
+      (21,18): 37408.9,
+      (22,0): 4109.87, 0.0529641, 1651, -1.76106e-18, -5.44527e-17,
+      (22,5): 1.36035e-14, 3.63025e-13, -4.38081e-11, -9.54821e-10,
+      (22,9): 7.61745e-08, 1.24572e-06, -7.73028e-05, -0.000823129,
+      (22,13): 0.0460208, 0.251403, -15.0821, -48.6296, 2132.44, 25380.3,
+      (23,0): 4139.86, 0.0533542, 1651, 3.15905e-19, -9.24126e-18,
+      (23,5): -2.36239e-15, 6.73799e-14, 7.00871e-12, -1.96739e-10,
+      (23,9): -1.03887e-08, 2.95008e-07, 7.82872e-06, -0.000251394,
+      (23,13): -0.00247685, 0.153125, -0.119434, -100.728, 215.477, 46330.7,
+      (24,0): 4170.29, 0.05375, 1651, 4.24526e-19, -4.20993e-18,
+      (24,5): -3.27334e-15, 3.25564e-14, 1.0268e-11, -9.94629e-11,
+      (24,9): -1.68298e-08, 1.55555e-07, 1.53417e-05, -0.000144186,
+      (24,13): -0.00753177, 0.111683, 1.6908, -97.2324, -121.153, 51417,
+      (25,0): 4201.17, 0.0541515, 1651, 3.49056e-19, 2.085e-17, -2.33298e-15,
+      (25,6): -1.48522e-13, 6.09669e-12, 4.22245e-10, -7.81796e-09,
+      (25,10): -6.04973e-07, 4.96566e-06, 0.000440285, -0.0011819, -0.107848,
+      (25,15): -0.220645, -69.5837, 105.003, 54712.3,
+      (26,0): 4232.51, 0.054559, 1651, 2.38969e-19, 1.02676e-17, -1.7722e-15,
+      (26,6): -7.31169e-14, 5.29628e-12, 2.07105e-10, -8.12217e-09,
+      (26,10): -2.93653e-07, 6.67125e-06, 0.000203743, -0.00266195,
+      (26,14): -0.0213662, 0.278456, -82.122, 37.5166, 57130.7,
+      (27,0): 4264.32, 0.0549725, 1651, -5.54798e-20, -1.39111e-17,
+      (27,5): 2.09898e-16, 1.01823e-13, 9.61111e-14, -2.9708e-10,
+      (27,9): -1.5036e-09, 4.4135e-07, 2.62732e-06, -0.000363312,
+      (27,13): -0.00176576, 0.198696, 0.328351, -120.342, 23.0188, 61574.9,
+      (28,0): 4296.61, 0.0553922, 1651, -4.06346e-20, 4.71577e-18,
+      (28,5): 3.52503e-16, -3.69942e-14, -1.13078e-12, 1.16074e-10,
+      (28,9): 1.60276e-09, -1.82571e-07, -8.298e-07, 0.000136306,
+      (28,13): -0.000101835, 0.000640941, 0.152708, -92.7403, -88.1847,
+      (28,18): 63870.5,
+      (29,0): 4329.4, 0.0558183, 1651, -1.18433e-18, -6.5081e-17,
+      (29,5): 8.55624e-15, 4.97254e-13, -2.37029e-11, -1.52151e-09,
+      (29,9): 2.9998e-08, 2.37105e-06, -1.31847e-05, -0.00197267,
+      (29,13): -0.00660027, 0.843328, 8.33885, -191.046, -2288.55, 48913.1,
+      (30,0): 4362.69, 0.0562508, 1651, -1.57802e-19, 1.85332e-17,
+      (30,5): 1.05166e-15, -1.51264e-13, -2.11289e-12, 4.82646e-10,
+      (30,9): -1.88885e-10, -7.4397e-07, 5.58107e-06, 0.000526802,
+      (30,13): -0.00602688, -0.0682656, 1.09603, -118.942, 781.385, 65097.4,
+      (31,0): 4396.5, 0.05669, 1651, 2.91787e-19, 7.74083e-19, -2.38365e-15,
+      (31,6): -3.78099e-15, 7.73959e-12, 4.13379e-12, -1.26298e-08,
+      (31,10): 9.26255e-09, 1.06822e-05, -3.82293e-05, -0.00412102,
+      (31,14): 0.0808362, 0.223579, -114.769, 186.796, 75367.5,
+      (32,0): 4430.84, 0.0571359, 1651, 6.76529e-20, 4.35502e-18,
+      (32,5): -4.83403e-16, -3.15705e-14, 1.29082e-12, 8.72558e-11,
+      (32,9): -1.45086e-09, -1.09824e-07, 2.04029e-07, 4.29111e-05,
+      (32,13): 0.00108206, 0.0604424, -1.05672, -117.283, 318.391, 79157.5,
+      (33,0): 4465.72, 0.0575888, 1651, -1.64967e-19, 4.31937e-18,
+      (33,5): 1.53978e-15, -3.36026e-14, -5.74619e-12, 1.00721e-10,
+      (33,9): 1.09371e-08, -1.41073e-07, -1.12038e-05, 7.44566e-05,
+      (33,13): 0.00602175, 0.048539, -1.60219, -120.424, 171.541, 85075.5,
+      (34,0): 4501.15, 0.0580488, 1651, 8.8458e-20, 1.12933e-17,
+      (34,5): -6.75524e-16, -9.06113e-14, 2.09215e-12, 2.86285e-10,
+      (34,9): -3.36503e-09, -4.45792e-07, 2.86099e-06, 0.000336428,
+      (34,13): -0.000850892, -0.0596811, -0.530841, -106.176, 345.731,
+      (34,18): 87407.9,
+      (35,0): 4537.15, 0.0585162, 1651, -2.83523e-19, 5.195e-19, 2.6408e-15,
+      (35,6): -3.98277e-15, -9.96041e-12, 8.99194e-12, 1.94921e-08,
+      (35,10): 2.31249e-09, -2.10769e-05, -4.39624e-05, 0.0124642, 0.0985079,
+      (35,15): -3.81774, -134.607, 494.123, 93847,
+      (36,0): 4573.73, 0.0589909, 1651, -1.11134e-19, -6.10203e-19,
+      (36,5): 8.72274e-16, 3.54704e-15, -2.51368e-12, -8.33841e-12,
+      (36,9): 2.98105e-09, 1.62706e-08, -6.03063e-07, -4.14418e-05,
+      (36,13): -0.0013125, 0.0912139, 0.539009, -135.153, 94.8826, 98405.1,
+      (37,0): 4610.91, 0.0594734, 1651, 8.21423e-20, 8.93126e-21,
+      (37,5): -8.54822e-16, -2.01352e-15, 3.60963e-12, 1.42527e-11,
+      (37,9): -7.90569e-09, -3.59071e-08, 9.45388e-06, 2.71786e-05,
+      (37,13): -0.0057862, 0.0459476, 1.28984, -126.901, 69.9456, 103164,
+      (38,0): 4648.69, 0.0599636, 1651, 8.89313e-20, -1.02182e-18,
+      (38,5): -8.50135e-16, 9.96401e-15, 3.27629e-12, -3.8519e-11,
+      (38,9): -6.45617e-09, 7.74272e-08, 6.7145e-06, -9.7012e-05,
+      (38,13): -0.00318621, 0.111089, 0.0955009, -142.4, 275.442, 108656,
+      (39,0): 4687.1, 0.0604619, 1651, -5.24858e-20, 1.22629e-18,
+      (39,5): 4.74377e-16, -1.19006e-14, -1.68661e-12, 4.52248e-11,
+      (39,9): 3.02651e-09, -8.25021e-08, -3.04756e-06, 6.11475e-05,
+      (39,13): 0.00209099, 0.0363066, -1.26743, -131.991, 403.272, 113319,
+      (40,0): 4726.15, 0.0609684, 1651, -5.93692e-20, -6.17767e-19,
+      (40,5): 5.23998e-16, 3.97118e-15, -1.80013e-12, -7.87231e-12,
+      (40,9): 3.03158e-09, 3.00252e-09, -2.66454e-06, -3.05674e-06,
+      (40,13): 0.00146364, 0.050103, -0.880171, -127.459, 329.208, 114819,
+      (41,0): 4765.86, 0.0614834, 1651, 1.56571e-20, -5.77468e-19,
+      (41,5): -1.97834e-16, 4.29887e-15, 9.89208e-13, -1.09777e-11,
+      (41,9): -2.48794e-09, 1.01522e-08, 3.23688e-06, -7.51612e-06,
+      (41,13): -0.0018334, 0.0473243, -0.0368877, -125.997, 263.314, 118662,
+      (42,0): 4806.24, 0.062007, 1651, -2.6816e-20, 1.84896e-18, 2.81488e-16,
+      (42,6): -1.79727e-14, -1.18395e-12, 6.92972e-11, 2.59949e-09,
+      (42,10): -1.32446e-07, -3.33463e-06, 0.000119622, 0.00279651,
+      (42,14): -0.00190478, -1.64409, -123.758, 411.993, 121714,
+      (43,0): 4847.31, 0.0625395, 1651, -6.74327e-19, -2.28225e-17,
+      (43,5): 6.59484e-15, 2.19487e-13, -2.56726e-11, -8.50432e-10,
+      (43,9): 5.00755e-08, 1.69459e-06, -4.96338e-05, -0.00183115, 0.0203507,
+      (43,14): 1.03981, 1.3339, -313.25, -2506.69, 100502,
+      (44,0): 4889.08, 0.0630811, 1651, -2.70048e-19, -1.50353e-18,
+      (44,5): 2.74106e-15, 5.75524e-15, -1.10333e-11, 1.67109e-11,
+      (44,9): 2.21255e-08, -1.13321e-07, -2.25733e-05, 0.000179073, 0.010689,
+      (44,14): -0.0446378, -2.65873, -128.973, 1321.7, 116447,
+      (45,0): 4931.59, 0.063632, 1651, -3.19527e-20, -1.49972e-18,
+      (45,5): 3.1804e-16, 1.35176e-14, -1.30031e-12, -4.73186e-11,
+      (45,9): 2.89055e-09, 8.18478e-08, -3.98638e-06, -8.06668e-05,
+      (45,13): 0.00375387, 0.0812882, -2.43316, -133.512, 800.108, 131228,
+      (46,0): 4974.84, 0.0641926, 1651, 3.06692e-22, -1.90191e-18,
+      (46,5): -1.13602e-16, 1.77453e-14, 1.01944e-12, -6.53115e-11,
+      (46,9): -3.54817e-09, 1.21415e-07, 5.84875e-06, -0.000128018,
+      (46,13): -0.00433062, 0.110909, 0.752098, -143.288, 346.546, 136819,
+      (47,0): 5018.86, 0.064763, 1651, 3.30225e-20, 2.05273e-18, -3.1755e-16,
+      (47,6): -1.98332e-14, 1.20351e-12, 7.60531e-11, -2.22292e-09,
+      (47,10): -1.46427e-07, 1.84462e-06, 0.000141657, 1.38432e-05,
+      (47,14): -0.0305108, -1.1586, -106.916, 601.148, 135055,
+      (48,0): 5063.66, 0.0653435, 1651, -6.79766e-20, -1.53291e-18,
+      (48,5): 7.12127e-16, 1.44659e-14, -2.95216e-12, -5.32767e-11,
+      (48,9): 6.13874e-09, 9.70176e-08, -6.75776e-06, -9.63251e-05,
+      (48,13): 0.00405586, 0.0815567, -1.71614, -125.695, 608.493, 136425,
+      (49,0): 5109.27, 0.0659344, 1651, -2.87997e-20, -9.93819e-19,
+      (49,5): 3.00625e-16, 9.78142e-15, -1.25689e-12, -3.77872e-11,
+      (49,9): 2.7177e-09, 7.30067e-08, -3.36352e-06, -7.96164e-05,
+      (49,13): 0.00270602, 0.0783208, -1.73051, -126.746, 680.089, 139123,
+      (50,0): 5155.71, 0.066536, 1651, -1.11599e-19, -3.62112e-18,
+      (50,5): 1.22004e-15, 3.73678e-14, -5.32961e-12, -1.53031e-10,
+      (50,9): 1.18411e-08, 3.16379e-07, -1.41159e-05, -0.00035122,
+      (50,13): 0.00888863, 0.22812, -3.00646, -157.176, 639.718, 140071,
+      (51,0): 5203, 0.0671485, 1651, 2.04422e-20, -1.28036e-18, -2.58142e-16,
+      (51,6): 1.29987e-14, 1.27548e-12, -5.06065e-11, -3.09535e-09,
+      (51,10): 9.39706e-08, 3.69151e-06, -8.77316e-05, -0.0015679, 0.0643965,
+      (51,15): -0.680193, -109.169, 672.865, 133267,
+      (52,0): 5251.17, 0.0677723, 1651, 1.55832e-20, 1.74498e-19,
+      (52,5): -1.99386e-16, -1.73397e-15, 1.02655e-12, 6.01129e-12,
+      (52,9): -2.68713e-09, -6.32564e-09, 3.6601e-06, -1.22174e-05,
+      (52,13): -0.00217081, 0.0534263, -0.138425, -114.034, 562.868, 133346,
+      (53,0): 5300.24, 0.0684077, 1651, -1.56794e-20, -5.068e-20,
+      (53,5): 1.82809e-16, 2.05168e-16, -8.40735e-13, 7.6368e-13, 1.9281e-09,
+      (53,10): -5.04301e-09, -2.32588e-06, 4.89776e-06, 0.00159838,
+      (53,14): 0.0238779, -1.05309, -93.301, 679.918, 125876,
+      (54,0): 5350.23, 0.0690551, 1651, -1.67516e-20, -8.23053e-19,
+      (54,5): 1.98483e-16, 9.07256e-15, -9.51549e-13, -3.95039e-11,
+      (54,9): 2.37657e-09, 8.64345e-08, -3.36057e-06, -0.000102798,
+      (54,13): 0.00289633, 0.0842882, -1.87585, -105.932, 927.265, 129398,
+      (55,0): 5401.18, 0.0697147, 1651, 1.10274e-20, 2.71547e-19,
+      (55,5): -1.36863e-16, -3.58534e-15, 6.7807e-13, 1.92921e-11,
+      (55,9): -1.68947e-09, -5.3545e-08, 2.13453e-06, 7.73683e-05,
+      (55,13): -0.000988831, -0.0364447, -0.610534, -69.9284, 800.139,
+      (55,18): 129123,
+      (56,0): 5453.11, 0.0703868, 1651, -4.49895e-21, 1.13366e-19,
+      (56,5): 5.2033e-17, -1.94687e-15, -2.35861e-13, 1.25397e-11,
+      (56,9): 5.44039e-10, -3.91489e-08, -7.62728e-07, 6.01542e-05,
+      (56,13): 0.000947594, -0.0254874, -1.24707, -73.1132, 933.579, 132597,
+      (57,0): 5506.04, 0.071072, 1651, 8.77256e-21, 7.36762e-19,
+      (57,5): -1.07917e-16, -9.42066e-15, 5.28463e-13, 4.83339e-11,
+      (57,9): -1.28628e-09, -1.26357e-07, 1.5075e-06, 0.000173783,
+      (57,13): -0.000377915, -0.101007, -1.01846, -52.9233, 989.721, 136299,
+      (58,0): 5560.01, 0.0717706, 1651, 5.21403e-21, 4.3417e-19,
+      (58,5): -7.01992e-17, -5.74616e-15, 3.87362e-13, 3.04821e-11,
+      (58,9): -1.10932e-09, -8.21772e-08, 1.66462e-06, 0.000115445,
+      (58,13): -0.000955709, -0.0626177, -0.598159, -63.0971, 931.114,
+      (58,18): 140458,
+      (59,0): 5615.06, 0.0724829, 1651, 1.17465e-20, 4.9535e-19,
+      (59,5): -1.62088e-16, -6.55859e-15, 9.07462e-13, 3.48712e-11,
+      (59,9): -2.62007e-09, -9.46777e-08, 4.04386e-06, 0.000135691,
+      (59,13): -0.00293606, -0.0811518, 0.205407, -54.0425, 793.211, 139492,
+      (60,0): 5671.2, 0.0732094, 1651, 1.41505e-21, 4.30208e-20,
+      (60,5): -2.31245e-17, -8.26868e-16, 1.50492e-13, 5.95594e-12,
+      (60,9): -4.86668e-10, -2.08834e-08, 7.58462e-07, 3.60316e-05,
+      (60,13): -0.000280529, -0.0142924, -0.72709, -72.0921, 820.528, 144482,
+      (61,0): 5728.48, 0.0739504, 1651, -8.12638e-22, 1.17417e-19,
+      (61,5): 1.09734e-17, -1.8624e-15, -6.25109e-14, 1.17932e-11,
+      (61,9): 2.11755e-10, -3.78813e-08, -5.21894e-07, 6.3096e-05,
+      (61,13): 0.00099539, -0.0380396, -1.33399, -58.6093, 934.639, 138892,
+      (62,0): 5786.92, 0.0747066, 1651, 8.655e-21, 4.45594e-19, -1.21873e-16,
+      (62,6): -6.19017e-15, 6.90181e-13, 3.45288e-11, -1.99408e-09,
+      (62,10): -9.84977e-08, 3.03241e-06, 0.000149923, -0.00207592,
+      (62,14): -0.104862, -0.113946, -28.0265, 886.508, 127413,
+      (63,0): 5846.57, 0.0754783, 1651, 6.4063e-21, 4.66876e-19,
+      (63,5): -8.47324e-17, -6.59654e-15, 4.44024e-13, 3.74405e-11,
+      (63,9): -1.16357e-09, -1.08897e-07, 1.53794e-06, 0.000169963,
+      (63,13): -0.000699651, -0.12477, -0.695914, -21.5152, 991.935, 132279,
+      (64,0): 5907.47, 0.0762659, 1651, 5.39063e-22, -2.35758e-19,
+      (64,5): -7.99752e-18, 3.09168e-15, 3.89907e-14, -1.57683e-11,
+      (64,9): -3.65596e-11, 3.9127e-08, -3.01742e-07, -4.87478e-05,
+      (64,13): 0.00115981, 0.0375703, -1.80667, -69.6181, 1289.53, 135812,
+      (65,0): 5969.64, 0.0770701, 1651, 4.81308e-21, 1.85416e-19,
+      (65,5): -7.03149e-17, -2.82745e-15, 4.10844e-13, 1.73326e-11,
+      (65,9): -1.21173e-09, -5.44094e-08, 1.82956e-06, 9.12342e-05,
+      (65,13): -0.00108473, -0.069066, -0.526029, -30.6164, 1037.09, 126786,
+      (66,0): 6033.14, 0.0778913, 1651, 6.09101e-21, 1.83475e-19,
+      (66,5): -9.2082e-17, -2.87449e-15, 5.58601e-13, 1.81864e-11,
+      (66,9): -1.72562e-09, -5.92181e-08, 2.80587e-06, 0.000103585,
+      (66,13): -0.00207895, -0.0839201, -0.0377097, -23.7397, 965.246,
+      (66,18): 128882,
+      (67,0): 6098.01, 0.0787302, 1651, 7.03874e-21, 3.45023e-19,
+      (67,5): -1.06433e-16, -5.26368e-15, 6.44886e-13, 3.22456e-11,
+      (67,9): -1.98804e-09, -1.01064e-07, 3.23092e-06, 0.000169695,
+      (67,13): -0.00242947, -0.137008, 0.0804724, -5.17216, 973.143, 129513,
+      (68,0): 6164.28, 0.0795872, 1651, 4.5907e-21, 2.00584e-19,
+      (68,5): -7.07431e-17, -3.20749e-15, 4.34453e-13, 2.06823e-11,
+      (68,9): -1.34215e-09, -6.86242e-08, 2.12354e-06, 0.000122922,
+      (68,13): -0.00137556, -0.106141, -0.429387, -9.82151, 1079.91, 129719,
+      (69,0): 6232.02, 0.0804629, 1651, 3.80791e-21, 1.84513e-19,
+      (69,5): -5.73315e-17, -2.82876e-15, 3.44596e-13, 1.74427e-11,
+      (69,9): -1.05434e-09, -5.55334e-08, 1.71179e-06, 9.68599e-05,
+      (69,13): -0.00126927, -0.0830409, -0.171432, -15.3547, 920.449, 129012,
+      (70,0): 6301.25, 0.0813581, 1651, 4.30569e-21, 1.75159e-19,
+      (70,5): -6.94737e-17, -2.72334e-15, 4.50728e-13, 1.68521e-11,
+      (70,9): -1.49383e-09, -5.28635e-08, 2.61487e-06, 8.81693e-05,
+      (70,13): -0.002088, -0.0687202, -0.0228509, -22.1673, 1056.81, 128005,
+      (71,0): 6372.04, 0.0822733, 1651, 7.51211e-22, 1.0451e-19,
+      (71,5): -1.12004e-17, -1.77778e-15, 6.50756e-14, 1.21135e-11,
+      (71,9): -1.77882e-10, -4.20355e-08, 1.7184e-07, 7.73558e-05,
+      (71,13): 0.000277363, -0.0647137, -1.02808, -25.4696, 1170.82, 137073,
+      (72,0): 6444.45, 0.0832092, 1651, 2.75481e-21, 1.30429e-19,
+      (72,5): -4.64739e-17, -2.27091e-15, 3.13252e-13, 1.58932e-11,
+      (72,9): -1.06921e-09, -5.70156e-08, 1.9062e-06, 0.000110063,
+      (72,13): -0.00152612, -0.103372, -0.0823385, -2.88197, 960.273, 133316,
+      (73,0): 6518.51, 0.0841666, 1651, -2.58918e-21, -1.26087e-19,
+      (73,5): 4.41941e-17, 2.00523e-15, -2.90537e-13, -1.18757e-11,
+      (73,9): 9.17513e-10, 3.05626e-08, -1.4542e-06, -2.56282e-05,
+      (73,13): 0.00135029, -0.00970933, -1.3546, -29.2948, 933.097, 126274,
+      (74,0): 6594.3, 0.0851461, 1651, -1.16691e-21, 2.15483e-19,
+      (74,5): 1.97526e-17, -3.96623e-15, -1.14014e-13, 2.87093e-11,
+      (74,9): 1.92826e-10, -1.02281e-07, 4.74074e-07, 0.000180235,
+      (74,13): -0.00193784, -0.124701, 1.27298, -35.6274, 1237.04, 133256,
+      (75,0): 6671.87, 0.0861487, 1651, 1.38297e-21, 8.43028e-20,
+      (75,5): -2.43779e-17, -1.5801e-15, 1.70322e-13, 1.193e-11,
+      (75,9): -5.93148e-10, -4.63418e-08, 1.03615e-06, 9.75588e-05,
+      (75,13): -0.000669087, -0.10236, -0.500793, 8.82663, 1115.57, 127092,
+      (76,0): 6751.29, 0.0871751, 1651, 5.60968e-22, -4.12184e-21,
+      (76,5): -9.49874e-18, 4.16462e-17, 6.1341e-14, 4.9467e-15,
+      (76,9): -1.81445e-10, -1.50962e-09, 1.95256e-07, 6.67133e-06,
+      (76,13): 0.000204188, -0.00660366, -0.859527, -37.1528, 1119.08,
+      (76,18): 138689,
+      (77,0): 6832.62, 0.0882261, 1651, 3.05894e-21, -1.89206e-20,
+      (77,5): -6.89396e-17, 8.00199e-18, 6.19543e-13, 3.14037e-12,
+      (77,9): -2.81955e-09, -2.67728e-08, 6.76454e-06, 8.91359e-05,
+      (77,13): -0.00790014, -0.122871, 3.14841, 19.4514, 561.023, 127866,
+      (78,0): 6915.94, 0.0893027, 1651, 1.44101e-21, -1.00883e-19,
+      (78,5): -2.69554e-17, 1.91022e-15, 1.91798e-13, -1.40624e-11,
+      (78,9): -6.30437e-10, 5.0432e-08, 8.60567e-07, -9.05542e-05,
+      (78,13): 1.93603e-05, 0.0798114, -1.25451, -63.8123, 1507.05, 127561,
+      (79,0): 7001.31, 0.0904058, 1651, 2.31551e-22, -1.12767e-20,
+      (79,5): -4.46094e-18, 1.99924e-16, 3.32236e-14, -1.3437e-12,
+      (79,9): -1.1643e-10, 4.14341e-09, 1.66235e-07, -5.48892e-06,
+      (79,13): 8.04417e-05, 0.00521506, -0.627512, -36.4741, 954.958, 130917,
+      (80,0): 7088.82, 0.0915364, 1651, 4.47837e-22, 1.1163e-20, -9.2187e-18,
+      (80,6): -2.42013e-16, 7.6175e-14, 2.09735e-12, -3.21234e-10,
+      (80,10): -9.18902e-09, 7.16326e-07, 2.08807e-05, -0.000730966,
+      (80,14): -0.0189978, -0.0509157, -27.2591, 820.937, 126131,
+      (81,0): 7178.54, 0.0926956, 1651, -2.07669e-22, -3.26762e-21,
+      (81,5): 4.7841e-18, 4.40178e-17, -4.47174e-14, -1.83952e-13,
+      (81,9): 2.13106e-10, -4.27697e-11, -5.30144e-07, 2.8287e-06,
+      (81,13): 0.000628651, -0.00766724, -0.372356, -14.4708, 488.315,
+      (81,18): 106275,
+      (82,0): 7270.56, 0.0938844, 1651, 2.58116e-22, 1.09082e-20,
+      (82,5): -5.99165e-18, -2.55955e-16, 5.69091e-14, 2.36539e-12,
+      (82,9): -2.82779e-10, -1.08369e-08, 7.69097e-07, 2.51597e-05,
+      (82,13): -0.0010423, -0.0244155, 0.343755, -17.169, 633.024, 106004,
+      (83,0): 7364.98, 0.0951041, 1651, 1.53184e-22, 3.58553e-21,
+      (83,5): -3.21518e-18, -8.15636e-17, 2.62e-14, 7.4785e-13, -1.02095e-10,
+      (83,10): -3.52542e-09, 1.7813e-07, 8.85301e-06, -3.1645e-05,
+      (83,14): -0.00873296, -0.385343, -21.456, 732.731, 106779,
+      (84,0): 7461.88, 0.0963558, 1651, 3.77539e-23, -2.15874e-21,
+      (84,5): -5.9481e-19, 5.58205e-17, 2.8773e-15, -5.66725e-13,
+      (84,9): -1.56467e-12, 2.8364e-09, -2.42459e-08, -7.19716e-06,
+      (84,13): 8.37849e-05, 0.0100981, -0.251861, -26.4338, 605.941, 102333,
+      (85,0): 7561.36, 0.0976408, 1651, 9.56587e-22, -2.80908e-20,
+      (85,5): -2.76937e-17, 4.02492e-16, 3.14498e-13, -1.0217e-12,
+      (85,9): -1.78235e-09, -9.83733e-09, 5.24041e-06, 6.40468e-05,
+      (85,13): -0.00734014, -0.12109, 3.49336, 37.5408, 18.3592, 96463.4,
+      (86,0): 7663.53, 0.0989604, 1651, 4.40987e-22, 1.77914e-20,
+      (86,5): -1.19499e-17, -3.49994e-16, 1.30797e-13, 2.44039e-12,
+      (86,9): -7.30538e-10, -6.54026e-09, 2.15263e-06, 1.10345e-06,
+      (86,13): -0.00304991, 0.0225138, 1.24334, -42.7238, 1181.35, 77712.2,
+      (87,0): 7768.5, 0.100316, 1651, 2.24003e-22, 5.14748e-21, -5.67739e-18,
+      (87,6): -1.27436e-16, 5.79519e-14, 1.27232e-12, -3.04466e-10,
+      (87,10): -6.5357e-09, 8.69363e-07, 1.81211e-05, -0.00128567,
+      (87,14): -0.0244684, 0.734511, -2.10503, 271.176, 81505.5,
+      (88,0): 7876.38, 0.10171, 1651, 3.70881e-24, -1.63682e-21,
+      (88,5): -1.33697e-19, 3.4225e-17, 1.79637e-15, -2.58506e-13,
+      (88,9): -1.16278e-11, 7.77453e-10, 3.68039e-08, -2.85826e-07,
+      (88,13): -3.80339e-05, -0.00168746, -0.104092, -11.5407, 384.498,
+      (88,18): 76411.7,
+      (89,0): 7987.3, 0.103142, 1651, 4.7317e-23, -7.8669e-22, -1.28202e-18,
+      (89,6): 2.06155e-17, 1.39542e-14, -2.15841e-13, -7.75465e-11,
+      (89,10): 1.133e-09, 2.28637e-07, -3.06202e-06, -0.00032049, 0.00473711,
+      (89,15): 0.0668253, -15.2629, 355.358, 71239.7,
+      (90,0): 8101.4, 0.104615, 1651, 1.40848e-23, 1.44842e-21, -2.66571e-19,
+      (90,6): -3.53506e-17, 1.55289e-15, 3.43012e-13, -3.47594e-13,
+      (90,10): -1.68374e-09, -2.95215e-08, 4.33626e-06, 0.000125127,
+      (90,14): -0.00439868, -0.263031, -11.1859, 345.467, 65841.7,
+      (91,0): 8218.8, 0.106132, 1651, 1.28352e-22, 8.49212e-22, -3.89303e-18,
+      (91,6): -2.03983e-17, 4.7881e-14, 1.95059e-13, -3.05652e-10,
+      (91,10): -9.7882e-10, 1.07331e-06, 2.90981e-06, -0.00200467,
+      (91,14): -0.0047526, 1.6781, -4.7136, -189.556, 54675.1,
+      (92,0): 8339.65, 0.107692, 1651, 1.74117e-24, -8.00854e-22,
+      (92,5): -3.80865e-20, 2.1037e-17, 1.19569e-16, -2.10169e-13,
+      (92,9): 3.04469e-12, 9.71328e-10, -3.33338e-08, -1.95163e-06,
+      (92,13): 0.0001436, 0.00155394, -0.327539, -8.70268, 447.017, 53659.4,
+      (93,0): 8464.11, 0.109299, 1651, -2.82621e-24, 3.44966e-22, 1.3781e-19,
+      (93,6): -1.08267e-17, -2.59771e-15, 1.31354e-13, 2.48498e-11,
+      (93,10): -7.54381e-10, -1.29813e-07, 1.92916e-06, 0.000365949,
+      (93,14): -0.000694923, -0.527683, -10.2061, 417.154, 50980.4,
+      (94,0): 8592.34, 0.110955, 1651, 3.4817e-23, 2.27632e-21, -1.0617e-18,
+      (94,6): -6.7918e-17, 1.30688e-14, 8.01484e-13, -8.38041e-11,
+      (94,10): -4.75061e-09, 3.02337e-07, 1.48687e-05, -0.000611696,
+      (94,14): -0.0233163, 0.587811, 9.03282, -10.9163, 45453,
+      (95,0): 8724.51, 0.112662, 1651, -2.62341e-23, -1.81285e-21,
+      (95,5): 8.85216e-19, 5.72671e-17, -1.21416e-14, -7.25841e-13,
+      (95,9): 8.62388e-11, 4.69796e-09, -3.31237e-07, -1.63431e-05,
+      (95,13): 0.000635639, 0.0297694, -0.444043, -30.2649, 72.1433, 49847.1,
+      (96,0): 8860.82, 0.114421, 1651, 2.13457e-23, 1.91586e-21,
+      (96,5): -6.93087e-19, -6.11562e-17, 9.09645e-15, 7.83575e-13,
+      (96,9): -6.18383e-11, -5.15359e-09, 2.31385e-07, 1.84694e-05,
+      (96,13): -0.000463029, -0.0350717, 0.413132, 26.6707, 20.2543, 34323.8,
+      (97,0): 9001.45, 0.116237, 1651, 4.89221e-24, -6.22278e-22,
+      (97,5): -2.25883e-19, 1.97591e-17, 4.13788e-15, -2.47978e-13,
+      (97,9): -3.92222e-11, 1.5314e-09, 2.07462e-07, -4.55053e-06,
+      (97,13): -0.000605544, 0.00438384, 0.867469, 1.39555, -371.622,
+      (97,18): 29642.9,
+      (98,0): 9146.62, 0.118111, 1651, -6.50895e-24, 7.38517e-23,
+      (98,5): 2.49781e-19, -3.06876e-18, -3.91971e-15, 4.81107e-14,
+      (98,9): 3.21441e-11, -3.71538e-10, -1.4524e-07, 1.56452e-06,
+      (98,13): 0.000349217, -0.00356894, -0.414124, -0.401045, 264.414,
+      (98,18): 36240.8,
+      (99,0): 9296.55, 0.120047, 1651, 3.1214e-24, -1.29021e-22,
+      (99,5): -1.03808e-19, 4.17503e-18, 1.24373e-15, -5.45863e-14,
+      (99,9): -5.78612e-12, 3.74042e-10, 6.48594e-10, -1.48543e-06,
+      (99,13): 6.69488e-05, 0.00401318, -0.125153, -10.7285, -12.1776,
+      (99,18): 32243.7,
+      (100,0): 9451.48, 0.122047, 1651, 5.21331e-24, 4.34479e-22,
+      (100,5): -1.87908e-19, -1.38031e-17, 2.7073e-15, 1.70153e-13,
+      (100,9): -1.95924e-11, -1.02887e-09, 7.17081e-08, 3.21993e-06,
+      (100,13): -0.000105116, -0.0051999, -0.0358334, 2.24527, 163.337,
+      (100,18): 17619.4,
+      (101,0): 9611.65, 0.124115, 1651, 1.51754e-24, -3.83149e-22,
+      (101,5): -6.696e-20, 1.34135e-17, 1.16128e-15, -1.79986e-13,
+      (101,9): -1.00884e-11, 1.1438e-09, 4.59054e-08, -3.38603e-06,
+      (101,13): -0.000101762, 0.00379186, 0.0715203, -2.70438, 94.4616,
+      (101,18): 18844.6,
+      (102,0): 9777.36, 0.126254, 1651, 1.46956e-24, -1.32974e-22,
+      (102,5): -6.8548e-20, 5.03843e-18, 1.29488e-15, -7.46128e-14,
+      (102,9): -1.26716e-11, 5.40192e-10, 6.78591e-08, -1.94176e-06,
+      (102,13): -0.00019059, 0.00313315, 0.232747, -3.23278, -53.6649,
+      (102,18): 16821.2,
+      (103,0): 9948.87, 0.128468, 1651, 3.89383e-25, -3.96418e-23,
+      (103,5): -1.92797e-20, 1.58605e-18, 3.88231e-16, -2.48166e-14,
+      (103,9): -4.08363e-12, 1.91183e-10, 2.38858e-08, -7.54319e-07,
+      (103,13): -7.56478e-05, 0.00151769, 0.113089, -2.64637, -64.326,
+      (103,18): 12256.4,
+      (104,0): 10126.5, 0.130761, 1651, 1.20458e-25, -2.0285e-23,
+      (104,5): -6.69685e-21, 9.25753e-19, 1.48099e-16, -1.705e-14,
+      (104,9): -1.67316e-12, 1.60195e-10, 1.02981e-08, -7.96491e-07,
+      (104,13): -3.44104e-05, 0.00198982, 0.0607401, -2.74856, -52.4199,
+      (104,18): 6934.04,
+      (105,0): 10310.6, 0.133137, 1651, -1.00369e-25, -3.09319e-24,
+      (105,5): 4.58794e-21, 1.225e-19, -8.38335e-17, -1.96817e-15,
+      (105,9): 7.7811e-13, 1.66054e-11, -3.85351e-09, -7.85719e-08,
+      (105,13): 9.79179e-06, 0.000206578, -0.0109832, -0.427922, -0.635473,
+      (105,18): 2223.82,
+      (106,0): 10501.5, 0.135602, 1651, -1.01068e-22, 1.63902e-21,
+      (106,5): 4.78168e-18, -9.57233e-17, -9.01153e-14, 2.1198e-12,
+      (106,9): 8.5542e-10, -2.27463e-08, -4.23406e-06, 0.000122508,
+      (106,13): 0.0100608, -0.299706, -8.75112, 229.822, 1724.27, -23590.3
+      }
+      ATTRIBUTE "NAME" {
+         DATATYPE  H5T_STRING {
+            STRSIZE H5T_VARIABLE;
+            STRPAD H5T_STR_NULLTERM;
+            CSET H5T_CSET_UTF8;
+            CTYPE H5T_C_S1;
+         }
+         DATASPACE  SCALAR
+         DATA {
+         (0): "Sirius"
+         }
+      }
+      ATTRIBUTE "SP_TYPE" {
+         DATATYPE  H5T_STRING {
+            STRSIZE H5T_VARIABLE;
+            STRPAD H5T_STR_NULLTERM;
+            CSET H5T_CSET_UTF8;
+            CTYPE H5T_C_S1;
+         }
+         DATASPACE  SCALAR
+         DATA {
+         (0): "A1V+DA"
+         }
+      }
+      ATTRIBUTE "V" {
+         DATATYPE  H5T_IEEE_F32LE
+         DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
+         DATA {
+         (0): -1.46
+         }
+      }
+   }
    DATASET "W Per" {
       DATATYPE  H5T_IEEE_F32LE
       DATASPACE  SIMPLE { ( 107, 19 ) / ( 107, 19 ) }
       DATA {
       (0,0): 3511.44, 0.044451, 1913, -1.1403e-25, 1.56386e-24, 6.60477e-22,
       (0,6): -4.31344e-21, -1.34855e-18, -3.42618e-18, 1.02131e-15,
       (0,10): 2.18948e-14, 1.61792e-14, -2.5002e-11, -2.78979e-10,
```

### Comparing `arcesetc-0.1/arcesetc/data/BD28_4211.0026.wfrmcpc.fits` & `arcesetc-0.3/arcesetc/data/BD28_4211.0026.wfrmcpc.fits`

 * *Files identical despite different names*

### Comparing `arcesetc-0.1/arcesetc/data/HIP107864.0003.wfrmcpc.fits` & `arcesetc-0.3/arcesetc/data/HIP107864.0003.wfrmcpc.fits`

 * *Files identical despite different names*

### Comparing `arcesetc-0.1/arcesetc/data/HR5191.0002.wfrmcpc.fits` & `arcesetc-0.3/arcesetc/data/HR5191.0002.wfrmcpc.fits`

 * *Files identical despite different names*

### Comparing `arcesetc-0.1/arcesetc/data/sptype_to_temp.json` & `arcesetc-0.3/arcesetc/data/sptype_to_temp.json`

 * *Files identical despite different names*

### Comparing `arcesetc-0.1/arcesetc/plots.py` & `arcesetc-0.3/arcesetc/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,39 +19,39 @@
 
     .. warning ::
         ``arcesetc`` doesn't know anything about saturation. Ye be warned!
 
     Parameters
     ----------
     sptype : str
-        Spectral type of the star. If
+        Spectral type of the star.
     wavelength : `~astropy.units.Quantity`
     V : float
-        V magnitude of the target
+        V magnitude of the target.
     exp_time : None or float
         If ``exp_time`` is a float, show the counts curve for that exposure
         time. Otherwise, use ``signal_to_noise`` to compute the appropriate
         exposure time.
     signal_to_noise : None or float
         If ``signal_to_noise`` is a float, compute the appropriate exposure time
         to generate the counts curve that has S/N = ``signal_to_noise`` at
         wavelength ``wavelength``. Otherwise, generate counts curve for
         exposure time ``exp_time``.
     kwargs : dict
-        All extra keyword arguments will be passed to the plot function
+        All extra keyword arguments will be passed to the plot function.
 
     Returns
     -------
     fig : `~matplotlib.pyplot.Figure`
         Matplotlib figure object.
     ax : `~matplotlib.pyplot.Axes`
-        Matplotlib axes object
+        Matplotlib axes object.
     exp_time : `~astropy.units.Quantity`
         Exposure time input, or computed to achieve S/N ratio
-        ``signal_to_noise`` at wavelength ``wavelength``
+        ``signal_to_noise`` at wavelength ``wavelength``.
 
     Examples
     --------
 
     Given an exposure time:
 
     >>> import matplotlib.pyplot as plt
@@ -110,39 +110,39 @@
 
     .. warning ::
         ``arcesetc`` doesn't know anything about saturation. Ye be warned!
 
     Parameters
     ----------
     sptype : str
-        Spectral type of the star. If
+        Spectral type of the star. 
     wavelength : `~astropy.units.Quantity`
     V : float
-        V magnitude of the target
+        V magnitude of the target.
     exp_time : None or float
         If ``exp_time`` is a float, show the S/N curve for that exposure time.
         Otherwise, use ``signal_to_noise`` to compute the appropriate exposure
         time.
     signal_to_noise : None or float
         If ``signal_to_noise`` is a float, compute the appropriate exposure time
         to generate the S/N curve that has S/N = ``signal_to_noise`` at
         wavelength ``wavelength``. Otherwise, generate S/N curve for
         exposure time ``exp_time``.
     kwargs : dict
-        All extra keyword arguments will be passed to the plot function
+        All extra keyword arguments will be passed to the plot function.
 
     Returns
     -------
     fig : `~matplotlib.pyplot.Figure`
         Matplotlib figure object.
     ax : `~matplotlib.pyplot.Axes`
-        Matplotlib axes object
+        Matplotlib axes object.
     exp_time : `~astropy.units.Quantity`
         Exposure time input, or computed to achieve S/N ratio
-        ``signal_to_noise`` at wavelength ``wavelength``
+        ``signal_to_noise`` at wavelength ``wavelength``.
 
     Examples
     --------
 
     Given an exposure time:
 
     >>> import matplotlib.pyplot as plt
```

### Comparing `arcesetc-0.1/arcesetc/tests/test_utils.py` & `arcesetc-0.3/arcesetc/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,91 +1,90 @@
 import os
 
 import astropy.units as u
 import numpy as np
 import pytest
 from astropy.io import fits
+from specutils import SpectrumCollection
 
-from .legacy_specutils import readspec
 from ..util import (reconstruct_order, closest_sptype, archive, scale_flux,
                     signal_to_noise_to_exp_time)
 
 path = os.path.dirname(__file__)
 
 
-@pytest.mark.parametrize("order", [30, 35, 41, 60, 65, 70, 75, 80, 90])
+@pytest.mark.parametrize("order,", [30, 35, 41, 60, 65, 70, 75, 80, 90])
 def test_reconstruct_order_B3V(order):
     """
     End-to-end functional test on several well-behaved orders of an early-type
     star.
     """
 
     fits_path = os.path.join(path, os.pardir, 'data',
                              'HR5191.0002.wfrmcpc.fits')
 
-    b3v = readspec.read_fits_spectrum1d(fits_path)
+    b3v = SpectrumCollection.read(fits_path)
     header = fits.getheader(fits_path)
 
     # Reconstruct the order for a star with the same V mag as the template
-
     wave, flux, sp_type, exp_time = reconstruct_order('B3V',
                                                       b3v[order].wavelength.mean(),
                                                       1.86,
                                                       exp_time=header['EXPTIME']*u.s)
 
     interp_flux = np.interp(b3v[order].wavelength, wave, flux)
-    np.testing.assert_allclose(b3v[order].flux, interp_flux, atol=500, rtol=1e-1)
+    np.testing.assert_allclose(b3v[order].flux.value, interp_flux, atol=500, rtol=1e-1)
     assert sp_type == 'B3V'
 
 
 @pytest.mark.parametrize("order", [30, 35, 41, 60, 65, 70, 75, 80, 90])
 def test_reconstruct_order_white_dwarf(order):
     """
     End-to-end functional test on several well-behaved orders of a white dwarf
     """
 
     fits_path = os.path.join(path, os.pardir, 'data',
                              'BD28_4211.0026.wfrmcpc.fits')
 
-    wd = readspec.read_fits_spectrum1d(fits_path)
+    wd = SpectrumCollection.read(fits_path)
     header = fits.getheader(fits_path)
 
     # Reconstruct the order for a star with the same V mag as the template
 
     wave, flux, sp_type, exp_time = reconstruct_order('sdO2VIIIHe5',
                                                       wd[order].wavelength.mean(),
                                                       10.58,
                                                       exp_time=header['EXPTIME']*u.s)
 
     interp_flux = np.interp(wd[order].wavelength, wave, flux)
-    np.testing.assert_allclose(wd[order].flux, interp_flux, atol=500, rtol=0.05)
+    np.testing.assert_allclose(wd[order].flux.value, interp_flux, atol=500, rtol=0.05)
     assert sp_type == 'sdO2VIIIHe5'
 
 
 @pytest.mark.parametrize("order", [30, 35, 41, 60, 65, 75, 80])
 def test_reconstruct_order_white_dwarf_2(order):
     """
     End-to-end functional test on several well-behaved orders of a white dwarf
     """
 
     fits_path = os.path.join(path, os.pardir, 'data',
                              'HIP107864.0003.wfrmcpc.fits')
 
-    wd = readspec.read_fits_spectrum1d(fits_path)
+    wd = SpectrumCollection.read(fits_path)
     header = fits.getheader(fits_path)
 
     # Reconstruct the order for a star with the same V mag as the template
 
     wave, flux, sp_type, exp_time = reconstruct_order('sdO2VIIIHe5',
                                                       wd[order].wavelength.mean(),
                                                       10.58,
                                                       exp_time=header['EXPTIME']*u.s)
 
     interp_flux = np.interp(wd[order].wavelength, wave, flux)
-    np.testing.assert_allclose(wd[order].flux, interp_flux, atol=500, rtol=0.2)
+    np.testing.assert_allclose(wd[order].flux.value, interp_flux, atol=500, rtol=0.2)
     assert sp_type == 'sdO2VIIIHe5'
 
 
 def test_closest_sptype():
     """Test the function that finds closest available sptype"""
     assert closest_sptype('G4V') == 'G5V'
     assert closest_sptype('B4V') == 'B3V'
```

### Comparing `arcesetc-0.1/arcesetc/util.py` & `arcesetc-0.3/arcesetc/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,24 +19,29 @@
 temps = np.array([sptype_to_temp[key] for key in spectral_types
                   if key in sptype_to_temp])
 
 
 def closest_sptype(sptype):
     """
     Return closest spectral type in the archive.
+    
+    If ``sptype`` is a dwarf star of spectral class V and
+    the exact spectral type is not present in the archive,
+    return the star with the closest spectral type to the 
+    input spectral type. 
 
     Parameters
     ----------
     sptype : str
-        Spectral type in the format: ``G2V``
+        Spectral type in the format: ``G2V``.
 
     Returns
     -------
     closest_spectral_type : str
-        Closest spectral type available in the archive
+        Closest spectral type available in the archive.
     """
     if sptype in sptypes:
         return sptype
     elif len(sptype) == 3 and sptype.endswith("V"):
         return spectral_types[np.argmin(np.abs(sptype_to_temp[sptype] - temps))]
     else:
         raise ValueError("We don't have a match to this spectral type. The "
@@ -47,83 +52,83 @@
 def closest_target(sptype):
     """
     Return target with the closest spectral type in the archive.
 
     Parameters
     ----------
     sptype : str
-        Spectral type in the format: ``G2V``
+        Spectral type in the format: ``G2V``.
 
     Returns
     -------
     target_name : str
-        Name of the target closest to spectral type ``sptype``
+        Name of the target closest to spectral type ``sptype``.
     closest_spectral_type : str
-        Closest spectral type available in the archive
+        Closest spectral type available in the archive.
     """
     closest_spectral_type = closest_sptype(sptype)
     return sptypes[closest_spectral_type], closest_spectral_type
 
 
 def available_sptypes():
     """
     Return a list of available spectral types in the archive.
 
     Returns
     -------
     sptypes : list
-        List of available spectral types
+        List of available spectral types.
     """
     return sorted(sptypes.keys())
 
 
 def get_closest_order(matrix, wavelength):
     """
     Return the spectral order index closest to wavelength ``wavelength``.
 
     Parameters
     ----------
     matrix : `~np.ndarray`
-        Matrix of blaze function curves from the archive
+        Matrix of blaze function curves from the archive.
     wavelength : `~astropy.units.Quantity`
         Wavelength of interest.
 
     Returns
     -------
     closest_order : int
-        Closest spectral order to wavelength ``wavelength``
+        Closest spectral order to wavelength ``wavelength``.
     """
     return np.argmin(np.abs(matrix[:, 0] - wavelength.to(u.Angstrom).value))
 
 
 def matrix_row_to_spectrum(matrix, closest_order):
     """
     Given a ``matrix`` from the archive and a spectral order index
     ``closest_order``, return the spectrum (wavelength and flux).
 
     Parameters
     ----------
     matrix : `~np.ndarray`
-        Matrix of blaze function curves from the archive
+        Matrix of blaze function curves from the archive.
     closest_order : int
-        Closest spectral order to wavelength ``wavelength``
+        Closest spectral order to wavelength ``wavelength``.
 
     Returns
     -------
     wave : `~astropy.units.Quantity`
-        Wavelengths
+        Wavelengths.
     flux : `~np.ndarray`
-        Fluxes in counts per second at each wavelength
+        Fluxes in counts per second at each wavelength.
     """
     lam_0, delta_lam, n_lam = matrix[closest_order][:3]
     polynomial_coeffs = matrix[closest_order][3:]
     wave = np.arange(lam_0 - n_lam*delta_lam/2, lam_0 + n_lam*delta_lam/2,
-                     delta_lam) * u.Angstrom
-    flux = np.polyval(polynomial_coeffs, wave-lam_0 * u.Angstrom)
-    return wave, flux
+                     delta_lam)
+    flux = np.polyval(polynomial_coeffs, wave-lam_0)
+    return wave * u.Angstrom, flux
 
 
 def scale_flux(dataset, V):
     """
     Parameters
     ----------
     dataset : `~h5py.File.dataset`
@@ -141,21 +146,21 @@
     Calculate the required exposure time to achieve signal-to-noise ratio
     ``signal_to_noise`` given the count rates ``flux`` as a function of
     wavelength ``wave``.
 
     Parameters
     ----------
     wave : `~astropy.units.Quantity`
-        Wavelengths
+        Wavelengths.
     flux : `~np.ndarray`
-        Flux in counts per second
+        Flux in counts per second.
     wavelength : `~astropy.units.Quantity`
-        Wavelength of interest at which the S/N is ``signal_to_noise``
+        Wavelength of interest at which the S/N is ``signal_to_noise``.
     signal_to_noise : float
-        Desired signal-to-noise
+        Desired signal-to-noise.
 
     Returns
     -------
     exp_time : `~astropy.units.Quantity`
         Exposure time that will yield signal-to-noise ``signal_to_noise`` at
         wavelength ``wavelength``.
     """
@@ -179,36 +184,36 @@
 
     .. warning ::
         ``arcesetc`` doesn't know anything about saturation. Ye be warned!
 
     Parameters
     ----------
     sptype : str
-        Spectral type of the star. If
+        Spectral type of the star.
     wavelength : `~astropy.units.Quantity`
     V : float
-        V magnitude of the target
+        V magnitude of the target.
     exp_time : None or float
         If ``exp_time`` is a float, show the counts curve for that exposure
         time. Otherwise, use ``signal_to_noise`` to compute the appropriate
         exposure time.
     signal_to_noise : None or float
         If ``signal_to_noise`` is a float, compute the appropriate exposure time
         to generate the counts curve that has S/N = ``signal_to_noise`` at
         wavelength ``wavelength``. Otherwise, generate counts curve for
         exposure time ``exp_time``.
 
     Returns
     -------
     wave : `~astropy.units.Quantity`
-        Wavelengths
+        Wavelengths.
     flux : `~np.ndarray`
-        Flux at each wavelength
+        Flux at each wavelength.
     exp_time : `~astropy.units.Quantity`
-        Exposure time input; or required to reach S/N of ``signal_to_noise``
+        Exposure time input; or required to reach S/N of ``signal_to_noise``.
     """
 
     target, closest_spectral_type = closest_target(sptype)
 
     matrix = archive[target][:]
 
     closest_order = get_closest_order(matrix, wavelength)
@@ -236,30 +241,30 @@
 
     .. warning ::
         ``arcesetc`` doesn't know anything about saturation. Ye be warned!
 
     Parameters
     ----------
     sptype : str
-        Spectral type of the star. If
+        Spectral type of the star.
     wavelength : `~astropy.units.Quantity`
         Wavelength of interest.
     V : float
-        V magnitude of the target
+        V magnitude of the target.
     signal_to_noise : float
         If ``signal_to_noise`` is a float, compute the appropriate exposure time
         to generate the S/N curve that has S/N = ``signal_to_noise`` at
         wavelength ``wavelength``. Otherwise, generate S/N curve for
         exposure time ``exp_time``.
 
     Returns
     -------
     exp_time : `~astropy.units.Quantity`
         Exposure time input, or computed to achieve S/N ratio
-        ``signal_to_noise`` at wavelength ``wavelength``
+        ``signal_to_noise`` at wavelength ``wavelength``.
 
     Examples
     --------
 
     How many seconds must one expose ARCES on a V=12 mag M0V star to get a S/N
     of 30 at the wavelength of H-alpha?
```

### Comparing `arcesetc-0.1/astropy_helpers/LICENSE.rst` & `arcesetc-0.3/licenses/BSD3.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-Copyright (c) 2014, Astropy Developers
-
+Copyright (c) 2018, Brett Morris & Trevor Dorn-Wallenstein
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `arcesetc-0.1/astropy_helpers/licenses/LICENSE_ASTROSCRAPPY.rst` & `arcesetc-0.3/licenses/TEMPLATE_LICENCE.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-# The OpenMP helpers include code heavily adapted from astroscrappy, released
-# under the following license:
-#
-# Copyright (c) 2015, Curtis McCully
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
-#
-# * Redistributions of source code must retain the above copyright notice, this
-#   list of conditions and the following disclaimer.
-# * Redistributions in binary form must reproduce the above copyright notice, this
-#   list of conditions and the following disclaimer in the documentation and/or
-#   other materials provided with the distribution.
-# * Neither the name of the Astropy Team nor the names of its contributors may be
-#   used to endorse or promote products derived from this software without
-#   specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-# WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
-# ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
-# ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+This project is based upon the Astropy package template
+(https://github.com/astropy/package-template/) which is licenced under the terms
+of the following licence.
+
+---
+
+Copyright (c) 2018, Astropy Developers
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without modification,
+are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+* Redistributions in binary form must reproduce the above copyright notice, this
+  list of conditions and the following disclaimer in the documentation and/or
+  other materials provided with the distribution.
+* Neither the name of the Astropy Team nor the names of its contributors may be
+  used to endorse or promote products derived from this software without
+  specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `arcesetc-0.1/docs/.ipynb_checkpoints/paper-checkpoint.md` & `arcesetc-0.3/docs/paper.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ---
-title: 'arcesetc: ARC Echelle Spectroscopic Exposure Time Calculator'
+title: 'arcesetc: ARC Echelle Spectrograph Exposure Time Calculator'
 tags:
   - Python
   - astronomy
   - spectroscopy
 authors:
   - name: Brett M. Morris
     orcid: 0000-0003-2528-3409
@@ -13,45 +13,70 @@
     affiliation: 1
   - name: Emily M. Levesque
     orcid: 0000-0003-2184-1581
     affiliation: 1
   - name: Charli Sakari
     orcid: 0000-0002-5095-4000
     affiliation: 1
+  - name: Doug Gies
+    orcid: 0000-0001-8537-3583
+    affiliation: 2
+  - name: Katherine Lester
+    orcid: 0000-0002-9903-9911
+    affiliation: 2
+  - name: Yuta Notsu
+    orcid: 0000-0002-0412-0849
+    affiliation: 3
+  - name: Allison Youngblood
+    orcid: 0000-0002-1176-3391
+    affiliation: 4
+  - name: Russet McMillan
+    affiliation: 5
+
 affiliations:
  - name: Astronomy Department, University of Washington, Seattle, WA, USA
    index: 1
-date: 1 Jan 2019
+ - name: Physics-Astronomy Department, Georgia State University, Atlanta, GA, USA
+   index: 2
+ - name: Department of Astronomy, Kyoto University, Sakyo Ward, Kyoto, Kyoto Prefecture 606-8501, Japan
+   index: 3
+ - name: NASA Goddard Space Flight Center, Greenbelt, MD, USA
+   index: 4
+ - name: Apache Point Observatory
+   index: 5
+date: 1 Feb 2019
 bibliography: paper.bib
 --- 
 
 # Summary
 
 The ARC Echelle Spectroscopic (ARCES) Exposure Time Calculator, or ``arcesetc``,
 is a simple exposure time calculator for the ARCES instrument on the 
 Astrophysical Research Consortium (ARC) 3.5 m Telescope at Apache Point 
-Observatory for stellar spectroscopy. Users can supply ``arcesetc`` functions 
+Observatory for stellar spectroscopy. Astronomers can use it to plan observations
+with the ARCES instrument. Users can supply ``arcesetc`` functions 
 with the spectral type of their target star, the V band magnitude, and either: 
 the desired exposure time in order to determine the counts and signal-to-noise
 ratio as a function of wavelength; or the desired signal-to-noise ratio at a 
 given wavelength to determine the required exposure time. 
 
 We estimate the count rates for stars as a function of wavelength by fitting 
 15th-order polynomials to each spectral order of real observations of a star of 
 each spectral type. These polynomial coefficients and some wavelength metadata
-are stored in an HDF5 archive for compactness and easy of reconstruction. Then
+are stored in an HDF5 archive for compactness and ease of reconstruction. Then
 upon calling ``arcesetc``, the archive is opened and the spectral order closest
 to the wavelength of interest is reconstructed from the polynomial 
 coefficients, for a star of the closest available spectral type to the one 
 requested. 
 
-At present, the stellar spectral types included in the ``arcesetc`` library
-span from late F to early M stars on the main sequence, a variety of M giants, 
-and one each of an O, B, and Wolf-Rayet star. Contributions from the community 
-are welcome to expand the library to include other spectral types.
+At present, the 79 stellar spectral types included in the ``arcesetc`` library
+span from mid F to mid M stars on the main sequence, a variety of M giants, 
+a handful of O and B, and a white dwarf and a Wolf-Rayet star. Contributions
+from the community are welcome to expand the library to include other spectral 
+types.
 
 ``arcesetc`` was built from the Astropy package-template, and thus includes 
 self-building documentation and continuous integration [@astropy:2018].
 
 # Acknowledgements
 
 We acknowledge guidance from Suzanne L. Hawley, and the invaluable
```

### Comparing `arcesetc-0.1/docs/arcesetc/gettingstarted.rst` & `arcesetc-0.3/docs/arcesetc/gettingstarted.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,31 +4,36 @@
 Exposure time to counts
 -----------------------
 
 Given an exposure time, spectral type, and V magnitude, what are the counts and
 signal-to-noise ratios we can collect using ARCES on the ARC 3.5 m Telescope at
 Apache Point Observatory?
 
-First, let's import the packages we'll use::
+First, let's import the packages we'll use:
+
+.. code-block:: python
 
     import matplotlib.pyplot as plt
     import astropy.units as u
 
     from arcesetc import plot_order_counts, plot_order_sn
 
-Then let's specify the properties of the observation that we're going to make::
+Then let's specify the properties of the observation that we're going to make:
 
+.. code-block:: python
 
     sptype = 'G4V'
     wavelength = 6562 * u.Angstrom
     exp_time = 30 * u.min
     V = 10
 
 Now let's make a plot of the number of counts we can expect in the order
-containing ``wavelength``, using `~arcesetc.plot_order_counts`::
+containing ``wavelength``, using `~arcesetc.plot_order_counts`:
+
+.. code-block:: python
 
     fig, ax, exp_time = plot_order_counts(sptype, wavelength, V, exp_time=exp_time)
     plt.show()
 
 
 .. plot::
 
@@ -42,15 +47,17 @@
     exp_time = 30 * u.min
     V = 10
 
     fig, ax, exp_time = plot_order_counts(sptype, wavelength, V, exp_time=exp_time)
     plt.show()
 
 Similarly, we can plot the signal-to-noise ratio using `~arcesetc.plot_order_sn`
-like so::
+like so:
+
+.. code-block:: python
 
     fig, ax, exp_time = plot_order_sn(sptype, wavelength, V, exp_time=exp_time)
     plt.show()
 
 .. plot::
 
     import matplotlib.pyplot as plt
@@ -75,15 +82,17 @@
 
 
 Signal-to-noise to exposure time
 --------------------------------
 
 Given a S/N at a particular wavelength, what's the appropriate exposure time? We
 can find out by supplying the desired ``signal_to_noise``, and ``arcesetc`` will
-compute the exposure time for you::
+compute the exposure time for you:
+
+.. code-block:: python
 
     import matplotlib.pyplot as plt
     import astropy.units as u
     from arcesetc import plot_order_sn
 
     sptype = 'B3V'
     wavelength = 3990 * u.Angstrom
@@ -110,15 +119,17 @@
 
 
 Wolf-Rayet Star
 ---------------
 
 We presently have one Wolf-Rayet star of spectral type ``WN8h``.
 You can see the funky effects of the strong emission lines on the S/N near
-H-alpha, for example::
+H-alpha, for example:
+
+.. code-block:: python
 
     import astropy.units as u
     from arcesetc import plot_order_sn
 
     sptype = 'WN8h'
     wavelength = 6562 * u.Angstrom
     signal_to_noise = 30
```

### Comparing `arcesetc-0.1/docs/arcesetc/nextsteps.rst` & `arcesetc-0.3/docs/arcesetc/nextsteps.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 No plots, just exposure times
 -----------------------------
 
 You can also calculate the exposure time required to obtain a given S/N using
 the `~arcesetc.signal_to_noise_to_exp_time` function. For example - how many
 seconds must one expose ARCES on a V=12 mag M0V star to get a S/N of 30 at the
-wavelength of H-alpha::
+wavelength of H-alpha:
+
+.. code-block:: python
 
     from arcesetc import signal_to_noise_to_exp_time
     import astropy.units as u
 
     sptype = 'M0V'
     wavelength = 6562 * u.Angstrom
     signal_to_noise = 30
@@ -24,28 +26,29 @@
 Available spectral types
 ------------------------
 
 You can see which spectral types are available with the
 `~arcesetc.available_sptypes` function.
 
 .. note::
+
     At present, the best coverage is for mid-F through mid-M type main
     sequence stars, with some M giants.
 
 Here's a color-magnitude diagram of the stars presently available in ``arcesetc``:
 
 .. image:: cmd.png
 
 How it works
 ------------
 
 We estimate the count rates for stars as a function of wavelength by fitting
 15th-order polynomials to each spectral order of real observations of a star of
 each spectral type. These polynomial coefficients and some wavelength metadata
-are stored in an HDF5 archive for compactness and easy of reconstruction. Then
+are stored in an HDF5 archive for compactness and ease of reconstruction. Then
 upon calling ``arcesetc``, the archive is opened and the spectral order closest
 to the wavelength of interest is reconstructed from the polynomial
 coefficients, for a star of the closest available spectral type to the one
 requested.
 
 .. warning::
 
@@ -54,10 +57,10 @@
 
 Run the tests
 -------------
 
 If you're contributing to ``arcesetc``, you can check that your updates don't
 break the API by running the tests like this in the source directory::
 
-    python setup.py test
+    tox -e test
 
-If the tests pass, you're ready to submit a pull request!
+If the tests pass, you're ready to submit a pull request!
```

### Comparing `arcesetc-0.1/docs/paper.bib` & `arcesetc-0.3/docs/paper.bib`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,56 @@
 @ARTICLE{astropy:2018,
-       author = {{The Astropy Collaboration} and {Price-Whelan}, A.~M. and
-        {Sip{\'{o}}cz}, B.~M. and {G{\"u}nther}, H.~M. and {Lim}, P.~L.
-        and {Crawford}, S.~M. and {Conseil}, S. and {Shupe}, D.~L. and
-        {Craig}, M.~W. and {Dencheva}, N. and {Ginsburg}, A. and
-        {VanderPlas}, J.~T. and {Bradley}, L.~D. and {P{\'e}rez-
-        Su{\'a}rez}, D. and {de Val-Borro}, M. and {Aldcroft}, T.~L. and
-        {Cruz}, K.~L. and {Robitaille}, T.~P. and {Tollerud}, E.~J. and
-        {Ardelean}, C. and {Babej}, T. and {Bachetti}, M. and {Bakanov},
-        A.~V. and {Bamford}, S.~P. and {Barentsen}, G. and {Barmby}, P.
-        and {Baumbach}, A. and {Berry}, K.~L. and {Biscani}, F. and
-        {Boquien}, M. and {Bostroem}, K.~A. and {Bouma}, L.~G. and
-        {Brammer}, G.~B. and {Bray}, E.~M. and {Breytenbach}, H. and
-        {Buddelmeijer}, H. and {Burke}, D.~J. and {Calderone}, G. and
-        {Cano Rodr{\'\i}guez}, J.~L. and {Cara}, M. and {Cardoso},
-        J.~V.~M. and {Cheedella}, S. and {Copin}, Y. and {Crichton}, D.
-        and {D{\'A}vella}, D. and {Deil}, C. and {Depagne}, {\'E}. and
-        {Dietrich}, J.~P. and {Donath}, A. and {Droettboom}, M. and
-        {Earl}, N. and {Erben}, T. and {Fabbro}, S. and {Ferreira},
-        L.~A. and {Finethy}, T. and {Fox}, R.~T. and {Garrison}, L.~H.
-        and {Gibbons}, S.~L.~J. and {Goldstein}, D.~A. and {Gommers}, R.
-        and {Greco}, J.~P. and {Greenfield}, P. and {Groener}, A.~M. and
-        {Grollier}, F. and {Hagen}, A. and {Hirst}, P. and {Homeier}, D.
-        and {Horton}, A.~J. and {Hosseinzadeh}, G. and {Hu}, L. and
-        {Hunkeler}, J.~S. and {Ivezi{\'c}}, {\v{Z}}. and {Jain}, A. and
-        {Jenness}, T. and {Kanarek}, G. and {Kendrew}, S. and {Kern},
-        N.~S. and {Kerzendorf}, W.~E. and {Khvalko}, A. and {King}, J.
-        and {Kirkby}, D. and {Kulkarni}, A.~M. and {Kumar}, A. and
-        {Lee}, A. and {Lenz}, D. and {Littlefair}, S.~P. and {Ma}, Z.
-        and {Macleod}, D.~M. and {Mastropietro}, M. and {McCully}, C.
-        and {Montagnac}, S. and {Morris}, B.~M. and {Mueller}, M. and
-        {Mumford}, S.~J. and {Muna}, D. and {Murphy}, N.~A. and
-        {Nelson}, S. and {Nguyen}, G.~H. and {Ninan}, J.~P. and
-        {N{\"o}the}, M. and {Ogaz}, S. and {Oh}, S. and {Parejko}, J.~K.
-        and {Parley}, N. and {Pascual}, S. and {Patil}, R. and {Patil},
-        A.~A. and {Plunkett}, A.~L. and {Prochaska}, J.~X. and
-        {Rastogi}, T. and {Reddy Janga}, V. and {Sabater}, J. and
-        {Sakurikar}, P. and {Seifert}, M. and {Sherbert}, L.~E. and
-        {Sherwood-Taylor}, H. and {Shih}, A.~Y. and {Sick}, J. and
-        {Silbiger}, M.~T. and {Singanamalla}, S. and {Singer}, L.~P. and
-        {Sladen}, P.~H. and {Sooley}, K.~A. and {Sornarajah}, S. and
-        {Streicher}, O. and {Teuben}, P. and {Thomas}, S.~W. and
-        {Tremblay}, G.~R. and {Turner}, J.~E.~H. and {Terr{\'o}n}, V.
-        and {van Kerkwijk}, M.~H. and {de la Vega}, A. and {Watkins},
-        L.~L. and {Weaver}, B.~A. and {Whitmore}, J.~B. and {Woillez},
-        J. and {Zabalza}, V.},
-        title = "{The Astropy Project: Building an inclusive, open-science project and
-        status of the v2.0 core package}",
-      journal = {ArXiv e-prints},
-     keywords = {Astrophysics - Instrumentation and Methods for Astrophysics},
-         year = 2018,
-        month = Jan,
-          eid = {arXiv:1801.02634},
-        pages = {arXiv:1801.02634},
-archivePrefix = {arXiv},
-       eprint = {1801.02634},
-       adsurl = {https://ui.adsabs.harvard.edu/#abs/2018arXiv180102634T},
-      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+   author = {{Astropy Collaboration} and {Price-Whelan}, A.~M. and {Sip{\H o}cz}, B.~M. and
+	{G{\"u}nther}, H.~M. and {Lim}, P.~L. and {Crawford}, S.~M. and
+	{Conseil}, S. and {Shupe}, D.~L. and {Craig}, M.~W. and {Dencheva}, N. and
+	{Ginsburg}, A. and {VanderPlas}, J.~T. and {Bradley}, L.~D. and
+	{P{\'e}rez-Su{\'a}rez}, D. and {de Val-Borro}, M. and {Aldcroft}, T.~L. and
+	{Cruz}, K.~L. and {Robitaille}, T.~P. and {Tollerud}, E.~J. and
+	{Ardelean}, C. and {Babej}, T. and {Bach}, Y.~P. and {Bachetti}, M. and
+	{Bakanov}, A.~V. and {Bamford}, S.~P. and {Barentsen}, G. and
+	{Barmby}, P. and {Baumbach}, A. and {Berry}, K.~L. and {Biscani}, F. and
+	{Boquien}, M. and {Bostroem}, K.~A. and {Bouma}, L.~G. and {Brammer}, G.~B. and
+	{Bray}, E.~M. and {Breytenbach}, H. and {Buddelmeijer}, H. and
+	{Burke}, D.~J. and {Calderone}, G. and {Cano Rodr{\'{\i}}guez}, J.~L. and
+	{Cara}, M. and {Cardoso}, J.~V.~M. and {Cheedella}, S. and {Copin}, Y. and
+	{Corrales}, L. and {Crichton}, D. and {D'Avella}, D. and {Deil}, C. and
+	{Depagne}, {\'E}. and {Dietrich}, J.~P. and {Donath}, A. and
+	{Droettboom}, M. and {Earl}, N. and {Erben}, T. and {Fabbro}, S. and
+	{Ferreira}, L.~A. and {Finethy}, T. and {Fox}, R.~T. and {Garrison}, L.~H. and
+	{Gibbons}, S.~L.~J. and {Goldstein}, D.~A. and {Gommers}, R. and
+	{Greco}, J.~P. and {Greenfield}, P. and {Groener}, A.~M. and
+	{Grollier}, F. and {Hagen}, A. and {Hirst}, P. and {Homeier}, D. and
+	{Horton}, A.~J. and {Hosseinzadeh}, G. and {Hu}, L. and {Hunkeler}, J.~S. and
+	{Ivezi{\'c}}, {\v Z}. and {Jain}, A. and {Jenness}, T. and {Kanarek}, G. and
+	{Kendrew}, S. and {Kern}, N.~S. and {Kerzendorf}, W.~E. and
+	{Khvalko}, A. and {King}, J. and {Kirkby}, D. and {Kulkarni}, A.~M. and
+	{Kumar}, A. and {Lee}, A. and {Lenz}, D. and {Littlefair}, S.~P. and
+	{Ma}, Z. and {Macleod}, D.~M. and {Mastropietro}, M. and {McCully}, C. and
+	{Montagnac}, S. and {Morris}, B.~M. and {Mueller}, M. and {Mumford}, S.~J. and
+	{Muna}, D. and {Murphy}, N.~A. and {Nelson}, S. and {Nguyen}, G.~H. and
+	{Ninan}, J.~P. and {N{\"o}the}, M. and {Ogaz}, S. and {Oh}, S. and
+	{Parejko}, J.~K. and {Parley}, N. and {Pascual}, S. and {Patil}, R. and
+	{Patil}, A.~A. and {Plunkett}, A.~L. and {Prochaska}, J.~X. and
+	{Rastogi}, T. and {Reddy Janga}, V. and {Sabater}, J. and {Sakurikar}, P. and
+	{Seifert}, M. and {Sherbert}, L.~E. and {Sherwood-Taylor}, H. and
+	{Shih}, A.~Y. and {Sick}, J. and {Silbiger}, M.~T. and {Singanamalla}, S. and
+	{Singer}, L.~P. and {Sladen}, P.~H. and {Sooley}, K.~A. and
+	{Sornarajah}, S. and {Streicher}, O. and {Teuben}, P. and {Thomas}, S.~W. and
+	{Tremblay}, G.~R. and {Turner}, J.~E.~H. and {Terr{\'o}n}, V. and
+	{van Kerkwijk}, M.~H. and {de la Vega}, A. and {Watkins}, L.~L. and
+	{Weaver}, B.~A. and {Whitmore}, J.~B. and {Woillez}, J. and
+	{Zabalza}, V. and {Astropy Contributors}},
+    title = "{The Astropy Project: Building an Open-science Project and Status of the v2.0 Core Package}",
+  journal = {\aj},
+archivePrefix = "arXiv",
+   eprint = {1801.02634},
+ primaryClass = "astro-ph.IM",
+ keywords = {methods: data analysis, methods: miscellaneous, methods: statistical, reference systems },
+     year = 2018,
+    month = sep,
+   volume = 156,
+      eid = {123},
+    pages = {123},
+      doi = {10.3847/1538-3881/aabc4f},
+   adsurl = {http://adsabs.harvard.edu/abs/2018AJ....156..123A},
+  adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
```

### Comparing `arcesetc-0.1/licenses/APACHE2.rst` & `arcesetc-0.3/licenses/APACHE2.rst`

 * *Files identical despite different names*

### Comparing `arcesetc-0.1/licenses/BSD2.rst` & `arcesetc-0.3/licenses/BSD2.rst`

 * *Files identical despite different names*

### Comparing `arcesetc-0.1/licenses/GPLv3.rst` & `arcesetc-0.3/licenses/GPLv3.rst`

 * *Files identical despite different names*

### Comparing `arcesetc-0.1/licenses/MIT.rst` & `arcesetc-0.3/licenses/MIT.rst`

 * *Files identical despite different names*

### Comparing `arcesetc-0.1/README.rst` & `arcesetc-0.3/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Exposure time calculator for APO/ARCES
 --------------------------------------
 
-.. image:: https://travis-ci.org/bmorris3/arcesetc.svg?branch=master
-    :target: https://travis-ci.org/bmorris3/arcesetc
+.. image:: https://github.com/bmorris3/arcesetc/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/bmorris3/arcesetc/actions/workflows/ci.yml
+   :alt: Testing status
 
 .. image:: https://readthedocs.org/projects/arcesetc/badge/?version=latest
     :target: https://arcesetc.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: http://img.shields.io/pypi/v/arcesetc.svg?text=version
     :target: https://pypi.python.org/pypi/arcesetc/
     :alt: Latest release
 
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
+    
+.. image:: http://joss.theoj.org/papers/10.21105/joss.01130/status.svg
+   :target: https://doi.org/10.21105/joss.01130
 
-.. image:: https://img.shields.io/badge/powered%20by-aesop-orange.svg?style=flat
-    :target: https://github.com/bmorris3/aesop
-    :alt: Powered by aesop badge
+.. image:: https://zenodo.org/badge/160124540.svg
+   :target: https://zenodo.org/badge/latestdoi/160124540
 
 Calculate S/N and exposure times for
 stellar spectroscopy with the `ARC Echelle Spectrograph (ARCES)
 <https://www.apo.nmsu.edu/arc35m/Instruments/ARCES/>`_ on the
 `ARC 3.5 m Telescope <https://www.apo.nmsu.edu/arc35m/>`_ at
 `Apache Point Observatory <https://www.apo.nmsu.edu>`_.
 
@@ -40,14 +43,30 @@
 each spectral type. These polynomial coefficients and some wavelength metadata
 are stored in an HDF5 archive for compactness and easy of reconstruction. Then
 upon calling ``arcesetc``, the archive is opened and the spectral order closest
 to the wavelength of interest is reconstructed from the polynomial
 coefficients, for a star of the closest available spectral type to the one
 requested. 
 
+
+Installation
+------------
+
+You can install ``arcesetc`` with pip::
+
+    pip install arcesetc
+
+You can install ``arcesetc`` from the source code by doing the following::
+
+    git clone https://github.com/bmorris3/arcesetc.git
+    cd arcesetc
+    pip install .
+
+``arcesetc`` requires python >=3.5, numpy, astropy, h5py, and matplotlib.
+
 For more information, `read the docs <https://arcesetc.readthedocs.io/>`_.
 
 License
 -------
 
 This project is Copyright (c) Brett Morris & Trevor Dorn-Wallenstein and licensed under
 the terms of the MIT license. This package is based upon
```

