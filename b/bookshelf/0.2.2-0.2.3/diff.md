# Comparing `tmp/bookshelf-0.2.2.tar.gz` & `tmp/bookshelf-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookshelf-0.2.2.tar", last modified: Thu Apr 13 11:40:35 2023, max compression
+gzip compressed data, was "bookshelf-0.2.3.tar", max compression
```

## Comparing `bookshelf-0.2.2.tar` & `bookshelf-0.2.3.tar`

### file list

```diff
@@ -1,132 +1,17 @@
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.397691 bookshelf-0.2.2/
--rw-r--r--   0 jared      (501) staff       (20)     5451 2022-07-17 06:52:23.000000 bookshelf-0.2.2/.gitignore
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.374893 bookshelf-0.2.2/.gitlab/
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.381200 bookshelf-0.2.2/.gitlab/issue_templates/
--rw-r--r--   0 jared      (501) staff       (20)      610 2023-03-13 23:04:16.000000 bookshelf-0.2.2/.gitlab/issue_templates/Bug.md
--rw-r--r--   0 jared      (501) staff       (20)      526 2023-03-13 23:04:16.000000 bookshelf-0.2.2/.gitlab/issue_templates/Feature_Request.md
--rw-r--r--   0 jared      (501) staff       (20)      559 2023-03-13 23:04:16.000000 bookshelf-0.2.2/.gitlab/issue_templates/New_Book.md
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.381607 bookshelf-0.2.2/.gitlab/merge_request_templates/
--rw-r--r--   0 jared      (501) staff       (20)      353 2023-03-13 23:04:16.000000 bookshelf-0.2.2/.gitlab/merge_request_templates/Default.md
--rw-r--r--   0 jared      (501) staff       (20)      333 2023-03-13 23:04:16.000000 bookshelf-0.2.2/.gitlab/merge_request_templates/New Book.md
--rw-r--r--   0 jared      (501) staff       (20)     2159 2023-04-13 11:35:17.000000 bookshelf-0.2.2/.gitlab-ci.yml
--rw-r--r--   0 jared      (501) staff       (20)      429 2022-07-17 06:52:23.000000 bookshelf-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 jared      (501) staff       (20)     4975 2023-04-13 11:35:17.000000 bookshelf-0.2.2/CHANGELOG.rst
--rw-r--r--   0 jared      (501) staff       (20)     1056 2023-03-13 23:04:16.000000 bookshelf-0.2.2/LICENSE
--rw-r--r--   0 jared      (501) staff       (20)     2656 2023-04-13 11:39:36.000000 bookshelf-0.2.2/Makefile
--rw-r--r--   0 jared      (501) staff       (20)     1953 2023-04-13 11:40:35.397806 bookshelf-0.2.2/PKG-INFO
--rw-r--r--   0 jared      (501) staff       (20)     5901 2023-04-13 11:35:17.000000 bookshelf-0.2.2/README.rst
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.382045 bookshelf-0.2.2/docs/
--rw-r--r--   0 jared      (501) staff       (20)      638 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/Makefile
--rw-r--r--   0 jared      (501) staff       (20)      769 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/make.bat
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.383550 bookshelf-0.2.2/docs/source/
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.383742 bookshelf-0.2.2/docs/source/_static/
--rw-r--r--   0 jared      (501) staff       (20)        0 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/_static/.gitkeep
--rw-r--r--   0 jared      (501) staff       (20)     2557 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/conf.py
--rw-r--r--   0 jared      (501) staff       (20)      986 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/configuration.rst
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.384219 bookshelf-0.2.2/docs/source/development/
--rw-r--r--   0 jared      (501) staff       (20)     5595 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/development/contributing.rst
--rw-r--r--   0 jared      (501) staff       (20)      176 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/development/index.rst
--rw-r--r--   0 jared      (501) staff       (20)      856 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/development/releasing.rst
--rw-r--r--   0 jared      (501) staff       (20)      363 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/index.rst
--rw-r--r--   0 jared      (501) staff       (20)      105 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/installation.rst
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.385099 bookshelf-0.2.2/docs/source/reference/
--rw-r--r--   0 jared      (501) staff       (20)       96 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/reference/bookshelf.book.rst
--rw-r--r--   0 jared      (501) staff       (20)      102 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/reference/bookshelf.errors.rst
--rw-r--r--   0 jared      (501) staff       (20)       99 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/reference/bookshelf.shelf.rst
--rw-r--r--   0 jared      (501) staff       (20)       99 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/reference/bookshelf.utils.rst
--rw-r--r--   0 jared      (501) staff       (20)      131 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/reference/index.rst
--rw-r--r--   0 jared      (501) staff       (20)     2568 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/usage.rst
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.385528 bookshelf-0.2.2/notebooks/
--rw-r--r--   0 jared      (501) staff       (20)     1212 2022-07-19 03:22:48.000000 bookshelf-0.2.2/notebooks/README.md
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.385943 bookshelf-0.2.2/notebooks/ceds/
--rw-r--r--   0 jared      (501) staff       (20)     5744 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/ceds/ceds.py
--rw-r--r--   0 jared      (501) staff       (20)     1328 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/ceds/ceds.yaml
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.375818 bookshelf-0.2.2/notebooks/examples/
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.386269 bookshelf-0.2.2/notebooks/examples/multiple_versions/
--rw-r--r--   0 jared      (501) staff       (20)     2706 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/examples/multiple_versions/multiple_versions.py
--rw-r--r--   0 jared      (501) staff       (20)      713 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/examples/multiple_versions/multiple_versions.yaml
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.386625 bookshelf-0.2.2/notebooks/examples/simple/
--rw-r--r--   0 jared      (501) staff       (20)     2486 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/examples/simple/simple.py
--rw-r--r--   0 jared      (501) staff       (20)      415 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/examples/simple/simple.yaml
--rw-r--r--   0 jared      (501) staff       (20)       63 2022-07-17 06:52:23.000000 bookshelf-0.2.2/notebooks/jupytext.toml
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.387107 bookshelf-0.2.2/notebooks/primap-hist/
--rw-r--r--   0 jared      (501) staff       (20)     4653 2023-04-13 05:34:27.000000 bookshelf-0.2.2/notebooks/primap-hist/primap-hist.py
--rw-r--r--   0 jared      (501) staff       (20)     2280 2023-03-14 01:59:54.000000 bookshelf-0.2.2/notebooks/primap-hist/primap-hist.yaml
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.387560 bookshelf-0.2.2/notebooks/rcmip-emissions/
--rw-r--r--   0 jared      (501) staff       (20)     1844 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/rcmip-emissions/rcmip-emissions.py
--rw-r--r--   0 jared      (501) staff       (20)      449 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/rcmip-emissions/rcmip-emissions.yaml
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.387914 bookshelf-0.2.2/notebooks/ssp-basic-elements/
--rw-r--r--   0 jared      (501) staff       (20)     2221 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/ssp-basic-elements/ssp-basic-elements.py
--rw-r--r--   0 jared      (501) staff       (20)     6775 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/ssp-basic-elements/ssp-basic-elements.yaml
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.388280 bookshelf-0.2.2/notebooks/un-wpp/
--rw-r--r--   0 jared      (501) staff       (20)     7209 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/un-wpp/un-wpp.py
--rw-r--r--   0 jared      (501) staff       (20)     1394 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/un-wpp/un-wpp.yaml
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.388876 bookshelf-0.2.2/notebooks/wdi/
--rw-r--r--   0 jared      (501) staff       (20)     6476 2023-03-13 23:06:52.000000 bookshelf-0.2.2/notebooks/wdi/wdi.py
--rw-r--r--   0 jared      (501) staff       (20)      866 2023-03-13 23:06:52.000000 bookshelf-0.2.2/notebooks/wdi/wdi.yaml
--rw-r--r--   0 jared      (501) staff       (20)      747 2023-04-12 05:55:19.000000 bookshelf-0.2.2/pyproject.toml
--rw-r--r--   0 jared      (501) staff       (20)     3137 2023-04-13 11:40:35.398352 bookshelf-0.2.2/setup.cfg
--rw-r--r--   0 jared      (501) staff       (20)       58 2022-07-16 02:39:36.000000 bookshelf-0.2.2/setup.py
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.376457 bookshelf-0.2.2/src/
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.390934 bookshelf-0.2.2/src/bookshelf/
--rw-r--r--   0 jared      (501) staff       (20)      686 2023-04-13 05:34:27.000000 bookshelf-0.2.2/src/bookshelf/__init__.py
--rw-r--r--   0 jared      (501) staff       (20)     9739 2023-04-13 11:35:17.000000 bookshelf-0.2.2/src/bookshelf/book.py
--rw-r--r--   0 jared      (501) staff       (20)     1284 2023-03-13 23:04:16.000000 bookshelf-0.2.2/src/bookshelf/cli.py
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.392456 bookshelf-0.2.2/src/bookshelf/commands/
--rw-r--r--   0 jared      (501) staff       (20)       21 2022-07-18 12:01:42.000000 bookshelf-0.2.2/src/bookshelf/commands/__init__.py
--rw-r--r--   0 jared      (501) staff       (20)     2239 2023-04-12 05:57:25.000000 bookshelf-0.2.2/src/bookshelf/commands/cmd_publish.py
--rw-r--r--   0 jared      (501) staff       (20)     1488 2023-03-13 23:04:16.000000 bookshelf-0.2.2/src/bookshelf/commands/cmd_run.py
--rw-r--r--   0 jared      (501) staff       (20)      518 2023-03-13 23:04:16.000000 bookshelf-0.2.2/src/bookshelf/constants.py
--rw-r--r--   0 jared      (501) staff       (20)      818 2023-03-13 23:04:16.000000 bookshelf-0.2.2/src/bookshelf/errors.py
--rw-r--r--   0 jared      (501) staff       (20)     8391 2023-03-13 23:04:16.000000 bookshelf-0.2.2/src/bookshelf/notebook.py
--rw-r--r--   0 jared      (501) staff       (20)     4581 2023-03-13 23:04:16.000000 bookshelf-0.2.2/src/bookshelf/schema.py
--rw-r--r--   0 jared      (501) staff       (20)    11970 2023-04-13 11:35:17.000000 bookshelf-0.2.2/src/bookshelf/shelf.py
--rw-r--r--   0 jared      (501) staff       (20)     6119 2023-04-13 05:34:27.000000 bookshelf-0.2.2/src/bookshelf/utils.py
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.391815 bookshelf-0.2.2/src/bookshelf.egg-info/
--rw-r--r--   0 jared      (501) staff       (20)     1953 2023-04-13 11:40:35.000000 bookshelf-0.2.2/src/bookshelf.egg-info/PKG-INFO
--rw-r--r--   0 jared      (501) staff       (20)     3110 2023-04-13 11:40:35.000000 bookshelf-0.2.2/src/bookshelf.egg-info/SOURCES.txt
--rw-r--r--   0 jared      (501) staff       (20)        1 2023-04-13 11:40:35.000000 bookshelf-0.2.2/src/bookshelf.egg-info/dependency_links.txt
--rw-r--r--   0 jared      (501) staff       (20)       49 2023-04-13 11:40:35.000000 bookshelf-0.2.2/src/bookshelf.egg-info/entry_points.txt
--rw-r--r--   0 jared      (501) staff       (20)      644 2023-04-13 11:40:35.000000 bookshelf-0.2.2/src/bookshelf.egg-info/requires.txt
--rw-r--r--   0 jared      (501) staff       (20)       10 2023-04-13 11:40:35.000000 bookshelf-0.2.2/src/bookshelf.egg-info/top_level.txt
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.392642 bookshelf-0.2.2/tests/
--rw-r--r--   0 jared      (501) staff       (20)      732 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/conftest.py
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.392814 bookshelf-0.2.2/tests/integration/
--rw-r--r--   0 jared      (501) staff       (20)      681 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/integration/test_simple.py
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.393087 bookshelf-0.2.2/tests/notebooks/
--rw-r--r--   0 jared      (501) staff       (20)     3243 2023-04-13 11:35:17.000000 bookshelf-0.2.2/tests/notebooks/test_notebooks.py
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.377637 bookshelf-0.2.2/tests/test-data/
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.377093 bookshelf-0.2.2/tests/test-data/v0.1.0/
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.393273 bookshelf-0.2.2/tests/test-data/v0.1.0/example/
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.393698 bookshelf-0.2.2/tests/test-data/v0.1.0/example/v1.0.0/
--rw-r--r--   0 jared      (501) staff       (20)      370 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.1.0/example/v1.0.0/datapackage.json
--rw-r--r--   0 jared      (501) staff       (20)    13117 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.1.0/example/v1.0.0/leakage_rates_low.csv
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.394119 bookshelf-0.2.2/tests/test-data/v0.1.0/example/v1.1.0/
--rw-r--r--   0 jared      (501) staff       (20)        5 2022-07-17 06:52:23.000000 bookshelf-0.2.2/tests/test-data/v0.1.0/example/v1.1.0/datapackage.json
--rw-r--r--   0 jared      (501) staff       (20)    13117 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.1.0/example/v1.1.0/leakage_rates_low.csv
--rw-r--r--   0 jared      (501) staff       (20)      304 2022-07-17 06:52:23.000000 bookshelf-0.2.2/tests/test-data/v0.1.0/example/volume.json
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.377396 bookshelf-0.2.2/tests/test-data/v0.2.0/
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.394294 bookshelf-0.2.2/tests/test-data/v0.2.0/example/
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.394640 bookshelf-0.2.2/tests/test-data/v0.2.0/example/v1.0.0_e001/
--rw-r--r--   0 jared      (501) staff       (20)      386 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.0/example/v1.0.0_e001/datapackage.json
--rw-r--r--   0 jared      (501) staff       (20)    13117 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.0/example/v1.0.0_e001/leakage_rates_low.csv
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.394968 bookshelf-0.2.2/tests/test-data/v0.2.0/example/v1.1.0_e001/
--rw-r--r--   0 jared      (501) staff       (20)        5 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.0/example/v1.1.0_e001/datapackage.json
--rw-r--r--   0 jared      (501) staff       (20)    13117 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.0/example/v1.1.0_e001/leakage_rates_low.csv
--rw-r--r--   0 jared      (501) staff       (20)      354 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.0/example/volume.json
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.377691 bookshelf-0.2.2/tests/test-data/v0.2.1/
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.395139 bookshelf-0.2.2/tests/test-data/v0.2.1/example/
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.395525 bookshelf-0.2.2/tests/test-data/v0.2.1/example/v1.0.0_e001/
--rw-r--r--   0 jared      (501) staff       (20)      406 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.1/example/v1.0.0_e001/datapackage.json
--rw-r--r--   0 jared      (501) staff       (20)    13117 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.1/example/v1.0.0_e001/leakage_rates_low.csv
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.396045 bookshelf-0.2.2/tests/test-data/v0.2.1/example/v1.1.0_e001/
--rw-r--r--   0 jared      (501) staff       (20)        5 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.1/example/v1.1.0_e001/datapackage.json
--rw-r--r--   0 jared      (501) staff       (20)    13117 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.1/example/v1.1.0_e001/leakage_rates_low.csv
--rw-r--r--   0 jared      (501) staff       (20)      402 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.1/example/volume.json
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.397397 bookshelf-0.2.2/tests/unit/
--rw-r--r--   0 jared      (501) staff       (20)     1953 2023-04-13 05:34:27.000000 bookshelf-0.2.2/tests/unit/conftest.py
--rw-r--r--   0 jared      (501) staff       (20)     3112 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/unit/test_book.py
--rw-r--r--   0 jared      (501) staff       (20)     4397 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/unit/test_cli.py
--rw-r--r--   0 jared      (501) staff       (20)     3951 2023-04-13 05:34:27.000000 bookshelf-0.2.2/tests/unit/test_notebook.py
--rw-r--r--   0 jared      (501) staff       (20)    10278 2023-04-13 05:34:27.000000 bookshelf-0.2.2/tests/unit/test_shelf.py
--rw-r--r--   0 jared      (501) staff       (20)     1529 2022-07-18 12:01:42.000000 bookshelf-0.2.2/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     1056 2023-07-24 01:42:55.866046 bookshelf-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3033 2023-07-27 05:47:14.496668 bookshelf-0.2.3/README.md
+-rw-r--r--   0        0        0     6611 2023-07-28 03:00:32.648459 bookshelf-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      245 2023-07-27 07:29:59.128986 bookshelf-0.2.3/src/bookshelf/__init__.py
+-rw-r--r--   0        0        0     9855 2023-07-27 07:29:59.128986 bookshelf-0.2.3/src/bookshelf/book.py
+-rw-r--r--   0        0        0     1427 2023-07-27 07:38:30.327987 bookshelf-0.2.3/src/bookshelf/cli.py
+-rw-r--r--   0        0        0       21 2023-07-24 01:42:55.870046 bookshelf-0.2.3/src/bookshelf/commands/__init__.py
+-rw-r--r--   0        0        0     2278 2023-07-27 07:29:59.128986 bookshelf-0.2.3/src/bookshelf/commands/cmd_publish.py
+-rw-r--r--   0        0        0     1440 2023-07-27 07:29:59.128986 bookshelf-0.2.3/src/bookshelf/commands/cmd_run.py
+-rw-r--r--   0        0        0      513 2023-07-27 07:29:59.128986 bookshelf-0.2.3/src/bookshelf/constants.py
+-rw-r--r--   0        0        0      896 2023-07-27 07:38:30.327987 bookshelf-0.2.3/src/bookshelf/errors.py
+-rw-r--r--   0        0        0     8282 2023-07-27 07:29:59.128986 bookshelf-0.2.3/src/bookshelf/notebook.py
+-rw-r--r--   0        0        0        0 2023-07-27 05:47:14.504668 bookshelf-0.2.3/src/bookshelf/py.typed
+-rw-r--r--   0        0        0     4532 2023-07-27 07:29:59.128986 bookshelf-0.2.3/src/bookshelf/schema.py
+-rw-r--r--   0        0        0    11972 2023-07-27 07:29:59.128986 bookshelf-0.2.3/src/bookshelf/shelf.py
+-rw-r--r--   0        0        0     6096 2023-07-27 07:29:59.128986 bookshelf-0.2.3/src/bookshelf/utils.py
+-rw-r--r--   0        0        0     4137 1970-01-01 00:00:00.000000 bookshelf-0.2.3/PKG-INFO
```

### Comparing `bookshelf-0.2.2/LICENSE` & `bookshelf-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.2/src/bookshelf/book.py` & `bookshelf-0.2.3/src/bookshelf/book.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
+Books
+
 A Book represents a single versioned dataset. A dataset can contain multiple resources
 each of which are loaded independently.
 """
 import glob
 import json
 import os.path
 import pathlib
-from typing import Any, Dict, Iterable, List, Optional, Union, cast
+from collections.abc import Iterable
+from typing import Any, Optional, Union, cast
 
 import datapackage
 import pooch
 import scmdata
 
 from bookshelf.schema import Edition, NotebookMetadata, Version
 from bookshelf.utils import (
@@ -188,15 +191,15 @@
         str
             The filename for the file in the local bookshelf
         """
         return os.path.join(self.local_bookshelf, self.name, self.long_version(), fname)
 
     def as_datapackage(self) -> datapackage.Package:
         """
-        Package representation of the book
+        Datapackage for the current book
 
         :mod:`datapackage` is used for handling the metadata. Modifying
         the package also modifies the Book.
 
         Returns
         -------
         :class:`datapackage.Package`
@@ -208,26 +211,26 @@
             local_fname = self.local_fname(fname)
             with open(local_fname) as file_handle:
                 file_data = json.load(file_handle)
 
             self._metadata = datapackage.Package(file_data)
         return self._metadata
 
-    def metadata(self) -> Dict[str, Any]:
+    def metadata(self) -> dict[str, Any]:
         """
         Metadata about the current book
 
         Returns
         -------
         dict
             Metadata about the Book
         """
-        return cast(Dict[str, Any], self.as_datapackage().descriptor)
+        return cast(dict[str, Any], self.as_datapackage().descriptor)
 
-    def files(self) -> List[str]:
+    def files(self) -> list[str]:
         """
         List of files that are locally available
 
         Since each Resource is fetched when first read the number of files present may
         be less than available on the remote bookshelf.
 
         Returns
