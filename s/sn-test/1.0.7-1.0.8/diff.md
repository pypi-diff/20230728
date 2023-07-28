# Comparing `tmp/sn_test-1.0.7.tar.gz` & `tmp/sn_test-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sn_test-1.0.7.tar", last modified: Fri Jul 28 08:14:32 2023, max compression
+gzip compressed data, was "dist/sn_test-1.0.8.tar", last modified: Fri Jul 28 11:27:16 2023, max compression
```

## Comparing `sn_test-1.0.7.tar` & `sn_test-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 08:14:32.000000 sn_test-1.0.7/
--rw-r--r--   0 mac        (501) staff       (20)     5081 2023-07-28 08:14:32.000000 sn_test-1.0.7/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     3180 2023-07-28 08:14:25.000000 sn_test-1.0.7/set_up.py
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-28 08:14:32.000000 sn_test-1.0.7/setup.cfg
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 08:14:32.000000 sn_test-1.0.7/sn_test/
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-07-21 08:42:56.000000 sn_test-1.0.7/sn_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      294 2023-07-21 06:40:48.000000 sn_test-1.0.7/sn_test/test_sn.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 08:14:32.000000 sn_test-1.0.7/sn_test.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     5081 2023-07-28 08:14:31.000000 sn_test-1.0.7/sn_test.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      202 2023-07-28 08:14:31.000000 sn_test-1.0.7/sn_test.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-28 08:14:31.000000 sn_test-1.0.7/sn_test.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-28 08:14:31.000000 sn_test-1.0.7/sn_test.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        8 2023-07-28 08:14:31.000000 sn_test-1.0.7/sn_test.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 11:27:16.000000 sn_test-1.0.8/
+-rw-r--r--   0 mac        (501) staff       (20)    15245 2023-07-28 11:27:16.000000 sn_test-1.0.8/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     3180 2023-07-28 11:27:12.000000 sn_test-1.0.8/set_up.py
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-28 11:27:16.000000 sn_test-1.0.8/setup.cfg
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 11:27:16.000000 sn_test-1.0.8/sn_test/
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-07-21 08:42:56.000000 sn_test-1.0.8/sn_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      294 2023-07-21 06:40:48.000000 sn_test-1.0.8/sn_test/test_sn.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 11:27:16.000000 sn_test-1.0.8/sn_test.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)    15245 2023-07-28 11:27:16.000000 sn_test-1.0.8/sn_test.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      202 2023-07-28 11:27:16.000000 sn_test-1.0.8/sn_test.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-28 11:27:16.000000 sn_test-1.0.8/sn_test.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-28 11:27:16.000000 sn_test-1.0.8/sn_test.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        8 2023-07-28 11:27:16.000000 sn_test-1.0.8/sn_test.egg-info/top_level.txt
```

### Comparing `sn_test-1.0.7/set_up.py` & `sn_test-1.0.8/set_up.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'sn_test'
 DESCRIPTION = 'shuainan test'
 URL = 'https://github.com/me/myproject'
 EMAIL = '15294627382@163.com'
 AUTHOR = 'shuainan'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.0.7'
+VERSION = '1.0.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'websocket'
 ]
```

