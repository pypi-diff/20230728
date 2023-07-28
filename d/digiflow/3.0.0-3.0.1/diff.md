# Comparing `tmp/digiflow-3.0.0.tar.gz` & `tmp/digiflow-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digiflow-3.0.0.tar", last modified: Tue Jul  4 11:46:51 2023, max compression
+gzip compressed data, was "digiflow-3.0.1.tar", last modified: Fri Jul 28 14:27:40 2023, max compression
```

## Comparing `digiflow-3.0.0.tar` & `digiflow-3.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-04 11:46:51.823577 digiflow-3.0.0/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1106 2023-07-03 13:56:57.000000 digiflow-3.0.0/LICENCE
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      205 2023-07-04 08:42:32.000000 digiflow-3.0.0/MANIFEST.in
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      427 2023-07-04 11:46:51.823577 digiflow-3.0.0/PKG-INFO
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1283 2023-07-04 11:42:59.000000 digiflow-3.0.0/README.md
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      688 2023-07-04 10:14:15.000000 digiflow-3.0.0/pyproject.toml
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       38 2023-07-04 11:46:51.823577 digiflow-3.0.0/setup.cfg
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-04 11:46:51.807576 digiflow-3.0.0/src/
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-04 11:46:51.811576 digiflow-3.0.0/src/digiflow/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      509 2023-07-03 13:38:30.000000 digiflow-3.0.0/src/digiflow/__init__.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    12685 2023-07-03 13:38:30.000000 digiflow-3.0.0/src/digiflow/digflow_identifier.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    10920 2023-07-04 07:12:14.000000 digiflow-3.0.0/src/digiflow/digiflow_export.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    11390 2023-07-03 13:38:30.000000 digiflow-3.0.0/src/digiflow/digiflow_generate.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    38976 2023-07-03 13:38:30.000000 digiflow-3.0.0/src/digiflow/digiflow_io.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    31754 2023-07-03 13:49:57.000000 digiflow-3.0.0/src/digiflow/digiflow_metadata.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    12200 2023-07-04 08:47:08.000000 digiflow-3.0.0/src/digiflow/digiflow_validate.py
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-04 11:46:51.811576 digiflow-3.0.0/src/digiflow/resources/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     2676 2023-07-04 07:49:18.000000 digiflow-3.0.0/src/digiflow/resources/digilife.ini
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-04 11:46:51.811576 digiflow-3.0.0/src/digiflow/resources/sch/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   162203 2023-07-03 13:38:30.000000 digiflow-3.0.0/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-medien.sch
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   125014 2023-07-03 13:38:30.000000 digiflow-3.0.0/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-zeitungen.sch
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-04 11:46:51.815576 digiflow-3.0.0/src/digiflow/resources/xsd/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    55541 2023-07-03 13:38:30.000000 digiflow-3.0.0/src/digiflow/resources/xsd/alto_4-2.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   135665 2023-07-03 13:38:30.000000 digiflow-3.0.0/src/digiflow/resources/xsd/mets_1-12.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    98153 2023-07-03 13:38:30.000000 digiflow-3.0.0/src/digiflow/resources/xsd/mix_2-0.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    52954 2023-07-03 13:38:30.000000 digiflow-3.0.0/src/digiflow/resources/xsd/mods_3-7.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    88414 2023-07-03 13:38:30.000000 digiflow-3.0.0/src/digiflow/resources/xsd/page_2019-07-15.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     3180 2023-07-03 13:38:30.000000 digiflow-3.0.0/src/digiflow/resources/xsd/xlink.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5840 2023-07-03 13:38:30.000000 digiflow-3.0.0/src/digiflow/resources/xsd/xml.xsd
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-04 11:46:51.815576 digiflow-3.0.0/src/digiflow/schematron/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)  7072788 2023-07-03 13:38:30.000000 digiflow-3.0.0/src/digiflow/schematron/schxslt-cli.jar
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-04 11:46:51.811576 digiflow-3.0.0/src/digiflow.egg-info/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      427 2023-07-04 11:46:51.000000 digiflow-3.0.0/src/digiflow.egg-info/PKG-INFO
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1148 2023-07-04 11:46:51.000000 digiflow-3.0.0/src/digiflow.egg-info/SOURCES.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        1 2023-07-04 11:46:51.000000 digiflow-3.0.0/src/digiflow.egg-info/dependency_links.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       27 2023-07-04 11:46:51.000000 digiflow-3.0.0/src/digiflow.egg-info/requires.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        9 2023-07-04 11:46:51.000000 digiflow-3.0.0/src/digiflow.egg-info/top_level.txt
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-04 11:46:51.823577 digiflow-3.0.0/tests/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    12481 2023-07-04 07:12:14.000000 digiflow-3.0.0/tests/test_digiflow_generate.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    21727 2023-07-04 07:12:14.000000 digiflow-3.0.0/tests/test_digiflow_identifier.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    54615 2023-07-04 07:12:14.000000 digiflow-3.0.0/tests/test_digiflow_io.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    22460 2023-07-04 07:50:20.000000 digiflow-3.0.0/tests/test_digiflow_metadata.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    18594 2023-07-04 08:44:03.000000 digiflow-3.0.0/tests/test_digiflow_validate.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    15559 2023-07-04 07:12:14.000000 digiflow-3.0.0/tests/test_export_saf.py
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.358120 digiflow-3.0.1/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1106 2023-07-03 13:56:57.000000 digiflow-3.0.1/LICENCE
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      205 2023-07-04 08:42:32.000000 digiflow-3.0.1/MANIFEST.in
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1728 2023-07-28 14:27:40.358120 digiflow-3.0.1/PKG-INFO
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1260 2023-07-04 12:02:04.000000 digiflow-3.0.1/README.md
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      709 2023-07-28 14:27:28.000000 digiflow-3.0.1/pyproject.toml
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       38 2023-07-28 14:27:40.358120 digiflow-3.0.1/setup.cfg
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.342120 digiflow-3.0.1/src/
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.346120 digiflow-3.0.1/src/digiflow/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      509 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/__init__.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    12685 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/digflow_identifier.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    10920 2023-07-04 07:12:14.000000 digiflow-3.0.1/src/digiflow/digiflow_export.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    11390 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/digiflow_generate.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    39028 2023-07-28 14:25:35.000000 digiflow-3.0.1/src/digiflow/digiflow_io.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    31754 2023-07-03 13:49:57.000000 digiflow-3.0.1/src/digiflow/digiflow_metadata.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    12200 2023-07-04 08:47:08.000000 digiflow-3.0.1/src/digiflow/digiflow_validate.py
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.346120 digiflow-3.0.1/src/digiflow/resources/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     2676 2023-07-04 07:49:18.000000 digiflow-3.0.1/src/digiflow/resources/digilife.ini
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.346120 digiflow-3.0.1/src/digiflow/resources/sch/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   162203 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-medien.sch
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   125014 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-zeitungen.sch
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.346120 digiflow-3.0.1/src/digiflow/resources/xsd/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    55541 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/xsd/alto_4-2.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   135665 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/xsd/mets_1-12.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    98153 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/xsd/mix_2-0.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    52954 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/xsd/mods_3-7.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    88414 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/xsd/page_2019-07-15.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     3180 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/xsd/xlink.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5840 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/xsd/xml.xsd
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.346120 digiflow-3.0.1/src/digiflow/schematron/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)  7072788 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/schematron/schxslt-cli.jar
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.346120 digiflow-3.0.1/src/digiflow.egg-info/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1728 2023-07-28 14:27:40.000000 digiflow-3.0.1/src/digiflow.egg-info/PKG-INFO
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1148 2023-07-28 14:27:40.000000 digiflow-3.0.1/src/digiflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        1 2023-07-28 14:27:40.000000 digiflow-3.0.1/src/digiflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       27 2023-07-28 14:27:40.000000 digiflow-3.0.1/src/digiflow.egg-info/requires.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        9 2023-07-28 14:27:40.000000 digiflow-3.0.1/src/digiflow.egg-info/top_level.txt
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.358120 digiflow-3.0.1/tests/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    12481 2023-07-04 07:12:14.000000 digiflow-3.0.1/tests/test_digiflow_generate.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    21727 2023-07-04 07:12:14.000000 digiflow-3.0.1/tests/test_digiflow_identifier.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    54615 2023-07-04 07:12:14.000000 digiflow-3.0.1/tests/test_digiflow_io.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    22460 2023-07-04 07:50:20.000000 digiflow-3.0.1/tests/test_digiflow_metadata.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    18594 2023-07-04 08:44:03.000000 digiflow-3.0.1/tests/test_digiflow_validate.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    15559 2023-07-04 07:12:14.000000 digiflow-3.0.1/tests/test_export_saf.py
```

### Comparing `digiflow-3.0.0/LICENCE` & `digiflow-3.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/README.md` & `digiflow-3.0.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # digital flow
 