@@ -249,15 +252,18 @@
         ----------
         name : str
             Unique name of the resource
         data : scmdata.ScmRun
             Timeseries data to add to the Book
         """
         fname = f"{name}.csv"
-        data.timeseries().sort_index().to_csv(self.local_fname(fname))
+
+        # TODO: this flag could be exposed in future
+        quoting = None  # csv.QUOTE_NONNUMERIC
+        data.timeseries().sort_index().to_csv(self.local_fname(fname), quoting=quoting)
         resource_hash = pooch.hashes.file_hash(self.local_fname(fname))
 
         metadata = self.as_datapackage()
         metadata.add_resource(
             {
                 "name": name,
                 "format": "CSV",
@@ -296,17 +302,15 @@
             Additional arguments passed to :class:`LocalBook`
 
         Returns
         -------
         LocalBook
             An instance of a local book with the datapackage setup
         """
-        book = LocalBook(
-            meta.name, version=meta.version, edition=meta.edition, **kwargs
-        )
+        book = LocalBook(meta.name, version=meta.version, edition=meta.edition, **kwargs)
         book._metadata = datapackage.Package(
             {
                 "name": meta.name,
                 "version": meta.version,
                 "private": meta.private,
                 "edition": meta.edition,
                 "resources": [],
```

### Comparing `bookshelf-0.2.2/src/bookshelf/cli.py` & `bookshelf-0.2.3/src/bookshelf/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 """
 Bookshelf CLI
 """
 import logging
 import os
+from typing import Optional
 
 import click
 import click_log
 import dotenv
 
 dotenv.load_dotenv()
 
 cmd_folder = os.path.abspath(os.path.join(os.path.dirname(__file__), "commands"))
 logger = logging.getLogger("bookshelf")
 
 
 class _CLICommands(click.MultiCommand):
-    def list_commands(self, ctx):
+    def list_commands(self, ctx: click.Context) -> list[str]:
         commands = []
         for filename in os.listdir(cmd_folder):
             if filename.endswith(".py") and filename.startswith("cmd_"):
                 commands.append(filename[4:-3])
         commands.sort()
         return commands
 
-    def get_command(self, ctx, cmd_name):
+    def get_command(self, ctx: click.Context, cmd_name: str) -> Optional[click.Command]:
         try:
             mod = __import__(f"bookshelf.commands.cmd_{cmd_name}", None, None, ["cli"])
         except ImportError:  # pragma: no cover
             return None
-        return mod.cli
+        return mod.cli  # type: ignore
 
 
 @click.command(cls=_CLICommands, name="bookshelf")
 @click.option("-q", "--quiet", is_flag=True)
-@click_log.simple_verbosity_option(logger)
+@click_log.simple_verbosity_option(logger)  # type: ignore
 @click.pass_context
-def main(ctx, quiet):
+def main(ctx, quiet) -> None:
     """
     Bookshelf for managing reusable datasets
     """
     ctx.ensure_object(dict)
 
     if not logger.hasHandlers():
         click_log.basic_config(logger)  # pragma: no cover
```

### Comparing `bookshelf-0.2.2/src/bookshelf/commands/cmd_publish.py` & `bookshelf-0.2.3/src/bookshelf/commands/cmd_publish.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 )
 @click.option(
     "--force",
     is_flag=True,
     help="Override the existing published data",
     default=False,
 )
-def cli(name: str, version: list[str], include_private: bool, force: bool) -> None:
+def cli(name: str, version: tuple[str, ...], include_private: bool, force: bool) -> None:
     """
     Build and upload a Book to the Bookshelf
 
     Uploading a Book requires the correct AWS credentials (until an authentication
     scheme is introduced). At Climate Resource we use aws-vault for managing multiple
     sets of AWS credentials. Documentation about the different sources of authentication
     can be found here: https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html
@@ -59,9 +59,9 @@
                     version=dataset_version,
                 )
                 logger.info(f"Finish building {name}@{book.long_version()}")
 
                 shelf = BookShelf()
                 shelf.publish(book, force=force)
             except Exception as exc:
-                logger.error(str(exc))
+                logger.exception(f"Unable to process {name}@{version}")
                 raise click.Abort() from exc
```

### Comparing `bookshelf-0.2.2/src/bookshelf/commands/cmd_run.py` & `bookshelf-0.2.3/src/bookshelf/commands/cmd_run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 run CLI command
 """
 import logging
-from typing import Tuple
 
 import click
 
 from bookshelf.notebook import get_available_versions, run_notebook
 
 logger = logging.getLogger(__name__)
 
@@ -32,28 +31,24 @@
 )
 @click.option(
     "-f",
     "--force",
     help="Override the existing output if the output directory isn't empty",
     is_flag=True,
 )
