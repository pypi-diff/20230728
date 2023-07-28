# Comparing `tmp/pipedrive-wrapper-1.0.6.tar.gz` & `tmp/pipedrive-wrapper-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipedrive-wrapper-1.0.6.tar", last modified: Thu Jul 27 21:26:47 2023, max compression
+gzip compressed data, was "pipedrive-wrapper-1.0.7.tar", last modified: Fri Jul 28 01:24:51 2023, max compression
```

## Comparing `pipedrive-wrapper-1.0.6.tar` & `pipedrive-wrapper-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 21:26:47.819090 pipedrive-wrapper-1.0.6/
--rw-rw-rw-   0        0        0     1092 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      705 2023-07-27 21:26:47.819090 pipedrive-wrapper-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       65 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 21:26:47.813088 pipedrive-wrapper-1.0.6/pipedrive/
--rw-rw-rw-   0        0        0        0 2023-05-07 15:48:01.000000 pipedrive-wrapper-1.0.6/pipedrive/__init__.py
--rw-rw-rw-   0        0        0     3904 2023-07-27 20:00:05.000000 pipedrive-wrapper-1.0.6/pipedrive/activity.py
--rw-rw-rw-   0        0        0     4242 2023-07-26 14:59:47.000000 pipedrive-wrapper-1.0.6/pipedrive/client.py
--rw-rw-rw-   0        0        0     6504 2023-07-27 19:52:36.000000 pipedrive-wrapper-1.0.6/pipedrive/deal.py
--rw-rw-rw-   0        0        0     1321 2023-07-26 14:59:47.000000 pipedrive-wrapper-1.0.6/pipedrive/deal_field.py
--rw-rw-rw-   0        0        0      855 2023-06-06 19:39:27.000000 pipedrive-wrapper-1.0.6/pipedrive/exceptions.py
--rw-rw-rw-   0        0        0     5537 2023-07-26 14:59:47.000000 pipedrive-wrapper-1.0.6/pipedrive/person.py
--rw-rw-rw-   0        0        0     3319 2023-06-06 19:04:08.000000 pipedrive-wrapper-1.0.6/pipedrive/util.py
-drwxrwxrwx   0        0        0        0 2023-07-27 21:26:47.818088 pipedrive-wrapper-1.0.6/pipedrive_wrapper.egg-info/
--rw-rw-rw-   0        0        0      705 2023-07-27 21:26:47.000000 pipedrive-wrapper-1.0.6/pipedrive_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-07-27 21:26:47.000000 pipedrive-wrapper-1.0.6/pipedrive_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 21:26:47.000000 pipedrive-wrapper-1.0.6/pipedrive_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-27 21:26:47.000000 pipedrive-wrapper-1.0.6/pipedrive_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-27 21:26:47.000000 pipedrive-wrapper-1.0.6/pipedrive_wrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 21:26:47.819090 pipedrive-wrapper-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-07-27 21:15:20.000000 pipedrive-wrapper-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 01:24:51.402421 pipedrive-wrapper-1.0.7/
+-rw-rw-rw-   0        0        0     1092 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      705 2023-07-28 01:24:51.402421 pipedrive-wrapper-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       65 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 01:24:51.391421 pipedrive-wrapper-1.0.7/pipedrive/
+-rw-rw-rw-   0        0        0        0 2023-05-07 15:48:01.000000 pipedrive-wrapper-1.0.7/pipedrive/__init__.py
+-rw-rw-rw-   0        0        0     3904 2023-07-27 20:00:05.000000 pipedrive-wrapper-1.0.7/pipedrive/activity.py
+-rw-rw-rw-   0        0        0     4242 2023-07-26 14:59:47.000000 pipedrive-wrapper-1.0.7/pipedrive/client.py
+-rw-rw-rw-   0        0        0     6512 2023-07-28 01:22:36.000000 pipedrive-wrapper-1.0.7/pipedrive/deal.py
+-rw-rw-rw-   0        0        0     1321 2023-07-26 14:59:47.000000 pipedrive-wrapper-1.0.7/pipedrive/deal_field.py
+-rw-rw-rw-   0        0        0      855 2023-06-06 19:39:27.000000 pipedrive-wrapper-1.0.7/pipedrive/exceptions.py
+-rw-rw-rw-   0        0        0     5537 2023-07-26 14:59:47.000000 pipedrive-wrapper-1.0.7/pipedrive/person.py
+-rw-rw-rw-   0        0        0     3319 2023-06-06 19:04:08.000000 pipedrive-wrapper-1.0.7/pipedrive/util.py
+drwxrwxrwx   0        0        0        0 2023-07-28 01:24:51.401419 pipedrive-wrapper-1.0.7/pipedrive_wrapper.egg-info/
+-rw-rw-rw-   0        0        0      705 2023-07-28 01:24:51.000000 pipedrive-wrapper-1.0.7/pipedrive_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-07-28 01:24:51.000000 pipedrive-wrapper-1.0.7/pipedrive_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 01:24:51.000000 pipedrive-wrapper-1.0.7/pipedrive_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 01:24:51.000000 pipedrive-wrapper-1.0.7/pipedrive_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-28 01:24:51.000000 pipedrive-wrapper-1.0.7/pipedrive_wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 01:24:51.402421 pipedrive-wrapper-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-07-28 01:24:43.000000 pipedrive-wrapper-1.0.7/setup.py
```

### Comparing `pipedrive-wrapper-1.0.6/LICENSE` & `pipedrive-wrapper-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.6/PKG-INFO` & `pipedrive-wrapper-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipedrive-wrapper
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python wrapper for the Pipedrive API
 Home-page: https://github.com/ppcantidio/pipedrive.py
 Author: Pedro Cantidio
 Author-email: ppcantidio@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pipedrive-wrapper-1.0.6/pipedrive/activity.py` & `pipedrive-wrapper-1.0.7/pipedrive/activity.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.6/pipedrive/client.py` & `pipedrive-wrapper-1.0.7/pipedrive/client.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.6/pipedrive/deal.py` & `pipedrive-wrapper-1.0.7/pipedrive/deal.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             "expected_close_date": expected_close_date,
             "probability": probability,
             "lost_reason": lost_reason,
             "visible_to": visible_to,
             "add_time": add_time,
         }
 
