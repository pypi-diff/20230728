# Comparing `tmp/pipedrive-wrapper-1.0.8.tar.gz` & `tmp/pipedrive-wrapper-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipedrive-wrapper-1.0.8.tar", last modified: Fri Jul 28 12:21:12 2023, max compression
+gzip compressed data, was "pipedrive-wrapper-1.0.9.tar", last modified: Fri Jul 28 12:54:18 2023, max compression
```

## Comparing `pipedrive-wrapper-1.0.8.tar` & `pipedrive-wrapper-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 12:21:12.384241 pipedrive-wrapper-1.0.8/
--rw-rw-rw-   0        0        0     1092 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      705 2023-07-28 12:21:12.383213 pipedrive-wrapper-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       65 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 12:21:12.360755 pipedrive-wrapper-1.0.8/pipedrive/
--rw-rw-rw-   0        0        0        0 2023-05-07 15:48:01.000000 pipedrive-wrapper-1.0.8/pipedrive/__init__.py
--rw-rw-rw-   0        0        0     3904 2023-07-27 20:00:05.000000 pipedrive-wrapper-1.0.8/pipedrive/activity.py
--rw-rw-rw-   0        0        0     4242 2023-07-26 14:59:47.000000 pipedrive-wrapper-1.0.8/pipedrive/client.py
--rw-rw-rw-   0        0        0     6401 2023-07-28 12:16:27.000000 pipedrive-wrapper-1.0.8/pipedrive/deal.py
--rw-rw-rw-   0        0        0     1321 2023-07-26 14:59:47.000000 pipedrive-wrapper-1.0.8/pipedrive/deal_field.py
--rw-rw-rw-   0        0        0      855 2023-06-06 19:39:27.000000 pipedrive-wrapper-1.0.8/pipedrive/exceptions.py
--rw-rw-rw-   0        0        0     5537 2023-07-26 14:59:47.000000 pipedrive-wrapper-1.0.8/pipedrive/person.py
--rw-rw-rw-   0        0        0     3319 2023-06-06 19:04:08.000000 pipedrive-wrapper-1.0.8/pipedrive/util.py
-drwxrwxrwx   0        0        0        0 2023-07-28 12:21:12.382213 pipedrive-wrapper-1.0.8/pipedrive_wrapper.egg-info/
--rw-rw-rw-   0        0        0      705 2023-07-28 12:21:12.000000 pipedrive-wrapper-1.0.8/pipedrive_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-07-28 12:21:12.000000 pipedrive-wrapper-1.0.8/pipedrive_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 12:21:12.000000 pipedrive-wrapper-1.0.8/pipedrive_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-28 12:21:12.000000 pipedrive-wrapper-1.0.8/pipedrive_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-28 12:21:12.000000 pipedrive-wrapper-1.0.8/pipedrive_wrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 12:21:12.384241 pipedrive-wrapper-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-07-28 12:17:06.000000 pipedrive-wrapper-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:18.386445 pipedrive-wrapper-1.0.9/
+-rw-rw-rw-   0        0        0     1092 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      705 2023-07-28 12:54:18.385445 pipedrive-wrapper-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       65 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:18.371420 pipedrive-wrapper-1.0.9/pipedrive/
+-rw-rw-rw-   0        0        0        0 2023-05-07 15:48:01.000000 pipedrive-wrapper-1.0.9/pipedrive/__init__.py
+-rw-rw-rw-   0        0        0     3903 2023-07-28 12:54:03.000000 pipedrive-wrapper-1.0.9/pipedrive/activity.py
+-rw-rw-rw-   0        0        0     4242 2023-07-26 14:59:47.000000 pipedrive-wrapper-1.0.9/pipedrive/client.py
+-rw-rw-rw-   0        0        0     6401 2023-07-28 12:16:27.000000 pipedrive-wrapper-1.0.9/pipedrive/deal.py
+-rw-rw-rw-   0        0        0     1321 2023-07-26 14:59:47.000000 pipedrive-wrapper-1.0.9/pipedrive/deal_field.py
+-rw-rw-rw-   0        0        0      855 2023-06-06 19:39:27.000000 pipedrive-wrapper-1.0.9/pipedrive/exceptions.py
+-rw-rw-rw-   0        0        0     5537 2023-07-26 14:59:47.000000 pipedrive-wrapper-1.0.9/pipedrive/person.py
+-rw-rw-rw-   0        0        0     3319 2023-06-06 19:04:08.000000 pipedrive-wrapper-1.0.9/pipedrive/util.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:18.384462 pipedrive-wrapper-1.0.9/pipedrive_wrapper.egg-info/
+-rw-rw-rw-   0        0        0      705 2023-07-28 12:54:18.000000 pipedrive-wrapper-1.0.9/pipedrive_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-07-28 12:54:18.000000 pipedrive-wrapper-1.0.9/pipedrive_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 12:54:18.000000 pipedrive-wrapper-1.0.9/pipedrive_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 12:54:18.000000 pipedrive-wrapper-1.0.9/pipedrive_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-28 12:54:18.000000 pipedrive-wrapper-1.0.9/pipedrive_wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 12:54:18.386445 pipedrive-wrapper-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-07-28 12:54:16.000000 pipedrive-wrapper-1.0.9/setup.py
```

### Comparing `pipedrive-wrapper-1.0.8/LICENSE` & `pipedrive-wrapper-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.8/PKG-INFO` & `pipedrive-wrapper-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipedrive-wrapper
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python wrapper for the Pipedrive API
 Home-page: https://github.com/ppcantidio/pipedrive.py
 Author: Pedro Cantidio
 Author-email: ppcantidio@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pipedrive-wrapper-1.0.8/pipedrive/activity.py` & `pipedrive-wrapper-1.0.9/pipedrive/activity.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,8 +94,8 @@
     def update_acitity(self, activity_id: int, done: bool = False):
         url_context = f"/activities/{activity_id}"
 
         payload = {}
         if done is not None:
             payload['done'] = int(done)
 
-        return self._client._post(url_context, payload)
+        return self._client.post(url_context, payload)
```

### Comparing `pipedrive-wrapper-1.0.8/pipedrive/client.py` & `pipedrive-wrapper-1.0.9/pipedrive/client.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.8/pipedrive/deal.py` & `pipedrive-wrapper-1.0.9/pipedrive/deal.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.8/pipedrive/deal_field.py` & `pipedrive-wrapper-1.0.9/pipedrive/deal_field.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.8/pipedrive/exceptions.py` & `pipedrive-wrapper-1.0.9/pipedrive/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.8/pipedrive/person.py` & `pipedrive-wrapper-1.0.9/pipedrive/person.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.8/pipedrive/util.py` & `pipedrive-wrapper-1.0.9/pipedrive/util.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.8/pipedrive_wrapper.egg-info/PKG-INFO` & `pipedrive-wrapper-1.0.9/pipedrive_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipedrive-wrapper
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python wrapper for the Pipedrive API
 Home-page: https://github.com/ppcantidio/pipedrive.py
 Author: Pedro Cantidio
 Author-email: ppcantidio@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pipedrive-wrapper-1.0.8/setup.py` & `pipedrive-wrapper-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="pipedrive-wrapper",
-    version="1.0.8",
+    version="1.0.9",
     author="Pedro Cantidio",
     author_email="ppcantidio@gmail.com",
     description="A Python wrapper for the Pipedrive API",
     long_description="A Python wrapper that simplifies interaction with the Pipedrive API",
     url="https://github.com/ppcantidio/pipedrive.py",
     packages=find_packages(exclude=["tests"]),
     classifiers=[
```

