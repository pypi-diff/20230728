# Comparing `tmp/pollination-direct-sun-hours.express-0.5.17.tar.gz` & `tmp/pollination-direct-sun-hours.express-0.5.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pollination-direct-sun-hours.express-0.5.17.tar", last modified: Thu Jul 27 19:18:42 2023, max compression
+gzip compressed data, was "pollination-direct-sun-hours.express-0.5.18.tar", last modified: Fri Jul 28 14:20:09 2023, max compression
```

## Comparing `pollination-direct-sun-hours.express-0.5.17.tar` & `pollination-direct-sun-hours.express-0.5.18.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:18:42.896944 pollination-direct-sun-hours.express-0.5.17/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:18:42.892944 pollination-direct-sun-hours.express-0.5.17/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:18:42.892944 pollination-direct-sun-hours.express-0.5.17/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-27 19:18:42.896944 pollination-direct-sun-hours.express-0.5.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:18:42.888944 pollination-direct-sun-hours.express-0.5.17/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:18:42.892944 pollination-direct-sun-hours.express-0.5.17/pollination/direct_sun_hours/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/pollination/direct_sun_hours/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/pollination/direct_sun_hours/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:18:42.896944 pollination-direct-sun-hours.express-0.5.17/pollination_direct_sun_hours.express.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-27 19:18:42.000000 pollination-direct-sun-hours.express-0.5.17/pollination_direct_sun_hours.express.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-27 19:18:42.000000 pollination-direct-sun-hours.express-0.5.17/pollination_direct_sun_hours.express.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:18:42.000000 pollination-direct-sun-hours.express-0.5.17/pollination_direct_sun_hours.express.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:18:42.000000 pollination-direct-sun-hours.express-0.5.17/pollination_direct_sun_hours.express.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-27 19:18:42.000000 pollination-direct-sun-hours.express-0.5.17/pollination_direct_sun_hours.express.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 19:18:42.000000 pollination-direct-sun-hours.express-0.5.17/pollination_direct_sun_hours.express.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 19:18:42.896944 pollination-direct-sun-hours.express-0.5.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:18:42.896944 pollination-direct-sun-hours.express-0.5.17/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-27 19:18:09.000000 pollination-direct-sun-hours.express-0.5.17/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:20:09.624141 pollination-direct-sun-hours.express-0.5.18/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:20:09.620141 pollination-direct-sun-hours.express-0.5.18/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:20:09.620141 pollination-direct-sun-hours.express-0.5.18/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-28 14:20:09.624141 pollination-direct-sun-hours.express-0.5.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:20:09.620141 pollination-direct-sun-hours.express-0.5.18/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:20:09.620141 pollination-direct-sun-hours.express-0.5.18/pollination/direct_sun_hours/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/pollination/direct_sun_hours/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/pollination/direct_sun_hours/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:20:09.624141 pollination-direct-sun-hours.express-0.5.18/pollination_direct_sun_hours.express.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-28 14:20:09.000000 pollination-direct-sun-hours.express-0.5.18/pollination_direct_sun_hours.express.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-28 14:20:09.000000 pollination-direct-sun-hours.express-0.5.18/pollination_direct_sun_hours.express.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:20:09.000000 pollination-direct-sun-hours.express-0.5.18/pollination_direct_sun_hours.express.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:20:09.000000 pollination-direct-sun-hours.express-0.5.18/pollination_direct_sun_hours.express.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 14:20:09.000000 pollination-direct-sun-hours.express-0.5.18/pollination_direct_sun_hours.express.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 14:20:09.000000 pollination-direct-sun-hours.express-0.5.18/pollination_direct_sun_hours.express.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 14:20:09.624141 pollination-direct-sun-hours.express-0.5.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:20:09.624141 pollination-direct-sun-hours.express-0.5.18/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 14:19:36.000000 pollination-direct-sun-hours.express-0.5.18/tests/validation_test.py
```

### Comparing `pollination-direct-sun-hours.express-0.5.17/.github/workflows/ci.yaml` & `pollination-direct-sun-hours.express-0.5.18/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-direct-sun-hours.express-0.5.17/.github/workflows/tests.yaml` & `pollination-direct-sun-hours.express-0.5.18/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-direct-sun-hours.express-0.5.17/LICENSE` & `pollination-direct-sun-hours.express-0.5.18/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-direct-sun-hours.express-0.5.17/PKG-INFO` & `pollination-direct-sun-hours.express-0.5.18/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-direct-sun-hours.express
-Version: 0.5.17
+Version: 0.5.18
 Summary: Direct sun hours recipe for Pollination.
 Home-page: https://github.com/pollination/direct-sun-hours
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-direct-sun-hours.express-0.5.17/README.md` & `pollination-direct-sun-hours.express-0.5.18/README.md`

 * *Files identical despite different names*

### Comparing `pollination-direct-sun-hours.express-0.5.17/pollination/direct_sun_hours/entry.py` & `pollination-direct-sun-hours.express-0.5.18/pollination/direct_sun_hours/entry.py`

 * *Files identical despite different names*

### Comparing `pollination-direct-sun-hours.express-0.5.17/pollination_direct_sun_hours.express.egg-info/PKG-INFO` & `pollination-direct-sun-hours.express-0.5.18/pollination_direct_sun_hours.express.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-direct-sun-hours.express
-Version: 0.5.17
+Version: 0.5.18
 Summary: Direct sun hours recipe for Pollination.
 Home-page: https://github.com/pollination/direct-sun-hours
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-direct-sun-hours.express-0.5.17/pollination_direct_sun_hours.express.egg-info/SOURCES.txt` & `pollination-direct-sun-hours.express-0.5.18/pollination_direct_sun_hours.express.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-direct-sun-hours.express-0.5.17/setup.py` & `pollination-direct-sun-hours.express-0.5.18/setup.py`

 * *Files identical despite different names*

