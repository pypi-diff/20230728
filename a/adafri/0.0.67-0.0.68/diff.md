# Comparing `tmp/adafri-0.0.67.tar.gz` & `tmp/adafri-0.0.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.67.tar", last modified: Fri Jul 28 03:56:58 2023, max compression
+gzip compressed data, was "adafri-0.0.68.tar", last modified: Fri Jul 28 05:11:26 2023, max compression
```

## Comparing `adafri-0.0.67.tar` & `adafri-0.0.68.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.365812 adafri-0.0.67/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-28 03:56:58.365398 adafri-0.0.67/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.328843 adafri-0.0.67/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-28 03:55:49.000000 adafri-0.0.67/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.339230 adafri-0.0.67/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.67/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.67/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.67/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.67/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    18729 2023-07-28 03:56:25.000000 adafri-0.0.67/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.340077 adafri-0.0.67/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.67/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.341138 adafri-0.0.67/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.67/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.344503 adafri-0.0.67/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.67/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.67/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.67/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.345592 adafri-0.0.67/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.67/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.347176 adafri-0.0.67/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.67/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.67/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.348144 adafri-0.0.67/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.67/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.348620 adafri-0.0.67/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.67/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.355464 adafri-0.0.67/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.67/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6848 2023-07-26 05:25:24.000000 adafri-0.0.67/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.67/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16141 2023-07-26 05:25:12.000000 adafri-0.0.67/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.67/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9462 2023-07-26 05:24:58.000000 adafri-0.0.67/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.67/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.358312 adafri-0.0.67/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.67/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.67/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.67/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.360149 adafri-0.0.67/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.67/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.67/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.360673 adafri-0.0.67/adafri/v1/mailing/
--rw-r--r--   0 ibrahima   (502) staff       (20)     7392 2023-07-26 04:34:01.000000 adafri-0.0.67/adafri/v1/mailing/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.361523 adafri-0.0.67/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.67/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.364314 adafri-0.0.67/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.67/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11624 2023-07-26 07:42:34.000000 adafri-0.0.67/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7346 2023-07-26 07:42:30.000000 adafri-0.0.67/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 03:56:58.331336 adafri-0.0.67/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-28 03:56:58.000000 adafri-0.0.67/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1250 2023-07-28 03:56:58.000000 adafri-0.0.67/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-28 03:56:58.000000 adafri-0.0.67/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-28 03:56:58.000000 adafri-0.0.67/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-28 03:56:58.365987 adafri-0.0.67/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.67/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.301290 adafri-0.0.68/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-28 05:11:26.300801 adafri-0.0.68/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.221979 adafri-0.0.68/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-28 05:11:04.000000 adafri-0.0.68/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.247822 adafri-0.0.68/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.68/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.68/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.68/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.68/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    18729 2023-07-28 03:56:25.000000 adafri-0.0.68/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.249158 adafri-0.0.68/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.68/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.250009 adafri-0.0.68/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.68/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.256763 adafri-0.0.68/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.68/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.68/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.68/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.260992 adafri-0.0.68/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.68/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.267556 adafri-0.0.68/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.68/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.68/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.274219 adafri-0.0.68/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.68/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.274855 adafri-0.0.68/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.68/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.283006 adafri-0.0.68/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.68/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6973 2023-07-28 05:09:47.000000 adafri-0.0.68/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5453 2023-07-28 05:10:44.000000 adafri-0.0.68/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16141 2023-07-26 05:25:12.000000 adafri-0.0.68/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.68/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9462 2023-07-26 05:24:58.000000 adafri-0.0.68/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.68/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.287801 adafri-0.0.68/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.68/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.68/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.68/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.292760 adafri-0.0.68/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.68/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.68/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.294537 adafri-0.0.68/adafri/v1/mailing/
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7392 2023-07-26 04:34:01.000000 adafri-0.0.68/adafri/v1/mailing/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.296466 adafri-0.0.68/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.68/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.299642 adafri-0.0.68/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.68/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11624 2023-07-26 07:42:34.000000 adafri-0.0.68/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7346 2023-07-26 07:42:30.000000 adafri-0.0.68/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 05:11:26.225086 adafri-0.0.68/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-28 05:11:26.000000 adafri-0.0.68/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1250 2023-07-28 05:11:26.000000 adafri-0.0.68/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-28 05:11:26.000000 adafri-0.0.68/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-28 05:11:26.000000 adafri-0.0.68/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-28 05:11:26.301496 adafri-0.0.68/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.68/setup.py
```

### Comparing `adafri-0.0.67/adafri/utils/country.py` & `adafri-0.0.68/adafri/utils/country.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/utils/phone_number.py` & `adafri-0.0.68/adafri/utils/phone_number.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/utils/response.py` & `adafri-0.0.68/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/utils/utils.py` & `adafri-0.0.68/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/v1/account/models/account.py` & `adafri-0.0.68/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/v1/account/models/account_fields.py` & `adafri-0.0.68/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.68/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.68/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.68/adafri/v1/auth/oauth/models/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     redirect_uris: list[str]
     scopes: list[str]
     scope: str
     client_id_issued_at: int
     createdAt: any
     allowed_redirect_uris: list[str]
     default_redirect_uri: str
