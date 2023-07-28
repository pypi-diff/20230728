# Comparing `tmp/hscan-2.7.0.tar.gz` & `tmp/hscan-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscan-2.7.0.tar", last modified: Thu Jul 13 11:07:59 2023, max compression
+gzip compressed data, was "hscan-2.7.1.tar", last modified: Fri Jul 28 01:37:12 2023, max compression
```

## Comparing `hscan-2.7.0.tar` & `hscan-2.7.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-07-13 11:07:59.401598 hscan-2.7.0/
--rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-07-13 11:07:59.401365 hscan-2.7.0/PKG-INFO
--rw-r--r--   0 jyanghe    (501) staff       (20)       80 2021-09-07 07:20:00.000000 hscan-2.7.0/README.md
--rw-r--r--   0 jyanghe    (501) staff       (20)     1032 2023-07-13 11:05:39.000000 hscan-2.7.0/Setup.py
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-07-13 11:07:59.391545 hscan-2.7.0/hscan.egg-info/
--rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-07-13 11:07:59.000000 hscan-2.7.0/hscan.egg-info/PKG-INFO
--rw-r--r--   0 jyanghe    (501) staff       (20)      548 2023-07-13 11:07:59.000000 hscan-2.7.0/hscan.egg-info/SOURCES.txt
--rw-r--r--   0 jyanghe    (501) staff       (20)        1 2023-07-13 11:07:59.000000 hscan-2.7.0/hscan.egg-info/dependency_links.txt
--rw-r--r--   0 jyanghe    (501) staff       (20)      227 2023-07-13 11:07:59.000000 hscan-2.7.0/hscan.egg-info/requires.txt
--rw-r--r--   0 jyanghe    (501) staff       (20)        5 2023-07-13 11:07:59.000000 hscan-2.7.0/hscan.egg-info/top_level.txt
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-07-13 11:07:59.395934 hscan-2.7.0/scan/
--rw-r--r--   0 jyanghe    (501) staff       (20)      181 2023-04-03 10:06:56.000000 hscan-2.7.0/scan/__init__.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      301 2021-09-04 15:30:38.000000 hscan-2.7.0/scan/common.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1195 2022-12-24 12:34:00.000000 hscan-2.7.0/scan/config.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      866 2023-06-26 06:03:50.000000 hscan-2.7.0/scan/crawl.py
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-07-13 11:07:59.400436 hscan-2.7.0/scan/database/
--rw-r--r--   0 jyanghe    (501) staff       (20)      235 2022-12-20 15:11:44.000000 hscan-2.7.0/scan/database/__init__.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     6325 2023-02-23 13:03:29.000000 hscan-2.7.0/scan/database/kafka.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1112 2021-09-06 03:30:11.000000 hscan-2.7.0/scan/database/mongodb.py
--rw-r--r--   0 jyanghe    (501) staff       (20)        0 2023-01-16 12:29:44.000000 hscan-2.7.0/scan/database/mysql.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      508 2021-09-06 03:30:20.000000 hscan-2.7.0/scan/database/oss.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      954 2022-09-09 07:43:05.000000 hscan-2.7.0/scan/database/pg.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     6093 2023-04-27 08:36:36.000000 hscan-2.7.0/scan/database/rabbitmq.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     2098 2022-12-22 03:15:19.000000 hscan-2.7.0/scan/database/redis.py
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-07-13 11:07:59.401058 hscan-2.7.0/scan/downloade/
--rw-r--r--   0 jyanghe    (501) staff       (20)        0 2021-09-01 10:54:34.000000 hscan-2.7.0/scan/downloade/__init__.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     6338 2023-07-13 11:04:06.000000 hscan-2.7.0/scan/downloade/downloader.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      529 2022-09-09 07:40:26.000000 hscan-2.7.0/scan/log.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     2790 2023-04-04 03:33:16.000000 hscan-2.7.0/scan/monitor.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1945 2022-04-29 03:52:46.000000 hscan-2.7.0/scan/response.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     9784 2022-12-27 08:14:30.000000 hscan-2.7.0/scan/spider.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1022 2023-06-19 03:37:35.000000 hscan-2.7.0/scan/util.py
--rw-r--r--   0 jyanghe    (501) staff       (20)       38 2023-07-13 11:07:59.401674 hscan-2.7.0/setup.cfg
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-07-28 01:37:12.329194 hscan-2.7.1/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-07-28 01:37:12.328720 hscan-2.7.1/PKG-INFO
+-rw-r--r--   0 jyanghe    (501) staff       (20)       80 2021-09-07 07:20:00.000000 hscan-2.7.1/README.md
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1032 2023-07-28 01:36:28.000000 hscan-2.7.1/Setup.py
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-07-28 01:37:12.313820 hscan-2.7.1/hscan.egg-info/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-07-28 01:37:12.000000 hscan-2.7.1/hscan.egg-info/PKG-INFO
+-rw-r--r--   0 jyanghe    (501) staff       (20)      548 2023-07-28 01:37:12.000000 hscan-2.7.1/hscan.egg-info/SOURCES.txt
+-rw-r--r--   0 jyanghe    (501) staff       (20)        1 2023-07-28 01:37:12.000000 hscan-2.7.1/hscan.egg-info/dependency_links.txt
+-rw-r--r--   0 jyanghe    (501) staff       (20)      227 2023-07-28 01:37:12.000000 hscan-2.7.1/hscan.egg-info/requires.txt
+-rw-r--r--   0 jyanghe    (501) staff       (20)        5 2023-07-28 01:37:12.000000 hscan-2.7.1/hscan.egg-info/top_level.txt
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-07-28 01:37:12.320431 hscan-2.7.1/scan/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      181 2023-04-03 10:06:56.000000 hscan-2.7.1/scan/__init__.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      301 2021-09-04 15:30:38.000000 hscan-2.7.1/scan/common.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1195 2022-12-24 12:34:00.000000 hscan-2.7.1/scan/config.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      866 2023-06-26 06:03:50.000000 hscan-2.7.1/scan/crawl.py
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-07-28 01:37:12.326027 hscan-2.7.1/scan/database/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      235 2022-12-20 15:11:44.000000 hscan-2.7.1/scan/database/__init__.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     6325 2023-02-23 13:03:29.000000 hscan-2.7.1/scan/database/kafka.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1112 2021-09-06 03:30:11.000000 hscan-2.7.1/scan/database/mongodb.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)        0 2023-01-16 12:29:44.000000 hscan-2.7.1/scan/database/mysql.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      508 2021-09-06 03:30:20.000000 hscan-2.7.1/scan/database/oss.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      954 2022-09-09 07:43:05.000000 hscan-2.7.1/scan/database/pg.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     6093 2023-04-27 08:36:36.000000 hscan-2.7.1/scan/database/rabbitmq.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     2098 2022-12-22 03:15:19.000000 hscan-2.7.1/scan/database/redis.py
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-07-28 01:37:12.327498 hscan-2.7.1/scan/downloade/
+-rw-r--r--   0 jyanghe    (501) staff       (20)        0 2021-09-01 10:54:34.000000 hscan-2.7.1/scan/downloade/__init__.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     6338 2023-07-13 11:04:06.000000 hscan-2.7.1/scan/downloade/downloader.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      529 2022-09-09 07:40:26.000000 hscan-2.7.1/scan/log.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     2790 2023-04-04 03:33:16.000000 hscan-2.7.1/scan/monitor.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1945 2022-04-29 03:52:46.000000 hscan-2.7.1/scan/response.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     9915 2023-07-28 01:36:10.000000 hscan-2.7.1/scan/spider.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1022 2023-06-19 03:37:35.000000 hscan-2.7.1/scan/util.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)       38 2023-07-28 01:37:12.329325 hscan-2.7.1/setup.cfg
```

### Comparing `hscan-2.7.0/Setup.py` & `hscan-2.7.1/Setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hscan",
-    version="2.7.0",
+    version="2.7.1",
     author="jyanghe",
     author_email="jyanghe1023@gmail.com",
     description="A python framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jyangHe/hscan",
     packages=setuptools.find_packages(),
