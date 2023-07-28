# Comparing `tmp/nexia-2.0.6.tar.gz` & `tmp/nexia-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexia-2.0.6.tar", last modified: Thu Nov  3 12:50:03 2022, max compression
+gzip compressed data, was "nexia-2.0.7.tar", last modified: Fri Jul 28 20:52:30 2023, max compression
```

## Comparing `nexia-2.0.6.tar` & `nexia-2.0.7.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2022-11-03 12:50:03.245812 nexia-2.0.6/
--rw-r--r--   0 bdraco     (501) staff       (20)      354 2022-07-07 01:00:50.000000 nexia-2.0.6/.coveragerc
--rw-r--r--   0 bdraco     (501) staff       (20)      292 2022-07-07 01:00:50.000000 nexia-2.0.6/.editorconfig
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2022-11-03 12:50:03.233648 nexia-2.0.6/.github/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2022-11-03 12:50:03.237645 nexia-2.0.6/.github/workflows/
--rw-r--r--   0 bdraco     (501) staff       (20)     1417 2022-10-13 22:18:50.000000 nexia-2.0.6/.github/workflows/ci.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)     1196 2022-07-07 01:00:50.000000 nexia-2.0.6/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)      219 2022-07-07 01:00:50.000000 nexia-2.0.6/AUTHORS.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      610 2022-07-07 01:00:50.000000 nexia-2.0.6/CHANGELOG.md
--rw-r--r--   0 bdraco     (501) staff       (20)     3478 2022-07-07 01:00:50.000000 nexia-2.0.6/CONTRIBUTING.rst
--rw-r--r--   0 bdraco     (501) staff       (20)       89 2022-07-07 01:00:50.000000 nexia-2.0.6/HISTORY.rst
--rw-r--r--   0 bdraco     (501) staff       (20)    11357 2022-07-07 01:00:50.000000 nexia-2.0.6/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      262 2022-07-07 01:00:50.000000 nexia-2.0.6/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     2201 2022-07-07 01:00:50.000000 nexia-2.0.6/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     1740 2022-11-03 12:50:03.245894 nexia-2.0.6/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)    13540 2022-07-07 01:00:50.000000 nexia-2.0.6/README.md
--rw-r--r--   0 bdraco     (501) staff       (20)      987 2022-07-07 01:00:50.000000 nexia-2.0.6/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)       66 2022-07-07 01:00:50.000000 nexia-2.0.6/build.sh
--rw-r--r--   0 bdraco     (501) staff       (20)     1420 2022-07-07 01:00:50.000000 nexia-2.0.6/delete_mobile_phones.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2022-11-03 12:50:03.239835 nexia-2.0.6/docs/
--rw-r--r--   0 bdraco     (501) staff       (20)      606 2022-07-07 01:00:50.000000 nexia-2.0.6/docs/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)       28 2022-07-07 01:00:50.000000 nexia-2.0.6/docs/authors.rst
--rw-r--r--   0 bdraco     (501) staff       (20)     4758 2022-07-07 01:00:50.000000 nexia-2.0.6/docs/conf.py
--rw-r--r--   0 bdraco     (501) staff       (20)       33 2022-07-07 01:00:50.000000 nexia-2.0.6/docs/contributing.rst
--rw-r--r--   0 bdraco     (501) staff       (20)       28 2022-07-07 01:00:50.000000 nexia-2.0.6/docs/history.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      302 2022-07-07 01:00:50.000000 nexia-2.0.6/docs/index.rst
--rw-r--r--   0 bdraco     (501) staff       (20)     1090 2022-07-07 01:00:50.000000 nexia-2.0.6/docs/installation.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      767 2022-07-07 01:00:50.000000 nexia-2.0.6/docs/make.bat
--rw-r--r--   0 bdraco     (501) staff       (20)       27 2022-07-07 01:00:50.000000 nexia-2.0.6/docs/readme.rst
--rw-r--r--   0 bdraco     (501) staff       (20)       65 2022-07-07 01:00:50.000000 nexia-2.0.6/docs/usage.rst
--rw-r--r--   0 bdraco     (501) staff       (20)     1223 2022-07-07 01:00:50.000000 nexia-2.0.6/dump_home_json.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1683 2022-07-07 01:00:50.000000 nexia-2.0.6/main.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2022-11-03 12:50:03.241133 nexia-2.0.6/nexia/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2022-11-03 12:50:03.242381 nexia-2.0.6/nexia/.github/
--rw-r--r--   0 bdraco     (501) staff       (20)      316 2022-07-07 01:00:50.000000 nexia-2.0.6/nexia/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 bdraco     (501) staff       (20)       35 2022-07-07 01:00:50.000000 nexia-2.0.6/nexia/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2393 2022-07-07 01:00:50.000000 nexia-2.0.6/nexia/automation.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1676 2022-07-07 01:00:50.000000 nexia-2.0.6/nexia/const.py
--rw-r--r--   0 bdraco     (501) staff       (20)    16925 2022-10-13 22:18:50.000000 nexia-2.0.6/nexia/home.py
--rw-r--r--   0 bdraco     (501) staff       (20)    23732 2022-11-03 12:47:47.000000 nexia-2.0.6/nexia/thermostat.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1595 2022-10-13 22:18:50.000000 nexia-2.0.6/nexia/util.py
--rw-r--r--   0 bdraco     (501) staff       (20)    18174 2022-10-27 03:51:10.000000 nexia-2.0.6/nexia/zone.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2022-11-03 12:50:03.242267 nexia-2.0.6/nexia.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     1740 2022-11-03 12:50:03.000000 nexia-2.0.6/nexia.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1256 2022-11-03 12:50:03.000000 nexia-2.0.6/nexia.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2022-11-03 12:50:03.000000 nexia-2.0.6/nexia.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2022-07-07 01:04:58.000000 nexia-2.0.6/nexia.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       15 2022-11-03 12:50:03.000000 nexia-2.0.6/nexia.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2022-11-03 12:50:03.000000 nexia-2.0.6/nexia.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      989 2022-07-07 01:00:50.000000 nexia-2.0.6/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       29 2022-07-07 01:00:50.000000 nexia-2.0.6/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      215 2022-10-13 22:18:50.000000 nexia-2.0.6/requirements_dev.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       74 2022-07-07 01:00:50.000000 nexia-2.0.6/requirements_tests.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      810 2022-11-03 12:50:03.246219 nexia-2.0.6/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1332 2022-11-03 12:49:48.000000 nexia-2.0.6/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2022-11-03 12:50:03.242652 nexia-2.0.6/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)       35 2022-07-07 01:00:50.000000 nexia-2.0.6/tests/__init__.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2022-11-03 12:50:03.245243 nexia-2.0.6/tests/fixtures/
--rw-r--r--   0 bdraco     (501) staff       (20)    49318 2022-07-07 01:00:50.000000 nexia-2.0.6/tests/fixtures/grouped_xl850.json
--rw-r--r--   0 bdraco     (501) staff       (20)    63578 2022-10-13 23:10:34.000000 nexia-2.0.6/tests/fixtures/issue_79891.json
--rw-r--r--   0 bdraco     (501) staff       (20)    81062 2022-07-07 01:00:50.000000 nexia-2.0.6/tests/fixtures/mobile_house_issue_33758.json
--rw-r--r--   0 bdraco     (501) staff       (20)   136860 2022-07-07 01:00:50.000000 nexia-2.0.6/tests/fixtures/mobile_house_issue_33968.json
--rw-r--r--   0 bdraco     (501) staff       (20)   115061 2022-07-07 01:00:50.000000 nexia-2.0.6/tests/fixtures/mobile_house_xl624.json
--rw-r--r--   0 bdraco     (501) staff       (20)   438382 2022-07-07 01:00:50.000000 nexia-2.0.6/tests/fixtures/mobile_houses_123456.json
--rw-r--r--   0 bdraco     (501) staff       (20)    35892 2022-07-07 01:00:50.000000 nexia-2.0.6/tests/fixtures/single_zone_xl1050.json
--rw-r--r--   0 bdraco     (501) staff       (20)    35901 2022-07-07 01:00:50.000000 nexia-2.0.6/tests/fixtures/single_zone_xl1050_system_off.json
--rw-r--r--   0 bdraco     (501) staff       (20)   316308 2022-11-03 12:47:47.000000 nexia-2.0.6/tests/fixtures/system_offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)   727861 2022-10-27 03:51:10.000000 nexia-2.0.6/tests/fixtures/xl1050.json
--rw-r--r--   0 bdraco     (501) staff       (20)    53227 2022-10-27 03:51:10.000000 nexia-2.0.6/tests/fixtures/xl824.json
--rw-r--r--   0 bdraco     (501) staff       (20)    40225 2022-11-03 12:47:47.000000 nexia-2.0.6/tests/test_home.py
--rw-r--r--   0 bdraco     (501) staff       (20)      858 2022-10-13 22:18:50.000000 nexia-2.0.6/tox.ini
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-07-28 20:52:30.248175 nexia-2.0.7/
+-rw-r--r--   0 bdraco     (501) staff       (20)      354 2022-07-07 01:00:50.000000 nexia-2.0.7/.coveragerc
+-rw-r--r--   0 bdraco     (501) staff       (20)      292 2022-07-07 01:00:50.000000 nexia-2.0.7/.editorconfig
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-07-28 20:52:30.240062 nexia-2.0.7/.github/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-07-28 20:52:30.242759 nexia-2.0.7/.github/workflows/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1422 2023-07-28 20:22:43.000000 nexia-2.0.7/.github/workflows/ci.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)     1196 2022-07-07 01:00:50.000000 nexia-2.0.7/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)      219 2022-07-07 01:00:50.000000 nexia-2.0.7/AUTHORS.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      610 2022-07-07 01:00:50.000000 nexia-2.0.7/CHANGELOG.md
+-rw-r--r--   0 bdraco     (501) staff       (20)     3478 2022-07-07 01:00:50.000000 nexia-2.0.7/CONTRIBUTING.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)       89 2022-07-07 01:00:50.000000 nexia-2.0.7/HISTORY.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)    11357 2022-07-07 01:00:50.000000 nexia-2.0.7/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      262 2022-07-07 01:00:50.000000 nexia-2.0.7/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     2201 2022-07-07 01:00:50.000000 nexia-2.0.7/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     1740 2023-07-28 20:52:30.248253 nexia-2.0.7/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)    13540 2022-07-07 01:00:50.000000 nexia-2.0.7/README.md
+-rw-r--r--   0 bdraco     (501) staff       (20)      987 2022-07-07 01:00:50.000000 nexia-2.0.7/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)       66 2022-07-07 01:00:50.000000 nexia-2.0.7/build.sh
+-rw-r--r--   0 bdraco     (501) staff       (20)     1420 2022-07-07 01:00:50.000000 nexia-2.0.7/delete_mobile_phones.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-07-28 20:52:30.243803 nexia-2.0.7/docs/
+-rw-r--r--   0 bdraco     (501) staff       (20)      606 2022-07-07 01:00:50.000000 nexia-2.0.7/docs/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)       28 2022-07-07 01:00:50.000000 nexia-2.0.7/docs/authors.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)     4758 2022-07-07 01:00:50.000000 nexia-2.0.7/docs/conf.py
+-rw-r--r--   0 bdraco     (501) staff       (20)       33 2022-07-07 01:00:50.000000 nexia-2.0.7/docs/contributing.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)       28 2022-07-07 01:00:50.000000 nexia-2.0.7/docs/history.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      302 2022-07-07 01:00:50.000000 nexia-2.0.7/docs/index.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)     1090 2022-07-07 01:00:50.000000 nexia-2.0.7/docs/installation.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      767 2022-07-07 01:00:50.000000 nexia-2.0.7/docs/make.bat
+-rw-r--r--   0 bdraco     (501) staff       (20)       27 2022-07-07 01:00:50.000000 nexia-2.0.7/docs/readme.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)       65 2022-07-07 01:00:50.000000 nexia-2.0.7/docs/usage.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)     1223 2022-07-07 01:00:50.000000 nexia-2.0.7/dump_home_json.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1683 2022-07-07 01:00:50.000000 nexia-2.0.7/main.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-07-28 20:52:30.244462 nexia-2.0.7/nexia/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-07-28 20:52:30.245236 nexia-2.0.7/nexia/.github/
+-rw-r--r--   0 bdraco     (501) staff       (20)      316 2022-07-07 01:00:50.000000 nexia-2.0.7/nexia/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 bdraco     (501) staff       (20)       35 2022-07-07 01:00:50.000000 nexia-2.0.7/nexia/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2393 2022-07-07 01:00:50.000000 nexia-2.0.7/nexia/automation.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1672 2023-07-28 20:22:43.000000 nexia-2.0.7/nexia/const.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    17058 2023-07-28 20:32:13.000000 nexia-2.0.7/nexia/home.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    23749 2023-07-28 20:32:13.000000 nexia-2.0.7/nexia/thermostat.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1595 2022-10-13 22:18:50.000000 nexia-2.0.7/nexia/util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    18174 2022-10-27 03:51:10.000000 nexia-2.0.7/nexia/zone.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-07-28 20:52:30.245121 nexia-2.0.7/nexia.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1740 2023-07-28 20:52:30.000000 nexia-2.0.7/nexia.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1285 2023-07-28 20:52:30.000000 nexia-2.0.7/nexia.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-07-28 20:52:30.000000 nexia-2.0.7/nexia.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2022-07-07 01:04:58.000000 nexia-2.0.7/nexia.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       15 2023-07-28 20:52:30.000000 nexia-2.0.7/nexia.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-07-28 20:52:30.000000 nexia-2.0.7/nexia.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      989 2022-07-07 01:00:50.000000 nexia-2.0.7/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       29 2022-07-07 01:00:50.000000 nexia-2.0.7/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      215 2023-07-28 20:49:50.000000 nexia-2.0.7/requirements_dev.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       74 2022-07-07 01:00:50.000000 nexia-2.0.7/requirements_tests.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      810 2023-07-28 20:52:30.248525 nexia-2.0.7/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1332 2023-07-28 20:51:32.000000 nexia-2.0.7/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-07-28 20:52:30.245478 nexia-2.0.7/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)       35 2022-07-07 01:00:50.000000 nexia-2.0.7/tests/__init__.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-07-28 20:52:30.247983 nexia-2.0.7/tests/fixtures/
+-rw-r--r--   0 bdraco     (501) staff       (20)    57304 2023-07-28 20:17:27.000000 nexia-2.0.7/tests/fixtures/eme_heat.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    49318 2022-07-07 01:00:50.000000 nexia-2.0.7/tests/fixtures/grouped_xl850.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    63578 2022-10-13 23:10:34.000000 nexia-2.0.7/tests/fixtures/issue_79891.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    81062 2022-07-07 01:00:50.000000 nexia-2.0.7/tests/fixtures/mobile_house_issue_33758.json
+-rw-r--r--   0 bdraco     (501) staff       (20)   136860 2022-07-07 01:00:50.000000 nexia-2.0.7/tests/fixtures/mobile_house_issue_33968.json
+-rw-r--r--   0 bdraco     (501) staff       (20)   115061 2022-07-07 01:00:50.000000 nexia-2.0.7/tests/fixtures/mobile_house_xl624.json
+-rw-r--r--   0 bdraco     (501) staff       (20)   438382 2022-07-07 01:00:50.000000 nexia-2.0.7/tests/fixtures/mobile_houses_123456.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    35892 2022-07-07 01:00:50.000000 nexia-2.0.7/tests/fixtures/single_zone_xl1050.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    35901 2022-07-07 01:00:50.000000 nexia-2.0.7/tests/fixtures/single_zone_xl1050_system_off.json
+-rw-r--r--   0 bdraco     (501) staff       (20)   316308 2022-11-03 12:47:47.000000 nexia-2.0.7/tests/fixtures/system_offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)   727861 2022-10-27 03:51:10.000000 nexia-2.0.7/tests/fixtures/xl1050.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    53227 2022-11-03 18:01:52.000000 nexia-2.0.7/tests/fixtures/xl824.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    42417 2023-07-28 20:17:27.000000 nexia-2.0.7/tests/test_home.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      865 2023-07-28 20:22:43.000000 nexia-2.0.7/tox.ini
```

### Comparing `nexia-2.0.6/.github/workflows/ci.yaml` & `nexia-2.0.7/.github/workflows/ci.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   - pull_request
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.9, "3.10"]
+        python-version: [3.9, "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v1
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
@@ -27,22 +27,22 @@
       run: TOXENV=lint tox
 
   coverage:
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        python-version: [3.9]
+        python-version: ["3.10"]
 
     steps:
     - uses: actions/checkout@v1
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
-        python-version: ${{ matrix.python-version }}      
+        python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install tox tox-gh-actions
     - name: Test with tox
       run: TOXENV=codecov tox
     - name: Upload coverage to Codecov
```

### Comparing `nexia-2.0.6/.gitignore` & `nexia-2.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/CHANGELOG.md` & `nexia-2.0.7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/CONTRIBUTING.rst` & `nexia-2.0.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/LICENSE` & `nexia-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/Makefile` & `nexia-2.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/PKG-INFO` & `nexia-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexia
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python library for connecting to nexia
 Home-page: https://github.com/bdraco/nexia
 Author: J. Nick Koston
 Author-email: nick@koston.org
 License: Apache Software License 2.0
 Keywords: nexia
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nexia-2.0.6/README.md` & `nexia-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/README.rst` & `nexia-2.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/delete_mobile_phones.py` & `nexia-2.0.7/delete_mobile_phones.py`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/docs/Makefile` & `nexia-2.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/docs/conf.py` & `nexia-2.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/docs/installation.rst` & `nexia-2.0.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/docs/make.bat` & `nexia-2.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/dump_home_json.py` & `nexia-2.0.7/dump_home_json.py`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/main.py` & `nexia-2.0.7/main.py`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/nexia/automation.py` & `nexia-2.0.7/nexia/automation.py`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/nexia/const.py` & `nexia-2.0.7/nexia/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 BRAND_NEXIA = "nexia"
 BRAND_ASAIR = "asair"
 BRAND_TRANE = "trane"
 
 NEXIA_ROOT_URL = "https://www.mynexia.com"
 NEXIA_IDENTIFIER = "com.tranetechnologies.nexia"
-ASAIR_ROOT_URL = "https://www.asairhome.com"
+ASAIR_ROOT_URL = "https://asairhome.com"
 ASAIR_IDENTIFIER = "com.tranetechnologies.asair"
 TRANE_ROOT_URL = "https://www.tranehome.com"
 TRANE_IDENTIFIER = "com.tranetechnologies.trane"
 
 MOBILE_URL_TEMPLATE = "{}/mobile"
 
 DEFAULT_DEVICE_NAME = "Home Automation"
```

### Comparing `nexia-2.0.6/nexia/home.py` & `nexia-2.0.7/nexia/home.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,19 @@
     MOBILE_URL_TEMPLATE,
     NEXIA_ROOT_URL,
     TRANE_ROOT_URL,
 )
 from .thermostat import NexiaThermostat
 from .util import load_or_create_uuid
 