-def cli(
-    name: str, output: str, force: bool, version: Tuple[str], include_private: bool
-) -> None:
+def cli(name: str, output: str, force: bool, version: tuple[str], include_private: bool) -> None:
     """
     Run a notebook
 
     This runs one of the notebooks used to generate a Book
     """
-    if not version:
+    if not len(version):
         all_versions = get_available_versions(name, include_private=include_private)
     else:
         all_versions = version
 
     for dataset_version in all_versions:
         try:
-            run_notebook(
-                name, output_directory=output, force=force, version=dataset_version
-            )
+            run_notebook(name, output_directory=output, force=force, version=dataset_version)
         except Exception as exc:
-            logger.error(f"Failed to run {name}: {exc}")
+            logger.error(f"Failed to run {name}: {exc}")  # noqa
             raise click.Abort() from exc
```

### Comparing `bookshelf-0.2.2/src/bookshelf/constants.py` & `bookshelf-0.2.3/src/bookshelf/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,10 @@
 DATA_DIR = os.path.join(ROOT_DIR, "data")
 RAW_DATA_DIR = os.path.join(DATA_DIR, "raw")
 TEST_DATA_DIR = os.path.join(ROOT_DIR, "tests", "test-data")
 PROCESSED_DATA_DIR = os.path.join(DATA_DIR, "processed", DATA_FORMAT_VERSION)
 
 
 DEFAULT_BOOKSHELF = (
-    f"https://cr-prod-datasets-bookshelf.s3.us-west-2.amazonaws.com"
-    f"/{DATA_FORMAT_VERSION}"
+    "https://cr-prod-datasets-bookshelf.s3.us-west-2.amazonaws.com" f"/{DATA_FORMAT_VERSION}"
 )
 ENV_PREFIX = "BOOKSHELF_"
