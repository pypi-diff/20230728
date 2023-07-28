# Comparing `tmp/FM15_bfr2geojson-0.0.5.tar.gz` & `tmp/FM15_bfr2geojson-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FM15_bfr2geojson-0.0.5.tar", last modified: Thu Jul 27 20:37:48 2023, max compression
+gzip compressed data, was "FM15_bfr2geojson-0.0.6.tar", last modified: Fri Jul 28 19:02:09 2023, max compression
```

## Comparing `FM15_bfr2geojson-0.0.5.tar` & `FM15_bfr2geojson-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-27 20:37:48.418892 FM15_bfr2geojson-0.0.5/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      523 2023-07-27 20:37:48.418892 FM15_bfr2geojson-0.0.5/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       18 2023-07-25 16:39:55.000000 FM15_bfr2geojson-0.0.5/README.md
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      657 2023-07-27 20:37:15.000000 FM15_bfr2geojson-0.0.5/pyproject.toml
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-07-27 20:37:48.418892 FM15_bfr2geojson-0.0.5/setup.cfg
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-27 20:37:48.416892 FM15_bfr2geojson-0.0.5/src/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-27 20:37:48.417893 FM15_bfr2geojson-0.0.5/src/FM15_bfr2geojson/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    29576 2023-07-27 20:36:38.000000 FM15_bfr2geojson-0.0.5/src/FM15_bfr2geojson/__init__.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-27 20:37:48.417893 FM15_bfr2geojson-0.0.5/src/FM15_bfr2geojson.egg-info/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      523 2023-07-27 20:37:48.000000 FM15_bfr2geojson-0.0.5/src/FM15_bfr2geojson.egg-info/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      233 2023-07-27 20:37:48.000000 FM15_bfr2geojson-0.0.5/src/FM15_bfr2geojson.egg-info/SOURCES.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-07-27 20:37:48.000000 FM15_bfr2geojson-0.0.5/src/FM15_bfr2geojson.egg-info/dependency_links.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       17 2023-07-27 20:37:48.000000 FM15_bfr2geojson-0.0.5/src/FM15_bfr2geojson.egg-info/top_level.txt
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:02:09.476087 FM15_bfr2geojson-0.0.6/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      523 2023-07-28 19:02:09.476087 FM15_bfr2geojson-0.0.6/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       18 2023-07-25 16:39:55.000000 FM15_bfr2geojson-0.0.6/README.md
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      657 2023-07-28 19:01:59.000000 FM15_bfr2geojson-0.0.6/pyproject.toml
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-07-28 19:02:09.476087 FM15_bfr2geojson-0.0.6/setup.cfg
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:02:09.474087 FM15_bfr2geojson-0.0.6/src/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:02:09.475087 FM15_bfr2geojson-0.0.6/src/FM15_bfr2geojson/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    29591 2023-07-28 19:01:05.000000 FM15_bfr2geojson-0.0.6/src/FM15_bfr2geojson/__init__.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-28 19:02:09.476087 FM15_bfr2geojson-0.0.6/src/FM15_bfr2geojson.egg-info/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      523 2023-07-28 19:02:09.000000 FM15_bfr2geojson-0.0.6/src/FM15_bfr2geojson.egg-info/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      233 2023-07-28 19:02:09.000000 FM15_bfr2geojson-0.0.6/src/FM15_bfr2geojson.egg-info/SOURCES.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-07-28 19:02:09.000000 FM15_bfr2geojson-0.0.6/src/FM15_bfr2geojson.egg-info/dependency_links.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       17 2023-07-28 19:02:09.000000 FM15_bfr2geojson-0.0.6/src/FM15_bfr2geojson.egg-info/top_level.txt
```

### Comparing `FM15_bfr2geojson-0.0.5/PKG-INFO` & `FM15_bfr2geojson-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FM15_bfr2geojson
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package for converting FM15(METAR) bufr encoded messages to geojson
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `FM15_bfr2geojson-0.0.5/pyproject.toml` & `FM15_bfr2geojson-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FM15_bfr2geojson"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Alexander Thompson", email="alexander.thompson@noaa.gov" },
 ]
 description = "Package for converting FM15(METAR) bufr encoded messages to geojson"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `FM15_bfr2geojson-0.0.5/src/FM15_bfr2geojson/__init__.py` & `FM15_bfr2geojson-0.0.6/src/FM15_bfr2geojson/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -627,15 +627,15 @@
                             "id": feature_id,
                             "conformsTo": ["http://www.wmo.int/spec/om-profile-1/1.0/req/geojson"],  # noqa
                             "reportId": f"ICAO_{icao}_{characteristic_date}T{characteristic_time}{id}",  # noqa
                             "type": "Feature",
                             "geometry": self.get_location(),
                             "properties": {
                                 # "identifier": feature_id,
-                                "icao_location_identifier": icao,
+                                "wigos_station_identifier": f"0-20000-0-{icao}",
                                 "phenomenonTime": phenomenon_time,
                                 "resultTime": result_time,
                                 "name": key,
                                 "value": value,
                                 "units": attributes["units"],
                                 "description": description,
                                 "metadata": metadata,
```

### Comparing `FM15_bfr2geojson-0.0.5/src/FM15_bfr2geojson.egg-info/PKG-INFO` & `FM15_bfr2geojson-0.0.6/src/FM15_bfr2geojson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FM15-bfr2geojson
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package for converting FM15(METAR) bufr encoded messages to geojson
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

