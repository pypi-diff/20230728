# Comparing `tmp/lb-telemetry-0.4.0.tar.gz` & `tmp/lb-telemetry-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/lhcb/lb-telemetry/dist/.tmp-kpa_0bwx/lb-telemetry-0.4.0.tar", last modified: Thu Jul 27 06:37:12 2023, max compression
+gzip compressed data, was "/builds/lhcb/lb-telemetry/dist/.tmp-dzgb9wa1/lb-telemetry-0.5.0.tar", last modified: Fri Jul 28 03:53:32 2023, max compression
```

## Comparing `lb-telemetry-0.4.0.tar` & `lb-telemetry-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/
--rw-r--r--   0 root         (0) root         (0)     2191 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1967 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/.mypy.ini
--rw-r--r--   0 root         (0) root         (0)      594 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    18151 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/.pylintrc
--rw-r--r--   0 root         (0) root         (0)    35065 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2577 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1903 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1414 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry/
--rw-r--r--   0 root         (0) root         (0)     7598 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/src/lb_telemetry/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/src/lb_telemetry/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2577 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      438 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/tests/
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6113 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/tests/test_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:53:32.000000 lb-telemetry-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-07-28 03:53:24.000000 lb-telemetry-0.5.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1908 2023-07-28 03:53:24.000000 lb-telemetry-0.5.0/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-28 03:53:24.000000 lb-telemetry-0.5.0/.mypy.ini
+-rw-r--r--   0 root         (0) root         (0)      594 2023-07-28 03:53:24.000000 lb-telemetry-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    18151 2023-07-28 03:53:24.000000 lb-telemetry-0.5.0/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)    35065 2023-07-28 03:53:24.000000 lb-telemetry-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2577 2023-07-28 03:53:32.000000 lb-telemetry-0.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-07-28 03:53:24.000000 lb-telemetry-0.5.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-07-28 03:53:24.000000 lb-telemetry-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 03:53:32.000000 lb-telemetry-0.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:53:32.000000 lb-telemetry-0.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:53:32.000000 lb-telemetry-0.5.0/src/lb_telemetry/
+-rw-r--r--   0 root         (0) root         (0)     7625 2023-07-28 03:53:24.000000 lb-telemetry-0.5.0/src/lb_telemetry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      889 2023-07-28 03:53:24.000000 lb-telemetry-0.5.0/src/lb_telemetry/__main__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 03:53:24.000000 lb-telemetry-0.5.0/src/lb_telemetry/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:53:32.000000 lb-telemetry-0.5.0/src/lb_telemetry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2577 2023-07-28 03:53:32.000000 lb-telemetry-0.5.0/src/lb_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      467 2023-07-28 03:53:32.000000 lb-telemetry-0.5.0/src/lb_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 03:53:32.000000 lb-telemetry-0.5.0/src/lb_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-28 03:53:32.000000 lb-telemetry-0.5.0/src/lb_telemetry.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-28 03:53:32.000000 lb-telemetry-0.5.0/src/lb_telemetry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 03:53:32.000000 lb-telemetry-0.5.0/src/lb_telemetry.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:53:32.000000 lb-telemetry-0.5.0/tests/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-28 03:53:24.000000 lb-telemetry-0.5.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6113 2023-07-28 03:53:24.000000 lb-telemetry-0.5.0/tests/test_logger.py
```

### Comparing `lb-telemetry-0.4.0/.gitignore` & `lb-telemetry-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.4.0/.gitlab-ci.yml` & `lb-telemetry-0.5.0/.gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -29,16 +29,15 @@
     - pip install pre-commit
   script:
     - pre-commit run --all-files
 
 mypy:
   stage: lint
   script:
-    - mypy src/lb_telemetry --explicit-package-bases
-  allow_failure: true
+    - mypy src/
 
 tests:
   stage: test
   needs: []
   script:
     - python -m pytest tests/ -v
   coverage: '/TOTAL.*\s+(\d+%)$/'
```

### Comparing `lb-telemetry-0.4.0/.pre-commit-config.yaml` & `lb-telemetry-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.4.0/.pylintrc` & `lb-telemetry-0.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.4.0/LICENSE` & `lb-telemetry-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.4.0/PKG-INFO` & `lb-telemetry-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lb-telemetry
-Version: 0.4.0
+Version: 0.5.0
 Summary: A utility for logging telemetry data from LHCb packages to MONIT
 Author-email: Cameron McClymont <cameron.duncan.mcclymont@cern.ch>, Daniel Cervenkov <daniel.cervenkov@cern.ch>, Chris Burr <christopher.burr@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/lhcb/lb-telemetry
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb/lb-telemetry/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `lb-telemetry-0.4.0/README.md` & `lb-telemetry-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.4.0/pyproject.toml` & `lb-telemetry-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.4.0/src/lb_telemetry/__init__.py` & `lb-telemetry-0.5.0/src/lb_telemetry/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
         try:
             response = requests.post(
                 self.send_url,
                 headers={
                     "Content-Type": "application/json",
                 },
                 data=json.dumps(payload),
+                timeout=5,
             )
         except requests.exceptions.RequestException as e:
             logzero.debug(
                 f"An error occurred while logging telemetry "
                 f"(this can happen when running from outside "
                 f"the CERN network): {e}"
             )
```

### Comparing `lb-telemetry-0.4.0/src/lb_telemetry.egg-info/PKG-INFO` & `lb-telemetry-0.5.0/src/lb_telemetry.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lb-telemetry
-Version: 0.4.0
+Version: 0.5.0
 Summary: A utility for logging telemetry data from LHCb packages to MONIT
 Author-email: Cameron McClymont <cameron.duncan.mcclymont@cern.ch>, Daniel Cervenkov <daniel.cervenkov@cern.ch>, Chris Burr <christopher.burr@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/lhcb/lb-telemetry
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb/lb-telemetry/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `lb-telemetry-0.4.0/tests/test_logger.py` & `lb-telemetry-0.5.0/tests/test_logger.py`

 * *Files identical despite different names*