```

### Comparing `bookshelf-0.2.2/src/bookshelf/errors.py` & `bookshelf-0.2.3/src/bookshelf/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 """
 Custom exceptions
 """
 
+from typing import Optional
+
 
 class UnknownBook(ValueError):
     """
     An unknown book is requested
     """
 
 
 class UnknownVersion(ValueError):
     """
     An unknown version is requested
     """
 
-    def __init__(self, name, version):
+    def __init__(self, name: str, version: Optional[str]):
         self.name = name
         self.version = version
         super().__init__()
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"Could not find {self.name}@{self.version}"
 
 
 class UnknownEdition(UnknownVersion):
     """
     An unknown edition is requested
     """
 
-    def __init__(self, name, version, edition):
+    def __init__(self, name: str, version: str, edition: int):
         super().__init__(name, version)
         self.edition = edition
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"Could not find {self.name}@{self.version} ed.{self.version}"
 
 
 class UploadError(ValueError):
     """
     Could not upload a book to the remote bookshelf
     """
```

### Comparing `bookshelf-0.2.2/src/bookshelf/notebook.py` & `bookshelf-0.2.3/src/bookshelf/notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """
 Functions to run/manage notebooks
 """
 import logging
 import os
 import shutil
-from typing import Any, Dict, Optional, Tuple
+from typing import Any, Optional
 
