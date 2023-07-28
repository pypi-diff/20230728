# Comparing `tmp/bbat-0.2.0.tar.gz` & `tmp/bbat-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbat-0.2.0.tar", last modified: Thu Jul 27 07:45:28 2023, max compression
+gzip compressed data, was "bbat-0.2.1.tar", last modified: Fri Jul 28 01:14:06 2023, max compression
```

## Comparing `bbat-0.2.0.tar` & `bbat-0.2.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.036938 bbat-0.2.0/
--rw-rw-rw-   0        0        0      289 2023-07-27 07:45:28.035939 bbat-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-11 11:39:46.000000 bbat-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.007691 bbat-0.2.0/bbat/
--rw-rw-rw-   0        0        0        0 2023-07-09 13:29:18.000000 bbat-0.2.0/bbat/__init__.py
--rw-rw-rw-   0        0        0     1931 2023-07-18 01:38:19.000000 bbat-0.2.0/bbat/config.py
--rw-rw-rw-   0        0        0     3115 2023-07-17 07:29:02.000000 bbat-0.2.0/bbat/crypto.py
--rw-rw-rw-   0        0        0     1230 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/date.py
-drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.019934 bbat-0.2.0/bbat/db/
--rw-rw-rw-   0        0        0        0 2023-07-09 13:50:02.000000 bbat-0.2.0/bbat/db/__init__.py
--rw-rw-rw-   0        0        0     5722 2023-07-19 08:56:34.000000 bbat-0.2.0/bbat/db/aio_mysql.py
--rw-rw-rw-   0        0        0     2632 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/db/aio_sqlite.py
--rw-rw-rw-   0        0        0     2054 2023-07-15 12:58:24.000000 bbat-0.2.0/bbat/db/mysql.py
--rw-rw-rw-   0        0        0      491 2023-07-17 08:36:20.000000 bbat-0.2.0/bbat/document.py
--rw-rw-rw-   0        0        0       30 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/hi.py
--rw-rw-rw-   0        0        0     1978 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/image.py
-drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.020938 bbat-0.2.0/bbat/llm/
--rw-rw-rw-   0        0        0        0 2023-07-11 14:42:42.000000 bbat-0.2.0/bbat/llm/__init__.py
--rw-rw-rw-   0        0        0     2416 2023-07-12 14:36:12.000000 bbat-0.2.0/bbat/llm/chatgpt.py
--rw-rw-rw-   0        0        0      920 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/log.py
--rw-rw-rw-   0        0        0      828 2023-07-12 11:52:42.000000 bbat-0.2.0/bbat/machine.py
--rw-rw-rw-   0        0        0     1868 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/notice.py
--rw-rw-rw-   0        0        0     2497 2023-07-10 11:37:38.000000 bbat-0.2.0/bbat/np.py
--rw-rw-rw-   0        0        0     1764 2023-07-18 01:35:45.000000 bbat-0.2.0/bbat/path.py
--rw-rw-rw-   0        0        0     4198 2023-07-11 15:55:34.000000 bbat-0.2.0/bbat/text.py
-drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.026939 bbat-0.2.0/bbat/web/
--rw-rw-rw-   0        0        0        0 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/__init__.py
--rw-rw-rw-   0        0        0     1685 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/client.py
--rw-rw-rw-   0        0        0      504 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/cors.py
--rw-rw-rw-   0        0        0     4501 2023-07-27 07:39:54.000000 bbat-0.2.0/bbat/web/db_server.py
--rw-rw-rw-   0        0        0      177 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/flask_app.py
--rw-rw-rw-   0        0        0     1566 2023-07-13 12:06:02.000000 bbat-0.2.0/bbat/web/sanic_app.py
-drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.032938 bbat-0.2.0/bbat/web/url_to_sql/
--rw-rw-rw-   0        0        0        0 2023-07-10 11:37:38.000000 bbat-0.2.0/bbat/web/url_to_sql/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/url_to_sql/field.py
--rw-rw-rw-   0        0        0     7452 2023-07-27 07:40:43.000000 bbat-0.2.0/bbat/web/url_to_sql/query.py
--rw-rw-rw-   0        0        0     2256 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/url_to_sql/relation.py
--rw-rw-rw-   0        0        0      722 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/url_to_sql/test.py
--rw-rw-rw-   0        0        0      964 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/url_to_sql/util.py
--rw-rw-rw-   0        0        0     1473 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/url_to_sql/where.py
--rw-rw-rw-   0        0        0     1614 2023-07-12 11:52:42.000000 bbat-0.2.0/bbat/zcli.py
-drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.015691 bbat-0.2.0/bbat.egg-info/
--rw-rw-rw-   0        0        0      289 2023-07-27 07:45:27.000000 bbat-0.2.0/bbat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      876 2023-07-27 07:45:27.000000 bbat-0.2.0/bbat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 07:45:27.000000 bbat-0.2.0/bbat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-27 07:45:27.000000 bbat-0.2.0/bbat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2023-07-27 07:45:27.000000 bbat-0.2.0/bbat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-27 07:45:27.000000 bbat-0.2.0/bbat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 07:45:28.036938 bbat-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1027 2023-07-27 07:44:22.000000 bbat-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.034938 bbat-0.2.0/test/
--rw-rw-rw-   0        0        0      209 2023-07-11 11:39:46.000000 bbat-0.2.0/test/test_config.py
--rw-rw-rw-   0        0        0      194 2023-07-11 11:39:46.000000 bbat-0.2.0/test/test_db_mysql.py
+drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.562837 bbat-0.2.1/
+-rw-rw-rw-   0        0        0      289 2023-07-28 01:14:06.561852 bbat-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-11 11:39:46.000000 bbat-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.413354 bbat-0.2.1/bbat/
+-rw-rw-rw-   0        0        0        0 2023-07-09 13:29:18.000000 bbat-0.2.1/bbat/__init__.py
+-rw-rw-rw-   0        0        0     1931 2023-07-18 01:38:19.000000 bbat-0.2.1/bbat/config.py
+-rw-rw-rw-   0        0        0     3115 2023-07-17 07:29:02.000000 bbat-0.2.1/bbat/crypto.py
+-rw-rw-rw-   0        0        0     1230 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/date.py
+drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.457235 bbat-0.2.1/bbat/db/
+-rw-rw-rw-   0        0        0        0 2023-07-09 13:50:02.000000 bbat-0.2.1/bbat/db/__init__.py
+-rw-rw-rw-   0        0        0     5722 2023-07-19 08:56:34.000000 bbat-0.2.1/bbat/db/aio_mysql.py
+-rw-rw-rw-   0        0        0     2632 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/db/aio_sqlite.py
+-rw-rw-rw-   0        0        0     2054 2023-07-15 12:58:24.000000 bbat-0.2.1/bbat/db/mysql.py
+-rw-rw-rw-   0        0        0      491 2023-07-17 08:36:20.000000 bbat-0.2.1/bbat/document.py
+-rw-rw-rw-   0        0        0       30 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/hi.py
+-rw-rw-rw-   0        0        0     1978 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/image.py
+drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.465240 bbat-0.2.1/bbat/llm/
+-rw-rw-rw-   0        0        0        0 2023-07-11 14:42:42.000000 bbat-0.2.1/bbat/llm/__init__.py
+-rw-rw-rw-   0        0        0     2416 2023-07-12 14:36:12.000000 bbat-0.2.1/bbat/llm/chatgpt.py
+-rw-rw-rw-   0        0        0      920 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/log.py
+-rw-rw-rw-   0        0        0      828 2023-07-12 11:52:42.000000 bbat-0.2.1/bbat/machine.py
+-rw-rw-rw-   0        0        0     1868 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/notice.py
+-rw-rw-rw-   0        0        0     2497 2023-07-10 11:37:38.000000 bbat-0.2.1/bbat/np.py
+-rw-rw-rw-   0        0        0     1764 2023-07-18 01:35:45.000000 bbat-0.2.1/bbat/path.py
+-rw-rw-rw-   0        0        0     4198 2023-07-11 15:55:34.000000 bbat-0.2.1/bbat/text.py
+drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.499230 bbat-0.2.1/bbat/web/
+-rw-rw-rw-   0        0        0        0 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/__init__.py
+-rw-rw-rw-   0        0        0     1685 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/client.py
+-rw-rw-rw-   0        0        0      504 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/cors.py
+-rw-rw-rw-   0        0        0     4501 2023-07-27 07:39:54.000000 bbat-0.2.1/bbat/web/db_server.py
+-rw-rw-rw-   0        0        0      177 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/flask_app.py
+-rw-rw-rw-   0        0        0     1566 2023-07-13 12:06:02.000000 bbat-0.2.1/bbat/web/sanic_app.py
+drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.548850 bbat-0.2.1/bbat/web/url_to_sql/
+-rw-rw-rw-   0        0        0        0 2023-07-10 11:37:38.000000 bbat-0.2.1/bbat/web/url_to_sql/__init__.py
+-rw-rw-rw-   0        0        0     1488 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/url_to_sql/field.py
+-rw-rw-rw-   0        0        0     7452 2023-07-27 07:40:43.000000 bbat-0.2.1/bbat/web/url_to_sql/query.py
+-rw-rw-rw-   0        0        0     2256 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/url_to_sql/relation.py
+-rw-rw-rw-   0        0        0      722 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/url_to_sql/test.py
+-rw-rw-rw-   0        0        0      964 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/url_to_sql/util.py
+-rw-rw-rw-   0        0        0     1473 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/url_to_sql/where.py
+-rw-rw-rw-   0        0        0     1614 2023-07-12 11:52:42.000000 bbat-0.2.1/bbat/zcli.py
+drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.434731 bbat-0.2.1/bbat.egg-info/
+-rw-rw-rw-   0        0        0      289 2023-07-28 01:14:06.000000 bbat-0.2.1/bbat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      876 2023-07-28 01:14:06.000000 bbat-0.2.1/bbat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 01:14:06.000000 bbat-0.2.1/bbat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-28 01:14:06.000000 bbat-0.2.1/bbat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2023-07-28 01:14:06.000000 bbat-0.2.1/bbat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-28 01:14:06.000000 bbat-0.2.1/bbat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 01:14:06.563838 bbat-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1027 2023-07-28 01:13:39.000000 bbat-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.560838 bbat-0.2.1/test/
+-rw-rw-rw-   0        0        0      209 2023-07-11 11:39:46.000000 bbat-0.2.1/test/test_config.py
+-rw-rw-rw-   0        0        0      194 2023-07-11 11:39:46.000000 bbat-0.2.1/test/test_db_mysql.py
```

### Comparing `bbat-0.2.0/bbat/config.py` & `bbat-0.2.1/bbat/config.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/crypto.py` & `bbat-0.2.1/bbat/crypto.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/date.py` & `bbat-0.2.1/bbat/date.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/db/aio_mysql.py` & `bbat-0.2.1/bbat/db/aio_mysql.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/db/aio_sqlite.py` & `bbat-0.2.1/bbat/db/aio_sqlite.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/db/mysql.py` & `bbat-0.2.1/bbat/db/mysql.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/image.py` & `bbat-0.2.1/bbat/image.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/llm/chatgpt.py` & `bbat-0.2.1/bbat/llm/chatgpt.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/log.py` & `bbat-0.2.1/bbat/log.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/machine.py` & `bbat-0.2.1/bbat/machine.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/notice.py` & `bbat-0.2.1/bbat/notice.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/np.py` & `bbat-0.2.1/bbat/np.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/path.py` & `bbat-0.2.1/bbat/path.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/text.py` & `bbat-0.2.1/bbat/text.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/web/client.py` & `bbat-0.2.1/bbat/web/client.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/web/db_server.py` & `bbat-0.2.1/bbat/web/db_server.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/web/sanic_app.py` & `bbat-0.2.1/bbat/web/sanic_app.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/web/url_to_sql/field.py` & `bbat-0.2.1/bbat/web/url_to_sql/field.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/web/url_to_sql/query.py` & `bbat-0.2.1/bbat/web/url_to_sql/query.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/web/url_to_sql/relation.py` & `bbat-0.2.1/bbat/web/url_to_sql/relation.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/web/url_to_sql/test.py` & `bbat-0.2.1/bbat/web/url_to_sql/test.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/web/url_to_sql/util.py` & `bbat-0.2.1/bbat/web/url_to_sql/util.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/web/url_to_sql/where.py` & `bbat-0.2.1/bbat/web/url_to_sql/where.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat/zcli.py` & `bbat-0.2.1/bbat/zcli.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/bbat.egg-info/SOURCES.txt` & `bbat-0.2.1/bbat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bbat-0.2.0/setup.py` & `bbat-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import setuptools
 
 name = "bbat"
-version = "0.2.0"
+version = "0.2.1"
 
 def _process_requirements():
     packages = open('requirements.txt').read().strip().split('\n')
     requires = []
     for pkg in packages:
         if pkg.startswith('git+ssh'):
             return_code = os.system('pip install {}'.format(pkg))
```

