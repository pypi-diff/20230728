# Comparing `tmp/metar2bufr-0.0.2.26.tar.gz` & `tmp/metar2bufr-0.0.2.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metar2bufr-0.0.2.26.tar", last modified: Fri Jul 28 19:43:00 2023, max compression
+gzip compressed data, was "metar2bufr-0.0.2.27.tar", last modified: Fri Jul 28 21:43:07 2023, max compression
```

## Comparing `metar2bufr-0.0.2.26.tar` & `metar2bufr-0.0.2.27.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:43:00.377088 metar2bufr-0.0.2.26/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1073 2023-07-13 16:23:37.000000 metar2bufr-0.0.2.26/LICENSE
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       39 2023-07-13 22:22:45.000000 metar2bufr-0.0.2.26/MANIFEST.in
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-07-28 19:43:00.377088 metar2bufr-0.0.2.26/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       85 2023-07-13 16:24:38.000000 metar2bufr-0.0.2.26/README.md
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      764 2023-07-28 19:42:26.000000 metar2bufr-0.0.2.26/pyproject.toml
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-07-28 19:43:00.377088 metar2bufr-0.0.2.26/setup.cfg
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:43:00.370088 metar2bufr-0.0.2.26/src/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:43:00.372088 metar2bufr-0.0.2.26/src/metar2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      164 2023-07-13 20:54:01.000000 metar2bufr-0.0.2.26/src/metar2bufr/__init__.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:43:00.373088 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:43:00.370088 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/build/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:43:00.370088 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/build/lib/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:43:00.374088 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/build/lib/csv2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:43:00.374088 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/csv2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/csv2bufr/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/csv2bufr/cli.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:43:00.370088 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/docs/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:43:00.374088 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/docs/source/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3056 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/docs/source/conf.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3330 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/setup.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:43:00.374088 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/tests/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8502 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    26208 2023-07-26 21:53:12.000000 metar2bufr-0.0.2.26/src/metar2bufr/icao_bufr_encoder.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:43:00.376088 metar2bufr-0.0.2.26/src/metar2bufr/metarDecoder/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 17:15:28.000000 metar2bufr-0.0.2.26/src/metar2bufr/metarDecoder/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    59241 2023-07-13 20:20:04.000000 metar2bufr-0.0.2.26/src/metar2bufr/metarDecoder/metarDecoders.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    82209 2023-07-13 16:28:08.000000 metar2bufr-0.0.2.26/src/metar2bufr/metarDecoder/tpg.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8261 2023-07-13 16:28:19.000000 metar2bufr-0.0.2.26/src/metar2bufr/metarDecoder/xmlConfig.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     6620 2023-07-13 20:39:39.000000 metar2bufr-0.0.2.26/src/metar2bufr/metarDecoder/xmlUtilities.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    23896 2023-07-28 19:42:12.000000 metar2bufr-0.0.2.26/src/metar2bufr/metar_bufr_encoder.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:43:00.376088 metar2bufr-0.0.2.26/src/metar2bufr/resources/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 22:08:27.000000 metar2bufr-0.0.2.26/src/metar2bufr/resources/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2793 2023-07-20 23:18:14.000000 metar2bufr-0.0.2.26/src/metar2bufr/resources/icao-metar-mappings.json
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2825 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.26/src/metar2bufr/resources/metar-mappings.json
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3136 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.26/src/metar2bufr/resources/metar-mappings2.json
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:43:00.373088 metar2bufr-0.0.2.26/src/metar2bufr.egg-info/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-07-28 19:43:00.000000 metar2bufr-0.0.2.26/src/metar2bufr.egg-info/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1107 2023-07-28 19:43:00.000000 metar2bufr-0.0.2.26/src/metar2bufr.egg-info/SOURCES.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-07-28 19:43:00.000000 metar2bufr-0.0.2.26/src/metar2bufr.egg-info/dependency_links.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       11 2023-07-28 19:43:00.000000 metar2bufr-0.0.2.26/src/metar2bufr.egg-info/top_level.txt
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 21:43:07.958461 metar2bufr-0.0.2.27/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1073 2023-07-13 16:23:37.000000 metar2bufr-0.0.2.27/LICENSE
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       39 2023-07-13 22:22:45.000000 metar2bufr-0.0.2.27/MANIFEST.in
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-07-28 21:43:07.958461 metar2bufr-0.0.2.27/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       85 2023-07-13 16:24:38.000000 metar2bufr-0.0.2.27/README.md
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      764 2023-07-28 21:42:24.000000 metar2bufr-0.0.2.27/pyproject.toml
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-07-28 21:43:07.958461 metar2bufr-0.0.2.27/setup.cfg
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 21:43:07.951460 metar2bufr-0.0.2.27/src/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 21:43:07.954460 metar2bufr-0.0.2.27/src/metar2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      164 2023-07-13 20:54:01.000000 metar2bufr-0.0.2.27/src/metar2bufr/__init__.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 21:43:07.955460 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 21:43:07.951460 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/build/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 21:43:07.951460 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/build/lib/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 21:43:07.955460 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/build/lib/csv2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 21:43:07.956461 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/csv2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/csv2bufr/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/csv2bufr/cli.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 21:43:07.952460 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/docs/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 21:43:07.956461 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/docs/source/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3056 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/docs/source/conf.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3330 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/setup.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 21:43:07.956461 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/tests/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8502 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    26208 2023-07-26 21:53:12.000000 metar2bufr-0.0.2.27/src/metar2bufr/icao_bufr_encoder.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 21:43:07.957460 metar2bufr-0.0.2.27/src/metar2bufr/metarDecoder/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 17:15:28.000000 metar2bufr-0.0.2.27/src/metar2bufr/metarDecoder/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    59241 2023-07-13 20:20:04.000000 metar2bufr-0.0.2.27/src/metar2bufr/metarDecoder/metarDecoders.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    82209 2023-07-13 16:28:08.000000 metar2bufr-0.0.2.27/src/metar2bufr/metarDecoder/tpg.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8261 2023-07-13 16:28:19.000000 metar2bufr-0.0.2.27/src/metar2bufr/metarDecoder/xmlConfig.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     6620 2023-07-13 20:39:39.000000 metar2bufr-0.0.2.27/src/metar2bufr/metarDecoder/xmlUtilities.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    23900 2023-07-28 21:42:03.000000 metar2bufr-0.0.2.27/src/metar2bufr/metar_bufr_encoder.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 21:43:07.958461 metar2bufr-0.0.2.27/src/metar2bufr/resources/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 22:08:27.000000 metar2bufr-0.0.2.27/src/metar2bufr/resources/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2793 2023-07-20 23:18:14.000000 metar2bufr-0.0.2.27/src/metar2bufr/resources/icao-metar-mappings.json
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2825 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.27/src/metar2bufr/resources/metar-mappings.json
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3136 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.27/src/metar2bufr/resources/metar-mappings2.json
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 21:43:07.954460 metar2bufr-0.0.2.27/src/metar2bufr.egg-info/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-07-28 21:43:07.000000 metar2bufr-0.0.2.27/src/metar2bufr.egg-info/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1107 2023-07-28 21:43:07.000000 metar2bufr-0.0.2.27/src/metar2bufr.egg-info/SOURCES.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-07-28 21:43:07.000000 metar2bufr-0.0.2.27/src/metar2bufr.egg-info/dependency_links.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       11 2023-07-28 21:43:07.000000 metar2bufr-0.0.2.27/src/metar2bufr.egg-info/top_level.txt
```

### Comparing `metar2bufr-0.0.2.26/LICENSE` & `metar2bufr-0.0.2.27/LICENSE`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/PKG-INFO` & `metar2bufr-0.0.2.27/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar2bufr
-Version: 0.0.2.26
+Version: 0.0.2.27
 Summary: Package for converting METAR TAC messages or an individual METAR message to BUFR4
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `metar2bufr-0.0.2.26/pyproject.toml` & `metar2bufr-0.0.2.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metar2bufr"
-version = "0.0.2.26"
+version = "0.0.2.27"
 authors = [
   { name="Alexander Thompson", email="alexander.thompson@noaa.gov" },
 ]
 description = "Package for converting METAR TAC messages or an individual METAR message to BUFR4"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py` & `metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py` & `metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py` & `metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/csv2bufr/__init__.py` & `metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/csv2bufr/__init__.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/csv2bufr/cli.py` & `metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/csv2bufr/cli.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py` & `metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/docs/source/conf.py` & `metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/setup.py` & `metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/setup.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py` & `metar2bufr-0.0.2.27/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/icao_bufr_encoder.py` & `metar2bufr-0.0.2.27/src/metar2bufr/icao_bufr_encoder.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/metarDecoder/metarDecoders.py` & `metar2bufr-0.0.2.27/src/metar2bufr/metarDecoder/metarDecoders.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/metarDecoder/tpg.py` & `metar2bufr-0.0.2.27/src/metar2bufr/metarDecoder/tpg.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/metarDecoder/xmlConfig.py` & `metar2bufr-0.0.2.27/src/metar2bufr/metarDecoder/xmlConfig.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/metarDecoder/xmlUtilities.py` & `metar2bufr-0.0.2.27/src/metar2bufr/metarDecoder/xmlUtilities.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/metar_bufr_encoder.py` & `metar2bufr-0.0.2.27/src/metar2bufr/metar_bufr_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,19 +288,19 @@
     #             output['sig_convec_'+str(i+1)] = decoded['sky']['str'][i][6:]
 
     #         #  TODO need to incorporate NSC and NCD values as described in section 15.9.1.3 of FM-15 manual
 
     if 'temps' in decoded:
         if 'air' in decoded['temps']:
             # metar records temperatures in Celsius. Need to convert to Kelvin for bufr
