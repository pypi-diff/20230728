# Comparing `tmp/sn_test-1.0.4.tar.gz` & `tmp/sn_test-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sn_test-1.0.4.tar", last modified: Fri Jul 21 06:53:51 2023, max compression
+gzip compressed data, was "dist/sn_test-1.0.5.tar", last modified: Fri Jul 28 07:51:35 2023, max compression
```

## Comparing `sn_test-1.0.4.tar` & `sn_test-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-21 06:53:51.000000 sn_test-1.0.4/
--rw-r--r--   0 mac        (501) staff       (20)      605 2023-07-21 06:53:51.000000 sn_test-1.0.4/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     3180 2023-07-21 06:53:36.000000 sn_test-1.0.4/set_up.py
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-21 06:53:51.000000 sn_test-1.0.4/setup.cfg
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-21 06:53:51.000000 sn_test-1.0.4/sn_test/
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-07-21 06:52:41.000000 sn_test-1.0.4/sn_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      294 2023-07-21 06:40:48.000000 sn_test-1.0.4/sn_test/test_sn.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-21 06:53:51.000000 sn_test-1.0.4/sn_test.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      605 2023-07-21 06:53:51.000000 sn_test-1.0.4/sn_test.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      202 2023-07-21 06:53:51.000000 sn_test-1.0.4/sn_test.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-21 06:53:51.000000 sn_test-1.0.4/sn_test.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-21 06:53:51.000000 sn_test-1.0.4/sn_test.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        8 2023-07-21 06:53:51.000000 sn_test-1.0.4/sn_test.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 07:51:35.000000 sn_test-1.0.5/
+-rw-r--r--   0 mac        (501) staff       (20)     4631 2023-07-28 07:51:35.000000 sn_test-1.0.5/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     3180 2023-07-28 07:51:17.000000 sn_test-1.0.5/set_up.py
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-28 07:51:35.000000 sn_test-1.0.5/setup.cfg
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 07:51:35.000000 sn_test-1.0.5/sn_test/
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-07-21 08:42:56.000000 sn_test-1.0.5/sn_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      294 2023-07-21 06:40:48.000000 sn_test-1.0.5/sn_test/test_sn.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 07:51:35.000000 sn_test-1.0.5/sn_test.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     4631 2023-07-28 07:51:35.000000 sn_test-1.0.5/sn_test.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      202 2023-07-28 07:51:35.000000 sn_test-1.0.5/sn_test.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-28 07:51:35.000000 sn_test-1.0.5/sn_test.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-28 07:51:35.000000 sn_test-1.0.5/sn_test.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        8 2023-07-28 07:51:35.000000 sn_test-1.0.5/sn_test.egg-info/top_level.txt
```

### Comparing `sn_test-1.0.4/set_up.py` & `sn_test-1.0.5/set_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'sn_test'
 DESCRIPTION = 'shuainan test'
 URL = 'https://github.com/me/myproject'
 EMAIL = '15294627382@163.com'
 AUTHOR = 'shuainan'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.0.4'
+VERSION = '1.0.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'websocket'
 ]
```

