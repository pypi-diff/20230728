# Comparing `tmp/pypx800v5-0.8.0.tar.gz` & `tmp/pypx800v5-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypx800v5-0.8.0.tar", last modified: Sat Dec  4 01:04:02 2021, max compression
+gzip compressed data, was "pypx800v5-0.9.0.tar", last modified: Sat Dec  4 01:27:27 2021, max compression
```

## Comparing `pypx800v5-0.8.0.tar` & `pypx800v5-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 matthieu  (1000) wheel      (998)        0 2021-12-04 01:04:02.219647 pypx800v5-0.8.0/
--rw-r--r--   0 matthieu  (1000) wheel      (998)     1065 2021-11-20 07:54:38.000000 pypx800v5-0.8.0/LICENSE
--rw-r--r--   0 matthieu  (1000) wheel      (998)     2144 2021-12-04 01:04:02.219647 pypx800v5-0.8.0/PKG-INFO
--rw-r--r--   0 matthieu  (1000) wheel      (998)     1679 2021-11-30 22:22:45.000000 pypx800v5-0.8.0/README.md
-drwxr-xr-x   0 matthieu  (1000) wheel      (998)        0 2021-12-04 01:04:02.219647 pypx800v5-0.8.0/pypx800v5/
--rw-r--r--   0 matthieu  (1000) wheel      (998)      920 2021-12-04 00:02:38.000000 pypx800v5-0.8.0/pypx800v5/__init__.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)      674 2021-12-04 00:11:49.000000 pypx800v5-0.8.0/pypx800v5/const.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)     1023 2021-11-28 20:05:36.000000 pypx800v5-0.8.0/pypx800v5/counter.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)      334 2021-11-28 14:32:35.000000 pypx800v5-0.8.0/pypx800v5/exceptions.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)      617 2021-11-30 22:36:25.000000 pypx800v5-0.8.0/pypx800v5/extension.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)    12328 2021-12-04 00:35:49.000000 pypx800v5-0.8.0/pypx800v5/ipx800.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)     1848 2021-11-29 21:36:15.000000 pypx800v5-0.8.0/pypx800v5/ipx800_io.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)      538 2021-11-30 22:48:33.000000 pypx800v5-0.8.0/pypx800v5/object.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)     1385 2021-12-01 18:32:44.000000 pypx800v5-0.8.0/pypx800v5/tempo.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)     4133 2021-11-28 17:54:03.000000 pypx800v5-0.8.0/pypx800v5/thermostat.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)      515 2021-11-28 14:30:44.000000 pypx800v5-0.8.0/pypx800v5/x24d.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)     1592 2021-11-28 20:02:37.000000 pypx800v5-0.8.0/pypx800v5/x4fp.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)     2221 2021-11-28 16:20:58.000000 pypx800v5-0.8.0/pypx800v5/x4vr.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)      512 2021-11-28 14:30:34.000000 pypx800v5-0.8.0/pypx800v5/x8d.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)     1057 2021-12-04 01:03:22.000000 pypx800v5-0.8.0/pypx800v5/x8r.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)     1670 2021-11-28 14:32:48.000000 pypx800v5-0.8.0/pypx800v5/xdimmer.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)     1657 2021-11-28 14:32:48.000000 pypx800v5-0.8.0/pypx800v5/xpwm.py
--rw-r--r--   0 matthieu  (1000) wheel      (998)     1242 2021-11-28 14:31:35.000000 pypx800v5-0.8.0/pypx800v5/xthl.py
-drwxr-xr-x   0 matthieu  (1000) wheel      (998)        0 2021-12-04 01:04:02.219647 pypx800v5-0.8.0/pypx800v5.egg-info/
--rw-r--r--   0 matthieu  (1000) wheel      (998)     2144 2021-12-04 01:04:02.000000 pypx800v5-0.8.0/pypx800v5.egg-info/PKG-INFO
--rw-r--r--   0 matthieu  (1000) wheel      (998)      518 2021-12-04 01:04:02.000000 pypx800v5-0.8.0/pypx800v5.egg-info/SOURCES.txt
--rw-r--r--   0 matthieu  (1000) wheel      (998)        1 2021-12-04 01:04:02.000000 pypx800v5-0.8.0/pypx800v5.egg-info/dependency_links.txt
--rw-r--r--   0 matthieu  (1000) wheel      (998)       10 2021-12-04 01:04:02.000000 pypx800v5-0.8.0/pypx800v5.egg-info/top_level.txt
--rw-r--r--   0 matthieu  (1000) wheel      (998)       38 2021-12-04 01:04:02.219647 pypx800v5-0.8.0/setup.cfg
--rw-r--r--   0 matthieu  (1000) wheel      (998)      644 2021-12-04 01:03:50.000000 pypx800v5-0.8.0/setup.py
+drwxr-xr-x   0 matthieu  (1000) wheel      (998)        0 2021-12-04 01:27:27.966714 pypx800v5-0.9.0/
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     1065 2021-11-20 07:54:38.000000 pypx800v5-0.9.0/LICENSE
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     2145 2021-12-04 01:27:27.966714 pypx800v5-0.9.0/PKG-INFO
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     1680 2021-12-04 01:26:48.000000 pypx800v5-0.9.0/README.md
+drwxr-xr-x   0 matthieu  (1000) wheel      (998)        0 2021-12-04 01:27:27.966714 pypx800v5-0.9.0/pypx800v5/
+-rw-r--r--   0 matthieu  (1000) wheel      (998)      920 2021-12-04 00:02:38.000000 pypx800v5-0.9.0/pypx800v5/__init__.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)      674 2021-12-04 00:11:49.000000 pypx800v5-0.9.0/pypx800v5/const.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     1023 2021-11-28 20:05:36.000000 pypx800v5-0.9.0/pypx800v5/counter.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)      334 2021-11-28 14:32:35.000000 pypx800v5-0.9.0/pypx800v5/exceptions.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)      617 2021-11-30 22:36:25.000000 pypx800v5-0.9.0/pypx800v5/extension.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)    12329 2021-12-04 01:23:34.000000 pypx800v5-0.9.0/pypx800v5/ipx800.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     1848 2021-11-29 21:36:15.000000 pypx800v5-0.9.0/pypx800v5/ipx800_io.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)      538 2021-11-30 22:48:33.000000 pypx800v5-0.9.0/pypx800v5/object.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     1385 2021-12-01 18:32:44.000000 pypx800v5-0.9.0/pypx800v5/tempo.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     4133 2021-11-28 17:54:03.000000 pypx800v5-0.9.0/pypx800v5/thermostat.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)      515 2021-11-28 14:30:44.000000 pypx800v5-0.9.0/pypx800v5/x24d.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     1592 2021-11-28 20:02:37.000000 pypx800v5-0.9.0/pypx800v5/x4fp.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     2221 2021-11-28 16:20:58.000000 pypx800v5-0.9.0/pypx800v5/x4vr.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)      512 2021-11-28 14:30:34.000000 pypx800v5-0.9.0/pypx800v5/x8d.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     1057 2021-12-04 01:03:22.000000 pypx800v5-0.9.0/pypx800v5/x8r.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     1670 2021-11-28 14:32:48.000000 pypx800v5-0.9.0/pypx800v5/xdimmer.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     1657 2021-11-28 14:32:48.000000 pypx800v5-0.9.0/pypx800v5/xpwm.py
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     1242 2021-11-28 14:31:35.000000 pypx800v5-0.9.0/pypx800v5/xthl.py
+drwxr-xr-x   0 matthieu  (1000) wheel      (998)        0 2021-12-04 01:27:27.966714 pypx800v5-0.9.0/pypx800v5.egg-info/
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     2145 2021-12-04 01:27:27.000000 pypx800v5-0.9.0/pypx800v5.egg-info/PKG-INFO
+-rw-r--r--   0 matthieu  (1000) wheel      (998)      518 2021-12-04 01:27:27.000000 pypx800v5-0.9.0/pypx800v5.egg-info/SOURCES.txt
+-rw-r--r--   0 matthieu  (1000) wheel      (998)        1 2021-12-04 01:27:27.000000 pypx800v5-0.9.0/pypx800v5.egg-info/dependency_links.txt
+-rw-r--r--   0 matthieu  (1000) wheel      (998)       10 2021-12-04 01:27:27.000000 pypx800v5-0.9.0/pypx800v5.egg-info/top_level.txt
+-rw-r--r--   0 matthieu  (1000) wheel      (998)       38 2021-12-04 01:27:27.970048 pypx800v5-0.9.0/setup.cfg
+-rw-r--r--   0 matthieu  (1000) wheel      (998)      644 2021-12-04 01:26:57.000000 pypx800v5-0.9.0/setup.py
```

### Comparing `pypx800v5-0.8.0/LICENSE` & `pypx800v5-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/PKG-INFO` & `pypx800v5-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypx800v5
-Version: 0.8.0
+Version: 0.9.0
 Summary: Control the IPX800V5 and its extensions.
 Home-page: https://github.com/aohzan/pypx800v5
 Author: Aohzan
 Author-email: aohzan@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,15 @@
 - X-4FP
 
 ## IPX800 parameters
 
 - host: ip or hostname (mandatory)
 - port: (default: `80`)
 - api_key: (mandatory)
