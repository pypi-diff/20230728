# Comparing `tmp/pyyardian-1.0.0.tar.gz` & `tmp/pyyardian-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyardian-1.0.0.tar", last modified: Fri Jul 28 06:11:54 2023, max compression
+gzip compressed data, was "pyyardian-1.0.1.tar", last modified: Fri Jul 28 06:32:35 2023, max compression
```

## Comparing `pyyardian-1.0.0.tar` & `pyyardian-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-28 06:11:54.005564 pyyardian-1.0.0/
--rw-r--r--   0 guang      (501) staff       (20)     1072 2023-07-25 08:04:44.000000 pyyardian-1.0.0/LICENSE
--rw-r--r--   0 guang      (501) staff       (20)      454 2023-07-28 06:11:54.005792 pyyardian-1.0.0/PKG-INFO
--rw-r--r--   0 guang      (501) staff       (20)      150 2023-07-25 08:09:39.000000 pyyardian-1.0.0/README.md
-drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-28 06:11:54.002085 pyyardian-1.0.0/pyyardian/
--rw-r--r--   0 guang      (501) staff       (20)      109 2023-07-28 06:10:37.000000 pyyardian-1.0.0/pyyardian/__init__.py
--rw-r--r--   0 guang      (501) staff       (20)     2725 2023-07-28 06:00:43.000000 pyyardian-1.0.0/pyyardian/async_client.py
--rw-r--r--   0 guang      (501) staff       (20)      365 2023-07-25 08:17:15.000000 pyyardian-1.0.0/pyyardian/const.py
--rw-r--r--   0 guang      (501) staff       (20)      196 2023-07-28 05:57:00.000000 pyyardian-1.0.0/pyyardian/exceptions.py
-drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-28 06:11:54.005075 pyyardian-1.0.0/pyyardian.egg-info/
--rw-r--r--   0 guang      (501) staff       (20)      454 2023-07-28 06:11:53.000000 pyyardian-1.0.0/pyyardian.egg-info/PKG-INFO
--rw-r--r--   0 guang      (501) staff       (20)      259 2023-07-28 06:11:53.000000 pyyardian-1.0.0/pyyardian.egg-info/SOURCES.txt
--rw-r--r--   0 guang      (501) staff       (20)        1 2023-07-28 06:11:53.000000 pyyardian-1.0.0/pyyardian.egg-info/dependency_links.txt
--rw-r--r--   0 guang      (501) staff       (20)       10 2023-07-28 06:11:53.000000 pyyardian-1.0.0/pyyardian.egg-info/top_level.txt
--rw-r--r--   0 guang      (501) staff       (20)      107 2023-07-28 06:11:54.007171 pyyardian-1.0.0/setup.cfg
--rw-r--r--   0 guang      (501) staff       (20)      570 2023-07-28 06:01:11.000000 pyyardian-1.0.0/setup.py
+drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-28 06:32:35.629242 pyyardian-1.0.1/
+-rw-r--r--   0 guang      (501) staff       (20)     1072 2023-07-25 08:04:44.000000 pyyardian-1.0.1/LICENSE
+-rw-r--r--   0 guang      (501) staff       (20)      454 2023-07-28 06:32:35.629471 pyyardian-1.0.1/PKG-INFO
+-rw-r--r--   0 guang      (501) staff       (20)      150 2023-07-25 08:09:39.000000 pyyardian-1.0.1/README.md
+drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-28 06:32:35.624115 pyyardian-1.0.1/pyyardian/
+-rw-r--r--   0 guang      (501) staff       (20)      109 2023-07-28 06:10:37.000000 pyyardian-1.0.1/pyyardian/__init__.py
+-rw-r--r--   0 guang      (501) staff       (20)     2746 2023-07-28 06:30:58.000000 pyyardian-1.0.1/pyyardian/async_client.py
+-rw-r--r--   0 guang      (501) staff       (20)      365 2023-07-25 08:17:15.000000 pyyardian-1.0.1/pyyardian/const.py
+-rw-r--r--   0 guang      (501) staff       (20)      196 2023-07-28 05:57:00.000000 pyyardian-1.0.1/pyyardian/exceptions.py
+drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-28 06:32:35.628493 pyyardian-1.0.1/pyyardian.egg-info/
+-rw-r--r--   0 guang      (501) staff       (20)      454 2023-07-28 06:32:35.000000 pyyardian-1.0.1/pyyardian.egg-info/PKG-INFO
+-rw-r--r--   0 guang      (501) staff       (20)      259 2023-07-28 06:32:35.000000 pyyardian-1.0.1/pyyardian.egg-info/SOURCES.txt
+-rw-r--r--   0 guang      (501) staff       (20)        1 2023-07-28 06:32:35.000000 pyyardian-1.0.1/pyyardian.egg-info/dependency_links.txt
+-rw-r--r--   0 guang      (501) staff       (20)       10 2023-07-28 06:32:35.000000 pyyardian-1.0.1/pyyardian.egg-info/top_level.txt
+-rw-r--r--   0 guang      (501) staff       (20)      107 2023-07-28 06:32:35.630292 pyyardian-1.0.1/setup.cfg
+-rw-r--r--   0 guang      (501) staff       (20)      570 2023-07-28 06:31:56.000000 pyyardian-1.0.1/setup.py
```

### Comparing `pyyardian-1.0.0/LICENSE` & `pyyardian-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyyardian-1.0.0/pyyardian/async_client.py` & `pyyardian-1.0.1/pyyardian/async_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
         iCode = resp.get("iCode", 0)
         if iCode == 0:
             return resp["result"]
         elif iCode == -1000:
             raise NotAuthorizedException()
         else:
-            raise Exception()
+            raise NetworkException()
 
     async def fetch_device_info(self):
         resp = await (
             await self._websession.request(
                 "GET",
                 f"{self._base_url}/API_GET_DEVICEINFO",
                 headers=self._base_header,
@@ -43,15 +43,15 @@
 
         iCode = resp.get("iCode", 0)
         if iCode == 0:
             return resp | MODEL_DETAIL[resp["model"]]
         elif iCode == -1000:
             raise NotAuthorizedException()
         else:
-            raise Exception()
+            raise NetworkException()
 
 
     async def fetch_active_zones(self):
         resp = await (
             await self._websession.request(
                 "GET",
                 f"{self._base_url}/API_ZONE_GET_OPENINGZONE",
@@ -62,15 +62,15 @@
 
         iCode = resp.get("iCode", 0)
         if iCode == 0:
             return resp["result"]
         elif iCode == -1000:
             raise NotAuthorizedException()
         else:
-            raise Exception()
+            raise NetworkException()
 
 
     async def fetch_zone_info(self, amount=8):
         oper_info = await self.fetch_oper_info()
         return oper_info["zones"][:amount]
 
     async def start_irrigation(self, zone_id, duration):
```

### Comparing `pyyardian-1.0.0/setup.py` & `pyyardian-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name="pyyardian",
-    version="1.0.0",
+    version="1.0.1",
     license="MIT",
     author="Marty Sun",
     author_email="marty.sun@aeonmatrix.com",
     description="A module for interacting with the Yardian irrigation controller",
     long_description=" Python module for interacting with the Yardian irrigation controller. This module communicates directly towards the IP address of the Yardian device.",
     long_description_content_type="text/markdown",
     url="https://github.com/h3l1o5/pyyardian",
```

