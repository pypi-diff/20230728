# Comparing `tmp/XoxoDay-0.0.30.tar.gz` & `tmp/XoxoDay-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XoxoDay-0.0.30.tar", last modified: Mon Jul 24 19:37:37 2023, max compression
+gzip compressed data, was "XoxoDay-0.0.31.tar", last modified: Fri Jul 28 07:51:00 2023, max compression
```

## Comparing `XoxoDay-0.0.30.tar` & `XoxoDay-0.0.31.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-24 19:37:37.666555 XoxoDay-0.0.30/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.30/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-07-24 19:37:37.666400 XoxoDay-0.0.30/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.30/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-24 19:37:37.662583 XoxoDay-0.0.30/XoxoDay/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-07-24 19:37:27.000000 XoxoDay-0.0.30/XoxoDay/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.30/XoxoDay/exception.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-24 19:37:37.663915 XoxoDay-0.0.30/XoxoDay/helper/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.30/XoxoDay/helper/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      700 2023-07-13 10:07:14.000000 XoxoDay-0.0.30/XoxoDay/helper/token.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      626 2023-07-13 10:07:14.000000 XoxoDay-0.0.30/XoxoDay/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-24 19:37:37.666038 XoxoDay-0.0.30/XoxoDay/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.30/XoxoDay/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1205 2023-06-23 20:31:24.000000 XoxoDay-0.0.30/XoxoDay/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.30/XoxoDay/service/placeOrder.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1892 2023-07-13 10:07:14.000000 XoxoDay-0.0.30/XoxoDay/service/token_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.30/XoxoDay/service/voucher.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     4371 2023-07-24 19:37:13.000000 XoxoDay-0.0.30/XoxoDay/service/xoxoday_service.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-24 19:37:37.663619 XoxoDay-0.0.30/XoxoDay.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-07-24 19:37:37.000000 XoxoDay-0.0.30/XoxoDay.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      483 2023-07-24 19:37:37.000000 XoxoDay-0.0.30/XoxoDay.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-07-24 19:37:37.000000 XoxoDay-0.0.30/XoxoDay.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-07-24 19:37:37.000000 XoxoDay-0.0.30/XoxoDay.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-07-24 19:37:37.000000 XoxoDay-0.0.30/XoxoDay.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-07-24 19:37:37.666605 XoxoDay-0.0.30/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-07-24 19:37:27.000000 XoxoDay-0.0.30/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-28 07:51:00.962004 XoxoDay-0.0.31/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.31/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-07-28 07:51:00.961839 XoxoDay-0.0.31/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.31/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-28 07:51:00.958473 XoxoDay-0.0.31/XoxoDay/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-07-28 07:50:45.000000 XoxoDay-0.0.31/XoxoDay/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.31/XoxoDay/exception.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-28 07:51:00.959649 XoxoDay-0.0.31/XoxoDay/helper/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.31/XoxoDay/helper/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      700 2023-07-13 10:07:14.000000 XoxoDay-0.0.31/XoxoDay/helper/token.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      626 2023-07-13 10:07:14.000000 XoxoDay-0.0.31/XoxoDay/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-28 07:51:00.961409 XoxoDay-0.0.31/XoxoDay/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.31/XoxoDay/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1257 2023-07-28 07:50:20.000000 XoxoDay-0.0.31/XoxoDay/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.31/XoxoDay/service/placeOrder.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1892 2023-07-13 10:07:14.000000 XoxoDay-0.0.31/XoxoDay/service/token_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.31/XoxoDay/service/voucher.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     4371 2023-07-24 19:37:13.000000 XoxoDay-0.0.31/XoxoDay/service/xoxoday_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-28 07:51:00.959384 XoxoDay-0.0.31/XoxoDay.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-07-28 07:51:00.000000 XoxoDay-0.0.31/XoxoDay.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      483 2023-07-28 07:51:00.000000 XoxoDay-0.0.31/XoxoDay.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-07-28 07:51:00.000000 XoxoDay-0.0.31/XoxoDay.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-07-28 07:51:00.000000 XoxoDay-0.0.31/XoxoDay.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-07-28 07:51:00.000000 XoxoDay-0.0.31/XoxoDay.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-07-28 07:51:00.962068 XoxoDay-0.0.31/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-07-28 07:50:49.000000 XoxoDay-0.0.31/setup.py
```

### Comparing `XoxoDay-0.0.30/LICENSE` & `XoxoDay-0.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.30/PKG-INFO` & `XoxoDay-0.0.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.30
+Version: 0.0.31
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.30/README.md` & `XoxoDay-0.0.31/README.md`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.30/XoxoDay/exception.py` & `XoxoDay-0.0.31/XoxoDay/exception.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.30/XoxoDay/helper/token.py` & `XoxoDay-0.0.31/XoxoDay/helper/token.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.30/XoxoDay/serializer.py` & `XoxoDay-0.0.31/XoxoDay/serializer.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.30/XoxoDay/service/http_service.py` & `XoxoDay-0.0.31/XoxoDay/service/http_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.REST_URL = REST_URL
 
     @staticmethod
     def parse_result(r):
         res = r.text.encode('utf-8')
         res = Serializer.loads(res)
         if r.status_code != 200:
-            raise XoxoDayException(res['error_description'])
+            raise XoxoDayException(res['error_description'] if "error_description" in res else res['errorInfo'])
         return res
 
     def post_request(self, url, request_body, headers):
         request_body = Serializer.dumps(request_body)
         r = requests.post(url, data=request_body, headers=headers)
         return self.parse_result(r)
```

### Comparing `XoxoDay-0.0.30/XoxoDay/service/token_service.py` & `XoxoDay-0.0.31/XoxoDay/service/token_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.30/XoxoDay/service/xoxoday_service.py` & `XoxoDay-0.0.31/XoxoDay/service/xoxoday_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.30/XoxoDay.egg-info/PKG-INFO` & `XoxoDay-0.0.31/XoxoDay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.30
+Version: 0.0.31
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.30/setup.py` & `XoxoDay-0.0.31/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='XoxoDay',
-    version="0.0.30",
+    version="0.0.31",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='XoxoDay Api Client For Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/XoxoDay.git',
     project_urls={
```