-        for key, value in payload:
+        for key, value in payload.items():
             if value is None:
                 del payload[key]
 
         result = self.client.put(url_context=url_context,  body=payload)
 
         return result
```

### Comparing `pipedrive-wrapper-1.0.6/pipedrive/deal_field.py` & `pipedrive-wrapper-1.0.7/pipedrive/deal_field.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.6/pipedrive/exceptions.py` & `pipedrive-wrapper-1.0.7/pipedrive/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.6/pipedrive/person.py` & `pipedrive-wrapper-1.0.7/pipedrive/person.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.6/pipedrive/util.py` & `pipedrive-wrapper-1.0.7/pipedrive/util.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.6/pipedrive_wrapper.egg-info/PKG-INFO` & `pipedrive-wrapper-1.0.7/pipedrive_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipedrive-wrapper
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python wrapper for the Pipedrive API
 Home-page: https://github.com/ppcantidio/pipedrive.py
 Author: Pedro Cantidio
 Author-email: ppcantidio@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pipedrive-wrapper-1.0.6/setup.py` & `pipedrive-wrapper-1.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="pipedrive-wrapper",
-    version="1.0.6",
+    version="1.0.7",
     author="Pedro Cantidio",
     author_email="ppcantidio@gmail.com",
     description="A Python wrapper for the Pipedrive API",
     long_description="A Python wrapper that simplifies interaction with the Pipedrive API",
     url="https://github.com/ppcantidio/pipedrive.py",
     packages=find_packages(exclude=["tests"]),
     classifiers=[
```