-![Python CI](https://github.com/ulb-sachsen-anhalt/digital-flow/actions/workflows/main-app.yml/badge.svg)
-[![PyPi version](https://badgen.net/pypi/v/digital-flow/)](https://pypi.org/project/digital-flow) ![PyPI - Downloads](https://img.shields.io/pypi/dm/digital-flow) ![PyPI - License](https://img.shields.io/pypi/l/digital-flow) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/digital-flow)
+![Python CI](https://github.com/ulb-sachsen-anhalt/digital-flow/actions/workflows/main.yml/badge.svg)
+[![PyPi version](https://badgen.net/pypi/v/digiflow/)](https://pypi.org/project/digiflow/) ![PyPI - Downloads](https://img.shields.io/pypi/dm/digiflow) ![PyPI - License](https://img.shields.io/pypi/l/digiflow) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/digiflow)
 
 Father's little helper for internal library digitalization workflows running on Linux-Systems.
 
 ## Testing
 
 Testing with tox uses different Python versions.
```

### Comparing `digiflow-3.0.0/pyproject.toml` & `digiflow-3.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digiflow"
-version = "3.0.0"
+version = "3.0.1"
 description = "Father's Little Digitization Workflow Helper"
+readme = "README.md"
 requires-python = ">=3.8"
 authors = [
 	{name = "Universitäts- und Landesbibliothek Sachsen-Anhalt", email = "development@bibliothek.uni-halle.de"}
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License"
```

### Comparing `digiflow-3.0.0/src/digiflow/digflow_identifier.py` & `digiflow-3.0.1/src/digiflow/digflow_identifier.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow/digiflow_export.py` & `digiflow-3.0.1/src/digiflow/digiflow_export.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow/digiflow_generate.py` & `digiflow-3.0.1/src/digiflow/digiflow_generate.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow/digiflow_io.py` & `digiflow-3.0.1/src/digiflow/digiflow_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -732,26 +732,26 @@
         if skip_resources:
             return loaded
 
         # inspect if additional file resources are requested
         mets_reader = MetsReader(self.path_mets, mets_digital_object_identifier)
 
         # get linked resources
-        for k in self.groups.keys():
+        for k in self.groups:
             self.groups[k] = mets_reader.get_filegrp_links(group=k)
 
         # if exist, download them too
         post_func = None
-        for k, vals in self.groups.items():
+        for k, linked_res_urls in self.groups.items():
             if k == self.key_ocr:
                 post_func = post_oai_store_ocr
-            for res_url in vals:
-                res_end = res_url.split('/')[-1]
-                res_path = self._calculate_path(k, res_end)
-                if self._handle_load(res_url, res_path, post_func):
+            for linked_res_url in linked_res_urls:
+                res_val_end = linked_res_url.split('/')[-1]
+                res_val_path = self._calculate_path(k, res_val_end)
+                if self._handle_load(linked_res_url, res_val_path, post_func):
                     loaded += 1
         return loaded
 
     def _handle_load(self, res_url, res_path, post_func, force_load=False):
         if self.store:
             stored_path = self.store.get(res_path)
             # if in store found ...
```

### Comparing `digiflow-3.0.0/src/digiflow/digiflow_metadata.py` & `digiflow-3.0.1/src/digiflow/digiflow_metadata.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow/digiflow_validate.py` & `digiflow-3.0.1/src/digiflow/digiflow_validate.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow/resources/digilife.ini` & `digiflow-3.0.1/src/digiflow/resources/digilife.ini`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-medien.sch` & `digiflow-3.0.1/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-medien.sch`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-zeitungen.sch` & `digiflow-3.0.1/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-zeitungen.sch`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow/resources/xsd/alto_4-2.xsd` & `digiflow-3.0.1/src/digiflow/resources/xsd/alto_4-2.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow/resources/xsd/mets_1-12.xsd` & `digiflow-3.0.1/src/digiflow/resources/xsd/mets_1-12.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow/resources/xsd/mix_2-0.xsd` & `digiflow-3.0.1/src/digiflow/resources/xsd/mix_2-0.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow/resources/xsd/mods_3-7.xsd` & `digiflow-3.0.1/src/digiflow/resources/xsd/mods_3-7.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow/resources/xsd/page_2019-07-15.xsd` & `digiflow-3.0.1/src/digiflow/resources/xsd/page_2019-07-15.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow/resources/xsd/xlink.xsd` & `digiflow-3.0.1/src/digiflow/resources/xsd/xlink.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow/resources/xsd/xml.xsd` & `digiflow-3.0.1/src/digiflow/resources/xsd/xml.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow/schematron/schxslt-cli.jar` & `digiflow-3.0.1/src/digiflow/schematron/schxslt-cli.jar`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/src/digiflow.egg-info/SOURCES.txt` & `digiflow-3.0.1/src/digiflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/tests/test_digiflow_generate.py` & `digiflow-3.0.1/tests/test_digiflow_generate.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/tests/test_digiflow_identifier.py` & `digiflow-3.0.1/tests/test_digiflow_identifier.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/tests/test_digiflow_io.py` & `digiflow-3.0.1/tests/test_digiflow_io.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/tests/test_digiflow_metadata.py` & `digiflow-3.0.1/tests/test_digiflow_metadata.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/tests/test_digiflow_validate.py` & `digiflow-3.0.1/tests/test_digiflow_validate.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.0/tests/test_export_saf.py` & `digiflow-3.0.1/tests/test_export_saf.py`

 * *Files identical despite different names*

