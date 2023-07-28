# Comparing `tmp/pyyardian-1.0.2.tar.gz` & `tmp/pyyardian-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyardian-1.0.2.tar", last modified: Fri Jul 28 06:42:37 2023, max compression
+gzip compressed data, was "pyyardian-1.0.3.tar", last modified: Fri Jul 28 06:46:12 2023, max compression
```

## Comparing `pyyardian-1.0.2.tar` & `pyyardian-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-28 06:42:37.181741 pyyardian-1.0.2/
--rw-r--r--   0 guang      (501) staff       (20)     1072 2023-07-25 08:04:44.000000 pyyardian-1.0.2/LICENSE
--rw-r--r--   0 guang      (501) staff       (20)      454 2023-07-28 06:42:37.181973 pyyardian-1.0.2/PKG-INFO
--rw-r--r--   0 guang      (501) staff       (20)      150 2023-07-25 08:09:39.000000 pyyardian-1.0.2/README.md
-drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-28 06:42:37.178736 pyyardian-1.0.2/pyyardian/
--rw-r--r--   0 guang      (501) staff       (20)      109 2023-07-28 06:10:37.000000 pyyardian-1.0.2/pyyardian/__init__.py
--rw-r--r--   0 guang      (501) staff       (20)     3105 2023-07-28 06:41:30.000000 pyyardian-1.0.2/pyyardian/async_client.py
--rw-r--r--   0 guang      (501) staff       (20)      365 2023-07-25 08:17:15.000000 pyyardian-1.0.2/pyyardian/const.py
--rw-r--r--   0 guang      (501) staff       (20)      196 2023-07-28 05:57:00.000000 pyyardian-1.0.2/pyyardian/exceptions.py
-drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-28 06:42:37.181111 pyyardian-1.0.2/pyyardian.egg-info/
--rw-r--r--   0 guang      (501) staff       (20)      454 2023-07-28 06:42:37.000000 pyyardian-1.0.2/pyyardian.egg-info/PKG-INFO
--rw-r--r--   0 guang      (501) staff       (20)      259 2023-07-28 06:42:37.000000 pyyardian-1.0.2/pyyardian.egg-info/SOURCES.txt
--rw-r--r--   0 guang      (501) staff       (20)        1 2023-07-28 06:42:37.000000 pyyardian-1.0.2/pyyardian.egg-info/dependency_links.txt
--rw-r--r--   0 guang      (501) staff       (20)       10 2023-07-28 06:42:37.000000 pyyardian-1.0.2/pyyardian.egg-info/top_level.txt
--rw-r--r--   0 guang      (501) staff       (20)      107 2023-07-28 06:42:37.182713 pyyardian-1.0.2/setup.cfg
--rw-r--r--   0 guang      (501) staff       (20)      570 2023-07-28 06:41:41.000000 pyyardian-1.0.2/setup.py
+drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-28 06:46:12.472937 pyyardian-1.0.3/
+-rw-r--r--   0 guang      (501) staff       (20)     1072 2023-07-25 08:04:44.000000 pyyardian-1.0.3/LICENSE
+-rw-r--r--   0 guang      (501) staff       (20)      454 2023-07-28 06:46:12.473180 pyyardian-1.0.3/PKG-INFO
+-rw-r--r--   0 guang      (501) staff       (20)      150 2023-07-25 08:09:39.000000 pyyardian-1.0.3/README.md
+drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-28 06:46:12.469036 pyyardian-1.0.3/pyyardian/
+-rw-r--r--   0 guang      (501) staff       (20)      109 2023-07-28 06:10:37.000000 pyyardian-1.0.3/pyyardian/__init__.py
+-rw-r--r--   0 guang      (501) staff       (20)     3143 2023-07-28 06:45:59.000000 pyyardian-1.0.3/pyyardian/async_client.py
+-rw-r--r--   0 guang      (501) staff       (20)      365 2023-07-25 08:17:15.000000 pyyardian-1.0.3/pyyardian/const.py
+-rw-r--r--   0 guang      (501) staff       (20)      196 2023-07-28 05:57:00.000000 pyyardian-1.0.3/pyyardian/exceptions.py
+drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-28 06:46:12.472474 pyyardian-1.0.3/pyyardian.egg-info/
+-rw-r--r--   0 guang      (501) staff       (20)      454 2023-07-28 06:46:12.000000 pyyardian-1.0.3/pyyardian.egg-info/PKG-INFO
+-rw-r--r--   0 guang      (501) staff       (20)      259 2023-07-28 06:46:12.000000 pyyardian-1.0.3/pyyardian.egg-info/SOURCES.txt
+-rw-r--r--   0 guang      (501) staff       (20)        1 2023-07-28 06:46:12.000000 pyyardian-1.0.3/pyyardian.egg-info/dependency_links.txt
+-rw-r--r--   0 guang      (501) staff       (20)       10 2023-07-28 06:46:12.000000 pyyardian-1.0.3/pyyardian.egg-info/top_level.txt
+-rw-r--r--   0 guang      (501) staff       (20)      107 2023-07-28 06:46:12.475513 pyyardian-1.0.3/setup.cfg
+-rw-r--r--   0 guang      (501) staff       (20)      570 2023-07-28 06:46:07.000000 pyyardian-1.0.3/setup.py
```

### Comparing `pyyardian-1.0.2/LICENSE` & `pyyardian-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyyardian-1.0.2/pyyardian/async_client.py` & `pyyardian-1.0.3/pyyardian/async_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,69 +19,68 @@
                 await self._websession.request(
                     "GET",
                     f"{self._base_url}/API_MGR_GET_OPERINFO",
                     headers=self._base_header,
                     timeout=DEFAULT_TIMEOUT,
                 )
             ).json()