+
+class LoginFailedException(Exception):
+    """Login failed."""
+
+
 MAX_LOGIN_ATTEMPTS = 4
 TIMEOUT = 20
 
 _LOGGER = logging.getLogger(__name__)
 
 DEVICES_ELEMENT = 0
 AUTOMATIONS_ELEMENT = 1
@@ -221,16 +226,16 @@
         :param error_text: str
         :param request: response
         :return: None
         """
         if request is None or request.status != 200:
             if request is not None:
                 text = await request.text()
-                raise Exception(f"{error_text}\n{text}")
-            raise Exception(f"No response from session. {error_text}")
+                raise ValueError(f"{error_text}\n{text}")
+            raise ValueError(f"No response from session. {error_text}")
 
     async def _find_house_id(self) -> None:
         """Finds the house id if none is provided."""
         request = await self.post_url(
             self.API_MOBILE_SESSION_URL,
             {"app_version": APP_VERSION, "device_uuid": str(self._uuid)},
         )
@@ -239,37 +244,37 @@
                 loads=orjson.loads  # pylint: disable=no-member
             )
             if ts_json:
                 data = ts_json["result"]["_links"]["child"][0]["data"]
                 self.house_id = data["id"]
                 self._name = data["name"]
             else:
-                raise Exception("Nothing in the JSON")
+                raise ValueError("Nothing in the JSON")
         else:
             await self._check_response(
                 "Failed to get house id JSON, session probably timed out",
                 request,
             )
 
     def update_from_json(self, json_dict: dict[str, Any]) -> None:
         """Update the json from the houses endpoint if fetched externally."""
         self._name = json_dict["result"]["name"]
         self.devices_json = _extract_devices_from_houses_json(json_dict)
         self.automations_json = _extract_automations_from_houses_json(json_dict)
         self._update_devices()
         self._update_automations()
 
-    async def update(self, force_update: bool = True) -> None:
+    async def update(self, force_update: bool = True) -> dict[str, Any] | None:
         """
         Forces a status update from nexia
         :return: None
         """
         if not self.mobile_id:
             # not yet authenticated
-            return
+            return None
 
         headers = {}
         if self._last_update_etag:
             headers["If-None-Match"] = self._last_update_etag
 
         response = await self._get_url(
             self.API_MOBILE_HOUSES_URL.format(house_id=self.house_id), headers=headers
@@ -295,18 +300,18 @@
         ts_json = await response.json()
         if ts_json:
             self._name = ts_json["result"]["name"]
             self.devices_json = _extract_devices_from_houses_json(ts_json)
             self.automations_json = _extract_automations_from_houses_json(ts_json)
             self._last_update_etag = response.headers.get("etag")
         else:
-            raise Exception("Nothing in the JSON")
+            raise ValueError("Nothing in the JSON")
         self._update_devices()
         self._update_automations()
-        return
+        return ts_json
 
     def _update_devices(self):
         self.last_update = datetime.datetime.now()
         children = []
         for child in self.devices_json:
             type_ = child.get("type")
             if not type_ or "thermostat" in type_:
@@ -385,30 +390,30 @@
             request = await self.post_url(self.API_MOBILE_ACCOUNTS_SIGN_IN_URL, payload)
 
             if request is None or request.status not in (302, 200):
                 self.login_attempts_left -= 1
             await self._check_response("Failed to login", request)
 
             if request.url == self.AUTH_FORGOTTEN_PASSWORD_STRING:
-                raise Exception(
+                raise LoginFailedException(
                     f"Failed to login, getting redirected to {request.url}"
                     f". Try to login manually on the website."
                 )
 
             json_dict = await request.json(
                 loads=orjson.loads  # pylint: disable=no-member
             )
             if json_dict.get("success") is not True:
                 error_text = json_dict.get("error", "Unknown Error")
-                raise Exception(f"Failed to login, {error_text}")
+                raise LoginFailedException(f"Failed to login, {error_text}")
 
             self.mobile_id = json_dict["result"]["mobile_id"]
             self.api_key = json_dict["result"]["api_key"]
         else:
-            raise Exception(
+            raise LoginFailedException(
                 f"Failed to login after {MAX_LOGIN_ATTEMPTS} attempts! Any "
                 f"more attempts may lock your account!"
             )
 
         if not self.house_id:
             await self._find_house_id()
```

### Comparing `nexia-2.0.6/nexia/thermostat.py` & `nexia-2.0.7/nexia/thermostat.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     @property
     def is_online(self):
         """
         Returns whether the thermostat is online or not.
         :return: bool
         """
-        return self.get_system_status().upper() != 'NOT CONNECTED'
+        return self.get_system_status().upper() != "NOT CONNECTED"
 
     def _get_thermostat_advanced_info_label(self, label):
         """
         Lookup advanced_info in the thermostat features and find the value of the
         requested label.
         """
         advanced_info = self._get_thermostat_features_key("advanced_info")
@@ -235,15 +235,15 @@
     def is_emergency_heat_active(self):
         """
         Returns True if the emergency/aux heat is active
         :return: bool
         """
         if self.has_emergency_heat():
             return self.get_thermostat_settings_key("emergency_heat")["current_value"]
-        raise Exception("This system does not support emergency heat")
+        raise RuntimeError("This system does not support emergency heat")
 
     ########################################################################
     # System Universal Get Methods
 
     def get_fan_modes(self):
         """
         Returns the list of fan modes the device supports
