# Comparing `tmp/pollination-ladybug-radiance-0.2.0.tar.gz` & `tmp/pollination-ladybug-radiance-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-ladybug-radiance-0.2.0.tar", last modified: Thu Jul 27 13:34:25 2023, max compression
+gzip compressed data, was "dist/pollination-ladybug-radiance-0.2.1.tar", last modified: Fri Jul 28 10:50:26 2023, max compression
```

## Comparing `pollination-ladybug-radiance-0.2.0.tar` & `pollination-ladybug-radiance-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:25.000000 pollination-ladybug-radiance-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:25.000000 pollination-ladybug-radiance-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:25.000000 pollination-ladybug-radiance-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-27 13:34:25.000000 pollination-ladybug-radiance-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:25.000000 pollination-ladybug-radiance-0.2.0/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:25.000000 pollination-ladybug-radiance-0.2.0/pollination/ladybug_radiance/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/pollination/ladybug_radiance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/pollination/ladybug_radiance/direct_sunhours.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/pollination/ladybug_radiance/radiation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:25.000000 pollination-ladybug-radiance-0.2.0/pollination/ladybug_radiance/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/pollination/ladybug_radiance/scripts/direct_sunhours.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/pollination/ladybug_radiance/scripts/incident_radiation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:25.000000 pollination-ladybug-radiance-0.2.0/pollination_ladybug_radiance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-27 13:34:24.000000 pollination-ladybug-radiance-0.2.0/pollination_ladybug_radiance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-27 13:34:25.000000 pollination-ladybug-radiance-0.2.0/pollination_ladybug_radiance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:34:24.000000 pollination-ladybug-radiance-0.2.0/pollination_ladybug_radiance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:33:40.000000 pollination-ladybug-radiance-0.2.0/pollination_ladybug_radiance.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-27 13:34:24.000000 pollination-ladybug-radiance-0.2.0/pollination_ladybug_radiance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 13:34:24.000000 pollination-ladybug-radiance-0.2.0/pollination_ladybug_radiance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 13:34:25.000000 pollination-ladybug-radiance-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:25.000000 pollination-ladybug-radiance-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-27 13:33:17.000000 pollination-ladybug-radiance-0.2.0/tests/radiation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:50:26.000000 pollination-ladybug-radiance-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:50:26.000000 pollination-ladybug-radiance-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:50:26.000000 pollination-ladybug-radiance-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-28 10:50:26.000000 pollination-ladybug-radiance-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:50:26.000000 pollination-ladybug-radiance-0.2.1/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:50:26.000000 pollination-ladybug-radiance-0.2.1/pollination/ladybug_radiance/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/pollination/ladybug_radiance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/pollination/ladybug_radiance/direct_sunhours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/pollination/ladybug_radiance/radiation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:50:26.000000 pollination-ladybug-radiance-0.2.1/pollination/ladybug_radiance/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/pollination/ladybug_radiance/scripts/direct_sunhours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/pollination/ladybug_radiance/scripts/incident_radiation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:50:26.000000 pollination-ladybug-radiance-0.2.1/pollination_ladybug_radiance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-28 10:50:26.000000 pollination-ladybug-radiance-0.2.1/pollination_ladybug_radiance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-28 10:50:26.000000 pollination-ladybug-radiance-0.2.1/pollination_ladybug_radiance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:50:26.000000 pollination-ladybug-radiance-0.2.1/pollination_ladybug_radiance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:49:51.000000 pollination-ladybug-radiance-0.2.1/pollination_ladybug_radiance.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 10:50:26.000000 pollination-ladybug-radiance-0.2.1/pollination_ladybug_radiance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 10:50:26.000000 pollination-ladybug-radiance-0.2.1/pollination_ladybug_radiance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 10:50:26.000000 pollination-ladybug-radiance-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:50:26.000000 pollination-ladybug-radiance-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/tests/direct_sunhours_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-28 10:49:32.000000 pollination-ladybug-radiance-0.2.1/tests/radiation_test.py
```

### Comparing `pollination-ladybug-radiance-0.2.0/.github/workflows/ci.yaml` & `pollination-ladybug-radiance-0.2.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-ladybug-radiance-0.2.0/.github/workflows/dependency-release.yaml` & `pollination-ladybug-radiance-0.2.1/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `pollination-ladybug-radiance-0.2.0/.github/workflows/tests.yaml` & `pollination-ladybug-radiance-0.2.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-ladybug-radiance-0.2.0/LICENSE` & `pollination-ladybug-radiance-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-ladybug-radiance-0.2.0/PKG-INFO` & `pollination-ladybug-radiance-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-ladybug-radiance
-Version: 0.2.0
+Version: 0.2.1
 Summary: Ladybug Radiance plugin for Pollination.
 Home-page: https://github.com/pollination/pollination-ladybug-radiance
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-ladybug-radiance-0.2.0/README.md` & `pollination-ladybug-radiance-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pollination-ladybug-radiance-0.2.0/pollination/ladybug_radiance/__init__.py` & `pollination-ladybug-radiance-0.2.1/pollination/ladybug_radiance/__init__.py`

 * *Files identical despite different names*

