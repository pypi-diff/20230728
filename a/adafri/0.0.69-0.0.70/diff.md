# Comparing `tmp/adafri-0.0.69.tar.gz` & `tmp/adafri-0.0.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.69.tar", last modified: Fri Jul 28 06:10:32 2023, max compression
+gzip compressed data, was "adafri-0.0.70.tar", last modified: Fri Jul 28 08:15:18 2023, max compression
```

## Comparing `adafri-0.0.69.tar` & `adafri-0.0.70.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.869047 adafri-0.0.69/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-28 06:10:32.868466 adafri-0.0.69/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.827485 adafri-0.0.69/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-28 06:10:28.000000 adafri-0.0.69/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.835425 adafri-0.0.69/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.69/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.69/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.69/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.69/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    18729 2023-07-28 03:56:25.000000 adafri-0.0.69/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.836855 adafri-0.0.69/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.69/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.838134 adafri-0.0.69/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.69/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.841375 adafri-0.0.69/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.69/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.69/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.69/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.842900 adafri-0.0.69/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.69/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.844589 adafri-0.0.69/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.69/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.69/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.845967 adafri-0.0.69/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.69/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.846915 adafri-0.0.69/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.69/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.856116 adafri-0.0.69/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.69/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6973 2023-07-28 05:09:47.000000 adafri-0.0.69/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5453 2023-07-28 05:10:44.000000 adafri-0.0.69/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16141 2023-07-28 06:09:55.000000 adafri-0.0.69/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.69/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9462 2023-07-26 05:24:58.000000 adafri-0.0.69/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.69/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.859389 adafri-0.0.69/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.69/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.69/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.69/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.861651 adafri-0.0.69/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.69/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.69/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.862282 adafri-0.0.69/adafri/v1/mailing/
--rw-r--r--   0 ibrahima   (502) staff       (20)     7392 2023-07-26 04:34:01.000000 adafri-0.0.69/adafri/v1/mailing/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.863206 adafri-0.0.69/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.69/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.866529 adafri-0.0.69/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.69/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11624 2023-07-26 07:42:34.000000 adafri-0.0.69/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7346 2023-07-26 07:42:30.000000 adafri-0.0.69/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 06:10:32.829828 adafri-0.0.69/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-28 06:10:32.000000 adafri-0.0.69/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1250 2023-07-28 06:10:32.000000 adafri-0.0.69/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-28 06:10:32.000000 adafri-0.0.69/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-28 06:10:32.000000 adafri-0.0.69/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-28 06:10:32.869296 adafri-0.0.69/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.69/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.177224 adafri-0.0.70/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-28 08:15:18.176752 adafri-0.0.70/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.133098 adafri-0.0.70/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-28 08:15:10.000000 adafri-0.0.70/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.141056 adafri-0.0.70/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.70/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.70/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.70/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.70/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    18952 2023-07-28 07:08:29.000000 adafri-0.0.70/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.142500 adafri-0.0.70/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.70/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.143558 adafri-0.0.70/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.70/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.146522 adafri-0.0.70/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.70/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.70/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.70/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.147292 adafri-0.0.70/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.70/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.149399 adafri-0.0.70/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.70/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.70/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.150700 adafri-0.0.70/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.70/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.151177 adafri-0.0.70/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      933 2023-07-28 08:08:06.000000 adafri-0.0.70/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.165974 adafri-0.0.70/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6973 2023-07-28 05:09:47.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6304 2023-07-28 07:52:06.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/code.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2444 2023-07-28 08:09:16.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/code_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16141 2023-07-28 06:11:41.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9462 2023-07-26 05:24:58.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.168950 adafri-0.0.70/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.70/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.70/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.70/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.171204 adafri-0.0.70/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.70/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.70/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.171919 adafri-0.0.70/adafri/v1/mailing/
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7392 2023-07-26 04:34:01.000000 adafri-0.0.70/adafri/v1/mailing/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.172893 adafri-0.0.70/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.70/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.175933 adafri-0.0.70/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.70/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11624 2023-07-26 07:42:34.000000 adafri-0.0.70/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7382 2023-07-28 08:13:51.000000 adafri-0.0.70/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.135467 adafri-0.0.70/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-28 08:15:18.000000 adafri-0.0.70/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-07-28 08:15:18.000000 adafri-0.0.70/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-28 08:15:18.000000 adafri-0.0.70/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-28 08:15:18.000000 adafri-0.0.70/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-28 08:15:18.177489 adafri-0.0.70/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.70/setup.py
```

### Comparing `adafri-0.0.69/adafri/utils/country.py` & `adafri-0.0.70/adafri/utils/country.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.69/adafri/utils/phone_number.py` & `adafri-0.0.70/adafri/utils/phone_number.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.69/adafri/utils/response.py` & `adafri-0.0.70/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.69/adafri/utils/utils.py` & `adafri-0.0.70/adafri/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import hashlib
 from cryptography.fernet import Fernet
 import os
 import base64
 from datetime import (date, datetime)
 from urllib.parse import urlparse, parse_qs
 import re
