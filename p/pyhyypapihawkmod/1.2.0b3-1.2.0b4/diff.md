# Comparing `tmp/pyhyypapihawkmod-1.2.0b3.tar.gz` & `tmp/pyhyypapihawkmod-1.2.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.2.0b3.tar", last modified: Fri Jul 28 18:43:51 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.2.0b4.tar", last modified: Fri Jul 28 18:58:57 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.2.0b3.tar` & `pyhyypapihawkmod-1.2.0b4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 18:43:51.950086 pyhyypapihawkmod-1.2.0b3/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b3/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b3/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-07-28 18:43:51.949075 pyhyypapihawkmod-1.2.0b3/PKG-INFO
--rw-rw-rw-   0        0        0     2415 2023-07-28 18:20:05.000000 pyhyypapihawkmod-1.2.0b3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 18:43:51.931039 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-07-28 18:18:42.000000 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0    11525 2023-07-28 18:42:47.000000 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    29564 2023-07-28 18:42:49.000000 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4026 2023-07-28 18:18:42.000000 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-07-28 18:18:42.000000 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:43:51.945567 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-07-28 18:43:51.000000 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-07-28 18:43:51.000000 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 18:43:51.000000 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-28 18:43:51.000000 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 18:43:51.000000 pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 18:43:51.950086 pyhyypapihawkmod-1.2.0b3/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-07-28 18:42:45.000000 pyhyypapihawkmod-1.2.0b3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:58:57.111541 pyhyypapihawkmod-1.2.0b4/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b4/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b4/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-07-28 18:58:57.109522 pyhyypapihawkmod-1.2.0b4/PKG-INFO
+-rw-rw-rw-   0        0        0     2415 2023-07-28 18:20:05.000000 pyhyypapihawkmod-1.2.0b4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 18:58:57.086983 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-07-28 18:18:42.000000 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0    11768 2023-07-28 18:57:11.000000 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    29564 2023-07-28 18:42:49.000000 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4026 2023-07-28 18:18:42.000000 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-07-28 18:18:42.000000 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:58:57.106028 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-07-28 18:58:56.000000 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-07-28 18:58:57.000000 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 18:58:56.000000 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-28 18:58:56.000000 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 18:58:56.000000 pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 18:58:57.111541 pyhyypapihawkmod-1.2.0b4/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-07-28 18:56:08.000000 pyhyypapihawkmod-1.2.0b4/setup.py
```

### Comparing `pyhyypapihawkmod-1.2.0b3/LICENSE.md` & `pyhyypapihawkmod-1.2.0b4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b3/PKG-INFO` & `pyhyypapihawkmod-1.2.0b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.2.0b3
+Version: 1.2.0b4
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.2.0b3/README.md` & `pyhyypapihawkmod-1.2.0b4/README.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/alarm_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,9 +289,14 @@
         
         message = {"Syncinfo" : syncinfo,
                    "Stateinfo" : stateinfo,
                    "notifications" : notificationinfo,
                    "zoneinfo" : zoneinfo,
                     }
         
+        _LOGGER.debug('------------------------------')
+        _LOGGER.debug('--------Start of debug--------')
         
-        return message
+        _LOGGER.debug(message)
+        
+        _LOGGER.debug('--------End of debug--------')
+        _LOGGER.debug('-----------------------------')
```

### Comparing `pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.2.0b3
+Version: 1.2.0b4
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.2.0b3/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.2.0b4/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b3/setup.py` & `pyhyypapihawkmod-1.2.0b4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.2.0b3",
+    version="1.2.0b4",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