-# pylint: disable=invalid-name
 try:
     import jupytext
 
     has_jupytext = True
 except ImportError:  # pragma: no cover
     jupytext = None
     has_jupytext = False
-# pylint: disable=invalid-name
 try:
     import papermill
 
     has_papermill = True
 except ImportError:  # pragma: no cover
     papermill = None
     has_papermill = False
@@ -65,15 +63,15 @@
 
     return nb_directory
 
 
 def _load_nb_config(
     name: str,
     nb_directory: Optional[str] = None,
-) -> Tuple[ConfigSchema, Dict[str, Any]]:
+) -> tuple[ConfigSchema, dict[str, Any]]:
     nb_directory = get_notebook_directory(nb_directory)
 
     metadata_fname = name
     if nb_directory and not os.path.isabs(name):
         metadata_fname = os.path.join(nb_directory, name)
 
     # If a directory is provided assume that the config is similarly named
@@ -98,15 +96,15 @@
     name: str,
     version: Optional[Version] = None,
     nb_directory: Optional[str] = None,
 ) -> NotebookMetadata:
     """
     Load notebook metadata
 
-    Attempts to search :param:`nb_directory` for a metadata YAML file. This YAML file
+    Attempts to search {param}`nb_directory` for a metadata YAML file. This YAML file
     contains information about the dataset that is being processed. See NotebookMetadata
     for a description of the available options.
 
     The assumed filename format for versioned data is {name}_{version}.yaml where
     name matches the notebook name and the name as specified in the NotebookMetadata
 
     Parameters
@@ -183,35 +181,31 @@
 
     Returns
     -------
     LocalBook
         The generated book
     """
     if not has_papermill:
-        raise ImportError(
-            "papermill is not installed. Run 'pip install bookshelf[notebooks]'"
-        )
+        raise ImportError("papermill is not installed. Run 'pip install bookshelf[notebooks]'")
     if not has_jupytext:
-        raise ImportError(
-            "jupytext is not installed. Run 'pip install bookshelf[notebooks]'"
-        )
+        raise ImportError("jupytext is not installed. Run 'pip install bookshelf[notebooks]'")
 
     short_name = name.split("/")[-1]
 
     # Verify metadata
     metadata = load_nb_metadata(name, version=version, nb_directory=nb_directory)
     nb_fname = metadata.source_file.replace(".yaml", ".py")
 
     if not os.path.exists(nb_fname):
         raise FileNotFoundError(f"Could not find notebook: {nb_fname}")
 
     logger.info(f"Loaded metadata from {metadata.source_file}")
     if metadata.name != short_name:  # pragma: no cover
         raise ValueError(
-            f"name in metadata does not match the name of the notebook "
+            "name in metadata does not match the name of the notebook "
             f"({metadata.name} != {name}"
         )
     logger.info(f"Processing {metadata.long_name()}")
 
     if output_directory is None:
         output_directory = os.path.join(PROCESSED_DATA_DIR, short_name)
 
@@ -247,15 +241,15 @@
     shelf = BookShelf(path=output_directory)
     book = shelf.load(short_name, metadata.version, edition=metadata.edition)
 
     logger.info(f"Notebook run successfully with hash: {book.hash()}")
     return book
 
 
-def get_available_versions(name: str, include_private: bool = False) -> list[str]:
+def get_available_versions(name: str, include_private: bool = False) -> tuple[str, ...]:
     """
     Get a list of available versions of a book
 
     Parameters
     ----------
     name
         Package name
@@ -268,8 +262,8 @@
     """
     config, _ = _load_nb_config(name)
 
     versions = config.versions
     if not include_private:
         versions = [v for v in versions if not v.private]
 
-    return [v.version for v in versions]
+    return tuple(v.version for v in versions)
```

### Comparing `bookshelf-0.2.2/src/bookshelf/schema.py` & `bookshelf-0.2.3/src/bookshelf/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Schema
 """
-from typing import Any, Dict, List, Optional
+from typing import Any, Optional
 
 import pooch
-from pydantic import BaseModel, Field  # pylint: disable=no-name-in-module
+from pydantic import BaseModel, Field
 
 from bookshelf.utils import get_env_var
 
 Version = str
 Edition = int
 
 
@@ -27,15 +27,15 @@
 class VolumeMeta(BaseModel):
     """
     Schema for a given Volume (A collection of Books with the same name)
     """
 
     name: str
     license: str  # A change in license will require a new volume
-    versions: List[BookVersion]
+    versions: list[BookVersion]
 
     def get_latest_version(self) -> Version:
         """
         Get the latest version for a volume
 
         Returns
         -------
