# Comparing `tmp/aioscrapy_redis-0.1.tar.gz` & `tmp/aioscrapy_redis-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\aioscrapy_redis-0.1.tar", last modified: Fri Feb 19 10:10:39 2021, max compression
+gzip compressed data, was "aioscrapy_redis-0.3.tar", last modified: Fri Jul 28 02:09:58 2023, max compression
```

## Comparing `aioscrapy_redis-0.1.tar` & `aioscrapy_redis-0.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2021-02-19 10:10:39.000000 aioscrapy_redis-0.1/
--rw-rw-rw-   0        0        0     1383 2021-02-19 10:10:39.000000 aioscrapy_redis-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      613 2021-02-19 10:07:03.000000 aioscrapy_redis-0.1/README.md
-drwxrwxrwx   0        0        0        0 2021-02-19 10:10:39.000000 aioscrapy_redis-0.1/aioscrapy_redis/
--rw-rw-rw-   0        0        0       32 2020-04-07 01:45:44.000000 aioscrapy_redis-0.1/aioscrapy_redis/__init__.py
-drwxrwxrwx   0        0        0        0 2021-02-19 10:10:39.000000 aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/
--rw-rw-rw-   0        0        0      193 2020-04-07 01:45:44.000000 aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/__init__.py
--rw-rw-rw-   0        0        0      192 2020-07-27 05:53:14.000000 aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/common.py
--rw-rw-rw-   0        0        0     1218 2021-01-05 09:44:53.000000 aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/connection.py
--rw-rw-rw-   0        0        0      727 2020-04-07 01:45:44.000000 aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/defaults.py
--rw-rw-rw-   0        0        0     2820 2021-02-19 08:59:08.000000 aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/dupefilter.py
--rw-rw-rw-   0        0        0      263 2020-04-07 01:45:44.000000 aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/picklecompat.py
--rw-rw-rw-   0        0        0     1201 2021-02-19 08:59:08.000000 aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/pipelines.py
-drwxrwxrwx   0        0        0        0 2021-02-19 10:10:39.000000 aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/utils/
--rw-rw-rw-   0        0        0       72 2020-04-07 01:45:44.000000 aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/utils/__init__.py
--rw-rw-rw-   0        0        0      912 2020-08-04 09:23:58.000000 aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/utils/decorators.py
--rw-rw-rw-   0        0        0     1396 2020-04-07 01:45:44.000000 aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/utils/exceptions.py
--rw-rw-rw-   0        0        0     3743 2021-01-05 09:52:49.000000 aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/utils/misc.py
--rw-rw-rw-   0        0        0    11894 2021-01-05 09:44:53.000000 aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/utils/python.py
--rw-rw-rw-   0        0        0     2474 2021-01-05 09:44:53.000000 aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/utils/reqser.py
-drwxrwxrwx   0        0        0        0 2021-02-19 10:10:39.000000 aioscrapy_redis-0.1/aioscrapy_redis/core/
--rw-rw-rw-   0        0        0       24 2020-04-07 01:45:44.000000 aioscrapy_redis-0.1/aioscrapy_redis/core/__init__.py
-drwxrwxrwx   0        0        0        0 2021-02-19 10:10:39.000000 aioscrapy_redis-0.1/aioscrapy_redis/core/downloader/
--rw-rw-rw-   0        0        0       24 2020-04-07 01:45:44.000000 aioscrapy_redis-0.1/aioscrapy_redis/core/downloader/__init__.py
--rw-rw-rw-   0        0        0     5889 2021-02-19 09:08:54.000000 aioscrapy_redis-0.1/aioscrapy_redis/core/downloader/downloader.py
--rw-rw-rw-   0        0        0     7870 2021-02-19 09:15:44.000000 aioscrapy_redis-0.1/aioscrapy_redis/core/engine.py
--rw-rw-rw-   0        0        0     2130 2021-02-19 09:17:19.000000 aioscrapy_redis-0.1/aioscrapy_redis/core/scheduler.py
--rw-rw-rw-   0        0        0     3297 2021-02-19 09:20:38.000000 aioscrapy_redis-0.1/aioscrapy_redis/core/spider.py
-drwxrwxrwx   0        0        0        0 2021-02-19 10:10:39.000000 aioscrapy_redis-0.1/aioscrapy_redis/downloadermiddlewares/
--rw-rw-rw-   0        0        0       72 2020-04-07 01:45:44.000000 aioscrapy_redis-0.1/aioscrapy_redis/downloadermiddlewares/__init__.py
--rw-rw-rw-   0        0        0      310 2021-02-19 08:59:08.000000 aioscrapy_redis-0.1/aioscrapy_redis/downloadermiddlewares/middlewares.py
-drwxrwxrwx   0        0        0        0 2021-02-19 10:10:39.000000 aioscrapy_redis-0.1/aioscrapy_redis/https/
--rw-rw-rw-   0        0        0        0 2020-04-07 01:45:44.000000 aioscrapy_redis-0.1/aioscrapy_redis/https/__init__.py
--rw-rw-rw-   0        0        0     8210 2021-02-19 09:25:10.000000 aioscrapy_redis-0.1/aioscrapy_redis/https/form.py
--rw-rw-rw-   0        0        0      184 2021-01-05 09:35:42.000000 aioscrapy_redis-0.1/aioscrapy_redis/https/html.py
--rw-rw-rw-   0        0        0     3062 2021-02-19 09:23:49.000000 aioscrapy_redis-0.1/aioscrapy_redis/https/request.py
--rw-rw-rw-   0        0        0     3488 2021-02-19 09:21:56.000000 aioscrapy_redis-0.1/aioscrapy_redis/https/response.py
-drwxrwxrwx   0        0        0        0 2021-02-19 10:10:39.000000 aioscrapy_redis-0.1/aioscrapy_redis/utils/
--rw-rw-rw-   0        0        0       26 2020-04-07 01:45:44.000000 aioscrapy_redis-0.1/aioscrapy_redis/utils/__init__.py
--rw-rw-rw-   0        0        0     7352 2020-04-07 01:45:44.000000 aioscrapy_redis-0.1/aioscrapy_redis/utils/basesettings.py
--rw-rw-rw-   0        0        0     3996 2021-02-19 08:59:08.000000 aioscrapy_redis-0.1/aioscrapy_redis/utils/get_settings.py
--rw-rw-rw-   0        0        0   109627 2020-08-24 01:29:51.000000 aioscrapy_redis-0.1/aioscrapy_redis/utils/header_ua.py
--rw-rw-rw-   0        0        0      224 2020-04-13 08:22:49.000000 aioscrapy_redis-0.1/aioscrapy_redis/utils/http_proxy.py
--rw-rw-rw-   0        0        0     5539 2021-01-05 09:52:50.000000 aioscrapy_redis-0.1/aioscrapy_redis/utils/item.py
--rw-rw-rw-   0        0        0      755 2021-02-19 09:37:56.000000 aioscrapy_redis-0.1/aioscrapy_redis/utils/log.py
--rw-rw-rw-   0        0        0     2307 2021-02-19 09:38:29.000000 aioscrapy_redis-0.1/aioscrapy_redis/utils/logstats.py
--rw-rw-rw-   0        0        0     1223 2021-01-05 09:52:50.000000 aioscrapy_redis-0.1/aioscrapy_redis/utils/serialize.py
--rw-rw-rw-   0        0        0      104 2020-07-23 08:05:00.000000 aioscrapy_redis-0.1/aioscrapy_redis/utils/settings.py
--rw-rw-rw-   0        0        0     1688 2021-02-19 09:41:10.000000 aioscrapy_redis-0.1/aioscrapy_redis/utils/tools.py
--rw-rw-rw-   0        0        0      534 2020-08-04 08:56:10.000000 aioscrapy_redis-0.1/aioscrapy_redis/utils/trackref.py
-drwxrwxrwx   0        0        0        0 2021-02-19 10:10:39.000000 aioscrapy_redis-0.1/aioscrapy_redis.egg-info/
--rw-rw-rw-   0        0        0     1383 2021-02-19 10:10:38.000000 aioscrapy_redis-0.1/aioscrapy_redis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1767 2021-02-19 10:10:38.000000 aioscrapy_redis-0.1/aioscrapy_redis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-02-19 10:10:38.000000 aioscrapy_redis-0.1/aioscrapy_redis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-02-19 10:10:38.000000 aioscrapy_redis-0.1/aioscrapy_redis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      126 2021-02-19 10:10:38.000000 aioscrapy_redis-0.1/aioscrapy_redis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2021-02-19 10:10:38.000000 aioscrapy_redis-0.1/aioscrapy_redis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-02-19 10:10:39.000000 aioscrapy_redis-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1220 2021-02-19 10:00:17.000000 aioscrapy_redis-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:09:58.977824 aioscrapy_redis-0.3/
+-rw-rw-rw-   0        0        0     1383 2023-07-28 02:09:58.976826 aioscrapy_redis-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      613 2021-02-19 10:07:03.000000 aioscrapy_redis-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 02:09:58.868117 aioscrapy_redis-0.3/aioscrapy_redis/
+-rw-rw-rw-   0        0        0       32 2020-04-07 01:45:44.000000 aioscrapy_redis-0.3/aioscrapy_redis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:09:58.897039 aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/
+-rw-rw-rw-   0        0        0      193 2020-04-07 01:45:44.000000 aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/__init__.py
+-rw-rw-rw-   0        0        0      192 2020-07-27 05:53:14.000000 aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/common.py
+-rw-rw-rw-   0        0        0     1218 2021-01-05 09:44:53.000000 aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/connection.py
+-rw-rw-rw-   0        0        0      727 2020-04-07 01:45:44.000000 aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/defaults.py
+-rw-rw-rw-   0        0        0     2820 2021-02-19 08:59:08.000000 aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/dupefilter.py
+-rw-rw-rw-   0        0        0      263 2020-04-07 01:45:44.000000 aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/picklecompat.py
+-rw-rw-rw-   0        0        0     1201 2021-02-19 08:59:08.000000 aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/pipelines.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:09:58.910004 aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/utils/
+-rw-rw-rw-   0        0        0       72 2020-04-07 01:45:44.000000 aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/utils/__init__.py
+-rw-rw-rw-   0        0        0      912 2020-08-04 09:23:58.000000 aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/utils/decorators.py
+-rw-rw-rw-   0        0        0     1396 2020-04-07 01:45:44.000000 aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/utils/exceptions.py
+-rw-rw-rw-   0        0        0     4545 2023-07-28 02:06:49.000000 aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/utils/misc.py
+-rw-rw-rw-   0        0        0    11894 2021-01-05 09:44:53.000000 aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/utils/python.py
+-rw-rw-rw-   0        0        0     2474 2021-01-05 09:44:53.000000 aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/utils/reqser.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:09:58.920975 aioscrapy_redis-0.3/aioscrapy_redis/core/
+-rw-rw-rw-   0        0        0       24 2020-04-07 01:45:44.000000 aioscrapy_redis-0.3/aioscrapy_redis/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:09:58.923967 aioscrapy_redis-0.3/aioscrapy_redis/core/downloader/
+-rw-rw-rw-   0        0        0       24 2020-04-07 01:45:44.000000 aioscrapy_redis-0.3/aioscrapy_redis/core/downloader/__init__.py
+-rw-rw-rw-   0        0        0     5889 2021-02-19 09:08:54.000000 aioscrapy_redis-0.3/aioscrapy_redis/core/downloader/downloader.py
+-rw-rw-rw-   0        0        0     7870 2021-02-19 09:15:44.000000 aioscrapy_redis-0.3/aioscrapy_redis/core/engine.py
+-rw-rw-rw-   0        0        0     2130 2021-02-19 09:17:19.000000 aioscrapy_redis-0.3/aioscrapy_redis/core/scheduler.py
+-rw-rw-rw-   0        0        0     3297 2021-02-19 09:20:38.000000 aioscrapy_redis-0.3/aioscrapy_redis/core/spider.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:09:58.929951 aioscrapy_redis-0.3/aioscrapy_redis/downloadermiddlewares/
+-rw-rw-rw-   0        0        0       72 2020-04-07 01:45:44.000000 aioscrapy_redis-0.3/aioscrapy_redis/downloadermiddlewares/__init__.py
+-rw-rw-rw-   0        0        0      310 2021-02-19 08:59:08.000000 aioscrapy_redis-0.3/aioscrapy_redis/downloadermiddlewares/middlewares.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:09:58.939924 aioscrapy_redis-0.3/aioscrapy_redis/https/
+-rw-rw-rw-   0        0        0        0 2020-04-07 01:45:44.000000 aioscrapy_redis-0.3/aioscrapy_redis/https/__init__.py
+-rw-rw-rw-   0        0        0     8210 2021-02-19 09:25:10.000000 aioscrapy_redis-0.3/aioscrapy_redis/https/form.py
+-rw-rw-rw-   0        0        0      184 2021-01-05 09:35:42.000000 aioscrapy_redis-0.3/aioscrapy_redis/https/html.py
+-rw-rw-rw-   0        0        0     3062 2021-02-19 09:23:49.000000 aioscrapy_redis-0.3/aioscrapy_redis/https/request.py
+-rw-rw-rw-   0        0        0     3488 2021-02-19 09:21:56.000000 aioscrapy_redis-0.3/aioscrapy_redis/https/response.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:09:58.973834 aioscrapy_redis-0.3/aioscrapy_redis/utils/
+-rw-rw-rw-   0        0        0       29 2023-07-28 02:06:49.000000 aioscrapy_redis-0.3/aioscrapy_redis/utils/__init__.py
+-rw-rw-rw-   0        0        0     7774 2023-07-28 02:06:49.000000 aioscrapy_redis-0.3/aioscrapy_redis/utils/basesettings.py
+-rw-rw-rw-   0        0        0     3996 2021-02-19 08:59:08.000000 aioscrapy_redis-0.3/aioscrapy_redis/utils/get_settings.py
+-rw-rw-rw-   0        0        0   109627 2020-08-24 01:29:51.000000 aioscrapy_redis-0.3/aioscrapy_redis/utils/header_ua.py
+-rw-rw-rw-   0        0        0      224 2020-04-13 08:22:49.000000 aioscrapy_redis-0.3/aioscrapy_redis/utils/http_proxy.py
+-rw-rw-rw-   0        0        0     5539 2021-01-05 09:52:50.000000 aioscrapy_redis-0.3/aioscrapy_redis/utils/item.py
+-rw-rw-rw-   0        0        0      755 2021-02-19 09:37:56.000000 aioscrapy_redis-0.3/aioscrapy_redis/utils/log.py
+-rw-rw-rw-   0        0        0     2307 2021-02-19 09:38:29.000000 aioscrapy_redis-0.3/aioscrapy_redis/utils/logstats.py
+-rw-rw-rw-   0        0        0     1223 2021-01-05 09:52:50.000000 aioscrapy_redis-0.3/aioscrapy_redis/utils/serialize.py
+-rw-rw-rw-   0        0        0      104 2020-07-23 08:05:00.000000 aioscrapy_redis-0.3/aioscrapy_redis/utils/settings.py
+-rw-rw-rw-   0        0        0     1688 2021-02-19 09:41:10.000000 aioscrapy_redis-0.3/aioscrapy_redis/utils/tools.py
+-rw-rw-rw-   0        0        0      534 2020-08-04 08:56:10.000000 aioscrapy_redis-0.3/aioscrapy_redis/utils/trackref.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:09:58.882079 aioscrapy_redis-0.3/aioscrapy_redis.egg-info/
+-rw-rw-rw-   0        0        0     1383 2023-07-28 02:09:58.000000 aioscrapy_redis-0.3/aioscrapy_redis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1767 2023-07-28 02:09:58.000000 aioscrapy_redis-0.3/aioscrapy_redis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 02:09:58.000000 aioscrapy_redis-0.3/aioscrapy_redis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 02:09:58.000000 aioscrapy_redis-0.3/aioscrapy_redis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      126 2023-07-28 02:09:58.000000 aioscrapy_redis-0.3/aioscrapy_redis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-28 02:09:58.000000 aioscrapy_redis-0.3/aioscrapy_redis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 02:09:58.977824 aioscrapy_redis-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1269 2023-07-28 02:09:39.000000 aioscrapy_redis-0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aioscrapy_redis-0.1/PKG-INFO` & `aioscrapy_redis-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioscrapy_redis
-Version: 0.1
+Version: 0.3
 Summary: A mini spider framework, Integrate aiohttp into scrapy
 Home-page: https://github.com/pythonlw/aioscrapy_redis
 Author: 道法自然_Tor
 Author-email: 1540310556@qq.com
 License: Apache License v2
 Description: Python async library for web scraping
         PyPI version License: MIT
