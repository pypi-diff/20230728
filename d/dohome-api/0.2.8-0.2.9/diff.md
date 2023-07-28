# Comparing `tmp/dohome_api-0.2.8.tar.gz` & `tmp/dohome_api-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dohome_api-0.2.8.tar", last modified: Thu Jul 27 23:01:33 2023, max compression
+gzip compressed data, was "dohome_api-0.2.9.tar", last modified: Fri Jul 28 00:18:16 2023, max compression
```

## Comparing `dohome_api-0.2.8.tar` & `dohome_api-0.2.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-27 23:01:33.347721 dohome_api-0.2.8/
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1072 2023-02-11 09:02:15.000000 dohome_api-0.2.8/LICENSE
--rw-r--r--   0 mishamyrt   (501) staff       (20)      870 2023-07-27 23:01:33.347494 dohome_api-0.2.8/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)      519 2023-02-11 09:02:15.000000 dohome_api-0.2.8/README.md
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-27 23:01:33.343750 dohome_api-0.2.8/dohome_api/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      221 2023-02-11 09:31:28.000000 dohome_api-0.2.8/dohome_api/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      722 2023-02-11 09:02:15.000000 dohome_api-0.2.8/dohome_api/commands.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-27 23:01:33.344420 dohome_api-0.2.8/dohome_api/gateway/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      106 2023-02-11 09:29:34.000000 dohome_api-0.2.8/dohome_api/gateway/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      130 2023-02-11 09:23:55.000000 dohome_api-0.2.8/dohome_api/gateway/constants.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      134 2023-02-11 09:28:31.000000 dohome_api-0.2.8/dohome_api/gateway/exceptions.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1805 2023-02-11 09:28:56.000000 dohome_api-0.2.8/dohome_api/gateway/gateway.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      561 2023-02-11 09:20:17.000000 dohome_api-0.2.8/dohome_api/gateway/utils.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-27 23:01:33.345583 dohome_api-0.2.8/dohome_api/light/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      175 2023-02-11 09:09:28.000000 dohome_api-0.2.8/dohome_api/light/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      269 2023-02-11 09:02:15.000000 dohome_api-0.2.8/dohome_api/light/brightness.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1132 2023-07-27 21:46:01.000000 dohome_api-0.2.8/dohome_api/light/broadcast.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      246 2023-02-11 09:06:56.000000 dohome_api-0.2.8/dohome_api/light/exceptions.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     4178 2023-02-11 09:10:41.000000 dohome_api-0.2.8/dohome_api/light/light.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      426 2023-02-11 09:02:15.000000 dohome_api-0.2.8/dohome_api/light/request.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      693 2023-02-11 09:02:15.000000 dohome_api-0.2.8/dohome_api/light/temperature.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      579 2023-02-11 09:02:15.000000 dohome_api-0.2.8/dohome_api/light/uint8.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-27 23:01:33.346419 dohome_api-0.2.8/dohome_api/transport/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      163 2023-02-11 09:02:15.000000 dohome_api-0.2.8/dohome_api/transport/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1662 2023-07-27 23:00:54.000000 dohome_api-0.2.8/dohome_api/transport/broadcast.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      168 2023-02-11 09:02:15.000000 dohome_api-0.2.8/dohome_api/transport/constants.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1080 2023-02-11 09:02:15.000000 dohome_api-0.2.8/dohome_api/transport/direct.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      333 2023-02-11 09:02:15.000000 dohome_api-0.2.8/dohome_api/transport/interface.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      852 2023-02-11 09:02:15.000000 dohome_api-0.2.8/dohome_api/transport/util.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-27 23:01:33.347171 dohome_api-0.2.8/dohome_api.egg-info/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      870 2023-07-27 23:01:33.000000 dohome_api-0.2.8/dohome_api.egg-info/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)      884 2023-07-27 23:01:33.000000 dohome_api-0.2.8/dohome_api.egg-info/SOURCES.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2023-07-27 23:01:33.000000 dohome_api-0.2.8/dohome_api.egg-info/dependency_links.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)       33 2023-07-27 23:01:33.000000 dohome_api-0.2.8/dohome_api.egg-info/requires.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)       11 2023-07-27 23:01:33.000000 dohome_api-0.2.8/dohome_api.egg-info/top_level.txt
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-27 23:01:33.347303 dohome_api-0.2.8/scripts/
--rwxr-xr-x   0 mishamyrt   (501) staff       (20)     2129 2023-02-11 09:18:35.000000 dohome_api-0.2.8/scripts/dohome_rgb
--rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2023-07-27 23:01:33.347765 dohome_api-0.2.8/setup.cfg
--rw-r--r--   0 mishamyrt   (501) staff       (20)      935 2023-02-11 09:31:48.000000 dohome_api-0.2.8/setup.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-28 00:18:16.025060 dohome_api-0.2.9/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1072 2023-02-11 09:02:15.000000 dohome_api-0.2.9/LICENSE
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      870 2023-07-28 00:18:16.024918 dohome_api-0.2.9/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      519 2023-02-11 09:02:15.000000 dohome_api-0.2.9/README.md
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-28 00:18:16.020716 dohome_api-0.2.9/dohome_api/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      221 2023-02-11 09:31:28.000000 dohome_api-0.2.9/dohome_api/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      722 2023-02-11 09:02:15.000000 dohome_api-0.2.9/dohome_api/commands.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-28 00:18:16.021595 dohome_api-0.2.9/dohome_api/gateway/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      106 2023-02-11 09:29:34.000000 dohome_api-0.2.9/dohome_api/gateway/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      130 2023-02-11 09:23:55.000000 dohome_api-0.2.9/dohome_api/gateway/constants.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      134 2023-02-11 09:28:31.000000 dohome_api-0.2.9/dohome_api/gateway/exceptions.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1805 2023-02-11 09:28:56.000000 dohome_api-0.2.9/dohome_api/gateway/gateway.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      561 2023-02-11 09:20:17.000000 dohome_api-0.2.9/dohome_api/gateway/utils.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-28 00:18:16.022693 dohome_api-0.2.9/dohome_api/light/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      175 2023-02-11 09:09:28.000000 dohome_api-0.2.9/dohome_api/light/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      269 2023-02-11 09:02:15.000000 dohome_api-0.2.9/dohome_api/light/brightness.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1132 2023-07-27 21:46:01.000000 dohome_api-0.2.9/dohome_api/light/broadcast.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      246 2023-02-11 09:06:56.000000 dohome_api-0.2.9/dohome_api/light/exceptions.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     4178 2023-02-11 09:10:41.000000 dohome_api-0.2.9/dohome_api/light/light.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      426 2023-02-11 09:02:15.000000 dohome_api-0.2.9/dohome_api/light/request.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      693 2023-02-11 09:02:15.000000 dohome_api-0.2.9/dohome_api/light/temperature.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      579 2023-02-11 09:02:15.000000 dohome_api-0.2.9/dohome_api/light/uint8.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-28 00:18:16.023851 dohome_api-0.2.9/dohome_api/transport/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      163 2023-02-11 09:02:15.000000 dohome_api-0.2.9/dohome_api/transport/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1662 2023-07-27 23:00:54.000000 dohome_api-0.2.9/dohome_api/transport/broadcast.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      168 2023-02-11 09:02:15.000000 dohome_api-0.2.9/dohome_api/transport/constants.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1080 2023-02-11 09:02:15.000000 dohome_api-0.2.9/dohome_api/transport/direct.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      333 2023-02-11 09:02:15.000000 dohome_api-0.2.9/dohome_api/transport/interface.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      852 2023-02-11 09:02:15.000000 dohome_api-0.2.9/dohome_api/transport/util.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-28 00:18:16.024583 dohome_api-0.2.9/dohome_api.egg-info/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      870 2023-07-28 00:18:16.000000 dohome_api-0.2.9/dohome_api.egg-info/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      884 2023-07-28 00:18:16.000000 dohome_api-0.2.9/dohome_api.egg-info/SOURCES.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2023-07-28 00:18:16.000000 dohome_api-0.2.9/dohome_api.egg-info/dependency_links.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       33 2023-07-28 00:18:16.000000 dohome_api-0.2.9/dohome_api.egg-info/requires.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       11 2023-07-28 00:18:16.000000 dohome_api-0.2.9/dohome_api.egg-info/top_level.txt
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-28 00:18:16.024716 dohome_api-0.2.9/scripts/
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)     2129 2023-02-11 09:18:35.000000 dohome_api-0.2.9/scripts/dohome_rgb
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2023-07-28 00:18:16.025102 dohome_api-0.2.9/setup.cfg
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      935 2023-02-11 09:31:48.000000 dohome_api-0.2.9/setup.py
```

### Comparing `dohome_api-0.2.8/LICENSE` & `dohome_api-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.8/PKG-INFO` & `dohome_api-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dohome_api
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library for controlling smart bulbs that are controlled by the DoIT protocol
 Author: Mikhael Khrustik
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dohome_api-0.2.8/README.md` & `dohome_api-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.8/dohome_api/commands.py` & `dohome_api-0.2.9/dohome_api/commands.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.8/dohome_api/gateway/gateway.py` & `dohome_api-0.2.9/dohome_api/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.8/dohome_api/gateway/utils.py` & `dohome_api-0.2.9/dohome_api/gateway/utils.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.8/dohome_api/light/broadcast.py` & `dohome_api-0.2.9/dohome_api/light/broadcast.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.8/dohome_api/light/light.py` & `dohome_api-0.2.9/dohome_api/light/light.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.8/dohome_api/light/temperature.py` & `dohome_api-0.2.9/dohome_api/light/temperature.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.8/dohome_api/light/uint8.py` & `dohome_api-0.2.9/dohome_api/light/uint8.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.8/dohome_api/transport/broadcast.py` & `dohome_api-0.2.9/dohome_api/transport/broadcast.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.8/dohome_api/transport/direct.py` & `dohome_api-0.2.9/dohome_api/transport/direct.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.8/dohome_api/transport/util.py` & `dohome_api-0.2.9/dohome_api/transport/util.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.8/dohome_api.egg-info/PKG-INFO` & `dohome_api-0.2.9/dohome_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dohome-api
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library for controlling smart bulbs that are controlled by the DoIT protocol
 Author: Mikhael Khrustik
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dohome_api-0.2.8/dohome_api.egg-info/SOURCES.txt` & `dohome_api-0.2.9/dohome_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.8/scripts/dohome_rgb` & `dohome_api-0.2.9/scripts/dohome_rgb`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.8/setup.py` & `dohome_api-0.2.9/setup.py`

 * *Files identical despite different names*

