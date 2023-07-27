# Comparing `tmp/gandai-1.3.6.tar.gz` & `tmp/gandai-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.3.6.tar", last modified: Wed Jul 26 17:55:47 2023, max compression
+gzip compressed data, was "gandai-1.3.7.tar", last modified: Thu Jul 27 23:04:00 2023, max compression
```

## Comparing `gandai-1.3.6.tar` & `gandai-1.3.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-26 17:55:47.838841 gandai-1.3.6/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.3.6/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-26 17:55:47.838725 gandai-1.3.6/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-26 17:55:47.833822 gandai-1.3.6/gandai/
--rw-r--r--   0 parker     (501) staff       (20)       46 2023-07-17 18:25:43.000000 gandai-1.3.6/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-26 17:55:47.836801 gandai-1.3.6/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      264 2023-07-17 18:43:09.000000 gandai-1.3.6/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.3.6/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4120 2023-07-25 17:01:01.000000 gandai-1.3.6/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-26 14:50:18.000000 gandai-1.3.6/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.3.6/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2023-07-17 18:43:09.000000 gandai-1.3.6/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3757 2023-07-25 19:02:34.000000 gandai-1.3.6/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.3.6/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1373 2023-07-23 18:54:58.000000 gandai-1.3.6/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4285 2023-07-26 14:50:18.000000 gandai-1.3.6/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6151 2023-07-17 18:43:10.000000 gandai-1.3.6/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    31858 2023-07-26 14:50:18.000000 gandai-1.3.6/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2221 2023-07-26 13:45:26.000000 gandai-1.3.6/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.3.6/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    17500 2023-07-26 17:54:47.000000 gandai-1.3.6/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2368 2023-07-25 17:01:00.000000 gandai-1.3.6/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1759 2023-07-25 20:25:00.000000 gandai-1.3.6/gandai/auth.py
--rw-r--r--   0 parker     (501) staff       (20)     1200 2023-07-17 18:25:43.000000 gandai-1.3.6/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1631 2023-07-25 19:02:05.000000 gandai-1.3.6/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)      402 2023-07-23 18:54:56.000000 gandai-1.3.6/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)     3030 2023-07-25 23:46:20.000000 gandai-1.3.6/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-26 17:55:47.837502 gandai-1.3.6/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.3.6/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-26 17:55:47.837978 gandai-1.3.6/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.3.6/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.3.6/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.3.6/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.3.6/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.3.6/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-26 17:55:47.838549 gandai-1.3.6/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.3.6/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3061 2023-07-17 18:25:43.000000 gandai-1.3.6/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     2683 2023-07-17 18:25:43.000000 gandai-1.3.6/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    20866 2023-07-26 14:03:27.000000 gandai-1.3.6/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1069 2023-07-25 20:41:48.000000 gandai-1.3.6/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)    11623 2023-07-26 17:54:47.000000 gandai-1.3.6/gandai/sources.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-26 17:55:47.834247 gandai-1.3.6/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-26 17:55:47.000000 gandai-1.3.6/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1275 2023-07-26 17:55:47.000000 gandai-1.3.6/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-26 17:55:47.000000 gandai-1.3.6/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-07-26 17:55:47.000000 gandai-1.3.6/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      383 2023-07-26 17:55:31.000000 gandai-1.3.6/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-26 17:55:47.838871 gandai-1.3.6/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.3.6/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-27 23:04:00.633497 gandai-1.3.7/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.3.7/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-27 23:04:00.633390 gandai-1.3.7/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-27 23:04:00.628603 gandai-1.3.7/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)       46 2023-07-17 18:25:43.000000 gandai-1.3.7/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-27 23:04:00.631469 gandai-1.3.7/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      264 2023-07-17 18:43:09.000000 gandai-1.3.7/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.3.7/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4120 2023-07-27 20:57:53.000000 gandai-1.3.7/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.3.7/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.3.7/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2023-07-17 18:43:09.000000 gandai-1.3.7/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3757 2023-07-27 21:29:01.000000 gandai-1.3.7/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.3.7/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1373 2023-07-27 20:52:17.000000 gandai-1.3.7/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4285 2023-07-27 20:52:17.000000 gandai-1.3.7/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6151 2023-07-17 18:43:10.000000 gandai-1.3.7/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    30266 2023-07-27 21:29:01.000000 gandai-1.3.7/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2221 2023-07-26 13:45:26.000000 gandai-1.3.7/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.3.7/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17500 2023-07-27 21:29:01.000000 gandai-1.3.7/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2368 2023-07-27 20:52:17.000000 gandai-1.3.7/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1759 2023-07-27 20:52:17.000000 gandai-1.3.7/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1200 2023-07-17 18:25:43.000000 gandai-1.3.7/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1631 2023-07-27 21:16:13.000000 gandai-1.3.7/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)      402 2023-07-27 20:52:17.000000 gandai-1.3.7/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)     3030 2023-07-27 20:52:17.000000 gandai-1.3.7/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-27 23:04:00.632190 gandai-1.3.7/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.3.7/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-27 23:04:00.632652 gandai-1.3.7/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.3.7/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.3.7/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.3.7/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.3.7/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.3.7/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-27 23:04:00.633193 gandai-1.3.7/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.3.7/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3061 2023-07-17 18:25:43.000000 gandai-1.3.7/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     2683 2023-07-17 18:25:43.000000 gandai-1.3.7/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    21313 2023-07-27 21:23:57.000000 gandai-1.3.7/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1069 2023-07-25 20:41:48.000000 gandai-1.3.7/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)    11623 2023-07-27 21:01:14.000000 gandai-1.3.7/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-27 23:04:00.629073 gandai-1.3.7/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-27 23:04:00.000000 gandai-1.3.7/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1275 2023-07-27 23:04:00.000000 gandai-1.3.7/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-27 23:04:00.000000 gandai-1.3.7/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-07-27 23:04:00.000000 gandai-1.3.7/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      383 2023-07-27 23:03:40.000000 gandai-1.3.7/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-27 23:04:00.633526 gandai-1.3.7/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.3.7/setup.py
```

### Comparing `gandai-1.3.6/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.3.7/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.3.7/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xccffbf64 (Tue Jul 25 17:01:00 2023 UTC)
+moddate:  0x01d9c264 (Thu Jul 27 20:52:17 2023 UTC)
 files sz: 2368
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `gandai-1.3.6/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.3.7/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x9c2fc064 (Tue Jul 25 20:25:00 2023 UTC)
+moddate:  0x01d9c264 (Thu Jul 27 20:52:17 2023 UTC)
 files sz: 1759
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `gandai-1.3.6/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.3.7/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.3.7/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.3.7/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x2d1cc064 (Tue Jul 25 19:02:05 2023 UTC)
+moddate:  0x9ddec264 (Thu Jul 27 21:16:13 2023 UTC)
 files sz: 1631
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `gandai-1.3.6/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.3.7/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.3.7/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8077bd64 (Sun Jul 23 18:54:56 2023 UTC)
+moddate:  0x01d9c264 (Thu Jul 27 20:52:17 2023 UTC)
 files sz: 402
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `gandai-1.3.6/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.3.7/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xcc5ec064 (Tue Jul 25 23:46:20 2023 UTC)
+moddate:  0x01d9c264 (Thu Jul 27 20:52:17 2023 UTC)
 files sz: 3030
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `gandai-1.3.6/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.3.7/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.3.7/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xaf27c164 (Wed Jul 26 14:03:27 2023 UTC)
-files sz: 20866
+moddate:  0x6de0c264 (Thu Jul 27 21:23:57 2023 UTC)
+files sz: 21313
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -16,25 +16,24 @@
       00000000005a1a640a65166602640b84045a1b640c6517640d6517660464
       0e84045a1c640f6514640d65146604641084045a1d64116519640d651966
       04641284045a1e64136515640d65156604641484045a1f64156505652019
       000000000000000000641665216417652064186520640d6401660a641984
       045a22641a65056504190000000000000000006416652164176520640d64
       016608641b84045a23640d65076a2400000000000000006602641c84045a
       25640d65076a2400000000000000006602641d84045a26641e84005a2764
-      0d65076a2400000000000000006602641f84045a28642f64166521641865
+      0d65076a2400000000000000006602641f84045a28642e64166521641865
       206604642084055a2964166521640d65076a240000000000000000660464
       2184045a2a64166521640d65076a2400000000000000006604642284045a
-      2b64166521640d65076a2400000000000000006604642384045a2c641665
-      21640d65076a2400000000000000006604642484045a2d640d65076a2400
-      000000000000006602642584045a2e64166521640d65076a240000000000
-      0000006604642684045a2f64166521640d65076a24000000000000000066
-      04642784045a3064166521640d65196604642884045a3164296520640d65
-      166604642a84045a32642b6521640d65176604642c84045a33640a651664
-      0d64016604642d84045a3464116519640d64016604642e84045a35640153
-      00
+      2b64166521640d65076a2400000000000000006604642384045a2c640d65
+      076a2400000000000000006602642484045a2d64166521640d65076a2400
+      000000000000006604642584045a2e64166521640d65076a240000000000
+      0000006604642684045a2f64166521640d65196604642784045a30642865
+      20640d65166604642984045a31642a6521640d65176604642b84045a3264
+      0a6516640d64016604642c84045a3364116519640d64016604642d84045a
+      3464015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (json)
                  8 STORE_NAME               0 (json)
    
@@ -194,189 +193,179 @@
    107         292 LOAD_CONST               1 (None)
    
    105         294 BUILD_TUPLE             10
                296 LOAD_CONST              25 (<code object insert_targets_from_domains, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 105>)
                298 MAKE_FUNCTION            4 (annotations)
                300 STORE_NAME              34 (insert_targets_from_domains)
    
-   157         302 LOAD_CONST              26 ('companies')
+   162         302 LOAD_CONST              26 ('companies')
    
-   158         304 LOAD_NAME                5 (List)
+   163         304 LOAD_NAME                5 (List)
                306 LOAD_NAME                4 (Any)
                308 BINARY_SUBSCR
    
-   157         318 LOAD_CONST              22 ('search_uid')
+   162         318 LOAD_CONST              22 ('search_uid')
    
-   158         320 LOAD_NAME               33 (int)
+   163         320 LOAD_NAME               33 (int)
    
-   157         322 LOAD_CONST              23 ('actor_key')
+   162         322 LOAD_CONST              23 ('actor_key')
    
-   158         324 LOAD_NAME               32 (str)
+   163         324 LOAD_NAME               32 (str)
    
-   157         326 LOAD_CONST              13 ('return')
+   162         326 LOAD_CONST              13 ('return')
    
-   159         328 LOAD_CONST               1 (None)
+   164         328 LOAD_CONST               1 (None)
    
-   157         330 BUILD_TUPLE              8
-               332 LOAD_CONST              27 (<code object insert_companies_as_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 157>)
+   162         330 BUILD_TUPLE              8
+               332 LOAD_CONST              27 (<code object insert_companies_as_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 162>)
                334 MAKE_FUNCTION            4 (annotations)
                336 STORE_NAME              35 (insert_companies_as_targets)
    
-   211         338 LOAD_CONST              13 ('return')
+   216         338 LOAD_CONST              13 ('return')
                340 LOAD_NAME                7 (pd)
                342 LOAD_ATTR               36 (DataFrame)
                352 BUILD_TUPLE              2
-               354 LOAD_CONST              28 (<code object top_actor_per_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 211>)
+               354 LOAD_CONST              28 (<code object top_actor_per_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 216>)
                356 MAKE_FUNCTION            4 (annotations)
                358 STORE_NAME              37 (top_actor_per_search)
    
-   249         360 LOAD_CONST              13 ('return')
+   254         360 LOAD_CONST              13 ('return')
                362 LOAD_NAME                7 (pd)
                364 LOAD_ATTR               36 (DataFrame)
                374 BUILD_TUPLE              2
-               376 LOAD_CONST              29 (<code object search_event_count_by_type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 249>)
+               376 LOAD_CONST              29 (<code object search_event_count_by_type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 254>)
                378 MAKE_FUNCTION            4 (annotations)
                380 STORE_NAME              38 (search_event_count_by_type)
    
-   265         382 LOAD_CONST              30 (<code object search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 265>)
+   270         382 LOAD_CONST              30 (<code object search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 270>)
                384 MAKE_FUNCTION            0
                386 STORE_NAME              39 (search)
    
-   307         388 LOAD_CONST              13 ('return')
+   312         388 LOAD_CONST              13 ('return')
                390 LOAD_NAME                7 (pd)
                392 LOAD_ATTR               36 (DataFrame)
                402 BUILD_TUPLE              2
-               404 LOAD_CONST              31 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 307>)
+               404 LOAD_CONST              31 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 312>)
                406 MAKE_FUNCTION            4 (annotations)
                408 STORE_NAME              40 (actor)
    
-   321         410 LOAD_CONST              47 ((None,))
+   326         410 LOAD_CONST              46 ((None,))
                412 LOAD_CONST              22 ('search_uid')
                414 LOAD_NAME               33 (int)
                416 LOAD_CONST              24 ('last_event_type')
                418 LOAD_NAME               32 (str)
                420 BUILD_TUPLE              4
-               422 LOAD_CONST              32 (<code object search_target_by_last_event_type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 321>)
+               422 LOAD_CONST              32 (<code object search_target_by_last_event_type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 326>)
                424 MAKE_FUNCTION            5 (defaults, annotations)
                426 STORE_NAME              41 (search_target_by_last_event_type)
    
-   390         428 LOAD_CONST              22 ('search_uid')
+   456         428 LOAD_CONST              22 ('search_uid')
                430 LOAD_NAME               33 (int)
                432 LOAD_CONST              13 ('return')
                434 LOAD_NAME                7 (pd)
                436 LOAD_ATTR               36 (DataFrame)
                446 BUILD_TUPLE              4
-               448 LOAD_CONST              33 (<code object search_target_export, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 390>)
+               448 LOAD_CONST              33 (<code object target_count, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 456>)
                450 MAKE_FUNCTION            4 (annotations)
-               452 STORE_NAME              42 (search_target_export)
+               452 STORE_NAME              42 (target_count)
    
-   449         454 LOAD_CONST              22 ('search_uid')
+   486         454 LOAD_CONST              22 ('search_uid')
                456 LOAD_NAME               33 (int)
                458 LOAD_CONST              13 ('return')
                460 LOAD_NAME                7 (pd)
                462 LOAD_ATTR               36 (DataFrame)
                472 BUILD_TUPLE              4
-               474 LOAD_CONST              34 (<code object target_count, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 449>)
+               474 LOAD_CONST              34 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 486>)
                476 MAKE_FUNCTION            4 (annotations)
-               478 STORE_NAME              43 (target_count)
+               478 STORE_NAME              43 (event)
    
-   479         480 LOAD_CONST              22 ('search_uid')
+   498         480 LOAD_CONST              22 ('search_uid')
                482 LOAD_NAME               33 (int)
                484 LOAD_CONST              13 ('return')
                486 LOAD_NAME                7 (pd)
                488 LOAD_ATTR               36 (DataFrame)
                498 BUILD_TUPLE              4
-               500 LOAD_CONST              35 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 479>)
+               500 LOAD_CONST              35 (<code object unique_domains, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 498>)
                502 MAKE_FUNCTION            4 (annotations)
-               504 STORE_NAME              44 (event)
+               504 STORE_NAME              44 (unique_domains)
    
-   491         506 LOAD_CONST              22 ('search_uid')
-               508 LOAD_NAME               33 (int)
-               510 LOAD_CONST              13 ('return')
-               512 LOAD_NAME                7 (pd)
-               514 LOAD_ATTR               36 (DataFrame)
-               524 BUILD_TUPLE              4
-               526 LOAD_CONST              36 (<code object unique_domains, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 491>)
-               528 MAKE_FUNCTION            4 (annotations)
-               530 STORE_NAME              45 (unique_domains)
-   
-   503         532 LOAD_CONST              13 ('return')
+   510         506 LOAD_CONST              13 ('return')
+               508 LOAD_NAME                7 (pd)
+               510 LOAD_ATTR               36 (DataFrame)
+               520 BUILD_TUPLE              2
+               522 LOAD_CONST              36 (<code object company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 510>)
+               524 MAKE_FUNCTION            4 (annotations)
+               526 STORE_NAME              45 (company)
+   
+   521         528 LOAD_CONST              22 ('search_uid')
+               530 LOAD_NAME               33 (int)
+               532 LOAD_CONST              13 ('return')
                534 LOAD_NAME                7 (pd)
                536 LOAD_ATTR               36 (DataFrame)
-               546 BUILD_TUPLE              2
-               548 LOAD_CONST              37 (<code object company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 503>)
+               546 BUILD_TUPLE              4
+               548 LOAD_CONST              37 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 521>)
                550 MAKE_FUNCTION            4 (annotations)
-               552 STORE_NAME              46 (company)
+               552 STORE_NAME              46 (checkpoint)
    
-   514         554 LOAD_CONST              22 ('search_uid')
+   534         554 LOAD_CONST              22 ('search_uid')
                556 LOAD_NAME               33 (int)
                558 LOAD_CONST              13 ('return')
                560 LOAD_NAME                7 (pd)
                562 LOAD_ATTR               36 (DataFrame)
                572 BUILD_TUPLE              4
-               574 LOAD_CONST              38 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 514>)
+               574 LOAD_CONST              38 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 534>)
                576 MAKE_FUNCTION            4 (annotations)
-               578 STORE_NAME              47 (checkpoint)
+               578 STORE_NAME              47 (comment_by_domain)
    
-   527         580 LOAD_CONST              22 ('search_uid')
+   555         580 LOAD_CONST              22 ('search_uid')
                582 LOAD_NAME               33 (int)
                584 LOAD_CONST              13 ('return')
-               586 LOAD_NAME                7 (pd)
-               588 LOAD_ATTR               36 (DataFrame)
-               598 BUILD_TUPLE              4
-               600 LOAD_CONST              39 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 527>)
-               602 MAKE_FUNCTION            4 (annotations)
-               604 STORE_NAME              48 (comment_by_domain)
-   
-   548         606 LOAD_CONST              22 ('search_uid')
-               608 LOAD_NAME               33 (int)
-               610 LOAD_CONST              13 ('return')
-               612 LOAD_NAME               25 (Search)
-               614 BUILD_TUPLE              4
-               616 LOAD_CONST              40 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 548>)
-               618 MAKE_FUNCTION            4 (annotations)
-               620 STORE_NAME              49 (find_search_by_uid)
-   
-   566         622 LOAD_CONST              41 ('domain')
-               624 LOAD_NAME               32 (str)
-               626 LOAD_CONST              13 ('return')
-               628 LOAD_NAME               22 (Company)
-               630 BUILD_TUPLE              4
-               632 LOAD_CONST              42 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 566>)
-               634 MAKE_FUNCTION            4 (annotations)
-               636 STORE_NAME              50 (find_company_by_domain)
-   
-   582         638 LOAD_CONST              43 ('event_id')
-               640 LOAD_NAME               33 (int)
-               642 LOAD_CONST              13 ('return')
-               644 LOAD_NAME               23 (Event)
-               646 BUILD_TUPLE              4
-               648 LOAD_CONST              44 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 582>)
-               650 MAKE_FUNCTION            4 (annotations)
-               652 STORE_NAME              51 (find_event_by_id)
-   
-   601         654 LOAD_CONST              10 ('company')
-               656 LOAD_NAME               22 (Company)
-               658 LOAD_CONST              13 ('return')
+               586 LOAD_NAME               25 (Search)
+               588 BUILD_TUPLE              4
+               590 LOAD_CONST              39 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 555>)
+               592 MAKE_FUNCTION            4 (annotations)
+               594 STORE_NAME              48 (find_search_by_uid)
+   
+   573         596 LOAD_CONST              40 ('domain')
+               598 LOAD_NAME               32 (str)
+               600 LOAD_CONST              13 ('return')
+               602 LOAD_NAME               22 (Company)
+               604 BUILD_TUPLE              4
+               606 LOAD_CONST              41 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 573>)
+               608 MAKE_FUNCTION            4 (annotations)
+               610 STORE_NAME              49 (find_company_by_domain)
+   
+   589         612 LOAD_CONST              42 ('event_id')
+               614 LOAD_NAME               33 (int)
+               616 LOAD_CONST              13 ('return')
+               618 LOAD_NAME               23 (Event)
+               620 BUILD_TUPLE              4
+               622 LOAD_CONST              43 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 589>)
+               624 MAKE_FUNCTION            4 (annotations)
+               626 STORE_NAME              50 (find_event_by_id)
+   
+   608         628 LOAD_CONST              10 ('company')
+               630 LOAD_NAME               22 (Company)
+               632 LOAD_CONST              13 ('return')
+               634 LOAD_CONST               1 (None)
+               636 BUILD_TUPLE              4
+               638 LOAD_CONST              44 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 608>)
+               640 MAKE_FUNCTION            4 (annotations)
+               642 STORE_NAME              51 (update_company)
+   
+   635         644 LOAD_CONST              17 ('search')
+               646 LOAD_NAME               25 (Search)
+               648 LOAD_CONST              13 ('return')
+               650 LOAD_CONST               1 (None)
+               652 BUILD_TUPLE              4
+               654 LOAD_CONST              45 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 635>)
+               656 MAKE_FUNCTION            4 (annotations)
+               658 STORE_NAME              52 (update_search)
                660 LOAD_CONST               1 (None)
-               662 BUILD_TUPLE              4
-               664 LOAD_CONST              45 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 601>)
-               666 MAKE_FUNCTION            4 (annotations)
-               668 STORE_NAME              52 (update_company)
-   
-   628         670 LOAD_CONST              17 ('search')
-               672 LOAD_NAME               25 (Search)
-               674 LOAD_CONST              13 ('return')
-               676 LOAD_CONST               1 (None)
-               678 BUILD_TUPLE              4
-               680 LOAD_CONST              46 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 628>)
-               682 MAKE_FUNCTION            4 (annotations)
-               684 STORE_NAME              53 (update_search)
-               686 LOAD_CONST               1 (None)
-               688 RETURN_VALUE
+               662 RETURN_VALUE
    consts
       0
       None
       ('asdict',)
       ('Any', 'List')
       ('from_dict',)
       ('load_dotenv',)
@@ -929,29 +918,33 @@
          stacksize : 10
          flags     : 3
          code
             0x97007401000000000000000000007403000000000000000000007c01ac
             01a6010000ab010000000000000000640219000000000000000000a60100
             00ab0100000000000000007d04640384007c004400a6000000ab00000000
             00000000007d057405000000000000000000007c057c047a0a0000a60100
-            00ab0100000000000000007d06740600000000000000000000a004000000
-            0000000000000000000000000000000000a6000000ab0000000000000000
-            0035007d077c0644005d597d087c07a00500000000000000000000000000
-            00000000000000740d000000000000000000006a07000000000000000064
-            04a6010000ab01000000000000000064027c086901a6020000ab02000000
-            000000000001007c07a00500000000000000000000000000000000000000
-            00740d000000000000000000006a0700000000000000006405a6010000ab
-            0100000000000000007c017c027c087c0364069c04a6020000ab02000000
-            000000000001008c5a7c07a0080000000000000000000000000000000000
-            000000a6000000ab0000000000000000000100640764076407a6020000ab
-            02000000000000000001006e0b2300310073047702780359007701010059
-            00010001007413000000000000000000007c06a6010000ab010000000000
-            0000007413000000000000000000007c05a00a0000000000000000000000
-            0000000000000000007c04a6010000ab010000000000000000a6010000ab
-            01000000000000000064089c027d097c095300
+            00ab0100000000000000007d067401000000000000000000007403000000
+            000000000000007c01ac01a6010000ab0100000000000000006402190000
+            00000000000000a6010000ab0100000000000000007d04640484007c0044
+            00a6000000ab0000000000000000007d057405000000000000000000007c
+            057c047a0a0000a6010000ab0100000000000000007d0674060000000000
+            0000000000a0040000000000000000000000000000000000000000a60000
+            00ab00000000000000000035007d077c0644005d597d087c07a005000000
+            0000000000000000000000000000000000740d000000000000000000006a
+            0700000000000000006405a6010000ab01000000000000000064027c0869
+            01a6020000ab02000000000000000001007c07a005000000000000000000
+            0000000000000000000000740d000000000000000000006a070000000000
+            0000006406a6010000ab0100000000000000007c017c027c087c0364079c
+            04a6020000ab02000000000000000001008c5a7c07a00800000000000000
+            00000000000000000000000000a6000000ab000000000000000000010064
+            0864086408a6020000ab02000000000000000001006e0b23003100730477
+            0278035900770101005900010001007413000000000000000000007c06a6
+            010000ab0100000000000000007413000000000000000000007c05a00a00
+            000000000000000000000000000000000000007c04a6010000ab01000000
+            0000000000a6010000ab01000000000000000064099c027d097c095300
          105           0 RESUME                   0
          
          112           2 LOAD_GLOBAL              1 (NULL + set)
                       14 LOAD_GLOBAL              3 (NULL + unique_domains)
                       26 LOAD_FAST                1 (search_uid)
                       28 KW_NAMES                 1
                       30 PRECALL                  1
@@ -974,121 +967,149 @@
                      108 LOAD_FAST                5 (new_domains)
                      110 LOAD_FAST                4 (existing_domains)
                      112 BINARY_OP               10 (-)
                      116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               6 (domains_to_insert)
          
-         118         132 LOAD_GLOBAL              6 (db)
-                     144 LOAD_METHOD              4 (connect)
-                     166 PRECALL                  0
-                     170 CALL                     0
-                     180 BEFORE_WITH
-                     182 STORE_FAST               7 (con)
-         
-         119         184 LOAD_FAST                6 (domains_to_insert)
-                     186 GET_ITER
-                 >>  188 FOR_ITER                89 (to 368)
-                     190 STORE_FAST               8 (domain)
-         
-         121         192 LOAD_FAST                7 (con)
-                     194 LOAD_METHOD              5 (execute)
-         
-         122         216 LOAD_GLOBAL             13 (NULL + sqlalchemy)
-                     228 LOAD_ATTR                7 (text)
-         
-         123         238 LOAD_CONST               4 ('\n                    INSERT INTO company (domain) \n                    VALUES(:domain)\n                    ON CONFLICT DO NOTHING\n                    ')
-         
-         122         240 PRECALL                  1
-                     244 CALL                     1
-         
-         129         254 LOAD_CONST               2 ('domain')
-                     256 LOAD_FAST                8 (domain)
-                     258 BUILD_MAP                1
-         
-         121         260 PRECALL                  2
-                     264 CALL                     2
-                     274 POP_TOP
-         
-         132         276 LOAD_FAST                7 (con)
-                     278 LOAD_METHOD              5 (execute)
-         
-         133         300 LOAD_GLOBAL             13 (NULL + sqlalchemy)
-                     312 LOAD_ATTR                7 (text)
+         117         132 LOAD_GLOBAL              1 (NULL + set)
+                     144 LOAD_GLOBAL              3 (NULL + unique_domains)
+                     156 LOAD_FAST                1 (search_uid)
+                     158 KW_NAMES                 1
+                     160 PRECALL                  1
+                     164 CALL                     1
+                     174 LOAD_CONST               2 ('domain')
+                     176 BINARY_SUBSCR
+                     186 PRECALL                  1
+                     190 CALL                     1
+                     200 STORE_FAST               4 (existing_domains)
+         
+         119         202 LOAD_CONST               4 (<code object <setcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 119>)
+                     204 MAKE_FUNCTION            0
+                     206 LOAD_FAST                0 (domains)
+                     208 GET_ITER
+                     210 PRECALL                  0
+                     214 CALL                     0
+                     224 STORE_FAST               5 (new_domains)
+         
+         121         226 LOAD_GLOBAL              5 (NULL + list)
+                     238 LOAD_FAST                5 (new_domains)
+                     240 LOAD_FAST                4 (existing_domains)
+                     242 BINARY_OP               10 (-)
+                     246 PRECALL                  1
+                     250 CALL                     1
+                     260 STORE_FAST               6 (domains_to_insert)
          
-         134         322 LOAD_CONST               5 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ON CONFLICT DO NOTHING\n                    ')
+         123         262 LOAD_GLOBAL              6 (db)
+                     274 LOAD_METHOD              4 (connect)
+                     296 PRECALL                  0
+                     300 CALL                     0
+                     310 BEFORE_WITH
+                     312 STORE_FAST               7 (con)
+         
+         124         314 LOAD_FAST                6 (domains_to_insert)
+                     316 GET_ITER
+                 >>  318 FOR_ITER                89 (to 498)
+                     320 STORE_FAST               8 (domain)
+         
+         126         322 LOAD_FAST                7 (con)
+                     324 LOAD_METHOD              5 (execute)
+         
+         127         346 LOAD_GLOBAL             13 (NULL + sqlalchemy)
+                     358 LOAD_ATTR                7 (text)
+         
+         128         368 LOAD_CONST               5 ('\n                    INSERT INTO company (domain) \n                    VALUES(:domain)\n                    ON CONFLICT DO NOTHING\n                    ')
+         
+         127         370 PRECALL                  1
+                     374 CALL                     1
+         
+         134         384 LOAD_CONST               2 ('domain')
+                     386 LOAD_FAST                8 (domain)
+                     388 BUILD_MAP                1
+         
+         126         390 PRECALL                  2
+                     394 CALL                     2
+                     404 POP_TOP
+         
+         137         406 LOAD_FAST                7 (con)
+                     408 LOAD_METHOD              5 (execute)
+         
+         138         430 LOAD_GLOBAL             13 (NULL + sqlalchemy)
+                     442 LOAD_ATTR                7 (text)
+         
+         139         452 LOAD_CONST               6 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ON CONFLICT DO NOTHING\n                    ')
+         
+         138         454 PRECALL                  1
+                     458 CALL                     1
+         
+         146         468 LOAD_FAST                1 (search_uid)
+         
+         147         470 LOAD_FAST                2 (actor_key)
+         
+         148         472 LOAD_FAST                8 (domain)
+         
+         149         474 LOAD_FAST                3 (last_event_type)
+         
+         145         476 LOAD_CONST               7 (('search_uid', 'actor_key', 'domain', 'type'))
+                     478 BUILD_CONST_KEY_MAP      4
+         
+         137         480 PRECALL                  2
+                     484 CALL                     2
+                     494 POP_TOP
+                     496 JUMP_BACKWARD           90 (to 318)
+         
+         153     >>  498 LOAD_FAST                7 (con)
+                     500 LOAD_METHOD              8 (commit)
+                     522 PRECALL                  0
+                     526 CALL                     0
+                     536 POP_TOP
+         
+         123         538 LOAD_CONST               8 (None)
+                     540 LOAD_CONST               8 (None)
+                     542 LOAD_CONST               8 (None)
+                     544 PRECALL                  2
+                     548 CALL                     2
+                     558 POP_TOP
+                     560 JUMP_FORWARD            11 (to 584)
+                 >>  562 PUSH_EXC_INFO
+                     564 WITH_EXCEPT_START
+                     566 POP_JUMP_FORWARD_IF_TRUE     4 (to 576)
+                     568 RERAISE                  2
+                 >>  570 COPY                     3
+                     572 POP_EXCEPT
+                     574 RERAISE                  1
+                 >>  576 POP_TOP
+                     578 POP_EXCEPT
+                     580 POP_TOP
+                     582 POP_TOP
+         
+         156     >>  584 LOAD_GLOBAL             19 (NULL + len)
+                     596 LOAD_FAST                6 (domains_to_insert)
+                     598 PRECALL                  1
+                     602 CALL                     1
          
-         133         324 PRECALL                  1
-                     328 CALL                     1
-         
-         141         338 LOAD_FAST                1 (search_uid)
-         
-         142         340 LOAD_FAST                2 (actor_key)
-         
-         143         342 LOAD_FAST                8 (domain)
-         
-         144         344 LOAD_FAST                3 (last_event_type)
-         
-         140         346 LOAD_CONST               6 (('search_uid', 'actor_key', 'domain', 'type'))
-                     348 BUILD_CONST_KEY_MAP      4
-         
-         132         350 PRECALL                  2
-                     354 CALL                     2
-                     364 POP_TOP
-                     366 JUMP_BACKWARD           90 (to 188)
-         
-         148     >>  368 LOAD_FAST                7 (con)
-                     370 LOAD_METHOD              8 (commit)
-                     392 PRECALL                  0
-                     396 CALL                     0
-                     406 POP_TOP
-         
-         118         408 LOAD_CONST               7 (None)
-                     410 LOAD_CONST               7 (None)
-                     412 LOAD_CONST               7 (None)
-                     414 PRECALL                  2
-                     418 CALL                     2
-                     428 POP_TOP
-                     430 JUMP_FORWARD            11 (to 454)
-                 >>  432 PUSH_EXC_INFO
-                     434 WITH_EXCEPT_START
-                     436 POP_JUMP_FORWARD_IF_TRUE     4 (to 446)
-                     438 RERAISE                  2
-                 >>  440 COPY                     3
-                     442 POP_EXCEPT
-                     444 RERAISE                  1
-                 >>  446 POP_TOP
-                     448 POP_EXCEPT
-                     450 POP_TOP
-                     452 POP_TOP
-         
-         151     >>  454 LOAD_GLOBAL             19 (NULL + len)
-                     466 LOAD_FAST                6 (domains_to_insert)
-                     468 PRECALL                  1
-                     472 CALL                     1
-         
-         152         482 LOAD_GLOBAL             19 (NULL + len)
-                     494 LOAD_FAST                5 (new_domains)
-                     496 LOAD_METHOD             10 (intersection)
-                     518 LOAD_FAST                4 (existing_domains)
-                     520 PRECALL                  1
-                     524 CALL                     1
-                     534 PRECALL                  1
-                     538 CALL                     1
-         
-         150         548 LOAD_CONST               8 (('inserted', 'duplicates'))
-                     550 BUILD_CONST_KEY_MAP      2
-                     552 STORE_FAST               9 (resp)
-         
-         154         554 LOAD_FAST                9 (resp)
-                     556 RETURN_VALUE
-         ExceptionTable:
-           182 to 406 -> 432 [1] lasti
-           432 to 438 -> 440 [3] lasti
-           446 to 446 -> 440 [3] lasti
+         157         612 LOAD_GLOBAL             19 (NULL + len)
+                     624 LOAD_FAST                5 (new_domains)
+                     626 LOAD_METHOD             10 (intersection)
+                     648 LOAD_FAST                4 (existing_domains)
+                     650 PRECALL                  1
+                     654 CALL                     1
+                     664 PRECALL                  1
+                     668 CALL                     1
+         
+         155         678 LOAD_CONST               9 (('inserted', 'duplicates'))
+                     680 BUILD_CONST_KEY_MAP      2
+                     682 STORE_FAST               9 (resp)
+         
+         159         684 LOAD_FAST                9 (resp)
+                     686 RETURN_VALUE
+         ExceptionTable:
+           312 to 536 -> 562 [1] lasti
+           562 to 568 -> 570 [3] lasti
+           576 to 576 -> 570 [3] lasti
          consts
             '\n    Takes in domains, inserts targets into a review stage, where they will\n    try to be enriched on process event\n    '
             ('search_uid',)
             'domain'
             code
                argcount  : 1
                nlocals   : 2
@@ -1121,29 +1142,66 @@
                varnames   ('.0', 'domain')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '<setcomp>'
                firstlineno 114
                lnotab 0x
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 5
+               flags     : 19
+               code
+                  0x970068007c005d1a7d0164007c017600af067401000000000000000000
+                  006a0100000000000000007c01a6010000ab01000000000000000092028c
+                  1b5300
+               119           0 RESUME                   0
+                             2 BUILD_SET                0
+                             4 LOAD_FAST                0 (.0)
+                       >>    6 FOR_ITER                26 (to 60)
+                             8 STORE_FAST               1 (domain)
+                            10 LOAD_CONST               0 ('.')
+                            12 LOAD_FAST                1 (domain)
+                            14 CONTAINS_OP              0
+                            16 POP_JUMP_BACKWARD_IF_FALSE     6 (to 6)
+                            18 LOAD_GLOBAL              1 (NULL + helpers)
+                            30 LOAD_ATTR                1 (clean_domain)
+                            40 LOAD_FAST                1 (domain)
+                            42 PRECALL                  1
+                            46 CALL                     1
+                            56 SET_ADD                  2
+                            58 JUMP_BACKWARD           27 (to 6)
+                       >>   60 RETURN_VALUE
+               consts
+                  '.'
+               names      ('helpers', 'clean_domain')
+               varnames   ('.0', 'domain')
+               freevars   ()
+               cellvars   ()
+               filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
+               name       '<setcomp>'
+               firstlineno 119
+               lnotab 0x
             '\n                    INSERT INTO company (domain) \n                    VALUES(:domain)\n                    ON CONFLICT DO NOTHING\n                    '
             '\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ON CONFLICT DO NOTHING\n                    '
             ('search_uid', 'actor_key', 'domain', 'type')
             None
             ('inserted', 'duplicates')
          names      ('set', 'unique_domains', 'list', 'db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit', 'len', 'intersection')
          varnames   ('domains', 'search_uid', 'actor_key', 'last_event_type', 'existing_domains', 'new_domains', 'domains_to_insert', 'con', 'domain', 'resp')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_targets_from_domains'
          firstlineno 105
          lnotab
-            0x0207460218022402340108021801160102ff0e0706f8100b1801160102
-            ff0e0802010201020102fc04f8121028e22e211c0142fe0604
+            0x0207460218022401460218022402340108021801160102ff0e0706f810
+            0b1801160102ff0e0802010201020102fc04f8121028e22e211c0142fe06
+            04
       'companies'
       code
          argcount  : 3
          nlocals   : 6
          stacksize : 10
          flags     : 3
          code
@@ -1169,168 +1227,168 @@
             0000000000740f000000000000000000006a080000000000000000640ea6
             010000ab0100000000000000007c017c027c05a004000000000000000000
             00000000000000000000006402a6010000ab010000000000000000640f64
             109c04a6020000ab020000000000000000010090018c107c04a009000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             000100640364036403a6020000ab02000000000000000001006403530023
             00310073047702780359007701010059000100010064035300
-         157           0 RESUME                   0
+         162           0 RESUME                   0
          
-         161           2 LOAD_GLOBAL              1 (NULL + unique_domains)
+         166           2 LOAD_GLOBAL              1 (NULL + unique_domains)
                       14 LOAD_FAST                1 (search_uid)
                       16 KW_NAMES                 1
                       18 PRECALL                  1
                       22 CALL                     1
                       32 LOAD_CONST               2 ('domain')
                       34 BINARY_SUBSCR
                       44 LOAD_METHOD              1 (to_list)
                       66 PRECALL                  0
                       70 CALL                     0
                       80 STORE_FAST               3 (existing_search_domains)
          
-         162          82 LOAD_GLOBAL              4 (db)
+         167          82 LOAD_GLOBAL              4 (db)
                       94 LOAD_METHOD              3 (connect)
                      116 PRECALL                  0
                      120 CALL                     0
                      130 BEFORE_WITH
                      132 STORE_FAST               4 (con)
          
-         163         134 LOAD_FAST                0 (companies)
+         168         134 LOAD_FAST                0 (companies)
                      136 GET_ITER
                  >>  138 EXTENDED_ARG             1
                      140 FOR_ITER               270 (to 682)
                      142 STORE_FAST               5 (company)
          
-         164         144 LOAD_FAST                5 (company)
+         169         144 LOAD_FAST                5 (company)
                      146 LOAD_METHOD              4 (get)
                      168 LOAD_CONST               2 ('domain')
                      170 PRECALL                  1
                      174 CALL                     1
                      184 POP_JUMP_FORWARD_IF_NOT_NONE    20 (to 226)
          
-         165         186 LOAD_GLOBAL             11 (NULL + print)
+         170         186 LOAD_GLOBAL             11 (NULL + print)
                      198 LOAD_CONST               4 ('Missing domain: ')
                      200 LOAD_FAST                5 (company)
                      202 FORMAT_VALUE             0
                      204 LOAD_CONST               5 ('. Skipping')
                      206 BUILD_STRING             3
                      208 PRECALL                  1
                      212 CALL                     1
                      222 POP_TOP
          
-         166         224 JUMP_BACKWARD           44 (to 138)
+         171         224 JUMP_BACKWARD           44 (to 138)
          
-         169     >>  226 LOAD_FAST                5 (company)
+         174     >>  226 LOAD_FAST                5 (company)
                      228 LOAD_CONST               2 ('domain')
                      230 BINARY_SUBSCR
                      240 LOAD_FAST                3 (existing_search_domains)
                      242 CONTAINS_OP              0
                      244 POP_JUMP_FORWARD_IF_FALSE    26 (to 298)
          
-         170         246 LOAD_GLOBAL             11 (NULL + print)
+         175         246 LOAD_GLOBAL             11 (NULL + print)
                      258 LOAD_CONST               6 ('Skipping ')
                      260 LOAD_FAST                5 (company)
                      262 LOAD_CONST               2 ('domain')
                      264 BINARY_SUBSCR
                      274 FORMAT_VALUE             0
                      276 LOAD_CONST               7 (' as already a target')
                      278 BUILD_STRING             3
                      280 PRECALL                  1
                      284 CALL                     1
                      294 POP_TOP
          
-         171         296 JUMP_BACKWARD           80 (to 138)
+         176         296 JUMP_BACKWARD           80 (to 138)
          
-         173     >>  298 LOAD_GLOBAL             11 (NULL + print)
+         178     >>  298 LOAD_GLOBAL             11 (NULL + print)
                      310 LOAD_CONST               8 ('Adding ')
                      312 LOAD_FAST                5 (company)
                      314 LOAD_CONST               2 ('domain')
                      316 BINARY_SUBSCR
                      326 FORMAT_VALUE             0
                      328 LOAD_CONST               9 (' as target')
                      330 BUILD_STRING             3
                      332 PRECALL                  1
                      336 CALL                     1
                      346 POP_TOP
          
-         175         348 LOAD_FAST                4 (con)
+         180         348 LOAD_FAST                4 (con)
                      350 LOAD_METHOD              6 (execute)
          
-         176         372 LOAD_GLOBAL             15 (NULL + sqlalchemy)
+         181         372 LOAD_GLOBAL             15 (NULL + sqlalchemy)
                      384 LOAD_ATTR                8 (text)
          
-         177         394 LOAD_CONST              10 ('\n                    INSERT INTO company (domain, name, description) \n                    VALUES(:domain, :name, :description)\n                    ON CONFLICT DO NOTHING\n                    ')
+         182         394 LOAD_CONST              10 ('\n                    INSERT INTO company (domain, name, description) \n                    VALUES(:domain, :name, :description)\n                    ON CONFLICT DO NOTHING\n                    ')
          
-         176         396 PRECALL                  1
+         181         396 PRECALL                  1
                      400 CALL                     1
          
-         184         410 LOAD_FAST                5 (company)
+         189         410 LOAD_FAST                5 (company)
                      412 LOAD_METHOD              4 (get)
                      434 LOAD_CONST               2 ('domain')
                      436 PRECALL                  1
                      440 CALL                     1
          
-         185         450 LOAD_FAST                5 (company)
+         190         450 LOAD_FAST                5 (company)
                      452 LOAD_METHOD              4 (get)
                      474 LOAD_CONST              11 ('name')
                      476 PRECALL                  1
                      480 CALL                     1
          
-         186         490 LOAD_FAST                5 (company)
+         191         490 LOAD_FAST                5 (company)
                      492 LOAD_METHOD              4 (get)
                      514 LOAD_CONST              12 ('description')
                      516 PRECALL                  1
                      520 CALL                     1
          
-         183         530 LOAD_CONST              13 (('domain', 'name', 'description'))
+         188         530 LOAD_CONST              13 (('domain', 'name', 'description'))
                      532 BUILD_CONST_KEY_MAP      3
          
-         175         534 PRECALL                  2
+         180         534 PRECALL                  2
                      538 CALL                     2
                      548 POP_TOP
          
-         190         550 LOAD_FAST                4 (con)
+         195         550 LOAD_FAST                4 (con)
                      552 LOAD_METHOD              6 (execute)
          
-         191         574 LOAD_GLOBAL             15 (NULL + sqlalchemy)
+         196         574 LOAD_GLOBAL             15 (NULL + sqlalchemy)
                      586 LOAD_ATTR                8 (text)
          
-         192         596 LOAD_CONST              14 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ')
+         197         596 LOAD_CONST              14 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ')
          
-         191         598 PRECALL                  1
+         196         598 PRECALL                  1
                      602 CALL                     1
          
-         198         612 LOAD_FAST                1 (search_uid)
+         203         612 LOAD_FAST                1 (search_uid)
          
-         199         614 LOAD_FAST                2 (actor_key)
+         204         614 LOAD_FAST                2 (actor_key)
          
-         200         616 LOAD_FAST                5 (company)
+         205         616 LOAD_FAST                5 (company)
                      618 LOAD_METHOD              4 (get)
                      640 LOAD_CONST               2 ('domain')
                      642 PRECALL                  1
                      646 CALL                     1
          
-         201         656 LOAD_CONST              15 ('create')
+         206         656 LOAD_CONST              15 ('create')
          
-         197         658 LOAD_CONST              16 (('search_uid', 'actor_key', 'domain', 'type'))
+         202         658 LOAD_CONST              16 (('search_uid', 'actor_key', 'domain', 'type'))
                      660 BUILD_CONST_KEY_MAP      4
          
-         190         662 PRECALL                  2
+         195         662 PRECALL                  2
                      666 CALL                     2
                      676 POP_TOP
                      678 EXTENDED_ARG             1
                      680 JUMP_BACKWARD          272 (to 138)
          
-         205     >>  682 LOAD_FAST                4 (con)
+         210     >>  682 LOAD_FAST                4 (con)
                      684 LOAD_METHOD              9 (commit)
                      706 PRECALL                  0
                      710 CALL                     0
                      720 POP_TOP
          
-         162         722 LOAD_CONST               3 (None)
+         167         722 LOAD_CONST               3 (None)
                      724 LOAD_CONST               3 (None)
                      726 LOAD_CONST               3 (None)
                      728 PRECALL                  2
                      732 CALL                     2
                      742 POP_TOP
                      744 LOAD_CONST               3 (None)
                      746 RETURN_VALUE
@@ -1371,15 +1429,15 @@
             ('search_uid', 'actor_key', 'domain', 'type')
          names      ('unique_domains', 'to_list', 'db', 'connect', 'get', 'print', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('companies', 'search_uid', 'actor_key', 'existing_search_domains', 'con', 'company')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_companies_as_targets'
-         firstlineno 157
+         firstlineno 162
          lnotab
             0x0204500134010a012a012601020314013201020232021801160102ff0e
             082801280128fd04f8100f1801160102ff0e0702010201280102fc04f914
             0f28d5
       code
          argcount  : 0
          nlocals   : 4
@@ -1393,55 +1451,55 @@
             00a6010000ab0100000000000000007d02740b000000000000000000006a
             0600000000000000007c02a0070000000000000000000000000000000000
             000000a6000000ab0000000000000000007c02a008000000000000000000
             0000000000000000000000a6000000ab000000000000000000ac02a60200
             00ab0200000000000000007d037c036302640064006400a6020000ab0200
             000000000000000100530023003100730477027803590077010100590001
             00010064005300
-         211           0 RESUME                   0
+         216           0 RESUME                   0
          
-         212           2 LOAD_GLOBAL              0 (db)
+         217           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         213          54 LOAD_CONST               1 ("\n        WITH ranked_actors AS (\n            SELECT \n                a.name,\n                s.uid AS search_uid,\n                COUNT(e.id) AS total_validate_count,\n                ROW_NUMBER() OVER (\n                    PARTITION BY s.uid\n                    ORDER BY COUNT(e.id) DESC\n                ) as rn\n            FROM \n                event e\n            INNER JOIN \n                actor a ON a.key = e.actor_key\n            INNER JOIN \n                search s ON s.uid = e.search_uid\n            WHERE\n                a.type = 'research' AND \n                e.type = 'validate' \n            GROUP BY \n                a.name, s.uid\n        )\n        SELECT \n            name, \n            search_uid, \n            total_validate_count\n        FROM \n            ranked_actors\n        WHERE \n            rn = 1;\n        ")
+         218          54 LOAD_CONST               1 ("\n        WITH ranked_actors AS (\n            SELECT \n                a.name,\n                s.uid AS search_uid,\n                COUNT(e.id) AS total_validate_count,\n                ROW_NUMBER() OVER (\n                    PARTITION BY s.uid\n                    ORDER BY COUNT(e.id) DESC\n                ) as rn\n            FROM \n                event e\n            INNER JOIN \n                actor a ON a.key = e.actor_key\n            INNER JOIN \n                search s ON s.uid = e.search_uid\n            WHERE\n                a.type = 'research' AND \n                e.type = 'validate' \n            GROUP BY \n                a.name, s.uid\n        )\n        SELECT \n            name, \n            search_uid, \n            total_validate_count\n        FROM \n            ranked_actors\n        WHERE \n            rn = 1;\n        ")
                       56 STORE_FAST               1 (statement)
          
-         245          58 LOAD_FAST                0 (conn)
+         250          58 LOAD_FAST                0 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         246         136 LOAD_GLOBAL             11 (NULL + pd)
+         251         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         247         252 LOAD_FAST                3 (df)
+         252         252 LOAD_FAST                3 (df)
          
-         212         254 SWAP                     2
+         217         254 SWAP                     2
                      256 LOAD_CONST               0 (None)
                      258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 PRECALL                  2
                      266 CALL                     2
                      276 POP_TOP
                      278 RETURN_VALUE
@@ -1468,15 +1526,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'top_actor_per_search'
-         firstlineno 211
+         firstlineno 216
          lnotab 0x0201340104204e01740102dd
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
@@ -1491,54 +1549,54 @@
             000000000000007d027c02a0090000000000000000000000000000000000
             000000640364046405ac06a6030000ab030000000000000000a00a000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00a00b00000000000000000000000000000000000000006407a6010000ab
             0100000000000000007d027c026302640064006400a6020000ab02000000
             000000000001005300230031007304770278035900770101005900010001
             0064005300
-         249           0 RESUME                   0
+         254           0 RESUME                   0
          
-         250           2 LOAD_GLOBAL              0 (db)
+         255           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         251          54 LOAD_FAST                0 (conn)
+         256          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         252          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         257          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         253         100 LOAD_CONST               1 ("\n                SELECT search_uid, type, count(DISTINCT domain)\n                FROM event\n                WHERE type in ('create','advance', 'validate', 'send', 'accept')\n                GROUP BY search_uid, type\n                ")
+         258         100 LOAD_CONST               1 ("\n                SELECT search_uid, type, count(DISTINCT domain)\n                FROM event\n                WHERE type in ('create','advance', 'validate', 'send', 'accept')\n                GROUP BY search_uid, type\n                ")
          
-         252         102 PRECALL                  1
+         257         102 PRECALL                  1
                      106 CALL                     1
          
-         251         116 PRECALL                  1
+         256         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         261         132 LOAD_GLOBAL             11 (NULL + pd)
+         266         132 LOAD_GLOBAL             11 (NULL + pd)
                      144 LOAD_ATTR                6 (DataFrame)
                      154 LOAD_FAST                1 (result)
                      156 LOAD_METHOD              7 (fetchall)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 LOAD_FAST                1 (result)
                      194 LOAD_METHOD              8 (keys)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 KW_NAMES                 2
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_FAST               2 (df)
          
-         262         248 LOAD_FAST                2 (df)
+         267         248 LOAD_FAST                2 (df)
                      250 LOAD_METHOD              9 (pivot)
                      272 LOAD_CONST               3 ('search_uid')
                      274 LOAD_CONST               4 ('type')
                      276 LOAD_CONST               5 ('count')
                      278 KW_NAMES                 6
                      280 PRECALL                  3
                      284 CALL                     3
@@ -1547,17 +1605,17 @@
                      320 CALL                     0
                      330 LOAD_METHOD             11 (fillna)
                      352 LOAD_CONST               7 (0)
                      354 PRECALL                  1
                      358 CALL                     1
                      368 STORE_FAST               2 (df)
          
-         263         370 LOAD_FAST                2 (df)
+         268         370 LOAD_FAST                2 (df)
          
-         250         372 SWAP                     2
+         255         372 SWAP                     2
                      374 LOAD_CONST               0 (None)
                      376 LOAD_CONST               0 (None)
                      378 LOAD_CONST               0 (None)
                      380 PRECALL                  2
                      384 CALL                     2
                      394 POP_TOP
                      396 RETURN_VALUE
@@ -1589,15 +1647,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'pivot', 'reset_index', 'fillna')
          varnames   ('conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_event_count_by_type'
-         firstlineno 249
+         firstlineno 254
          lnotab 0x020134011801160102ff0eff100a74017a0102f3
       code
          argcount  : 0
          nlocals   : 5
          stacksize : 7
          flags     : 3
          code
@@ -1618,119 +1676,119 @@
             00a6000000ab000000000000000000640364046405ac06a6040000ab0400
             000000000000007d037c03a00d0000000000000000000000000000000000
             0000006700640ba2016700640ca201ac0da6020000ab0200000000000000
             007d037c03a00e0000000000000000000000000000000000000000640ea6
             010000ab0100000000000000007d03640064006400a6020000ab02000000
             000000000001006e0b230031007304770278035900770101005900010001
             007c035300
-         265           0 RESUME                   0
+         270           0 RESUME                   0
          
-         266           2 LOAD_GLOBAL              0 (db)
+         271           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         267          54 LOAD_CONST               1 ("\n        SELECT \n            s.uid,\n            s.label,\n            (SELECT COUNT(*) \n            FROM event e\n            WHERE \n            e.search_uid = s.uid AND e.created >= EXTRACT(EPOCH FROM (NOW() - INTERVAL '7 days')) and type = 'validate'\n            ) AS recent_validate_count\n        FROM \n            search s;\n        ")
+         272          54 LOAD_CONST               1 ("\n        SELECT \n            s.uid,\n            s.label,\n            (SELECT COUNT(*) \n            FROM event e\n            WHERE \n            e.search_uid = s.uid AND e.created >= EXTRACT(EPOCH FROM (NOW() - INTERVAL '7 days')) and type = 'validate'\n            ) AS recent_validate_count\n        FROM \n            search s;\n        ")
                       56 STORE_FAST               1 (statement)
          
-         279          58 LOAD_FAST                0 (conn)
+         284          58 LOAD_FAST                0 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         280         136 LOAD_GLOBAL             11 (NULL + pd)
+         285         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         282         252 LOAD_FAST                3 (df)
+         287         252 LOAD_FAST                3 (df)
                      254 LOAD_METHOD              9 (merge)
          
-         283         276 LOAD_GLOBAL             21 (NULL + top_actor_per_search)
+         288         276 LOAD_GLOBAL             21 (NULL + top_actor_per_search)
                      288 PRECALL                  0
                      292 CALL                     0
                      302 LOAD_CONST               3 ('uid')
                      304 LOAD_CONST               4 ('search_uid')
                      306 LOAD_CONST               5 ('left')
          
-         282         308 KW_NAMES                 6
+         287         308 KW_NAMES                 6
                      310 PRECALL                  4
                      314 CALL                     4
                      324 STORE_FAST               3 (df)
          
-         286         326 LOAD_CONST               7 (<code object _set_group, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 286>)
+         291         326 LOAD_CONST               7 (<code object _set_group, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 291>)
                      328 MAKE_FUNCTION            0
                      330 STORE_FAST               4 (_set_group)
          
-         294         332 LOAD_FAST                3 (df)
+         299         332 LOAD_FAST                3 (df)
                      334 LOAD_METHOD             11 (apply)
                      356 LOAD_FAST                4 (_set_group)
                      358 LOAD_CONST               8 (1)
                      360 KW_NAMES                 9
                      362 PRECALL                  2
                      366 CALL                     2
                      376 LOAD_FAST                3 (df)
                      378 LOAD_CONST              10 ('group')
                      380 STORE_SUBSCR
          
-         296         384 LOAD_FAST                3 (df)
+         301         384 LOAD_FAST                3 (df)
                      386 LOAD_METHOD              9 (merge)
                      408 LOAD_GLOBAL             25 (NULL + search_event_count_by_type)
                      420 PRECALL                  0
                      424 CALL                     0
                      434 LOAD_CONST               3 ('uid')
                      436 LOAD_CONST               4 ('search_uid')
                      438 LOAD_CONST               5 ('left')
                      440 KW_NAMES                 6
                      442 PRECALL                  4
                      446 CALL                     4
                      456 STORE_FAST               3 (df)
          
-         298         458 LOAD_FAST                3 (df)
+         303         458 LOAD_FAST                3 (df)
                      460 LOAD_METHOD             13 (sort_values)
          
-         299         482 BUILD_LIST               0
+         304         482 BUILD_LIST               0
                      484 LOAD_CONST              11 (('group', 'recent_validate_count', 'total_validate_count', 'label'))
                      486 LIST_EXTEND              1
          
-         300         488 BUILD_LIST               0
+         305         488 BUILD_LIST               0
                      490 LOAD_CONST              12 ((False, False, False, True))
                      492 LIST_EXTEND              1
          
-         298         494 KW_NAMES                13
+         303         494 KW_NAMES                13
                      496 PRECALL                  2
                      500 CALL                     2
                      510 STORE_FAST               3 (df)
          
-         303         512 LOAD_FAST                3 (df)
+         308         512 LOAD_FAST                3 (df)
                      514 LOAD_METHOD             14 (fillna)
                      536 LOAD_CONST              14 ('')
                      538 PRECALL                  1
                      542 CALL                     1
                      552 STORE_FAST               3 (df)
          
-         266         554 LOAD_CONST               0 (None)
+         271         554 LOAD_CONST               0 (None)
                      556 LOAD_CONST               0 (None)
                      558 LOAD_CONST               0 (None)
                      560 PRECALL                  2
                      564 CALL                     2
                      574 POP_TOP
                      576 JUMP_FORWARD            11 (to 600)
                  >>  578 PUSH_EXC_INFO
@@ -1741,15 +1799,15 @@
                      588 POP_EXCEPT
                      590 RERAISE                  1
                  >>  592 POP_TOP
                      594 POP_EXCEPT
                      596 POP_TOP
                      598 POP_TOP
          
-         305     >>  600 LOAD_FAST                3 (df)
+         310     >>  600 LOAD_FAST                3 (df)
                      602 RETURN_VALUE
          ExceptionTable:
            52 to 552 -> 578 [1] lasti
            578 to 584 -> 586 [3] lasti
            592 to 592 -> 586 [3] lasti
          consts
             None
@@ -1764,37 +1822,37 @@
                nlocals   : 1
                stacksize : 2
                flags     : 19
                code
                   0x97007c0064011900000000000000000064026b04000000007202640353
                   007c0064041900000000000000000064056b040000000072026406530064
                   075300
-               286           0 RESUME                   0
+               291           0 RESUME                   0
                
-               287           2 LOAD_FAST                0 (row)
+               292           2 LOAD_FAST                0 (row)
                              4 LOAD_CONST               1 ('recent_validate_count')
                              6 BINARY_SUBSCR
                             16 LOAD_CONST               2 (0)
                             18 COMPARE_OP               4 (>)
                             24 POP_JUMP_FORWARD_IF_FALSE     2 (to 30)
                
-               288          26 LOAD_CONST               3 ('Trending Searches')
+               293          26 LOAD_CONST               3 ('Trending Searches')
                             28 RETURN_VALUE
                
-               289     >>   30 LOAD_FAST                0 (row)
+               294     >>   30 LOAD_FAST                0 (row)
                             32 LOAD_CONST               4 ('total_validate_count')
                             34 BINARY_SUBSCR
                             44 LOAD_CONST               5 (25)
                             46 COMPARE_OP               4 (>)
                             52 POP_JUMP_FORWARD_IF_FALSE     2 (to 58)
                
-               290          54 LOAD_CONST               6 ('Top Searches')
+               295          54 LOAD_CONST               6 ('Top Searches')
                             56 RETURN_VALUE
                
-               292     >>   58 LOAD_CONST               7 ('All Searches')
+               297     >>   58 LOAD_CONST               7 ('All Searches')
                             60 RETURN_VALUE
                consts
                   None
                   'recent_validate_count'
                   0
                   'Trending Searches'
                   'total_validate_count'
@@ -1803,30 +1861,30 @@
                   'All Searches'
                names      ()
                varnames   ('row',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '_set_group'
-               firstlineno 286
+               firstlineno 291
                lnotab 0x02011801040118010402
             1
             ('axis',)
             'group'
             ('group', 'recent_validate_count', 'total_validate_count', 'label')
             (False, False, False, True)
             ('by', 'ascending')
             ''
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'merge', 'top_actor_per_search', 'apply', 'search_event_count_by_type', 'sort_values', 'fillna')
          varnames   ('conn', 'statement', 'result', 'df', '_set_group')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search'
-         firstlineno 265
+         firstlineno 270
          lnotab
             0x02013401040c4e017402180120ff1204060834024a021801060106fe12
             052adb2e27
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
@@ -1840,66 +1898,66 @@
             00000000007c01a0070000000000000000000000000000000000000000a6
             000000ab0000000000000000007c01a00800000000000000000000000000
             00000000000000a6000000ab000000000000000000ac02a6020000ab0200
             000000000000007d027c02a0090000000000000000000000000000000000
             00000067006403a201ac02a6010000ab0100000000000000007d027c0263
             02640064006400a6020000ab020000000000000000010053002300310073
             047702780359007701010059000100010064005300
-         307           0 RESUME                   0
+         312           0 RESUME                   0
          
-         308           2 LOAD_GLOBAL              0 (db)
+         313           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         309          54 LOAD_FAST                0 (conn)
+         314          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         310          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         315          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         311         100 LOAD_CONST               1 ('\n                SELECT * FROM actor\n                ')
+         316         100 LOAD_CONST               1 ('\n                SELECT * FROM actor\n                ')
          
-         310         102 PRECALL                  1
+         315         102 PRECALL                  1
                      106 CALL                     1
          
-         309         116 PRECALL                  1
+         314         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         316         132 LOAD_GLOBAL             11 (NULL + pd)
+         321         132 LOAD_GLOBAL             11 (NULL + pd)
                      144 LOAD_ATTR                6 (DataFrame)
                      154 LOAD_FAST                1 (result)
                      156 LOAD_METHOD              7 (fetchall)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 LOAD_FAST                1 (result)
                      194 LOAD_METHOD              8 (keys)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 KW_NAMES                 2
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_FAST               2 (df)
          
-         317         248 LOAD_FAST                2 (df)
+         322         248 LOAD_FAST                2 (df)
                      250 LOAD_METHOD              9 (drop)
                      272 BUILD_LIST               0
                      274 LOAD_CONST               3 (('id', 'created', 'updated'))
                      276 LIST_EXTEND              1
                      278 KW_NAMES                 2
                      280 PRECALL                  1
                      284 CALL                     1
                      294 STORE_FAST               2 (df)
          
-         318         296 LOAD_FAST                2 (df)
+         323         296 LOAD_FAST                2 (df)
          
-         308         298 SWAP                     2
+         313         298 SWAP                     2
                      300 LOAD_CONST               0 (None)
                      302 LOAD_CONST               0 (None)
                      304 LOAD_CONST               0 (None)
                      306 PRECALL                  2
                      310 CALL                     2
                      320 POP_TOP
                      322 RETURN_VALUE
@@ -1927,15 +1985,15 @@
             ('id', 'created', 'updated')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'drop')
          varnames   ('conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'actor'
-         firstlineno 307
+         firstlineno 312
          lnotab 0x020134011801160102ff0eff10077401300102f6
       code
          argcount  : 2
          nlocals   : 8
          stacksize : 7
          flags     : 3
          code
@@ -1958,60 +2016,60 @@
             00000000000000a00e000000000000000000000000000000000000000064
             086405a6020000ab0200000000000000007c076a0d0000000000000000a0
             0e00000000000000000000000000000000000000006409a6010000ab0100
             00000000000000640a6b0200000000ac0ba6020000ab0200000000000000
             007d05740b000000000000000000006a0f00000000000000007c05640c19
             000000000000000000a6010000ab0100000000000000007c05640c3c0000
             007c055300
-         321           0 RESUME                   0
+         326           0 RESUME                   0
          
-         322           2 LOAD_CONST               1 ("\n        SELECT \n            e.id, \n            e.search_uid, \n            e.domain, \n            e.data, \n            e.type AS last_event_type, \n            e.created AS updated,\n            a.name AS updated_by,\n            c.name as name,\n            c.uid as dealcloud_id,\n            c.description as description,\n            c.meta as meta,\n            (c.meta->>'employees') AS employees,\n            (c.meta->>'ownership') AS ownership,\n            (c.meta->>'linkedin') AS linkedin,\n            (r.data->>'rating') AS rating\n        FROM (\n            SELECT \n                search_uid, \n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type NOT IN ('comment','rating','generate','criteria')\n                AND search_uid = :search_uid\n            GROUP BY \n                domain, search_uid\n        ) AS max_event\n        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid \n        JOIN company c ON c.domain = e.domain\n        JOIN actor a ON a.key = e.actor_key\n        LEFT JOIN (\n            SELECT \n                search_uid,\n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type = 'rating'\n            GROUP BY \n                domain, search_uid\n        ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid\n        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;\n    ")
+         327           2 LOAD_CONST               1 ("\n        SELECT \n            e.id, \n            e.search_uid, \n            e.domain, \n            e.data, \n            e.type AS last_event_type, \n            e.created AS updated,\n            a.name AS updated_by,\n            c.name as name,\n            c.uid as dealcloud_id,\n            c.description as description,\n            (c.meta->>'year_founded') AS year_founded,\n            (c.meta->>'employees') AS employees,\n            (c.meta->>'headquarters') AS headquarters,\n            (c.meta->>'ownership') AS ownership,\n            (c.meta->>'linkedin') AS linkedin,\n            (r.data->>'rating') AS rating,\n            c.meta as meta\n        FROM (\n            SELECT \n                search_uid, \n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type NOT IN ('comment','rating','generate','criteria')\n                AND search_uid = :search_uid\n            GROUP BY \n                domain, search_uid\n        ) AS max_event\n        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid \n        JOIN company c ON c.domain = e.domain\n        JOIN actor a ON a.key = e.actor_key\n        LEFT JOIN (\n            SELECT \n                search_uid,\n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type = 'rating'\n            GROUP BY \n                domain, search_uid\n        ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid\n        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;\n    ")
                        4 STORE_FAST               2 (statement)
          
-         369           6 LOAD_GLOBAL              0 (db)
+         376           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               3 (conn)
          
-         370          58 LOAD_FAST                3 (conn)
+         377          58 LOAD_FAST                3 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         371          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         378          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         372         120 LOAD_FAST                0 (search_uid)
+         379         120 LOAD_FAST                0 (search_uid)
                      122 LOAD_FAST                1 (last_event_type)
                      124 LOAD_CONST               2 (('search_uid', 'last_event_type'))
                      126 BUILD_CONST_KEY_MAP      2
          
-         370         128 PRECALL                  2
+         377         128 PRECALL                  2
                      132 CALL                     2
                      142 STORE_FAST               4 (result)
          
-         374         144 LOAD_GLOBAL             11 (NULL + pd)
+         381         144 LOAD_GLOBAL             11 (NULL + pd)
                      156 LOAD_ATTR                6 (DataFrame)
                      166 LOAD_FAST                4 (result)
                      168 LOAD_METHOD              7 (fetchall)
                      190 PRECALL                  0
                      194 CALL                     0
                      204 LOAD_FAST                4 (result)
                      206 LOAD_METHOD              8 (keys)
                      228 PRECALL                  0
                      232 CALL                     0
                      242 KW_NAMES                 3
                      244 PRECALL                  2
                      248 CALL                     2
                      258 STORE_FAST               5 (targets)
          
-         369         260 LOAD_CONST               0 (None)
+         376         260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 LOAD_CONST               0 (None)
                      266 PRECALL                  2
                      270 CALL                     2
                      280 POP_TOP
                      282 JUMP_FORWARD            11 (to 306)
                  >>  284 PUSH_EXC_INFO
@@ -2022,90 +2080,90 @@
                      294 POP_EXCEPT
                      296 RERAISE                  1
                  >>  298 POP_TOP
                      300 POP_EXCEPT
                      302 POP_TOP
                      304 POP_TOP
          
-         376     >>  306 LOAD_FAST                5 (targets)
+         383     >>  306 LOAD_FAST                5 (targets)
                      308 LOAD_FAST                5 (targets)
                      310 LOAD_CONST               4 ('last_event_type')
                      312 BINARY_SUBSCR
                      322 LOAD_FAST                1 (last_event_type)
                      324 COMPARE_OP               2 (==)
                      330 BINARY_SUBSCR
                      340 STORE_FAST               5 (targets)
          
-         377         342 LOAD_GLOBAL             19 (NULL + comment_by_domain)
+         384         342 LOAD_GLOBAL             19 (NULL + comment_by_domain)
                      354 LOAD_FAST                0 (search_uid)
                      356 PRECALL                  1
                      360 CALL                     1
                      370 STORE_FAST               6 (comments)
          
-         378         372 LOAD_FAST                5 (targets)
+         385         372 LOAD_FAST                5 (targets)
                      374 LOAD_METHOD             10 (merge)
                      396 LOAD_FAST                6 (comments)
                      398 LOAD_CONST               5 ('domain')
                      400 LOAD_CONST               6 ('left')
                      402 KW_NAMES                 7
                      404 PRECALL                  3
                      408 CALL                     3
                      418 STORE_FAST               5 (targets)
          
-         381         420 LOAD_GLOBAL             23 (NULL + find_search_by_uid)
+         388         420 LOAD_GLOBAL             23 (NULL + find_search_by_uid)
                      432 LOAD_FAST                0 (search_uid)
                      434 PRECALL                  1
                      438 CALL                     1
                      448 STORE_FAST               7 (search)
          
-         382         450 LOAD_FAST                5 (targets)
+         389         450 LOAD_FAST                5 (targets)
                      452 LOAD_METHOD             12 (sort_values)
          
-         383         474 LOAD_FAST                7 (search)
+         390         474 LOAD_FAST                7 (search)
                      476 LOAD_ATTR               13 (sort)
                      486 LOAD_METHOD             14 (get)
                      508 LOAD_CONST               8 ('field')
                      510 LOAD_CONST               5 ('domain')
                      512 PRECALL                  2
                      516 CALL                     2
          
-         384         526 LOAD_FAST                7 (search)
+         391         526 LOAD_FAST                7 (search)
                      528 LOAD_ATTR               13 (sort)
                      538 LOAD_METHOD             14 (get)
                      560 LOAD_CONST               9 ('order')
                      562 PRECALL                  1
                      566 CALL                     1
                      576 LOAD_CONST              10 ('asc')
                      578 COMPARE_OP               2 (==)
          
-         382         584 KW_NAMES                11
+         389         584 KW_NAMES                11
                      586 PRECALL                  2
                      590 CALL                     2
                      600 STORE_FAST               5 (targets)
          
-         386         602 LOAD_GLOBAL             11 (NULL + pd)
+         393         602 LOAD_GLOBAL             11 (NULL + pd)
                      614 LOAD_ATTR               15 (to_numeric)
                      624 LOAD_FAST                5 (targets)
                      626 LOAD_CONST              12 ('employees')
                      628 BINARY_SUBSCR
                      638 PRECALL                  1
                      642 CALL                     1
                      652 LOAD_FAST                5 (targets)
                      654 LOAD_CONST              12 ('employees')
                      656 STORE_SUBSCR
          
-         387         660 LOAD_FAST                5 (targets)
+         394         660 LOAD_FAST                5 (targets)
                      662 RETURN_VALUE
          ExceptionTable:
            56 to 258 -> 284 [1] lasti
            284 to 290 -> 292 [3] lasti
            298 to 298 -> 292 [3] lasti
          consts
             None
-            "\n        SELECT \n            e.id, \n            e.search_uid, \n            e.domain, \n            e.data, \n            e.type AS last_event_type, \n            e.created AS updated,\n            a.name AS updated_by,\n            c.name as name,\n            c.uid as dealcloud_id,\n            c.description as description,\n            c.meta as meta,\n            (c.meta->>'employees') AS employees,\n            (c.meta->>'ownership') AS ownership,\n            (c.meta->>'linkedin') AS linkedin,\n            (r.data->>'rating') AS rating\n        FROM (\n            SELECT \n                search_uid, \n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type NOT IN ('comment','rating','generate','criteria')\n                AND search_uid = :search_uid\n            GROUP BY \n                domain, search_uid\n        ) AS max_event\n        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid \n        JOIN company c ON c.domain = e.domain\n        JOIN actor a ON a.key = e.actor_key\n        LEFT JOIN (\n            SELECT \n                search_uid,\n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type = 'rating'\n            GROUP BY \n                domain, search_uid\n        ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid\n        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;\n    "
+            "\n        SELECT \n            e.id, \n            e.search_uid, \n            e.domain, \n            e.data, \n            e.type AS last_event_type, \n            e.created AS updated,\n            a.name AS updated_by,\n            c.name as name,\n            c.uid as dealcloud_id,\n            c.description as description,\n            (c.meta->>'year_founded') AS year_founded,\n            (c.meta->>'employees') AS employees,\n            (c.meta->>'headquarters') AS headquarters,\n            (c.meta->>'ownership') AS ownership,\n            (c.meta->>'linkedin') AS linkedin,\n            (r.data->>'rating') AS rating,\n            c.meta as meta\n        FROM (\n            SELECT \n                search_uid, \n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type NOT IN ('comment','rating','generate','criteria')\n                AND search_uid = :search_uid\n            GROUP BY \n                domain, search_uid\n        ) AS max_event\n        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid \n        JOIN company c ON c.domain = e.domain\n        JOIN actor a ON a.key = e.actor_key\n        LEFT JOIN (\n            SELECT \n                search_uid,\n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type = 'rating'\n            GROUP BY \n                domain, search_uid\n        ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid\n        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;\n    "
             ('search_uid', 'last_event_type')
             ('columns',)
             'last_event_type'
             'domain'
             'left'
             ('on', 'how')
             'field'
@@ -2115,180 +2173,80 @@
             'employees'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'comment_by_domain', 'merge', 'find_search_by_uid', 'sort_values', 'sort', 'get', 'to_numeric')
          varnames   ('search_uid', 'last_event_type', 'statement', 'conn', 'result', 'targets', 'comments', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_target_by_last_event_type'
-         firstlineno 321
+         firstlineno 326
          lnotab
-            0x0201042f34011801260108fe100474fb2e0724011e0130031e01180134
+            0x0201043134011801260108fe100474fb2e0724011e0130031e01180134
             013afe12043a01
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
-            0x970064017d01740000000000000000000000a001000000000000000000
-            0000000000000000000000a6000000ab00000000000000000035007d027c
-            02a002000000000000000000000000000000000000000074070000000000
-            00000000006a0400000000000000007c01a6010000ab0100000000000000
-            0064027c006901a6020000ab0200000000000000007d03740b0000000000
-            00000000006a0600000000000000007c03a0070000000000000000000000
-            000000000000000000a6000000ab0000000000000000007c03a008000000
-            0000000000000000000000000000000000a6000000ab0000000000000000
-            00ac03a6020000ab0200000000000000007d04640464046404a6020000ab
-            02000000000000000001006e0b2300310073047702780359007701010059
-            00010001007c045300
-         390           0 RESUME                   0
-         
-         393           2 LOAD_CONST               1 ("\n        SELECT \n            e.id, \n            e.search_uid, \n            e.domain, \n            e.type AS last_event_type, \n            to_timestamp(e.created) AS updated,\n            c.meta as meta,\n            (r.data->>'rating') AS rating\n        FROM (\n            SELECT \n                search_uid, \n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type NOT IN ('comment','rating','generate','criteria') \n                AND search_uid = :search_uid\n            GROUP BY \n                domain, search_uid\n        ) AS max_event\n        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid \n        JOIN company c ON c.domain = e.domain\n        LEFT JOIN (\n            SELECT \n                search_uid,\n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type = 'rating'\n            GROUP BY \n                domain, search_uid\n        ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid\n        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;\n    ")
-                       4 STORE_FAST               1 (statement)
-         
-         431           6 LOAD_GLOBAL              0 (db)
-                      18 LOAD_METHOD              1 (connect)
-                      40 PRECALL                  0
-                      44 CALL                     0
-                      54 BEFORE_WITH
-                      56 STORE_FAST               2 (conn)
-         
-         432          58 LOAD_FAST                2 (conn)
-                      60 LOAD_METHOD              2 (execute)
-         
-         433          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
-                      94 LOAD_ATTR                4 (text)
-                     104 LOAD_FAST                1 (statement)
-                     106 PRECALL                  1
-                     110 CALL                     1
-         
-         434         120 LOAD_CONST               2 ('search_uid')
-                     122 LOAD_FAST                0 (search_uid)
-                     124 BUILD_MAP                1
-         
-         432         126 PRECALL                  2
-                     130 CALL                     2
-                     140 STORE_FAST               3 (result)
-         
-         436         142 LOAD_GLOBAL             11 (NULL + pd)
-                     154 LOAD_ATTR                6 (DataFrame)
-                     164 LOAD_FAST                3 (result)
-                     166 LOAD_METHOD              7 (fetchall)
-                     188 PRECALL                  0
-                     192 CALL                     0
-                     202 LOAD_FAST                3 (result)
-                     204 LOAD_METHOD              8 (keys)
-                     226 PRECALL                  0
-                     230 CALL                     0
-                     240 KW_NAMES                 3
-                     242 PRECALL                  2
-                     246 CALL                     2
-                     256 STORE_FAST               4 (targets)
-         
-         431         258 LOAD_CONST               4 (None)
-                     260 LOAD_CONST               4 (None)
-                     262 LOAD_CONST               4 (None)
-                     264 PRECALL                  2
-                     268 CALL                     2
-                     278 POP_TOP
-                     280 JUMP_FORWARD            11 (to 304)
-                 >>  282 PUSH_EXC_INFO
-                     284 WITH_EXCEPT_START
-                     286 POP_JUMP_FORWARD_IF_TRUE     4 (to 296)
-                     288 RERAISE                  2
-                 >>  290 COPY                     3
-                     292 POP_EXCEPT
-                     294 RERAISE                  1
-                 >>  296 POP_TOP
-                     298 POP_EXCEPT
-                     300 POP_TOP
-                     302 POP_TOP
-         
-         445     >>  304 LOAD_FAST                4 (targets)
-                     306 RETURN_VALUE
-         ExceptionTable:
-           56 to 256 -> 282 [1] lasti
-           282 to 288 -> 290 [3] lasti
-           296 to 296 -> 290 [3] lasti
-         consts
-            'Returns all the targets not in rejected or created'
-            "\n        SELECT \n            e.id, \n            e.search_uid, \n            e.domain, \n            e.type AS last_event_type, \n            to_timestamp(e.created) AS updated,\n            c.meta as meta,\n            (r.data->>'rating') AS rating\n        FROM (\n            SELECT \n                search_uid, \n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type NOT IN ('comment','rating','generate','criteria') \n                AND search_uid = :search_uid\n            GROUP BY \n                domain, search_uid\n        ) AS max_event\n        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid \n        JOIN company c ON c.domain = e.domain\n        LEFT JOIN (\n            SELECT \n                search_uid,\n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type = 'rating'\n            GROUP BY \n                domain, search_uid\n        ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid\n        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;\n    "
-            'search_uid'
-            ('columns',)
-            None
-         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
-         varnames   ('search_uid', 'statement', 'conn', 'result', 'targets')
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
-         name       'search_target_export'
-         firstlineno 390
-         lnotab 0x0203042634011801260106fe100474fb2e0e
-      code
-         argcount  : 1
-         nlocals   : 5
-         stacksize : 6
-         flags     : 3
-         code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d0164017d027c
             01a002000000000000000000000000000000000000000074070000000000
             00000000006a0400000000000000007c02a6010000ab0100000000000000
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         449           0 RESUME                   0
+         456           0 RESUME                   0
          
-         450           2 LOAD_GLOBAL              0 (db)
+         457           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         451          54 LOAD_CONST               1 ("\n            SELECT \n                e.type AS last_event_type,\n                COUNT(e.type)\n            FROM (\n                SELECT \n                    search_uid, \n                    domain, \n                    MAX(created) AS max_created\n                FROM \n                    event\n                WHERE \n                    type NOT IN ('comment','rating','generate','criteria')\n                    and search_uid = :search_uid\n                GROUP BY \n                    domain, search_uid\n            ) AS max_event\n            JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid\n            GROUP BY e.type;\n        ")
+         458          54 LOAD_CONST               1 ("\n            SELECT \n                e.type AS last_event_type,\n                COUNT(e.type)\n            FROM (\n                SELECT \n                    search_uid, \n                    domain, \n                    MAX(created) AS max_created\n                FROM \n                    event\n                WHERE \n                    type NOT IN ('comment','rating','generate','criteria')\n                    and search_uid = :search_uid\n                GROUP BY \n                    domain, search_uid\n            ) AS max_event\n            JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid\n            GROUP BY e.type;\n        ")
                       56 STORE_FAST               2 (statement)
          
-         471          58 LOAD_FAST                1 (conn)
+         478          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         472          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         479          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         473         120 LOAD_CONST               2 ('search_uid')
+         480         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         471         126 PRECALL                  2
+         478         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         475         142 LOAD_GLOBAL             11 (NULL + pd)
+         482         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         450         258 LOAD_CONST               0 (None)
+         457         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2299,15 +2257,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         476     >>  304 LOAD_FAST                4 (df)
+         483     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -2316,15 +2274,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'target_count'
-         firstlineno 449
+         firstlineno 456
          lnotab 0x0201340104141801260106fe100474e72e1a
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -2335,56 +2293,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         479           0 RESUME                   0
+         486           0 RESUME                   0
          
-         480           2 LOAD_GLOBAL              0 (db)
+         487           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         481          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         488          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         486          58 LOAD_FAST                1 (conn)
+         493          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         487         142 LOAD_GLOBAL             11 (NULL + pd)
+         494         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         480         258 LOAD_CONST               0 (None)
+         487         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2395,15 +2353,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         488     >>  304 LOAD_FAST                4 (df)
+         495     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -2412,15 +2370,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event'
-         firstlineno 479
+         firstlineno 486
          lnotab 0x020134010405540174f92e08
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -2431,56 +2389,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         491           0 RESUME                   0
+         498           0 RESUME                   0
          
-         492           2 LOAD_GLOBAL              0 (db)
+         499           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         493          54 LOAD_CONST               1 ('\n                SELECT distinct(domain)\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         500          54 LOAD_CONST               1 ('\n                SELECT distinct(domain)\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         498          58 LOAD_FAST                1 (conn)
+         505          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         499         142 LOAD_GLOBAL             11 (NULL + pd)
+         506         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         492         258 LOAD_CONST               0 (None)
+         499         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2491,15 +2449,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         500     >>  304 LOAD_FAST                4 (df)
+         507     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -2508,15 +2466,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'unique_domains'
-         firstlineno 491
+         firstlineno 498
          lnotab 0x020134010405540174f92e08
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -2527,53 +2485,53 @@
             00a6010000ab0100000000000000007d02740b000000000000000000006a
             0600000000000000007c02a0070000000000000000000000000000000000
             000000a6000000ab0000000000000000007c02a008000000000000000000
             0000000000000000000000a6000000ab000000000000000000ac02a60200
             00ab0200000000000000007d03640064006400a6020000ab020000000000
             00000001006e0b230031007304770278035900770101005900010001007c
             035300
-         503           0 RESUME                   0
+         510           0 RESUME                   0
          
-         504           2 LOAD_GLOBAL              0 (db)
+         511           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         505          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n            ')
+         512          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n            ')
                       56 STORE_FAST               1 (statement)
          
-         509          58 LOAD_FAST                0 (conn)
+         516          58 LOAD_FAST                0 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         510         136 LOAD_GLOBAL             11 (NULL + pd)
+         517         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         504         252 LOAD_CONST               0 (None)
+         511         252 LOAD_CONST               0 (None)
                      254 LOAD_CONST               0 (None)
                      256 LOAD_CONST               0 (None)
                      258 PRECALL                  2
                      262 CALL                     2
                      272 POP_TOP
                      274 JUMP_FORWARD            11 (to 298)
                  >>  276 PUSH_EXC_INFO
@@ -2584,15 +2542,15 @@
                      286 POP_EXCEPT
                      288 RERAISE                  1
                  >>  290 POP_TOP
                      292 POP_EXCEPT
                      294 POP_TOP
                      296 POP_TOP
          
-         511     >>  298 LOAD_FAST                3 (df)
+         518     >>  298 LOAD_FAST                3 (df)
                      300 RETURN_VALUE
          ExceptionTable:
            52 to 250 -> 276 [1] lasti
            276 to 282 -> 284 [3] lasti
            290 to 290 -> 284 [3] lasti
          consts
             None
@@ -2600,15 +2558,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'company'
-         firstlineno 503
+         firstlineno 510
          lnotab 0x0201340104044e0174fa2e07
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -2619,56 +2577,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         514           0 RESUME                   0
+         521           0 RESUME                   0
          
-         515           2 LOAD_GLOBAL              0 (db)
+         522           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         516          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n                JOIN event ON checkpoint.event_id = event.id\n                WHERE search_uid = :search_uid\n            ')
+         523          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n                JOIN event ON checkpoint.event_id = event.id\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         522          58 LOAD_FAST                1 (conn)
+         529          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         523         142 LOAD_GLOBAL             11 (NULL + pd)
+         530         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         515         258 LOAD_CONST               0 (None)
+         522         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2679,15 +2637,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         524     >>  304 LOAD_FAST                4 (df)
+         531     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -2696,15 +2654,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'checkpoint'
-         firstlineno 514
+         firstlineno 521
          lnotab 0x020134010406540174f82e09
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -2719,59 +2677,59 @@
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c04a009000000000000000000000000000000000000000064
             04a6010000ab010000000000000000a00a00000000000000000000000000
             000000000000006405640684006901a6010000ab010000000000000000a0
             0b0000000000000000000000000000000000000000a6000000ab00000000
             00000000005300
-         527           0 RESUME                   0
+         534           0 RESUME                   0
          
-         528           2 LOAD_GLOBAL              0 (db)
+         535           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         529          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
+         536          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
                       56 STORE_FAST               2 (statement)
          
-         536          58 LOAD_FAST                1 (conn)
+         543          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         537          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         544          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         538         120 LOAD_CONST               2 ('search_uid')
+         545         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         536         126 PRECALL                  2
+         543         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         540         142 LOAD_GLOBAL             11 (NULL + pd)
+         547         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         528         258 LOAD_CONST               0 (None)
+         535         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2782,22 +2740,22 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         542     >>  304 LOAD_FAST                4 (df)
+         549     >>  304 LOAD_FAST                4 (df)
                      306 LOAD_METHOD              9 (groupby)
                      328 LOAD_CONST               4 ('domain')
                      330 PRECALL                  1
                      334 CALL                     1
                      344 LOAD_METHOD             10 (agg)
                      366 LOAD_CONST               5 ('comment')
-                     368 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 542>)
+                     368 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 549>)
                      370 MAKE_FUNCTION            0
                      372 BUILD_MAP                1
                      374 PRECALL                  1
                      378 CALL                     1
                      388 LOAD_METHOD             11 (reset_index)
                      410 PRECALL                  0
                      414 CALL                     0
@@ -2817,37 +2775,37 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 19
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   005300
-               542           0 RESUME                   0
+               549           0 RESUME                   0
                              2 LOAD_GLOBAL              1 (NULL + list)
                             14 LOAD_FAST                0 (x)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RETURN_VALUE
                consts
                   None
                names      ('list',)
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '<lambda>'
-               firstlineno 542
+               firstlineno 549
                lnotab 0x
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'groupby', 'agg', 'reset_index')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'comment_by_domain'
-         firstlineno 527
+         firstlineno 534
          lnotab 0x0201340104071801260106fe100474f42e0e
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -2862,41 +2820,41 @@
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000007d05741900
             0000000000000000007c056a0d0000000000000000a6010000ab01000000
             000000000001007c055300
-         548           0 RESUME                   0
+         555           0 RESUME                   0
          
-         549           2 LOAD_GLOBAL              0 (db)
+         556           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         550          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
+         557          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         555          58 LOAD_FAST                1 (conn)
+         562          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         549         142 LOAD_CONST               0 (None)
+         556         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -2907,24 +2865,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         557     >>  188 LOAD_FAST                3 (result)
+         564     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         558         210 LOAD_CONST               0 (None)
+         565         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         560     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         567     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -2932,29 +2890,29 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         561         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         568         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Search)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 STORE_FAST               5 (search)
          
-         562         386 LOAD_GLOBAL             25 (NULL + print)
+         569         386 LOAD_GLOBAL             25 (NULL + print)
                      398 LOAD_FAST                5 (search)
                      400 LOAD_ATTR               13 (label)
                      410 PRECALL                  1
                      414 CALL                     1
                      424 POP_TOP
          
-         563         426 LOAD_FAST                5 (search)
+         570         426 LOAD_FAST                5 (search)
                      428 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
            166 to 172 -> 174 [3] lasti
            180 to 180 -> 174 [3] lasti
          consts
             None
@@ -2963,15 +2921,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Search', 'print', 'label')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'obj', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_uid'
-         firstlineno 548
+         firstlineno 555
          lnotab 0x02013401040554fa2e081601040282012a012801
       'domain'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -2985,41 +2943,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         566           0 RESUME                   0
+         573           0 RESUME                   0
          
-         567           2 LOAD_GLOBAL              0 (db)
+         574           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         568          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
+         575          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         573          58 LOAD_FAST                1 (conn)
+         580          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('domain')
                      122 LOAD_FAST                0 (domain)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         567         142 LOAD_CONST               0 (None)
+         574         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3030,24 +2988,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         575     >>  188 LOAD_FAST                3 (result)
+         582     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         576         210 LOAD_CONST               0 (None)
+         583         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         578     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         585     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3055,15 +3013,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         579         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         586         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Company)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -3076,15 +3034,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
          varnames   ('domain', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_company_by_domain'
-         firstlineno 566
+         firstlineno 573
          lnotab 0x02013401040554fa2e08160104028201
       'event_id'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3098,41 +3056,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         582           0 RESUME                   0
+         589           0 RESUME                   0
          
-         583           2 LOAD_GLOBAL              0 (db)
+         590           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         584          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
+         591          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         589          58 LOAD_FAST                1 (conn)
+         596          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('event_id')
                      122 LOAD_FAST                0 (event_id)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         583         142 LOAD_CONST               0 (None)
+         590         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3143,24 +3101,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         591     >>  188 LOAD_FAST                3 (result)
+         598     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         592         210 LOAD_CONST               0 (None)
+         599         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         594     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         601     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3168,15 +3126,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         595         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         602         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Event)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -3189,15 +3147,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Event')
          varnames   ('event_id', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_event_by_id'
-         firstlineno 582
+         firstlineno 589
          lnotab 0x02013401040554fa2e08160104028201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 11
          flags     : 3
          code
@@ -3208,68 +3166,68 @@
             007c006a0500000000000000007c006a0600000000000000007c006a0700
             000000000000007c006a0800000000000000007413000000000000000000
             006a0a00000000000000007c006a0b0000000000000000a6010000ab0100
             0000000000000064029c05a6020000ab02000000000000000001007c01a0
             0c0000000000000000000000000000000000000000a6000000ab00000000
             00000000000100640064006400a6020000ab020000000000000000010064
             0053002300310073047702780359007701010059000100010064005300
-         601           0 RESUME                   0
+         608           0 RESUME                   0
          
-         602           2 LOAD_GLOBAL              0 (db)
+         609           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         603          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
+         610          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         614          58 LOAD_FAST                1 (conn)
+         621          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         615          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         622          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         617         120 LOAD_FAST                0 (company)
+         624         120 LOAD_FAST                0 (company)
                      122 LOAD_ATTR                5 (uid)
          
-         618         132 LOAD_FAST                0 (company)
+         625         132 LOAD_FAST                0 (company)
                      134 LOAD_ATTR                6 (name)
          
-         619         144 LOAD_FAST                0 (company)
+         626         144 LOAD_FAST                0 (company)
                      146 LOAD_ATTR                7 (description)
          
-         620         156 LOAD_FAST                0 (company)
+         627         156 LOAD_FAST                0 (company)
                      158 LOAD_ATTR                8 (domain)
          
-         621         168 LOAD_GLOBAL             19 (NULL + json)
+         628         168 LOAD_GLOBAL             19 (NULL + json)
                      180 LOAD_ATTR               10 (dumps)
                      190 LOAD_FAST                0 (company)
                      192 LOAD_ATTR               11 (meta)
                      202 PRECALL                  1
                      206 CALL                     1
          
-         616         216 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'meta'))
+         623         216 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'meta'))
                      218 BUILD_CONST_KEY_MAP      5
          
-         614         220 PRECALL                  2
+         621         220 PRECALL                  2
                      224 CALL                     2
                      234 POP_TOP
          
-         625         236 LOAD_FAST                1 (conn)
+         632         236 LOAD_FAST                1 (conn)
                      238 LOAD_METHOD             12 (commit)
                      260 PRECALL                  0
                      264 CALL                     0
                      274 POP_TOP
          
-         602         276 LOAD_CONST               0 (None)
+         609         276 LOAD_CONST               0 (None)
                      278 LOAD_CONST               0 (None)
                      280 LOAD_CONST               0 (None)
                      282 PRECALL                  2
                      286 CALL                     2
                      296 POP_TOP
                      298 LOAD_CONST               0 (None)
                      300 RETURN_VALUE
@@ -3296,15 +3254,15 @@
             ('uid', 'name', 'description', 'domain', 'meta')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'uid', 'name', 'description', 'domain', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 601
+         firstlineno 608
          lnotab 0x02013401040b180126020c010c010c010c0130fb04fe100b28e9
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 10
          flags     : 3
          code
@@ -3319,79 +3277,79 @@
             00000000000000a6010000ab010000000000000000740b00000000000000
             0000006a0600000000000000007c006a0a0000000000000000a6010000ab
             0100000000000000007c006a0b000000000000000064029c05a6020000ab
             02000000000000000001007c01a00c000000000000000000000000000000
             0000000000a6000000ab0000000000000000000100640064006400a60200
             00ab02000000000000000001006400530023003100730477027803590077
             01010059000100010064005300
-         628           0 RESUME                   0
+         635           0 RESUME                   0
          
-         629           2 LOAD_GLOBAL              0 (db)
+         636           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         630          54 LOAD_FAST                1 (conn)
+         637          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         631          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         638          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         632         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion,\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
+         639         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion,\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
          
-         631         102 PRECALL                  1
+         638         102 PRECALL                  1
                      106 CALL                     1
          
-         644         116 LOAD_GLOBAL             11 (NULL + json)
+         651         116 LOAD_GLOBAL             11 (NULL + json)
                      128 LOAD_ATTR                6 (dumps)
                      138 LOAD_FAST                0 (search)
                      140 LOAD_ATTR                7 (sort)
                      150 PRECALL                  1
                      154 CALL                     1
          
-         645         164 LOAD_GLOBAL             11 (NULL + json)
+         652         164 LOAD_GLOBAL             11 (NULL + json)
                      176 LOAD_ATTR                6 (dumps)
                      186 LOAD_FAST                0 (search)
                      188 LOAD_ATTR                8 (inclusion)
                      198 PRECALL                  1
                      202 CALL                     1
          
-         646         212 LOAD_GLOBAL             11 (NULL + json)
+         653         212 LOAD_GLOBAL             11 (NULL + json)
                      224 LOAD_ATTR                6 (dumps)
                      234 LOAD_FAST                0 (search)
                      236 LOAD_ATTR                9 (exclusion)
                      246 PRECALL                  1
                      250 CALL                     1
          
-         647         260 LOAD_GLOBAL             11 (NULL + json)
+         654         260 LOAD_GLOBAL             11 (NULL + json)
                      272 LOAD_ATTR                6 (dumps)
                      282 LOAD_FAST                0 (search)
                      284 LOAD_ATTR               10 (meta)
                      294 PRECALL                  1
                      298 CALL                     1
          
-         648         308 LOAD_FAST                0 (search)
+         655         308 LOAD_FAST                0 (search)
                      310 LOAD_ATTR               11 (uid)
          
-         643         320 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'meta', 'uid'))
+         650         320 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'meta', 'uid'))
                      322 BUILD_CONST_KEY_MAP      5
          
-         630         324 PRECALL                  2
+         637         324 PRECALL                  2
                      328 CALL                     2
                      338 POP_TOP
          
-         651         340 LOAD_FAST                1 (conn)
+         658         340 LOAD_FAST                1 (conn)
                      342 LOAD_METHOD             12 (commit)
                      364 PRECALL                  0
                      368 CALL                     0
                      378 POP_TOP
          
-         629         380 LOAD_CONST               0 (None)
+         636         380 LOAD_CONST               0 (None)
                      382 LOAD_CONST               0 (None)
                      384 LOAD_CONST               0 (None)
                      386 PRECALL                  2
                      390 CALL                     2
                      400 POP_TOP
                      402 LOAD_CONST               0 (None)
                      404 RETURN_VALUE
@@ -3418,22 +3376,22 @@
             ('sort', 'inclusion', 'exclusion', 'meta', 'uid')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'json', 'dumps', 'sort', 'inclusion', 'exclusion', 'meta', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 628
+         firstlineno 635
          lnotab 0x020134011801160102ff0e0d30013001300130010cfb04f3101528ea
       (None,)
-   names      ('json', 'dataclasses', 'asdict', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'google.cloud.sql.connector', 'Connector', 'gandai', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Checkpoint', 'Company', 'Event', 'EventType', 'Search', 'db', 'insert_company', 'insert_event', 'insert_actor', 'insert_search', 'insert_checkpoint', 'str', 'int', 'insert_targets_from_domains', 'insert_companies_as_targets', 'DataFrame', 'top_actor_per_search', 'search_event_count_by_type', 'search', 'actor', 'search_target_by_last_event_type', 'search_target_export', 'target_count', 'event', 'unique_domains', 'company', 'checkpoint', 'comment_by_domain', 'find_search_by_uid', 'find_company_by_domain', 'find_event_by_id', 'update_company', 'update_search')
+   names      ('json', 'dataclasses', 'asdict', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'google.cloud.sql.connector', 'Connector', 'gandai', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Checkpoint', 'Company', 'Event', 'EventType', 'Search', 'db', 'insert_company', 'insert_event', 'insert_actor', 'insert_search', 'insert_checkpoint', 'str', 'int', 'insert_targets_from_domains', 'insert_companies_as_targets', 'DataFrame', 'top_actor_per_search', 'search_event_count_by_type', 'search', 'actor', 'search_target_by_last_event_type', 'target_count', 'event', 'unique_domains', 'company', 'checkpoint', 'comment_by_domain', 'find_search_by_uid', 'find_company_by_domain', 'find_event_by_id', 'update_company', 'update_search')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020108010c011002080108010c010c010c0214020c010c01200214
       060c0e1015100f1013100d02010eff020102ff020102ff020102ff020202
-      fe083402010eff020102ff020102ff020202fe083616261610062a160e12
-      451a3b1a1e1a0c1a0c160b1a0d1a15101210101013101b
+      fe083902010eff020102ff020102ff020202fe083616261610062a160e12
+      7f00031a1e1a0c1a0c160b1a0d1a15101210101013101b
```

