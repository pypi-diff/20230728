# Comparing `tmp/zzq-strings-sum-0.5.3.tar.gz` & `tmp/zzq-strings-sum-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zzq-strings-sum-0.5.3.tar", last modified: Fri Jul 28 05:28:36 2023, max compression
+gzip compressed data, was "zzq-strings-sum-0.5.4.tar", last modified: Fri Jul 28 05:46:20 2023, max compression
```

## Comparing `zzq-strings-sum-0.5.3.tar` & `zzq-strings-sum-0.5.4.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:28:36.142814 zzq-strings-sum-0.5.3/
--rw-r--r--   0 zzq        (501) staff       (20)     1122 2023-07-28 05:28:36.142697 zzq-strings-sum-0.5.3/PKG-INFO
--rw-r--r--   0 zzq        (501) staff       (20)      880 2023-07-28 05:02:28.000000 zzq-strings-sum-0.5.3/README.md
--rw-r--r--   0 zzq        (501) staff       (20)       38 2023-07-28 05:28:36.142855 zzq-strings-sum-0.5.3/setup.cfg
--rw-r--r--   0 zzq        (501) staff       (20)      451 2023-07-28 05:28:32.000000 zzq-strings-sum-0.5.3/setup.py
-drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:28:36.142024 zzq-strings-sum-0.5.3/src/
--rw-r--r--   0 zzq        (501) staff       (20)      240 2023-07-28 05:28:22.000000 zzq-strings-sum-0.5.3/src/__init__.py
--rw-r--r--   0 zzq        (501) staff       (20)     2686 2023-07-28 04:47:09.000000 zzq-strings-sum-0.5.3/src/apitable_databus_client.py
--rw-r--r--   0 zzq        (501) staff       (20)      181 2023-07-28 05:28:22.000000 zzq-strings-sum-0.5.3/src/z_test_module.py
-drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:28:36.142550 zzq-strings-sum-0.5.3/zzq_strings_sum.egg-info/
--rw-r--r--   0 zzq        (501) staff       (20)     1122 2023-07-28 05:28:36.000000 zzq-strings-sum-0.5.3/zzq_strings_sum.egg-info/PKG-INFO
--rw-r--r--   0 zzq        (501) staff       (20)      280 2023-07-28 05:28:36.000000 zzq-strings-sum-0.5.3/zzq_strings_sum.egg-info/SOURCES.txt
--rw-r--r--   0 zzq        (501) staff       (20)        1 2023-07-28 05:28:36.000000 zzq-strings-sum-0.5.3/zzq_strings_sum.egg-info/dependency_links.txt
--rw-r--r--   0 zzq        (501) staff       (20)        9 2023-07-28 05:28:36.000000 zzq-strings-sum-0.5.3/zzq_strings_sum.egg-info/requires.txt
--rw-r--r--   0 zzq        (501) staff       (20)        4 2023-07-28 05:28:36.000000 zzq-strings-sum-0.5.3/zzq_strings_sum.egg-info/top_level.txt
+drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:46:20.315505 zzq-strings-sum-0.5.4/
+-rw-r--r--   0 zzq        (501) staff       (20)     1122 2023-07-28 05:46:20.315384 zzq-strings-sum-0.5.4/PKG-INFO
+-rw-r--r--   0 zzq        (501) staff       (20)      880 2023-07-28 05:02:28.000000 zzq-strings-sum-0.5.4/README.md
+-rw-r--r--   0 zzq        (501) staff       (20)      444 2023-07-28 05:38:45.000000 zzq-strings-sum-0.5.4/pyproject.toml
+-rw-r--r--   0 zzq        (501) staff       (20)       38 2023-07-28 05:46:20.315546 zzq-strings-sum-0.5.4/setup.cfg
+-rw-r--r--   0 zzq        (501) staff       (20)      495 2023-07-28 05:46:17.000000 zzq-strings-sum-0.5.4/setup.py
+drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:46:20.314224 zzq-strings-sum-0.5.4/src/
+drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:46:20.315235 zzq-strings-sum-0.5.4/src/zzq_strings_sum.egg-info/
+-rw-r--r--   0 zzq        (501) staff       (20)     1122 2023-07-28 05:46:20.000000 zzq-strings-sum-0.5.4/src/zzq_strings_sum.egg-info/PKG-INFO
+-rw-r--r--   0 zzq        (501) staff       (20)      247 2023-07-28 05:46:20.000000 zzq-strings-sum-0.5.4/src/zzq_strings_sum.egg-info/SOURCES.txt
+-rw-r--r--   0 zzq        (501) staff       (20)        1 2023-07-28 05:46:20.000000 zzq-strings-sum-0.5.4/src/zzq_strings_sum.egg-info/dependency_links.txt
+-rw-r--r--   0 zzq        (501) staff       (20)        9 2023-07-28 05:46:20.000000 zzq-strings-sum-0.5.4/src/zzq_strings_sum.egg-info/requires.txt
+-rw-r--r--   0 zzq        (501) staff       (20)        1 2023-07-28 05:46:20.000000 zzq-strings-sum-0.5.4/src/zzq_strings_sum.egg-info/top_level.txt
```

### Comparing `zzq-strings-sum-0.5.3/PKG-INFO` & `zzq-strings-sum-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zzq-strings-sum
-Version: 0.5.3
+Version: 0.5.4
 Summary: A client for Databus API
 Home-page: UNKNOWN
 Author: zzq
 Author-email: zhaozhiqiang@vikadata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `zzq-strings-sum-0.5.3/README.md` & `zzq-strings-sum-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `zzq-strings-sum-0.5.3/zzq_strings_sum.egg-info/PKG-INFO` & `zzq-strings-sum-0.5.4/src/zzq_strings_sum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zzq-strings-sum
-Version: 0.5.3
+Version: 0.5.4
 Summary: A client for Databus API
 Home-page: UNKNOWN
 Author: zzq
 Author-email: zhaozhiqiang@vikadata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