@@ -43,15 +43,15 @@
         """
         ordered_versions = sorted([v.version for v in self.versions if not v.private])
         if not ordered_versions:
             raise ValueError("No published volumes")
 
         return ordered_versions[-1]
 
-    def get_version(self, version: Version) -> List[BookVersion]:
+    def get_version(self, version: Version) -> list[BookVersion]:
         """
         Get a set of books for a given version
 
         Returns
         -------
         List of matching books sorted by edition
         """
@@ -79,15 +79,15 @@
     Metadata about a dataset
 
     A dataset may consist of multiple files (:class:`FileDownloadInfo`)
     """
 
     url: Optional[str]
     doi: Optional[str]
-    files: List[FileDownloadInfo]
+    files: list[FileDownloadInfo]
     author: str
 
 
 class VersionMetadata(BaseModel):
     """
     Metadata about a single version of a book
     """
@@ -107,15 +107,15 @@
     name: str
     version: Version
     edition: Edition
     description: Optional[str]
     license: str
     source_file: str
     private: bool
-    metadata: Dict[str, Any]  # TODO: type this
+    metadata: dict[str, Any]  # TODO: type this
     dataset: DatasetMetadata
 
     def long_name(self) -> str:
         """
         Long name of the book
 
         Includes name and long version
@@ -188,9 +188,9 @@
     """
 
     name: str
     edition: Edition
     description: Optional[str]
     license: str
     source_file: str
-    metadata: Dict[str, Any]  # TODO: type this
-    versions: List[VersionMetadata]
+    metadata: dict[str, Any]  # TODO: type this
+    versions: list[VersionMetadata]
```

### Comparing `bookshelf-0.2.2/src/bookshelf/shelf.py` & `bookshelf-0.2.3/src/bookshelf/shelf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 A BookShelf is a collection of Books that can be queried and fetched as needed.
 """
 import json
 import logging
 import os
 import pathlib
-from typing import Iterable, List, Optional, Tuple, Union, cast
+from collections.abc import Iterable
+from typing import TYPE_CHECKING, Optional, Union, cast
 
 import boto3
 import boto3.exceptions
 import datapackage
 import requests.exceptions
 
 from bookshelf.book import LocalBook
@@ -19,14 +20,18 @@
     build_url,
     create_local_cache,
     fetch_file,
     get_env_var,
     get_remote_bookshelf,
 )
 
+if TYPE_CHECKING:
+    from mypy_boto3_s3.client import S3Client
+
+
 logger = logging.getLogger(__name__)
 
 
 def _fetch_volume_meta(
     name: str,
     remote_bookshelf: str,
     local_bookshelf: pathlib.Path,
@@ -61,21 +66,22 @@
 
     with open(str(local_fname)) as file_handle:
         data = json.load(file_handle)
 
     return VolumeMeta(**data)
 
 
-def _upload_file(s3, bucket, key, fname):  # pylint: disable=invalid-name
+def _upload_file(s3: "S3Client", bucket: str, key: str, fname: str) -> None:
     try:
         logger.info(f"Uploading {fname} to {bucket} - {key}")
         s3.upload_file(fname, bucket, key, ExtraArgs={"ACL": "public-read"})
     except boto3.exceptions.S3UploadFailedError as s3_error:
-        logger.exception(s3_error, exc_info=False)
-        raise UploadError(f"Failed to upload {fname} to s3") from s3_error
+        msg = f"Failed to upload {fname} to s3"
+        logger.exception(msg)
+        raise UploadError(msg) from s3_error
 
 
 def _update_volume_meta(book: LocalBook, remote_bookshelf: str) -> str:
     try:
         volume_meta = _fetch_volume_meta(
             book.name, remote_bookshelf, book.local_bookshelf, force=True
         )
@@ -159,17 +165,15 @@
         -------
         :class:`LocalBook`
             A book from which the resources can be accessed
         """
         if version is None or edition is None or force:
             version, edition = self._resolve_version(name, version, edition)
 
-        metadata_fragment = LocalBook.relative_path(
-            name, version, edition, "datapackage.json"
-        )
+        metadata_fragment = LocalBook.relative_path(name, version, edition, "datapackage.json")
         metadata_fname = self.path / metadata_fragment
 
         if not metadata_fname.exists():
             try:
                 url = build_url(
                     self.remote_bookshelf,
                     *LocalBook.path_parts(name, version, edition, "datapackage.json"),
@@ -180,15 +184,15 @@
                     known_hash=None,
                     force=force,
                 )
             except requests.exceptions.HTTPError as http_error:
                 raise UnknownVersion(name, version) from http_error
 
         if not metadata_fname.exists():