### Comparing `pollination-ladybug-radiance-0.2.0/pollination/ladybug_radiance/direct_sunhours.py` & `pollination-ladybug-radiance-0.2.1/pollination/ladybug_radiance/direct_sunhours.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,20 @@
     )
 
     context_mesh = Inputs.file(
         description='Path to a JSON file for input context mesh in Ladybug Geometry '
         'format.', path='context_geo.json', optional=True
     )
 
+    display_context = Inputs.bool(
+        description='Boolean to note whether the context geometry should be included '
+        'in the output visualization.',
+        default=False
+    )
+
     @script
     def run_direct_sunlight(self):
         return inspect.getsource(direct_sunhours)
 
     direct_sunlight_values = Outputs.file(
         description='direct sun hours values', path='results/results.json'
     )
```

### Comparing `pollination-ladybug-radiance-0.2.0/pollination/ladybug_radiance/radiation.py` & `pollination-ladybug-radiance-0.2.1/pollination/ladybug_radiance/radiation.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,12 +71,24 @@
     )
 
     context_mesh = Inputs.file(
         description='Path to a JSON file for input context mesh in Ladybug Geometry '
         'format.', path='context_geo.json', optional=True
     )
 
+    display_context = Inputs.bool(
+        description='Boolean to note whether the context geometry should be included '
+        'in the output visualization.',
+        default=False
+    )
+
     @script
     def run_incident_radiation(self):
         return inspect.getsource(incident_radiation)
 
-    radiation_values = Outputs.file(description='Radiation values', path='results.txt')
+    radiation_values = Outputs.file(
+        description='Radiation values', path='results/results.json'
+    )
+
+    visualization_set = Outputs.file(
+        description='Results visualization set', path='results/output.vsf'
+    )
```

### Comparing `pollination-ladybug-radiance-0.2.0/pollination_ladybug_radiance.egg-info/PKG-INFO` & `pollination-ladybug-radiance-0.2.1/pollination_ladybug_radiance.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-ladybug-radiance
-Version: 0.2.0
+Version: 0.2.1
 Summary: Ladybug Radiance plugin for Pollination.
 Home-page: https://github.com/pollination/pollination-ladybug-radiance
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-ladybug-radiance-0.2.0/pollination_ladybug_radiance.egg-info/SOURCES.txt` & `pollination-ladybug-radiance-0.2.1/pollination_ladybug_radiance.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 pollination_ladybug_radiance.egg-info/PKG-INFO
 pollination_ladybug_radiance.egg-info/SOURCES.txt
 pollination_ladybug_radiance.egg-info/dependency_links.txt
 pollination_ladybug_radiance.egg-info/not-zip-safe
 pollination_ladybug_radiance.egg-info/requires.txt
 pollination_ladybug_radiance.egg-info/top_level.txt
 tests/__init__.py
+tests/direct_sunhours_test.py
 tests/radiation_test.py
```

### Comparing `pollination-ladybug-radiance-0.2.0/setup.py` & `pollination-ladybug-radiance-0.2.1/setup.py`

 * *Files identical despite different names*