-
+        except:
+            raise NetworkException()
+        else:
             iCode = resp.get("iCode", 0)
             if iCode == 0:
                 return resp["result"]
             elif iCode == -1000:
                 raise NotAuthorizedException()
             else:
                 raise Exception()
-        except:
-            raise NetworkException()
-
 
 
     async def fetch_device_info(self):
         try:
             resp = await (
                 await self._websession.request(
                     "GET",
                     f"{self._base_url}/API_GET_DEVICEINFO",
                     headers=self._base_header,
                     timeout=DEFAULT_TIMEOUT,
                 )
             ).json()
-
+        except:
+            raise NetworkException()
+        else:
             iCode = resp.get("iCode", 0)
             if iCode == 0:
                 return resp | MODEL_DETAIL[resp["model"]]
             elif iCode == -1000:
                 raise NotAuthorizedException()
             else:
                 raise Exception()
-        except:
-            raise NetworkException()
 
 
     async def fetch_active_zones(self):
         try:
             resp = await (
                 await self._websession.request(
                     "GET",
                     f"{self._base_url}/API_ZONE_GET_OPENINGZONE",
                     headers=self._base_header,
                     timeout=DEFAULT_TIMEOUT,
                 )
             ).json()
-
+        except:
+            raise NetworkException()
+        else:
             iCode = resp.get("iCode", 0)
             if iCode == 0:
                 return resp["result"]
             elif iCode == -1000:
                 raise NotAuthorizedException()
             else:
                 raise Exception()
-        except:
-            raise NetworkException()
 
 
     async def fetch_zone_info(self, amount=8):
         oper_info = await self.fetch_oper_info()
         return oper_info["zones"][:amount]
 
     async def start_irrigation(self, zone_id, duration):
```

### Comparing `pyyardian-1.0.2/setup.py` & `pyyardian-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name="pyyardian",
-    version="1.0.2",
+    version="1.0.3",
     license="MIT",
     author="Marty Sun",
     author_email="marty.sun@aeonmatrix.com",
     description="A module for interacting with the Yardian irrigation controller",
     long_description=" Python module for interacting with the Yardian irrigation controller. This module communicates directly towards the IP address of the Yardian device.",
     long_description_content_type="text/markdown",
     url="https://github.com/h3l1o5/pyyardian",
```