+    allow_direct_grant_access: bool
+    token_endpoint_auth_methods: list[str]
     
     def __init__(self, client=None, default_redirect_uri=None, **kwargs):
         if type(client) is str:
             client = {"client_id": client} 
         (cls_object, keys, data_args) = init_class_kwargs(self, client, STANDARD_FIELDS, ClientFieldProps, CLIENT_COLLECTION, ['id'], **kwargs)
         super().__init__(**data_args);
         for key in keys:
@@ -136,15 +138,15 @@
     
     def check_client_secret(self, client_secret):
         return secrets.compare_digest(self.client_secret, client_secret)
     
     def check_endpoint_auth_method(self, method, endpoint):
         if endpoint == 'token':
             # if client table has ``token_endpoint_auth_method``
-            return self.token_endpoint_auth_method == method
+            return self.token_endpoint_auth_method == method or method in self.token_endpoint_auth_methods
         return True
     
     def check_grant_type(self, grant_type):
         return grant_type in self.grant_types
     
     def get_allowed_scope(self, scope):
         if not scope:
```

### Comparing `adafri-0.0.67/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.68/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,21 @@
     client_secret = "client_secret"
     redirect_uris = "redirect_uris"
     allowed_redirect_uris = "allowed_redirect_uris"
     uri = "uri"
     grant_types = "grant_types" 
     response_types = "response_types"
     token_endpoint_auth_method  = "token_endpoint_auth_method"
+    token_endpoint_auth_methods = "token_endpoint_auth_methods"
     scopes = "scopes"
     scope = "scope"
     client_id_issued_at = "client_id_issued_at"
     default_redirect_uri = "default_redirect_uri"
     created_at = "createdAt"
+    allow_direct_grant_access = "allow_direct_grant_access"
 
     @staticmethod
     def keys():
         return DictUtils.get_keys(ClientFieldProps);
 
     @staticmethod
     def filtered_keys(field, condition=True):
@@ -182,10 +184,28 @@
         "required": True,
         "mutable": False,
         "editable": False,
         "interactive": True,
         "default_value": 0,
         "pickable": True
     },
+    ClientFields.allow_direct_grant_access: {
+        "type": bool,
+        "required": True,
+        "mutable": True,
+        "editable":True,
+        "interactive": True,
+        "default_value": False,
+        "pickable": True
+    },
+    ClientFields.token_endpoint_auth_methods: {
+        "type": list,
+        "required": True,
+        "mutable": True,
+        "editable":True,
+        "interactive": True,
+        "default_value": [],
+        "pickable": True
+    }
 }
 
 STANDARD_FIELDS = ClientFields.filtered_keys('pickable', True)
```

### Comparing `adafri-0.0.67/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.68/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.68/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.68/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.68/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.68/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.68/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/v1/base/firebase_collection.py` & `adafri-0.0.68/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/v1/mailing/__init__.py` & `adafri-0.0.68/adafri/v1/mailing/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/v1/user/models/user.py` & `adafri-0.0.68/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri/v1/user/models/user_fields.py` & `adafri-0.0.68/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/adafri.egg-info/SOURCES.txt` & `adafri-0.0.68/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.67/setup.py` & `adafri-0.0.68/setup.py`

 * *Files identical despite different names*