+import random
 
 hash = hashlib.sha1(str(os.getenv('CRYPTO_KEY')).encode())
 ENCRYPTION_KEY = base64.b64encode(hash.hexdigest()[:32].encode()).decode();
 
 
 camel_pat = re.compile(r'([A-Z])')
 under_pat = re.compile(r'_([a-z])')
@@ -54,14 +55,20 @@
     try:
         if isBase64(data):
             return decode_base64(data)
         return data;
     except Exception as e:
         None
 
+def generate_random_code():
+    start = random.randint(2000, 5000)
+    start1 = random.randint(6000, 9000)
+    end = random.randint(start, random.randint(start, start1))
+    return random.randint(start, end)
+
 def format_query_filter(key: str, value: any, comparator: str):
     """
         key A key existing in document data
         @{value} The value used to compare
         comparator The method used to compare (==, in...)
     """
     query = {};
```

### Comparing `adafri-0.0.69/adafri/v1/account/models/account.py` & `adafri-0.0.70/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.69/adafri/v1/account/models/account_fields.py` & `adafri-0.0.70/adafri/v1/account/models/account_fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from  ....utils.utils import DictUtils 
+import os
 
-ACCOUNT_COLLECTION = "accounts";
+ACCOUNT_COLLECTION = os.environ.get('ACCOUNT_COLLECTION');
 
 @dataclass
 class AccountFields:
     id = "id"
     aacid = "aacid"
     account_value = "account_value"
     creationDate = "creationDate"
```

### Comparing `adafri-0.0.69/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.70/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.69/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.70/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.69/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.70/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 from dataclasses import dataclass
 from .....utils.utils import DictUtils
+import os
 
-CLIENT_COLLECTION = "clients_collection"
+CLIENT_COLLECTION = os.environ.get('CLIENT_COLLECTION')
 @dataclass
 class ClientFields:
     id = "id"
     name = "name"
     uid = "uid"
     description = "description"
     client_id = "client_id"
```

### Comparing `adafri-0.0.69/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.70/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.69/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.70/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 from dataclasses import dataclass
 from .....utils.utils import DictUtils
 from datetime import datetime, timedelta
+import os
 
-GRANT_COLLECTION = "clients_grant_collection";
+GRANT_COLLECTION = os.environ.get('GRANT_COLLECTION');
 
 def get_grant_expire_at(expires_in):
     return datetime.now() + timedelta(seconds=expires_in)
 @dataclass
 class GrantFields:
     id = "id"
     code = "code"
```

### Comparing `adafri-0.0.69/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.70/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.69/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.70/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass
 from .....utils import DictUtils
 from datetime import datetime, timedelta
+import os
 
-TOKEN_COLLECTION = "clients_token_collection";
+TOKEN_COLLECTION = os.environ.get('TOKEN_COLLECTION');
 
 def get_token_expire_at(expires_in):
     return datetime.now() + timedelta(seconds=expires_in)
 
 
 def is_expired(expired_at):
     return datetime.fromisoformat(expired_at) < datetime.now()
```

### Comparing `adafri-0.0.69/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.70/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.69/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.70/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.69/adafri/v1/base/firebase_collection.py` & `adafri-0.0.70/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.69/adafri/v1/mailing/__init__.py` & `adafri-0.0.70/adafri/v1/mailing/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.69/adafri/v1/user/models/user.py` & `adafri-0.0.70/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.69/adafri/v1/user/models/user_fields.py` & `adafri-0.0.70/adafri/v1/user/models/user_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from  ....utils.utils import DictUtils 
+import os
 
-USERS_COLLECTION = "users";
+USERS_COLLECTION = os.environ.get('USER_COLLECTION');
 
 @dataclass
 class UserFields:
     uid = "uid";
     email = 'email';
     password = 'password';
     displayName = 'displayName';
```

### Comparing `adafri-0.0.69/adafri.egg-info/SOURCES.txt` & `adafri-0.0.70/adafri.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 adafri/v1/auth/firebase_auth/__init__.py
 adafri/v1/auth/firebase_auth/firebase_auth.py
 adafri/v1/auth/models/__init__.py
 adafri/v1/auth/oauth/__init__.py
 adafri/v1/auth/oauth/models/__init__.py
 adafri/v1/auth/oauth/models/client.py
 adafri/v1/auth/oauth/models/client_fields.py
+adafri/v1/auth/oauth/models/code.py
+adafri/v1/auth/oauth/models/code_fields.py
 adafri/v1/auth/oauth/models/grant.py
 adafri/v1/auth/oauth/models/grant_fields.py
 adafri/v1/auth/oauth/models/token.py
 adafri/v1/auth/oauth/models/token_fields.py
 adafri/v1/auth/oauth/server/__init__.py
 adafri/v1/auth/oauth/server/oidc_server.py
 adafri/v1/auth/oauth/server/server.py
```

### Comparing `adafri-0.0.69/setup.py` & `adafri-0.0.70/setup.py`

 * *Files identical despite different names*