-            raise AssertionError()  # noqa
+            raise AssertionError()
 
         return LocalBook(name, version, edition, local_bookshelf=self.path)
 
     def is_available(
         self,
         name: str,
         version: Optional[Version] = None,
@@ -210,17 +214,17 @@
         Returns
         -------
         bool
             True if a Book with a matching name and version exists on the remote bookshelf
         """
         try:
             self._resolve_version(name, version, edition)
-            return True
         except (UnknownBook, UnknownVersion, UnknownEdition):
             return False
+        return True
 
     def is_cached(self, name: str, version: Version, edition: Edition) -> bool:
         """
         Check if a book with a matching name/version is cached on the local bookshelf
 
         Parameters
         ----------
@@ -236,17 +240,17 @@
         bool
             True if a matching book is cached locally
         """
         try:
             # Check if the metadata for the book can be successfully read
             book = LocalBook(name, version, edition, local_bookshelf=self.path)
             book.metadata()
-            return True
         except FileNotFoundError:
             return False
+        return True
 
     def publish(self, book: LocalBook, force: bool = False) -> None:
         """
         Publish a book to the remote bookshelf
 
         Parameters
         ----------
@@ -262,16 +266,16 @@
             more information about how to resolve this issue.
         """
         if self.is_available(book.name, book.version):
             remote_book = self.load(book.name, book.version)
 
             if remote_book.edition >= book.edition:
                 msg = (
-                    f"Edition value has not been increased "
-                    f"(remote: {remote_book.long_version()}, local: {book.long_version()})"
+                    "Edition value has not been increased (remote:"
+                    f" {remote_book.long_version()}, local: {book.long_version()})"
                 )
                 if not force:
                     raise UploadError(msg)
                 logger.error(msg)
             logger.warning("Uploading a new edition of an existing book")
         files = book.files()
 
@@ -287,15 +291,15 @@
                 continue
             if fname not in resource_fnames:
                 raise UploadError(f"Non-resource file {fname} found in book")
 
         # Upload using boto3 by default for testing
         # Maybe support other upload methods in future
 
-        s3 = boto3.client("s3")  # pylint: disable=invalid-name
+        s3 = boto3.client("s3")
         bucket = get_env_var("BUCKET", add_prefix=True)
         prefix = get_env_var("BUCKET_PREFIX", add_prefix=True)
 
         logger.info(f"Beginning to upload {book.name}@{book.version}")
         for resource_file in files:
             key = "/".join(
                 (
@@ -310,24 +314,22 @@
         # Update the metadata with the latest version information
         # Note that this doesn't have any guardrails and is susceptible to race conditions
         # Shouldn't be a problem for testing, but shouldn't be used in production
         meta_fname = _update_volume_meta(book, self.remote_bookshelf)
         key = "/".join((prefix, book.name, os.path.basename(meta_fname)))
         _upload_file(s3, bucket, key, meta_fname)
 
-        logger.info(
-            f"Book {book.name}@{book.version} ed.{book.edition} uploaded successfully"
-        )
+        logger.info(f"Book {book.name}@{book.version} ed.{book.edition} uploaded successfully")
 
     def _resolve_version(
         self,
         name: str,
         version: Optional[Version] = None,
         edition: Optional[Edition] = None,
-    ) -> Tuple[Version, Edition]:
+    ) -> tuple[Version, Edition]:
         # Update the package metadata
         try:
             meta = _fetch_volume_meta(name, self.remote_bookshelf, self.path)
         except requests.exceptions.HTTPError as http_error:
             raise UnknownBook(f"No metadata for {repr(name)}") from http_error
 
         if version is None:
@@ -341,15 +343,15 @@
         # Find edition
         if edition is None:
             edition = matching_version_books[-1].edition
         if edition not in [b.edition for b in matching_version_books]:
             raise UnknownEdition(name, version, edition)
         return version, edition
 
-    def list_versions(self, name: str) -> List[str]:
+    def list_versions(self, name: str) -> list[str]:
         """
         Get a list of available versions for a given Book
 
         Parameters
         ----------
         name: str
             Name of book
@@ -362,15 +364,15 @@
         try:
             meta = _fetch_volume_meta(name, self.remote_bookshelf, self.path)
         except requests.exceptions.HTTPError as http_error:
             raise UnknownBook(f"No metadata for {repr(name)}") from http_error
 
         return [version.version for version in meta.versions if not version.private]
 
-    def list_books(self) -> List[str]:
+    def list_books(self) -> list[str]:
         """
         Get a list of book names
 
         Returns
         -------
         list of str
             List of available books
```

### Comparing `bookshelf-0.2.2/src/bookshelf/utils.py` & `bookshelf-0.2.3/src/bookshelf/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 logger = logging.getLogger(__file__)
 
 
 def default_cache_location() -> str:
     r"""
     Determine the default cache location
 
-
     By default, local Books are stored in the default cache location unless overridden for
     a given :class:`bookshelf.BookShelf`. The default cache location is determined using
     the ``BOOKSHELF_CACHE_LOCATION`` or if that environment variable is not present, it
     falls back to an operating specific location. This location is determined using
     `appdirs <https://github.com/ActiveState/appdirs>`__ and may look like the following:
 
     * Mac: ``~/Library/Caches/bookshelf``
@@ -161,17 +160,15 @@
         )
 
     if force or not local_fname.exists():
         download(url, local_fname=local_fname, known_hash=known_hash)
         logger.info(f"{local_fname} downloaded from {url}")
 
     if not local_fname.exists():
-        raise FileNotFoundError(
-            f"Could not find file {local_fname}"
-        )  # pragma: no cover
+        raise FileNotFoundError(f"Could not find file {local_fname}")  # pragma: no cover
 
 
 def get_env_var(
     name: str,
     add_prefix: bool = True,
     raise_on_missing: bool = True,
     default: Any = None,
```

