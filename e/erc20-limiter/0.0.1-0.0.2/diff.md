# Comparing `tmp/erc20-limiter-0.0.1.tar.gz` & `tmp/erc20-limiter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erc20-limiter-0.0.1.tar", last modified: Fri Jul 28 12:40:00 2023, max compression
+gzip compressed data, was "erc20-limiter-0.0.2.tar", last modified: Fri Jul 28 12:43:40 2023, max compression
```

## Comparing `erc20-limiter-0.0.1.tar` & `erc20-limiter-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,31 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:40:00.236616 erc20-limiter-0.0.1/
--rw-r--r--   0 lash      (1000) lash      (1000)      693 2023-07-28 12:40:00.236616 erc20-limiter-0.0.1/PKG-INFO
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:40:00.233283 erc20-limiter-0.0.1/erc20_limiter/
--rw-r--r--   0 lash      (1000) lash      (1000)       29 2023-07-27 16:56:28.000000 erc20-limiter-0.0.1/erc20_limiter/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:40:00.236616 erc20-limiter-0.0.1/erc20_limiter/data/
--rw-r--r--   0 lash      (1000) lash      (1000)       66 2023-07-27 16:57:09.000000 erc20-limiter-0.0.1/erc20_limiter/data/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3409 2023-07-28 11:14:14.000000 erc20-limiter-0.0.1/erc20_limiter/limiter.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2768 2023-07-28 11:30:19.000000 erc20-limiter-0.0.1/erc20_limiter/token.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:40:00.236616 erc20-limiter-0.0.1/erc20_limiter/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-07-27 16:55:49.000000 erc20-limiter-0.0.1/erc20_limiter/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1938 2023-07-28 11:35:40.000000 erc20-limiter-0.0.1/erc20_limiter/unittest/base.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:40:00.236616 erc20-limiter-0.0.1/erc20_limiter.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      693 2023-07-28 12:40:00.000000 erc20-limiter-0.0.1/erc20_limiter.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      421 2023-07-28 12:40:00.000000 erc20-limiter-0.0.1/erc20_limiter.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-07-28 12:40:00.000000 erc20-limiter-0.0.1/erc20_limiter.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-07-28 12:40:00.000000 erc20-limiter-0.0.1/erc20_limiter.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       14 2023-07-28 12:40:00.000000 erc20-limiter-0.0.1/erc20_limiter.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      797 2023-07-28 12:40:00.236616 erc20-limiter-0.0.1/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      473 2023-07-28 12:36:47.000000 erc20-limiter-0.0.1/setup.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:40:00.236616 erc20-limiter-0.0.1/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)      825 2023-07-28 11:12:58.000000 erc20-limiter-0.0.1/tests/test_base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1590 2023-07-28 11:36:18.000000 erc20-limiter-0.0.1/tests/test_token_registry.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:43:40.253282 erc20-limiter-0.0.2/
+-rw-r--r--   0 lash      (1000) lash      (1000)       63 2023-07-28 12:43:39.000000 erc20-limiter-0.0.2/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      693 2023-07-28 12:43:40.253282 erc20-limiter-0.0.2/PKG-INFO
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:43:40.253282 erc20-limiter-0.0.2/erc20_limiter/
+-rw-r--r--   0 lash      (1000) lash      (1000)       29 2023-07-27 16:56:28.000000 erc20-limiter-0.0.2/erc20_limiter/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:43:40.253282 erc20-limiter-0.0.2/erc20_limiter/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)     4898 2023-07-28 11:44:53.000000 erc20-limiter-0.0.2/erc20_limiter/data/Limiter.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1602 2023-07-28 11:44:53.000000 erc20-limiter-0.0.2/erc20_limiter/data/Limiter.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     2279 2023-07-28 11:44:53.000000 erc20-limiter-0.0.2/erc20_limiter/data/Limiter.metadata.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     4814 2023-07-28 11:44:53.000000 erc20-limiter-0.0.2/erc20_limiter/data/LimiterTokenRegistry.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1338 2023-07-28 11:44:53.000000 erc20-limiter-0.0.2/erc20_limiter/data/LimiterTokenRegistry.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     2054 2023-07-28 11:44:53.000000 erc20-limiter-0.0.2/erc20_limiter/data/LimiterTokenRegistry.metadata.json
+-rw-r--r--   0 lash      (1000) lash      (1000)       66 2023-07-27 16:57:09.000000 erc20-limiter-0.0.2/erc20_limiter/data/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3409 2023-07-28 11:14:14.000000 erc20-limiter-0.0.2/erc20_limiter/limiter.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2768 2023-07-28 11:30:19.000000 erc20-limiter-0.0.2/erc20_limiter/token.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:43:40.253282 erc20-limiter-0.0.2/erc20_limiter/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-07-27 16:55:49.000000 erc20-limiter-0.0.2/erc20_limiter/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1938 2023-07-28 11:35:40.000000 erc20-limiter-0.0.2/erc20_limiter/unittest/base.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:43:40.253282 erc20-limiter-0.0.2/erc20_limiter.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      693 2023-07-28 12:43:40.000000 erc20-limiter-0.0.2/erc20_limiter.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      719 2023-07-28 12:43:40.000000 erc20-limiter-0.0.2/erc20_limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-07-28 12:43:40.000000 erc20-limiter-0.0.2/erc20_limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-07-28 12:43:40.000000 erc20-limiter-0.0.2/erc20_limiter.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       14 2023-07-28 12:43:40.000000 erc20-limiter-0.0.2/erc20_limiter.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-07-27 16:54:14.000000 erc20-limiter-0.0.2/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      797 2023-07-28 12:43:40.256615 erc20-limiter-0.0.2/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      473 2023-07-28 12:36:47.000000 erc20-limiter-0.0.2/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       58 2023-07-27 16:55:11.000000 erc20-limiter-0.0.2/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:43:40.253282 erc20-limiter-0.0.2/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)      825 2023-07-28 11:12:58.000000 erc20-limiter-0.0.2/tests/test_base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1590 2023-07-28 11:36:18.000000 erc20-limiter-0.0.2/tests/test_token_registry.py
```

### Comparing `erc20-limiter-0.0.1/PKG-INFO` & `erc20-limiter-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erc20-limiter
-Version: 0.0.1
+Version: 0.0.2
 Summary: ERC20 balance limit registry
 Home-page: https://holbrook.no/src/erc20-limiter/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `erc20-limiter-0.0.1/erc20_limiter/limiter.py` & `erc20-limiter-0.0.2/erc20_limiter/limiter.py`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.1/erc20_limiter/token.py` & `erc20-limiter-0.0.2/erc20_limiter/token.py`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.1/erc20_limiter/unittest/base.py` & `erc20-limiter-0.0.2/erc20_limiter/unittest/base.py`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.1/erc20_limiter.egg-info/PKG-INFO` & `erc20-limiter-0.0.2/erc20_limiter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erc20-limiter
-Version: 0.0.1
+Version: 0.0.2
 Summary: ERC20 balance limit registry
 Home-page: https://holbrook.no/src/erc20-limiter/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `erc20-limiter-0.0.1/setup.cfg` & `erc20-limiter-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = erc20-limiter
-version = 0.0.1
+version = 0.0.2
 description = ERC20 balance limit registry
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://holbrook.no/src/erc20-limiter/log.html
 keywords = 
 	dlt
 	blockchain
```

### Comparing `erc20-limiter-0.0.1/tests/test_base.py` & `erc20-limiter-0.0.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.1/tests/test_token_registry.py` & `erc20-limiter-0.0.2/tests/test_token_registry.py`

 * *Files identical despite different names*