-- request_timeout: timeout for request in seconds (default: `5`)
+- request_timeout: timeout for request in seconds (default: `30`)
 - session: aiohttp.client.ClientSession
 
 ## Example
 
 ```python
 import asyncio
```

### Comparing `pypx800v5-0.8.0/README.md` & `pypx800v5-0.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 - X-4FP
 
 ## IPX800 parameters
 
 - host: ip or hostname (mandatory)
 - port: (default: `80`)
 - api_key: (mandatory)
-- request_timeout: timeout for request in seconds (default: `5`)
+- request_timeout: timeout for request in seconds (default: `30`)
 - session: aiohttp.client.ClientSession
 
 ## Example
 
 ```python
 import asyncio
```

### Comparing `pypx800v5-0.8.0/pypx800v5/__init__.py` & `pypx800v5-0.9.0/pypx800v5/__init__.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5/const.py` & `pypx800v5-0.9.0/pypx800v5/const.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5/counter.py` & `pypx800v5-0.9.0/pypx800v5/counter.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5/extension.py` & `pypx800v5-0.9.0/pypx800v5/extension.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5/ipx800.py` & `pypx800v5-0.9.0/pypx800v5/ipx800.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """Class representing the IPX800 and its API."""
 
     def __init__(
         self,
         host: str,
         api_key: str,
         port: int = 80,
-        request_timeout: int = 5,
+        request_timeout: int = 30,
         session: ClientSession = None,
     ) -> None:
         """Init a IPX800 V5 API."""
         self.host = host
         self.port = port
         self._api_key = api_key
         self._request_timeout = request_timeout