```

### Comparing `aioscrapy_redis-0.1/README.md` & `aioscrapy_redis-0.3/README.md`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/connection.py` & `aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/connection.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/defaults.py` & `aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/defaults.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/dupefilter.py` & `aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/dupefilter.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/pipelines.py` & `aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/pipelines.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/utils/decorators.py` & `aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/utils/exceptions.py` & `aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/utils/python.py` & `aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/utils/python.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/aioscrapyredis/utils/reqser.py` & `aioscrapy_redis-0.3/aioscrapy_redis/aioscrapyredis/utils/reqser.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/core/downloader/downloader.py` & `aioscrapy_redis-0.3/aioscrapy_redis/core/downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/core/engine.py` & `aioscrapy_redis-0.3/aioscrapy_redis/core/engine.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/core/scheduler.py` & `aioscrapy_redis-0.3/aioscrapy_redis/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/core/spider.py` & `aioscrapy_redis-0.3/aioscrapy_redis/core/spider.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/https/form.py` & `aioscrapy_redis-0.3/aioscrapy_redis/https/form.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/https/request.py` & `aioscrapy_redis-0.3/aioscrapy_redis/https/request.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/https/response.py` & `aioscrapy_redis-0.3/aioscrapy_redis/https/response.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/utils/basesettings.py` & `aioscrapy_redis-0.3/aioscrapy_redis/utils/basesettings.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import copy
 
 import json
 import six
 from importlib import import_module
 from pprint import pformat
 from collections import MutableMapping
+import os, sys
 
 SETTINGS_PRIORITIES = {
     'default': 0,
     'command': 10,
     'project': 20,
     'spider': 30,
     'cmdline': 40,
@@ -125,14 +126,21 @@
             self.attributes[name].set(value, priority)
 
     def setdict(self, values, priority='project'):
         self.update(values, priority)
 
     def setmodule(self, module, priority='project'):
         self._assert_mutability()
+        sys.path.append(os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
+        current_path = os.path.dirname(os.path.realpath(sys.argv[0]))
+        if '/'.join(current_path.split('/')[:-2]):
+            sys.path.append('/'.join(current_path.split('/')[:-2]))
+        if '\\'.join(current_path.split('\\')[:-2]):
+            sys.path.append('\\'.join(current_path.split('\\')[:-2]))
+
         if isinstance(module, six.string_types):
             module = import_module(module)
         for key in dir(module):
             if key.isupper():
                 self.set(key, getattr(module, key), priority)
 
     def update(self, values, priority='project'):
```

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/utils/get_settings.py` & `aioscrapy_redis-0.3/aioscrapy_redis/utils/get_settings.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/utils/header_ua.py` & `aioscrapy_redis-0.3/aioscrapy_redis/utils/header_ua.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/utils/item.py` & `aioscrapy_redis-0.3/aioscrapy_redis/utils/item.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/utils/log.py` & `aioscrapy_redis-0.3/aioscrapy_redis/utils/log.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/utils/logstats.py` & `aioscrapy_redis-0.3/aioscrapy_redis/utils/logstats.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/utils/serialize.py` & `aioscrapy_redis-0.3/aioscrapy_redis/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/utils/tools.py` & `aioscrapy_redis-0.3/aioscrapy_redis/utils/tools.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis/utils/trackref.py` & `aioscrapy_redis-0.3/aioscrapy_redis/utils/trackref.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis.egg-info/PKG-INFO` & `aioscrapy_redis-0.3/aioscrapy_redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioscrapy-redis
-Version: 0.1
+Version: 0.3
 Summary: A mini spider framework, Integrate aiohttp into scrapy
 Home-page: https://github.com/pythonlw/aioscrapy_redis
 Author: 道法自然_Tor
 Author-email: 1540310556@qq.com
 License: Apache License v2
 Description: Python async library for web scraping
         PyPI version License: MIT
```

### Comparing `aioscrapy_redis-0.1/aioscrapy_redis.egg-info/SOURCES.txt` & `aioscrapy_redis-0.3/aioscrapy_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

