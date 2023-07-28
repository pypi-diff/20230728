# Comparing `tmp/tesla-ce-provider-fr-tfr-0.0.7.tar.gz` & `tmp/tesla-ce-provider-fr-tfr-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesla-ce-provider-fr-tfr-0.0.7.tar", last modified: Tue Jul 25 13:31:29 2023, max compression
+gzip compressed data, was "tesla-ce-provider-fr-tfr-0.0.8.tar", last modified: Fri Jul 28 18:02:00 2023, max compression
```

## Comparing `tesla-ce-provider-fr-tfr-0.0.7.tar` & `tesla-ce-provider-fr-tfr-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 13:31:19.000000 tesla-ce-provider-fr-tfr-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-25 13:31:19.000000 tesla-ce-provider-fr-tfr-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-25 13:31:19.000000 tesla-ce-provider-fr-tfr-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 13:31:19.000000 tesla-ce-provider-fr-tfr-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-25 13:31:19.000000 tesla-ce-provider-fr-tfr-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:31:29.237404 tesla-ce-provider-fr-tfr-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-25 13:31:29.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-25 13:31:29.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:31:29.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 13:31:29.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 13:31:29.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-25 13:31:19.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-25 13:31:19.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tests/tfr_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/data/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 13:31:28.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/data/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/data/options.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/tfr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:02:00.534236 tesla-ce-provider-fr-tfr-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-28 18:01:53.000000 tesla-ce-provider-fr-tfr-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 18:01:53.000000 tesla-ce-provider-fr-tfr-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-28 18:02:00.534236 tesla-ce-provider-fr-tfr-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-28 18:01:53.000000 tesla-ce-provider-fr-tfr-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 18:01:53.000000 tesla-ce-provider-fr-tfr-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:02:00.534236 tesla-ce-provider-fr-tfr-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-28 18:01:53.000000 tesla-ce-provider-fr-tfr-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:02:00.530236 tesla-ce-provider-fr-tfr-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:02:00.530236 tesla-ce-provider-fr-tfr-0.0.8/src/tesla_ce_provider_fr_tfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-28 18:02:00.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tesla_ce_provider_fr_tfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-28 18:02:00.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tesla_ce_provider_fr_tfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:02:00.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tesla_ce_provider_fr_tfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 18:02:00.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tesla_ce_provider_fr_tfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 18:02:00.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tesla_ce_provider_fr_tfr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:02:00.530236 tesla-ce-provider-fr-tfr-0.0.8/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-28 18:01:53.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-28 18:01:53.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-28 18:01:54.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tests/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-28 18:01:54.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-28 18:01:54.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-28 18:01:54.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tests/test_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-28 18:01:54.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tests/tfr_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:02:00.530236 tesla-ce-provider-fr-tfr-0.0.8/src/tfr/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-28 18:01:54.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tfr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:02:00.534236 tesla-ce-provider-fr-tfr-0.0.8/src/tfr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 18:02:00.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tfr/data/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-28 18:01:54.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tfr/data/options.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:02:00.534236 tesla-ce-provider-fr-tfr-0.0.8/src/tfr/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-28 18:01:54.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tfr/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-28 18:01:54.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tfr/provider/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-07-28 18:01:54.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tfr/provider/tfr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-07-28 18:01:54.000000 tesla-ce-provider-fr-tfr-0.0.8/src/tfr/provider/utils.py
```

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/LICENSE` & `tesla-ce-provider-fr-tfr-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/PKG-INFO` & `tesla-ce-provider-fr-tfr-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesla-ce-provider-fr-tfr
-Version: 0.0.7
+Version: 0.0.8
 Summary: TeSLA CE Face Recognition Provider
 Home-page: https://tesla-ce.github.io
 Author: Xavier Baro
 Author-email: xbaro@uoc.edu
 License: UNKNOWN
 Project-URL: Documentation, https://tesla-ce.github.io/provider-fr-tfr/
 Project-URL: Source, https://github.com/tesla-ce/provider-fr-tfr
```

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/README.md` & `tesla-ce-provider-fr-tfr-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/setup.py` & `tesla-ce-provider-fr-tfr-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/PKG-INFO` & `tesla-ce-provider-fr-tfr-0.0.8/src/tesla_ce_provider_fr_tfr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesla-ce-provider-fr-tfr
-Version: 0.0.7
+Version: 0.0.8
 Summary: TeSLA CE Face Recognition Provider
 Home-page: https://tesla-ce.github.io
 Author: Xavier Baro
 Author-email: xbaro@uoc.edu
 License: UNKNOWN
 Project-URL: Documentation, https://tesla-ce.github.io/provider-fr-tfr/
 Project-URL: Source, https://github.com/tesla-ce/provider-fr-tfr
```

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/SOURCES.txt` & `tesla-ce-provider-fr-tfr-0.0.8/src/tesla_ce_provider_fr_tfr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/src/tests/__init__.py` & `tesla-ce-provider-fr-tfr-0.0.8/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/src/tests/conftest.py` & `tesla-ce-provider-fr-tfr-0.0.8/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_notification.py` & `tesla-ce-provider-fr-tfr-0.0.8/src/tests/test_notification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_utils.py` & `tesla-ce-provider-fr-tfr-0.0.8/src/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_validation.py` & `tesla-ce-provider-fr-tfr-0.0.8/src/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_verification.py` & `tesla-ce-provider-fr-tfr-0.0.8/src/tests/test_verification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/src/tests/tfr_utils.py` & `tesla-ce-provider-fr-tfr-0.0.8/src/tests/tfr_utils.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/src/tfr/__init__.py` & `tesla-ce-provider-fr-tfr-0.0.8/src/tfr/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/src/tfr/data/options.json` & `tesla-ce-provider-fr-tfr-0.0.8/src/tfr/data/options.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.0.8'"}*

```diff
@@ -42,10 +42,10 @@
             }
         },
         "type": "object"
     },
     "queue": "fr_tfr",
     "service_port": null,
     "url": "https://github.com/tesla-ce/provider-fr-tfr",
-    "version": "0.0.7",
+    "version": "0.0.8",
     "warning_below": 0.6
 }
```

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/__init__.py` & `tesla-ce-provider-fr-tfr-0.0.8/src/tfr/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/models.py` & `tesla-ce-provider-fr-tfr-0.0.8/src/tfr/provider/models.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/tfr.py` & `tesla-ce-provider-fr-tfr-0.0.8/src/tfr/provider/tfr.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/utils.py` & `tesla-ce-provider-fr-tfr-0.0.8/src/tfr/provider/utils.py`

 * *Files identical despite different names*