```

### Comparing `hscan-2.7.0/hscan.egg-info/SOURCES.txt` & `hscan-2.7.1/hscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hscan-2.7.0/scan/config.py` & `hscan-2.7.1/scan/config.py`

 * *Files identical despite different names*

### Comparing `hscan-2.7.0/scan/crawl.py` & `hscan-2.7.1/scan/crawl.py`

 * *Files identical despite different names*

### Comparing `hscan-2.7.0/scan/database/kafka.py` & `hscan-2.7.1/scan/database/kafka.py`

 * *Files identical despite different names*

### Comparing `hscan-2.7.0/scan/database/mongodb.py` & `hscan-2.7.1/scan/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `hscan-2.7.0/scan/database/pg.py` & `hscan-2.7.1/scan/database/pg.py`

 * *Files identical despite different names*

### Comparing `hscan-2.7.0/scan/database/rabbitmq.py` & `hscan-2.7.1/scan/database/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `hscan-2.7.0/scan/database/redis.py` & `hscan-2.7.1/scan/database/redis.py`

 * *Files identical despite different names*

### Comparing `hscan-2.7.0/scan/downloade/downloader.py` & `hscan-2.7.1/scan/downloade/downloader.py`

 * *Files identical despite different names*

### Comparing `hscan-2.7.0/scan/log.py` & `hscan-2.7.1/scan/log.py`

 * *Files identical despite different names*

### Comparing `hscan-2.7.0/scan/monitor.py` & `hscan-2.7.1/scan/monitor.py`

 * *Files identical despite different names*

### Comparing `hscan-2.7.0/scan/response.py` & `hscan-2.7.1/scan/response.py`

 * *Files identical despite different names*

### Comparing `hscan-2.7.0/scan/spider.py` & `hscan-2.7.1/scan/spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,17 +185,21 @@
         if not self.rabbitmq:
             logger.error('The task queue connection is not initialized')
             return
         arguments = None
         # 优先级队列
         if self.config.rabbitmq().get('priority'):
             arguments = {'x-max-priority': int(self.config.rabbitmq().get('priority'))}
+        if self.config.rabbitmq().get('no_ack'):
+            no_ack = True
+        else:
+            no_ack = False
         while self.status:
             try:
-                await self.rabbitmq.consume(self.process, task_queue, arguments=arguments)
+                await self.rabbitmq.consume(self.process, task_queue, no_ack=no_ack, arguments=arguments)
             except Exception as e:
                 logger.error(e)
 
     async def redis_task(self):
         """
         分布式队列任务，在任务分发使用redis时
         """
```

### Comparing `hscan-2.7.0/scan/util.py` & `hscan-2.7.1/scan/util.py`

 * *Files identical despite different names*

