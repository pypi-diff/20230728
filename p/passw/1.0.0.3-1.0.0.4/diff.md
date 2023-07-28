# Comparing `tmp/passw-1.0.0.3.tar.gz` & `tmp/passw-1.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passw-1.0.0.3.tar", last modified: Tue Jul 25 11:06:35 2023, max compression
+gzip compressed data, was "passw-1.0.0.4.tar", last modified: Fri Jul 28 10:04:30 2023, max compression
```

## Comparing `passw-1.0.0.3.tar` & `passw-1.0.0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 11:06:35.332245 passw-1.0.0.3/
--rw-rw-r--   0 user      (1000) user      (1000)      257 2023-07-25 11:06:35.332245 passw-1.0.0.3/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 11:06:35.332245 passw-1.0.0.3/passw/
--rw-rw-r--   0 user      (1000) user      (1000)       36 2023-07-25 11:01:52.000000 passw-1.0.0.3/passw/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      773 2023-07-25 11:06:21.000000 passw-1.0.0.3/passw/generate_pass.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 11:06:35.332245 passw-1.0.0.3/passw.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      257 2023-07-25 11:06:35.000000 passw-1.0.0.3/passw.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      165 2023-07-25 11:06:35.000000 passw-1.0.0.3/passw.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 11:06:35.000000 passw-1.0.0.3/passw.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        6 2023-07-25 11:06:35.000000 passw-1.0.0.3/passw.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 11:06:35.332245 passw-1.0.0.3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      385 2023-07-25 11:06:29.000000 passw-1.0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:04:30.858371 passw-1.0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-28 10:04:30.858371 passw-1.0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 10:04:18.000000 passw-1.0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:04:30.858371 passw-1.0.0.4/passw/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 10:04:18.000000 passw-1.0.0.4/passw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-28 10:04:18.000000 passw-1.0.0.4/passw/generate_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:04:30.858371 passw-1.0.0.4/passw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-28 10:04:30.000000 passw-1.0.0.4/passw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-28 10:04:30.000000 passw-1.0.0.4/passw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:04:30.000000 passw-1.0.0.4/passw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 10:04:30.000000 passw-1.0.0.4/passw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:04:30.858371 passw-1.0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-28 10:04:18.000000 passw-1.0.0.4/setup.py
```

### Comparing `passw-1.0.0.3/passw/generate_pass.py` & `passw-1.0.0.4/passw/generate_pass.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,11 +16,11 @@
             any(c.isdigit() for c in password)):
             break
 
     return password
 
 
 def gen_pass():
-    pass_len = random.randint(6,12)
+    pass_len = random.randint(6,10)
     passw = generate_random_password(pass_len)
     return passw
```