-            air_temp = int(decoded['temps']['air'])
+            air_temp = float(decoded['temps']['air'])
             output['air_temp'] = air_temp + 273.15
         if 'dewpoint' in decoded['temps']:
             # metar records temperatures in Celsius. Need to convert to Kelvin for bufr
-            dewpoint_temp = int(decoded['temps']['dewpoint'])
+            dewpoint_temp = float(decoded['temps']['dewpoint'])
             output['dew_point_temp'] = dewpoint_temp + 273.15
 
     # if 'altimeter' in decoded:
     #     altimeter = float(decoded['altimeter']['value'])
     #     # metar records altimeter in inches of Mercury. need to convert to Pascals for bufr
     #     output['altimeter'] = round(altimeter*3386.39, 2)
     #     output['altimeter_uom'] = decoded['altimeter']['uom']
```

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/resources/icao-metar-mappings.json` & `metar2bufr-0.0.2.27/src/metar2bufr/resources/icao-metar-mappings.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/resources/metar-mappings.json` & `metar2bufr-0.0.2.27/src/metar2bufr/resources/metar-mappings.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr/resources/metar-mappings2.json` & `metar2bufr-0.0.2.27/src/metar2bufr/resources/metar-mappings2.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr.egg-info/PKG-INFO` & `metar2bufr-0.0.2.27/src/metar2bufr.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar2bufr
-Version: 0.0.2.26
+Version: 0.0.2.27
 Summary: Package for converting METAR TAC messages or an individual METAR message to BUFR4
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `metar2bufr-0.0.2.26/src/metar2bufr.egg-info/SOURCES.txt` & `metar2bufr-0.0.2.27/src/metar2bufr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

