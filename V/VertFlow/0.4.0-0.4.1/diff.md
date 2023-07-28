# Comparing `tmp/VertFlow-0.4.0.tar.gz` & `tmp/VertFlow-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VertFlow-0.4.0.tar", last modified: Fri May 12 15:20:08 2023, max compression
+gzip compressed data, was "VertFlow-0.4.1.tar", last modified: Fri Jul 28 13:25:33 2023, max compression
```

## Comparing `VertFlow-0.4.0.tar` & `VertFlow-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:08.001347 VertFlow-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-05-12 15:19:53.000000 VertFlow-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-12 15:20:08.001347 VertFlow-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-12 15:19:53.000000 VertFlow-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:07.997347 VertFlow-0.4.0/VertFlow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-12 15:20:07.000000 VertFlow-0.4.0/VertFlow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-12 15:20:07.000000 VertFlow-0.4.0/VertFlow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:20:07.000000 VertFlow-0.4.0/VertFlow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-12 15:20:07.000000 VertFlow-0.4.0/VertFlow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 15:20:07.000000 VertFlow-0.4.0/VertFlow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-12 15:20:08.001347 VertFlow-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-12 15:19:53.000000 VertFlow-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:07.997347 VertFlow-0.4.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-12 15:19:53.000000 VertFlow-0.4.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14795 2023-05-12 15:19:53.000000 VertFlow-0.4.0/src/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-12 15:19:53.000000 VertFlow-0.4.0/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-12 15:19:53.000000 VertFlow-0.4.0/src/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-05-12 15:19:53.000000 VertFlow-0.4.0/src/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-12 15:19:53.000000 VertFlow-0.4.0/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:08.001347 VertFlow-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-12 15:19:53.000000 VertFlow-0.4.0/test/test_cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-12 15:19:53.000000 VertFlow-0.4.0/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-12 15:19:53.000000 VertFlow-0.4.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:25:33.518962 VertFlow-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-07-28 13:25:17.000000 VertFlow-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-28 13:25:33.518962 VertFlow-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-28 13:25:17.000000 VertFlow-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:25:33.518962 VertFlow-0.4.1/VertFlow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-28 13:25:33.000000 VertFlow-0.4.1/VertFlow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-28 13:25:33.000000 VertFlow-0.4.1/VertFlow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:25:33.000000 VertFlow-0.4.1/VertFlow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 13:25:33.000000 VertFlow-0.4.1/VertFlow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 13:25:33.000000 VertFlow-0.4.1/VertFlow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-28 13:25:33.518962 VertFlow-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-28 13:25:17.000000 VertFlow-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:25:33.518962 VertFlow-0.4.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-28 13:25:17.000000 VertFlow-0.4.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14795 2023-07-28 13:25:17.000000 VertFlow-0.4.1/src/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-28 13:25:17.000000 VertFlow-0.4.1/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-28 13:25:17.000000 VertFlow-0.4.1/src/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-07-28 13:25:17.000000 VertFlow-0.4.1/src/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-28 13:25:17.000000 VertFlow-0.4.1/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:25:33.518962 VertFlow-0.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-28 13:25:17.000000 VertFlow-0.4.1/test/test_cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-07-28 13:25:17.000000 VertFlow-0.4.1/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-07-28 13:25:17.000000 VertFlow-0.4.1/test/test_utils.py
```

### Comparing `VertFlow-0.4.0/LICENSE` & `VertFlow-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `VertFlow-0.4.0/PKG-INFO` & `VertFlow-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VertFlow
-Version: 0.4.0
+Version: 0.4.1
 Summary: Apache Airflow operator for running Google Cloud Run Jobs using green energy
 Home-page: https://github.com/ovotech/VertFlow
 Author: OVO Energy
 Author-email: trading.dl@ovoenergy.com
 License: Apache 2.0
 Keywords: airflow,gcp,google,cloud run,cloud composer,green,environment,sustainability
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: VertFlow Version: 0.4.0 Summary: Apache Airflow
+Metadata-Version: 2.1 Name: VertFlow Version: 0.4.1 Summary: Apache Airflow
 operator for running Google Cloud Run Jobs using green energy Home-page: https:
 //github.com/ovotech/VertFlow Author: OVO Energy Author-email:
 trading.dl@ovoenergy.com License: Apache 2.0 Keywords: airflow,gcp,google,cloud
 run,cloud composer,green,environment,sustainability Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
                                     [logo]
                                    VertFlow
```

### Comparing `VertFlow-0.4.0/README.md` & `VertFlow-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `VertFlow-0.4.0/VertFlow.egg-info/PKG-INFO` & `VertFlow-0.4.1/VertFlow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VertFlow
-Version: 0.4.0
+Version: 0.4.1
 Summary: Apache Airflow operator for running Google Cloud Run Jobs using green energy
 Home-page: https://github.com/ovotech/VertFlow
 Author: OVO Energy
 Author-email: trading.dl@ovoenergy.com
 License: Apache 2.0
 Keywords: airflow,gcp,google,cloud run,cloud composer,green,environment,sustainability
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: VertFlow Version: 0.4.0 Summary: Apache Airflow
+Metadata-Version: 2.1 Name: VertFlow Version: 0.4.1 Summary: Apache Airflow
 operator for running Google Cloud Run Jobs using green energy Home-page: https:
 //github.com/ovotech/VertFlow Author: OVO Energy Author-email:
 trading.dl@ovoenergy.com License: Apache 2.0 Keywords: airflow,gcp,google,cloud
 run,cloud composer,green,environment,sustainability Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
                                     [logo]
                                    VertFlow
```

### Comparing `VertFlow-0.4.0/setup.py` & `VertFlow-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.4.0/src/__init__.py` & `VertFlow-0.4.1/src/__init__.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.4.0/src/cloud_run.py` & `VertFlow-0.4.1/src/cloud_run.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.4.0/src/constants.py` & `VertFlow-0.4.1/src/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     {"id": "europe-west8", "name": "Milan", "lat": 45.4641943, "lon": 9.1896346},
     {
         "id": "europe-west9",
         "name": "Paris",
         "lat": 48.8588897,
         "lon": 2.3200410217200766,
     },
+    {"id": "europe-west12", "name": "Turin", "lat": 45.0703, "lon": 7.6869},
+    {"id": "me-central1", "name": "Doha", "lat": 25.2854, "lon": 51.5310},
     {"id": "me-west1", "name": "Tel Aviv", "lat": 32.0852997, "lon": 34.7818064},
     {
         "id": "northamerica-northeast1",
         "name": "Montréal",
         "lat": 45.5031824,
         "lon": -73.5698065,
     },
```

### Comparing `VertFlow-0.4.0/src/data.py` & `VertFlow-0.4.1/src/data.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.4.0/src/operator.py` & `VertFlow-0.4.1/src/operator.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.4.0/src/utils.py` & `VertFlow-0.4.1/src/utils.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.4.0/test/test_cloud_run.py` & `VertFlow-0.4.1/test/test_cloud_run.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.4.0/test/test_data.py` & `VertFlow-0.4.1/test/test_data.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.4.0/test/test_utils.py` & `VertFlow-0.4.1/test/test_utils.py`

 * *Files identical despite different names*