@@ -272,29 +272,29 @@
         :return: float - the temperature, returns nan if invalid
         """
         if self.has_outdoor_temperature():
             outdoor_temp = self._get_thermostat_key("outdoor_temperature")
             if is_number(outdoor_temp):
                 return float(outdoor_temp)
             return float("Nan")
-        raise Exception("This system does not have an outdoor temperature sensor")
+        raise RuntimeError("This system does not have an outdoor temperature sensor")
 
     def get_relative_humidity(self):
         """
         Returns the indoor relative humidity as a percent (0-1)
         :return: float
         """
         if self.has_relative_humidity():
             try:
                 return float(self._get_thermostat_key("indoor_humidity")) / 100
             except ValueError:
                 # this has the value "--" when data is unavailable
                 return None
 
-        raise Exception("This system does not have a relative humidity sensor.")
+        raise RuntimeError("This system does not have a relative humidity sensor.")
 
     def get_current_compressor_speed(self):
         """
         Returns the variable compressor speed, if supported, as a percent (0-1)
         :return: float
         """
         thermostat_compressor_speed = self._get_thermostat_features_key_or_none(
@@ -441,15 +441,15 @@
         :return: None
         """
         if self.has_emergency_heat():
             await self._post_and_update_thermostat_json(
                 "emergency_heat", {"value": "true" if emergency_heat_on else "false"}
             )
         else:
-            raise Exception("This thermostat does not support emergency heat.")
+            raise RuntimeError("This thermostat does not support emergency heat.")
 
     async def set_humidity_setpoints(self, **kwargs):
         """
 
         :param dehumidify_setpoint: float - The dehumidify_setpoint, 0-1, disable: None
         :param humidify_setpoint: float - The humidify setpoint, 0-1, disable: None
         :return:
@@ -459,35 +459,35 @@
         humidify_setpoint = kwargs.get("humidify_setpoint", None)
 
         if dehumidify_setpoint is None and humidify_setpoint is None:
             # Do nothing
             return
 
         if not self.has_relative_humidity():
-            raise Exception(
+            raise RuntimeError(
                 "Setting target humidity is not supported on this thermostat."
             )
         (min_humidity, max_humidity) = self.get_humidity_setpoint_limits()
         if self.has_humidify_support():
             humidify_supported = True
             if humidify_setpoint is None:
                 humidify_setpoint = self.get_humidify_setpoint()
         else:
             if humidify_setpoint is not None:
-                raise SystemError("This thermostat does not support humidifying.")
+                raise RuntimeError("This thermostat does not support humidifying.")
             humidify_supported = False
             humidify_setpoint = 0
 
         if self.has_dehumidify_support():
             dehumidify_supported = True
             if dehumidify_setpoint is None:
                 dehumidify_setpoint = self.get_dehumidify_setpoint()
         else:
             if dehumidify_setpoint is not None:
-                raise SystemError("This thermostat does not support dehumidifying.")
+                raise RuntimeError("This thermostat does not support dehumidifying.")
             dehumidify_supported = False
             dehumidify_setpoint = 0
 
         # Clean up input
         dehumidify_setpoint = find_humidity_setpoint(dehumidify_setpoint)
         humidify_setpoint = find_humidity_setpoint(humidify_setpoint)
```

### Comparing `nexia-2.0.6/nexia/util.py` & `nexia-2.0.7/nexia/util.py`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/nexia/zone.py` & `nexia-2.0.7/nexia/zone.py`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/nexia.egg-info/PKG-INFO` & `nexia-2.0.7/nexia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexia
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python library for connecting to nexia
 Home-page: https://github.com/bdraco/nexia
 Author: J. Nick Koston
 Author-email: nick@koston.org
 License: Apache Software License 2.0
 Keywords: nexia
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nexia-2.0.6/nexia.egg-info/SOURCES.txt` & `nexia-2.0.7/nexia.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 nexia.egg-info/dependency_links.txt
 nexia.egg-info/not-zip-safe
 nexia.egg-info/requires.txt
 nexia.egg-info/top_level.txt
 nexia/.github/ISSUE_TEMPLATE.md
 tests/__init__.py
 tests/test_home.py
+tests/fixtures/eme_heat.json
 tests/fixtures/grouped_xl850.json
 tests/fixtures/issue_79891.json
 tests/fixtures/mobile_house_issue_33758.json
 tests/fixtures/mobile_house_issue_33968.json
 tests/fixtures/mobile_house_xl624.json
 tests/fixtures/mobile_houses_123456.json
 tests/fixtures/single_zone_xl1050.json
```

### Comparing `nexia-2.0.6/pylintrc` & `nexia-2.0.7/pylintrc`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/setup.cfg` & `nexia-2.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.0.6
+current_version = 2.0.7
 commit = True
 tag = True
 tag_name = {new_version}
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `nexia-2.0.6/setup.py` & `nexia-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     keywords="nexia",
     name="nexia",
     packages=find_packages(include=["nexia", "nexia.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/bdraco/nexia",
-    version="2.0.6",
+    version="2.0.7",
     zip_safe=False,
 )
```

### Comparing `nexia-2.0.6/tests/fixtures/grouped_xl850.json` & `nexia-2.0.7/tests/fixtures/grouped_xl850.json`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/tests/fixtures/issue_79891.json` & `nexia-2.0.7/tests/fixtures/issue_79891.json`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/tests/fixtures/mobile_house_issue_33758.json` & `nexia-2.0.7/tests/fixtures/mobile_house_issue_33758.json`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/tests/fixtures/mobile_house_issue_33968.json` & `nexia-2.0.7/tests/fixtures/mobile_house_issue_33968.json`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/tests/fixtures/mobile_house_xl624.json` & `nexia-2.0.7/tests/fixtures/mobile_house_xl624.json`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/tests/fixtures/mobile_houses_123456.json` & `nexia-2.0.7/tests/fixtures/mobile_houses_123456.json`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/tests/fixtures/single_zone_xl1050.json` & `nexia-2.0.7/tests/fixtures/single_zone_xl1050.json`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/tests/fixtures/single_zone_xl1050_system_off.json` & `nexia-2.0.7/tests/fixtures/single_zone_xl1050_system_off.json`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/tests/fixtures/system_offline.json` & `nexia-2.0.7/tests/fixtures/system_offline.json`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/tests/fixtures/xl1050.json` & `nexia-2.0.7/tests/fixtures/xl1050.json`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/tests/fixtures/xl824.json` & `nexia-2.0.7/tests/fixtures/xl824.json`

 * *Files identical despite different names*

### Comparing `nexia-2.0.6/tests/test_home.py` & `nexia-2.0.7/tests/test_home.py`

 * *Files 2% similar despite different names*

```diff
@@ -959,7 +959,59 @@
     assert zone.get_requested_mode() == "COOL"
     assert zone.get_presets() == ["None", "Home", "Away", "Sleep"]
     assert zone.get_preset() == "None"
     assert zone.get_status() == "Damper Open"
     assert zone.get_setpoint_status() == "Permanent Hold"
     assert zone.is_calling() is True
     assert zone.is_in_permanent_hold() is True
+
+
+
+async def test_emergency_heat(aiohttp_session):
+    """Test emergency heat."""
+    nexia = NexiaHome(aiohttp_session)
+    devices_json = json.loads(await load_fixture("eme_heat.json"))
+    nexia.update_from_json(devices_json)
+
+    thermostat_ids = nexia.get_thermostat_ids()
+    assert thermostat_ids == [3983351]
+
+    # Thermostat 1
+    thermostat = nexia.get_thermostat_by_id(3983351)
+    assert thermostat.get_model() == "XL850"
+    assert thermostat.get_firmware() == "5.9.6"
+    assert thermostat.get_dev_build_number() == "1614581867"
+    assert thermostat.get_device_id() == "00D68470"
+    assert thermostat.get_type() == "XL850"
+    assert thermostat.get_name() == 'XL850 Home'
+    assert thermostat.get_deadband() == 3
+    assert thermostat.get_setpoint_limits() == (55, 99)
+    assert thermostat.has_variable_fan_speed() is True
+    assert thermostat.get_unit() == "F"
+    assert thermostat.get_humidity_setpoint_limits() == (0.35, 0.65)
+    assert thermostat.get_fan_mode() == "On"
+    assert thermostat.get_fan_modes() == ["Auto", "On", "Circulate"]
+    assert thermostat.get_current_compressor_speed() == 0
+    assert thermostat.get_requested_compressor_speed() == 0
+    assert thermostat.has_dehumidify_support() is True
+    assert thermostat.has_humidify_support() is True
+    assert thermostat.has_emergency_heat() is True
+    assert thermostat.get_system_status() == 'Fan Running'
+    assert thermostat.has_air_cleaner() is True
+    assert thermostat.is_blower_active() is True
+    assert thermostat.is_online is True
+
+    zone_ids = thermostat.get_zone_ids()
+    assert zone_ids == [84326108]
+    zone = thermostat.get_zone_by_id(84326108)
+
+    assert zone.get_name() ==  'XL850 Home NativeZone'
+    assert zone.get_cooling_setpoint() == 99
+    assert zone.get_heating_setpoint() == 68
+    assert zone.get_current_mode() == "HEAT"
+    assert zone.get_requested_mode() == "HEAT"
+    assert zone.get_presets() == ["None", "Home", "Away", "Sleep"]
+    assert zone.get_preset() == "None"
+    assert zone.get_status() == "Idle"
+    assert zone.get_setpoint_status() == "Run Schedule - None"
+    assert zone.is_calling() is True
+    assert zone.is_in_permanent_hold() is False
```

### Comparing `nexia-2.0.6/tox.ini` & `nexia-2.0.7/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tox]
-envlist = py39, py310, lint
+envlist = py39, py310, py311, lint
 skip_missing_interpreters = True
 
 [testenv]
 setenv =
     PYTHONPATH = {toxinidir}:{toxinidir}/nexia
-whitelist_externals = /usr/bin/env
+allowlist_externals = /usr/bin/env
 install_command = /usr/bin/env LANG=C.UTF-8 pip install {opts} {packages}
 commands =
     py.test --basetemp={envtmpdir} --cov --cov-report term-missing
 deps =
     -r{toxinidir}/requirements.txt
     -r{toxinidir}/requirements_tests.txt
 
 [testenv:codecov]
 setenv =
     PYTHONPATH = {toxinidir}:{toxinidir}/nexia
-whitelist_externals = /usr/bin/env
+allowlist_externals = /usr/bin/env
 install_command = /usr/bin/env LANG=C.UTF-8 pip install {opts} {packages}
 deps =
     -r{toxinidir}/requirements.txt
     -r{toxinidir}/requirements_tests.txt
 commands =
     pytest --cov --cov-report=xml {posargs}
```