```

### Comparing `pypx800v5-0.8.0/pypx800v5/ipx800_io.py` & `pypx800v5-0.9.0/pypx800v5/ipx800_io.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5/object.py` & `pypx800v5-0.9.0/pypx800v5/object.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5/tempo.py` & `pypx800v5-0.9.0/pypx800v5/tempo.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5/thermostat.py` & `pypx800v5-0.9.0/pypx800v5/thermostat.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5/x24d.py` & `pypx800v5-0.9.0/pypx800v5/x24d.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5/x4fp.py` & `pypx800v5-0.9.0/pypx800v5/x4fp.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5/x4vr.py` & `pypx800v5-0.9.0/pypx800v5/x4vr.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5/x8d.py` & `pypx800v5-0.9.0/pypx800v5/x8d.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5/x8r.py` & `pypx800v5-0.9.0/pypx800v5/x8r.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5/xdimmer.py` & `pypx800v5-0.9.0/pypx800v5/xdimmer.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5/xpwm.py` & `pypx800v5-0.9.0/pypx800v5/xpwm.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5/xthl.py` & `pypx800v5-0.9.0/pypx800v5/xthl.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/pypx800v5.egg-info/PKG-INFO` & `pypx800v5-0.9.0/pypx800v5.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypx800v5
-Version: 0.8.0
+Version: 0.9.0
 Summary: Control the IPX800V5 and its extensions.
 Home-page: https://github.com/aohzan/pypx800v5
 Author: Aohzan
 Author-email: aohzan@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,15 @@
 - X-4FP
 
 ## IPX800 parameters
 
 - host: ip or hostname (mandatory)
 - port: (default: `80`)
 - api_key: (mandatory)
-- request_timeout: timeout for request in seconds (default: `5`)
+- request_timeout: timeout for request in seconds (default: `30`)
 - session: aiohttp.client.ClientSession
 
 ## Example
 
 ```python
 import asyncio
```

### Comparing `pypx800v5-0.8.0/pypx800v5.egg-info/SOURCES.txt` & `pypx800v5-0.9.0/pypx800v5.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypx800v5-0.8.0/setup.py` & `pypx800v5-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypx800v5",
-    version="0.8.0",
+    version="0.9.0",
     author="Aohzan",
     author_email="aohzan@gmail.com",
     description="Control the IPX800V5 and its extensions.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aohzan/pypx800v5",
     packages=setuptools.find_packages(),
```