### Comparing `gandai-1.3.6/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.3.7/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.3.7/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.3.7/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xe75dc164 (Wed Jul 26 17:54:47 2023 UTC)
+moddate:  0x1adbc264 (Thu Jul 27 21:01:14 2023 UTC)
 files sz: 11623
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `gandai-1.3.6/gandai/analytics.py` & `gandai-1.3.7/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/auth.py` & `gandai-1.3.7/gandai/auth.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/db.py` & `gandai-1.3.7/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/gpt.py` & `gandai-1.3.7/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/main.py` & `gandai-1.3.7/gandai/main.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.3.7/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/migrations/db_seed.py` & `gandai-1.3.7/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/migrations/dealcloud.py` & `gandai-1.3.7/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/migrations/sql/schema.sql` & `gandai-1.3.7/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/models.py` & `gandai-1.3.7/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/query.py` & `gandai-1.3.7/gandai/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,19 @@
     try to be enriched on process event
     """
     existing_domains = set(unique_domains(search_uid=search_uid)['domain'])
     
     new_domains = {helpers.clean_domain(domain) for domain in domains if "." in domain}
 
     domains_to_insert = list(new_domains - existing_domains)
+    existing_domains = set(unique_domains(search_uid=search_uid)['domain'])
+    
+    new_domains = {helpers.clean_domain(domain) for domain in domains if "." in domain}
+
+    domains_to_insert = list(new_domains - existing_domains)
 
     with db.connect() as con:
         for domain in domains_to_insert:
             # should these be in same transaction?
             con.execute(
                 sqlalchemy.text(
                     """
@@ -327,19 +332,21 @@
             e.data, 
             e.type AS last_event_type, 
             e.created AS updated,
             a.name AS updated_by,
             c.name as name,
             c.uid as dealcloud_id,
             c.description as description,
-            c.meta as meta,
+            (c.meta->>'year_founded') AS year_founded,
             (c.meta->>'employees') AS employees,
+            (c.meta->>'headquarters') AS headquarters,
             (c.meta->>'ownership') AS ownership,
             (c.meta->>'linkedin') AS linkedin,
-            (r.data->>'rating') AS rating
+            (r.data->>'rating') AS rating,
+            c.meta as meta
         FROM (
             SELECT 
                 search_uid, 
                 domain, 
                 MAX(created) AS max_created
             FROM 
                 event
@@ -383,70 +390,70 @@
         by=search.sort.get("field", "domain"),
         ascending=search.sort.get("order") == "asc",
     )
     targets['employees'] = pd.to_numeric(targets['employees'])
     return targets
 
 
-def search_target_export(search_uid: int) -> pd.DataFrame:
-    """Returns all the targets not in rejected or created"""
+# def search_target_export(search_uid: int) -> pd.DataFrame:
+#     """Returns all the targets not in rejected or created"""
 
-    statement = """
-        SELECT 
-            e.id, 
-            e.search_uid, 
-            e.domain, 
-            e.type AS last_event_type, 
-            to_timestamp(e.created) AS updated,
-            c.meta as meta,
-            (r.data->>'rating') AS rating
-        FROM (
-            SELECT 
-                search_uid, 
-                domain, 
-                MAX(created) AS max_created
-            FROM 
-                event
-            WHERE 
-                type NOT IN ('comment','rating','generate','criteria') 
-                AND search_uid = :search_uid
-            GROUP BY 
-                domain, search_uid
-        ) AS max_event
-        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid 
-        JOIN company c ON c.domain = e.domain
-        LEFT JOIN (
-            SELECT 
-                search_uid,
-                domain, 
-                MAX(created) AS max_created
-            FROM 
-                event
-            WHERE 
-                type = 'rating'
-            GROUP BY 
-                domain, search_uid
-        ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid
-        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;
-    """
-    with db.connect() as conn:
-        result = conn.execute(
-            sqlalchemy.text(statement),
-            {"search_uid": search_uid},
-        )
-        targets = pd.DataFrame(result.fetchall(), columns=result.keys())
-        # if len(targets) > 0:
-        #     targets = targets[~targets["last_event_type"].isin(["reject", "create"])]
-        #     meta = pd.json_normalize(targets["meta"], max_level=0)
-        #     targets = targets.merge(
-        #         meta, left_on=["domain"], right_on=["domain"], how="left"
-        #     )
-        #     targets = targets.drop(columns=["meta"])
-        #     targets = targets.sort_values(by=["last_event_type", "domain"])
-    return targets
+#     statement = """
+#         SELECT 
+#             e.id, 
+#             e.search_uid, 
+#             e.domain, 
+#             e.type AS last_event_type, 
+#             to_timestamp(e.created) AS updated,
+#             c.meta as meta,
+#             (r.data->>'rating') AS rating
+#         FROM (
+#             SELECT 
+#                 search_uid, 
+#                 domain, 
+#                 MAX(created) AS max_created
+#             FROM 
+#                 event
+#             WHERE 
+#                 type NOT IN ('comment','rating','generate','criteria') 
+#                 AND search_uid = :search_uid
+#             GROUP BY 
+#                 domain, search_uid
+#         ) AS max_event
+#         JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid 
+#         JOIN company c ON c.domain = e.domain
+#         LEFT JOIN (
+#             SELECT 
+#                 search_uid,
+#                 domain, 
+#                 MAX(created) AS max_created
+#             FROM 
+#                 event
+#             WHERE 
+#                 type = 'rating'
+#             GROUP BY 
+#                 domain, search_uid
+#         ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid
+#         LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;
+#     """
+#     with db.connect() as conn:
+#         result = conn.execute(
+#             sqlalchemy.text(statement),
+#             {"search_uid": search_uid},
+#         )
+#         targets = pd.DataFrame(result.fetchall(), columns=result.keys())
+#         if len(targets) > 0:
+#             targets = targets[~targets["last_event_type"].isin(["reject", "create"])]
+#         #     meta = pd.json_normalize(targets["meta"], max_level=0)
+#         #     targets = targets.merge(
+#         #         meta, left_on=["domain"], right_on=["domain"], how="left"
+#         #     )
+#         #     targets = targets.drop(columns=["meta"])
+#         #     targets = targets.sort_values(by=["last_event_type", "domain"])
+#     return targets
 
 
 
 def target_count(search_uid: int) -> pd.DataFrame:
     with db.connect() as conn:
         statement = """
             SELECT
```

### Comparing `gandai-1.3.6/gandai/secrets.py` & `gandai-1.3.7/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai/sources.py` & `gandai-1.3.7/gandai/sources.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.6/gandai.egg-info/SOURCES.txt` & `gandai-1.3.7/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

