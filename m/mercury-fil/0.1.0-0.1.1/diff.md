# Comparing `tmp/mercury_fil-0.1.0.tar.gz` & `tmp/mercury_fil-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury_fil-0.1.0.tar", max compression
+gzip compressed data, was "mercury_fil-0.1.1.tar", max compression
```

## Comparing `mercury_fil-0.1.0.tar` & `mercury_fil-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     7187 2023-07-25 07:23:07.471773 mercury_fil-0.1.0/README.md
--rw-r--r--   0        0        0      602 2023-07-27 23:05:54.801526 mercury_fil-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-07-21 06:08:07.446477 mercury_fil-0.1.0/src/mercury/__init__.py
--rw-r--r--   0        0        0     7555 2023-07-25 07:20:07.092852 mercury_fil-0.1.0/src/mercury/client.py
--rw-r--r--   0        0        0     7907 1970-01-01 00:00:00.000000 mercury_fil-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7301 2023-07-27 23:07:47.343364 mercury_fil-0.1.1/README.md
+-rw-r--r--   0        0        0      602 2023-07-27 23:08:05.844154 mercury_fil-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-07-21 06:08:07.446477 mercury_fil-0.1.1/src/mercury/__init__.py
+-rw-r--r--   0        0        0     7555 2023-07-25 07:20:07.092852 mercury_fil-0.1.1/src/mercury/client.py
+-rw-r--r--   0        0        0     8021 1970-01-01 00:00:00.000000 mercury_fil-0.1.1/PKG-INFO
```

### Comparing `mercury_fil-0.1.0/README.md` & `mercury_fil-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 brew install --cask google-cloud-sdk
 ```
 
 Other installation methods are [here](https://cloud.google.com/sdk/docs/install).
 
 ## installation
 
-`pip install mercury-py`
+`pip install mercury-fil`
 
 ## usage
 
 Make sure you're authenticated: `gcloud auth login`. 
 You'll also need to be in the right project: `gcloud config set project protocol-labs-data`.
 
 > 💡 Only query for columns (and the height range) that you need.
@@ -120,13 +120,20 @@
 
 [3662 rows x 3 columns]
 ```
 
 As with querying only data at the range of heights that you need, **only
 select columns that you need.**
 
+### supported tables
+
+- `fevm_contracts`
+- `derived_gas_outputs`
+- `miner_sector_events`
+- `miner_sector_infos`
+
 ## contributing
 
 To contribute, you'll need [Poetry](https://python-poetry.org/docs/#installing-with-pipx) 
 to install the dependencies.
 
 To run the tests, simply run `pytest`.
```

### Comparing `mercury_fil-0.1.0/pyproject.toml` & `mercury_fil-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mercury-fil"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python client for accessing Filecoin chain data."
 authors = ["Steph Samson <ayo@kasteph.com>"]
 license = "MIT, Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "mercury", from = "src" },
 ]
```

### Comparing `mercury_fil-0.1.0/src/mercury/client.py` & `mercury_fil-0.1.1/src/mercury/client.py`

 * *Files identical despite different names*

### Comparing `mercury_fil-0.1.0/PKG-INFO` & `mercury_fil-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-fil
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python client for accessing Filecoin chain data.
 License: MIT, Apache-2.0
 Keywords: filecoin,bigquery
 Author: Steph Samson
 Author-email: ayo@kasteph.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -35,15 +35,15 @@
 brew install --cask google-cloud-sdk
 ```
 
 Other installation methods are [here](https://cloud.google.com/sdk/docs/install).
 
 ## installation
 
-`pip install mercury-py`
+`pip install mercury-fil`
 
 ## usage
 
 Make sure you're authenticated: `gcloud auth login`. 
 You'll also need to be in the right project: `gcloud config set project protocol-labs-data`.
 
 > 💡 Only query for columns (and the height range) that you need.
@@ -140,14 +140,21 @@
 
 [3662 rows x 3 columns]
 ```
 
 As with querying only data at the range of heights that you need, **only
 select columns that you need.**
 
+### supported tables
+
+- `fevm_contracts`
+- `derived_gas_outputs`
+- `miner_sector_events`
+- `miner_sector_infos`
+
 ## contributing
 
 To contribute, you'll need [Poetry](https://python-poetry.org/docs/#installing-with-pipx) 
 to install the dependencies.
 
 To run the tests, simply run `pytest`.
```

