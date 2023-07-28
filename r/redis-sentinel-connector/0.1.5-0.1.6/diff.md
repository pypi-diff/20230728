# Comparing `tmp/redis_sentinel_connector-0.1.5.tar.gz` & `tmp/redis_sentinel_connector-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ronaldo/Documents/Projetos/redis_sentinel_connector/dist/tmphil4cvnd/redis_sentinel_connector-0.1.5.tar", last modified: Thu May 12 21:33:17 2022, max compression
+gzip compressed data, was "redis_sentinel_connector-0.1.6.tar", last modified: Fri Jul 28 17:56:08 2023, max compression
```

## Comparing `redis_sentinel_connector-0.1.5.tar` & `redis_sentinel_connector-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ronaldo    (502) staff       (20)        0 2022-05-12 21:33:17.426509 redis_sentinel_connector-0.1.5/
--rw-r--r--   0 ronaldo    (502) staff       (20)    35148 2021-10-13 23:07:38.000000 redis_sentinel_connector-0.1.5/LICENSE.txt
--rw-r--r--   0 ronaldo    (502) staff       (20)     1698 2022-05-12 21:33:17.426361 redis_sentinel_connector-0.1.5/PKG-INFO
--rw-r--r--   0 ronaldo    (502) staff       (20)     1165 2021-10-13 23:07:38.000000 redis_sentinel_connector-0.1.5/README.md
-drwxr-xr-x   0 ronaldo    (502) staff       (20)        0 2022-05-12 21:33:17.421779 redis_sentinel_connector-0.1.5/redis_sentinel_connector/
--rw-r--r--   0 ronaldo    (502) staff       (20)       44 2021-10-13 23:07:38.000000 redis_sentinel_connector-0.1.5/redis_sentinel_connector/__init__.py
--rw-r--r--   0 ronaldo    (502) staff       (20)     1682 2021-10-14 01:03:00.000000 redis_sentinel_connector-0.1.5/redis_sentinel_connector/redis_connector.py
-drwxr-xr-x   0 ronaldo    (502) staff       (20)        0 2022-05-12 21:33:17.426143 redis_sentinel_connector-0.1.5/redis_sentinel_connector.egg-info/
--rw-r--r--   0 ronaldo    (502) staff       (20)     1698 2022-05-12 21:33:17.000000 redis_sentinel_connector-0.1.5/redis_sentinel_connector.egg-info/PKG-INFO
--rw-r--r--   0 ronaldo    (502) staff       (20)      350 2022-05-12 21:33:17.000000 redis_sentinel_connector-0.1.5/redis_sentinel_connector.egg-info/SOURCES.txt
--rw-r--r--   0 ronaldo    (502) staff       (20)        1 2022-05-12 21:33:17.000000 redis_sentinel_connector-0.1.5/redis_sentinel_connector.egg-info/dependency_links.txt
--rw-r--r--   0 ronaldo    (502) staff       (20)       30 2022-05-12 21:33:17.000000 redis_sentinel_connector-0.1.5/redis_sentinel_connector.egg-info/requires.txt
--rw-r--r--   0 ronaldo    (502) staff       (20)       25 2022-05-12 21:33:17.000000 redis_sentinel_connector-0.1.5/redis_sentinel_connector.egg-info/top_level.txt
--rw-r--r--   0 ronaldo    (502) staff       (20)       38 2022-05-12 21:33:17.426556 redis_sentinel_connector-0.1.5/setup.cfg
--rw-r--r--   0 ronaldo    (502) staff       (20)      812 2022-05-12 21:32:47.000000 redis_sentinel_connector-0.1.5/setup.py
+drwxr-xr-x   0 ronaldo    (502) staff       (20)        0 2023-07-28 17:56:08.289328 redis_sentinel_connector-0.1.6/
+-rw-r--r--   0 ronaldo    (502) staff       (20)    35148 2021-10-13 23:07:38.000000 redis_sentinel_connector-0.1.6/LICENSE.txt
+-rw-r--r--   0 ronaldo    (502) staff       (20)     1698 2023-07-28 17:56:08.289136 redis_sentinel_connector-0.1.6/PKG-INFO
+-rw-r--r--   0 ronaldo    (502) staff       (20)     1165 2021-10-13 23:07:38.000000 redis_sentinel_connector-0.1.6/README.md
+drwxr-xr-x   0 ronaldo    (502) staff       (20)        0 2023-07-28 17:56:08.287857 redis_sentinel_connector-0.1.6/redis_sentinel_connector/
+-rw-r--r--   0 ronaldo    (502) staff       (20)       44 2021-10-13 23:07:38.000000 redis_sentinel_connector-0.1.6/redis_sentinel_connector/__init__.py
+-rw-r--r--   0 ronaldo    (502) staff       (20)     1889 2022-11-10 10:13:15.000000 redis_sentinel_connector-0.1.6/redis_sentinel_connector/redis_connector.py
+drwxr-xr-x   0 ronaldo    (502) staff       (20)        0 2023-07-28 17:56:08.288932 redis_sentinel_connector-0.1.6/redis_sentinel_connector.egg-info/
+-rw-r--r--   0 ronaldo    (502) staff       (20)     1698 2023-07-28 17:56:08.000000 redis_sentinel_connector-0.1.6/redis_sentinel_connector.egg-info/PKG-INFO
+-rw-r--r--   0 ronaldo    (502) staff       (20)      350 2023-07-28 17:56:08.000000 redis_sentinel_connector-0.1.6/redis_sentinel_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 ronaldo    (502) staff       (20)        1 2023-07-28 17:56:08.000000 redis_sentinel_connector-0.1.6/redis_sentinel_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 ronaldo    (502) staff       (20)       30 2023-07-28 17:56:08.000000 redis_sentinel_connector-0.1.6/redis_sentinel_connector.egg-info/requires.txt
+-rw-r--r--   0 ronaldo    (502) staff       (20)       25 2023-07-28 17:56:08.000000 redis_sentinel_connector-0.1.6/redis_sentinel_connector.egg-info/top_level.txt
+-rw-r--r--   0 ronaldo    (502) staff       (20)       38 2023-07-28 17:56:08.289377 redis_sentinel_connector-0.1.6/setup.cfg
+-rw-r--r--   0 ronaldo    (502) staff       (20)      812 2023-07-28 17:50:56.000000 redis_sentinel_connector-0.1.6/setup.py
```

### Comparing `redis_sentinel_connector-0.1.5/LICENSE.txt` & `redis_sentinel_connector-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `redis_sentinel_connector-0.1.5/PKG-INFO` & `redis_sentinel_connector-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis_sentinel_connector
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package that works with Redis Sentinel.
 Home-page: https://github.com/ronaldodduarte/redis_sentinel_connector
 Author: Ronaldo Duarte
 Author-email: ronaldoduarte@globo.com
 License: GNU
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `redis_sentinel_connector-0.1.5/README.md` & `redis_sentinel_connector-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `redis_sentinel_connector-0.1.5/redis_sentinel_connector/redis_connector.py` & `redis_sentinel_connector-0.1.6/redis_sentinel_connector/redis_connector.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,18 @@
         if cls not in cls._instances:
             cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
 class RedisConnector(metaclass=Singleton):
 
-    def __init__(self):
+    def __init__(self, socket_timeout=0.1):
         self.type = TYPE
         self.redis_url = REDIS_URL
+        self.socket_timeout = socket_timeout
 
     def connect(self, redis_url=None):
 
         if self.type == 'DEV':
             return redis.Redis()
         if self.type == 'TEST':
             return fakeredis.FakeStrictRedis(server=fakeredis.FakeServer())
@@ -34,16 +35,18 @@
 
         if not self.redis_url:
             raise Exception('You need to set REDIS_URL environment or set TYPE environment to [DEV || TEST] or '
                             'set the parameter redis_url in connect function.')
 
         hosts = self.get_hosts_from_redis_url()
 
-        return Sentinel([(host.split(':')[0], self.extract_port_from_host(host)) for host in hosts]).\
-            master_for(self.get_service_name(), password=self.get_password())
+        return Sentinel(
+            [(host.split(':')[0], self.extract_port_from_host(host)) for host in hosts],
+            socket_timeout=self.socket_timeout).master_for(self.get_service_name(), password=self.get_password(),
+                                                           socket_timeout=self.socket_timeout)
 
     def get_hosts_from_redis_url(self):
         return self.redis_url.split('@')[-1].split('/')[0].split(',')
 
     @staticmethod
     def extract_port_from_host(host):
         return host.split(':')[1]
```

### Comparing `redis_sentinel_connector-0.1.5/redis_sentinel_connector.egg-info/PKG-INFO` & `redis_sentinel_connector-0.1.6/redis_sentinel_connector.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-sentinel-connector
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package that works with Redis Sentinel.
 Home-page: https://github.com/ronaldodduarte/redis_sentinel_connector
 Author: Ronaldo Duarte
 Author-email: ronaldoduarte@globo.com
 License: GNU
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `redis_sentinel_connector-0.1.5/setup.py` & `redis_sentinel_connector-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="redis_sentinel_connector",
-    version="0.1.5",
+    version="0.1.6",
     author="Ronaldo Duarte",
     author_email="ronaldoduarte@globo.com",
     description="A package that works with Redis Sentinel.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ronaldodduarte/redis_sentinel_connector",
     install_requires=["redis==3.5.3", "fakeredis==1.6.1"],
```

