# Comparing `tmp/zzq-strings-sum-0.5.2.tar.gz` & `tmp/zzq-strings-sum-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zzq-strings-sum-0.5.2.tar", last modified: Fri Jul 28 05:21:54 2023, max compression
+gzip compressed data, was "zzq-strings-sum-0.5.3.tar", last modified: Fri Jul 28 05:28:36 2023, max compression
```

## Comparing `zzq-strings-sum-0.5.2.tar` & `zzq-strings-sum-0.5.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:21:54.847151 zzq-strings-sum-0.5.2/
--rw-r--r--   0 zzq        (501) staff       (20)     1122 2023-07-28 05:21:54.847015 zzq-strings-sum-0.5.2/PKG-INFO
--rw-r--r--   0 zzq        (501) staff       (20)      880 2023-07-28 05:02:28.000000 zzq-strings-sum-0.5.2/README.md
--rw-r--r--   0 zzq        (501) staff       (20)       38 2023-07-28 05:21:54.847204 zzq-strings-sum-0.5.2/setup.cfg
--rw-r--r--   0 zzq        (501) staff       (20)      451 2023-07-28 05:21:53.000000 zzq-strings-sum-0.5.2/setup.py
-drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:21:54.846046 zzq-strings-sum-0.5.2/src/
--rw-r--r--   0 zzq        (501) staff       (20)      209 2023-07-28 05:21:26.000000 zzq-strings-sum-0.5.2/src/__init__.py
--rw-r--r--   0 zzq        (501) staff       (20)     2686 2023-07-28 04:47:09.000000 zzq-strings-sum-0.5.2/src/apitable_databus_client.py
-drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:21:54.846841 zzq-strings-sum-0.5.2/zzq_strings_sum.egg-info/
--rw-r--r--   0 zzq        (501) staff       (20)     1122 2023-07-28 05:21:54.000000 zzq-strings-sum-0.5.2/zzq_strings_sum.egg-info/PKG-INFO
--rw-r--r--   0 zzq        (501) staff       (20)      259 2023-07-28 05:21:54.000000 zzq-strings-sum-0.5.2/zzq_strings_sum.egg-info/SOURCES.txt
--rw-r--r--   0 zzq        (501) staff       (20)        1 2023-07-28 05:21:54.000000 zzq-strings-sum-0.5.2/zzq_strings_sum.egg-info/dependency_links.txt
--rw-r--r--   0 zzq        (501) staff       (20)        9 2023-07-28 05:21:54.000000 zzq-strings-sum-0.5.2/zzq_strings_sum.egg-info/requires.txt
--rw-r--r--   0 zzq        (501) staff       (20)        4 2023-07-28 05:21:54.000000 zzq-strings-sum-0.5.2/zzq_strings_sum.egg-info/top_level.txt
+drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:28:36.142814 zzq-strings-sum-0.5.3/
+-rw-r--r--   0 zzq        (501) staff       (20)     1122 2023-07-28 05:28:36.142697 zzq-strings-sum-0.5.3/PKG-INFO
+-rw-r--r--   0 zzq        (501) staff       (20)      880 2023-07-28 05:02:28.000000 zzq-strings-sum-0.5.3/README.md
+-rw-r--r--   0 zzq        (501) staff       (20)       38 2023-07-28 05:28:36.142855 zzq-strings-sum-0.5.3/setup.cfg
+-rw-r--r--   0 zzq        (501) staff       (20)      451 2023-07-28 05:28:32.000000 zzq-strings-sum-0.5.3/setup.py
+drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:28:36.142024 zzq-strings-sum-0.5.3/src/
+-rw-r--r--   0 zzq        (501) staff       (20)      240 2023-07-28 05:28:22.000000 zzq-strings-sum-0.5.3/src/__init__.py
+-rw-r--r--   0 zzq        (501) staff       (20)     2686 2023-07-28 04:47:09.000000 zzq-strings-sum-0.5.3/src/apitable_databus_client.py
+-rw-r--r--   0 zzq        (501) staff       (20)      181 2023-07-28 05:28:22.000000 zzq-strings-sum-0.5.3/src/z_test_module.py
+drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:28:36.142550 zzq-strings-sum-0.5.3/zzq_strings_sum.egg-info/
+-rw-r--r--   0 zzq        (501) staff       (20)     1122 2023-07-28 05:28:36.000000 zzq-strings-sum-0.5.3/zzq_strings_sum.egg-info/PKG-INFO
+-rw-r--r--   0 zzq        (501) staff       (20)      280 2023-07-28 05:28:36.000000 zzq-strings-sum-0.5.3/zzq_strings_sum.egg-info/SOURCES.txt
+-rw-r--r--   0 zzq        (501) staff       (20)        1 2023-07-28 05:28:36.000000 zzq-strings-sum-0.5.3/zzq_strings_sum.egg-info/dependency_links.txt
+-rw-r--r--   0 zzq        (501) staff       (20)        9 2023-07-28 05:28:36.000000 zzq-strings-sum-0.5.3/zzq_strings_sum.egg-info/requires.txt
+-rw-r--r--   0 zzq        (501) staff       (20)        4 2023-07-28 05:28:36.000000 zzq-strings-sum-0.5.3/zzq_strings_sum.egg-info/top_level.txt
```

### Comparing `zzq-strings-sum-0.5.2/PKG-INFO` & `zzq-strings-sum-0.5.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zzq-strings-sum
-Version: 0.5.2
+Version: 0.5.3
 Summary: A client for Databus API
 Home-page: UNKNOWN
 Author: zzq
 Author-email: zhaozhiqiang@vikadata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `zzq-strings-sum-0.5.2/README.md` & `zzq-strings-sum-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `zzq-strings-sum-0.5.2/src/apitable_databus_client.py` & `zzq-strings-sum-0.5.3/src/apitable_databus_client.py`

 * *Files identical despite different names*

### Comparing `zzq-strings-sum-0.5.2/zzq_strings_sum.egg-info/PKG-INFO` & `zzq-strings-sum-0.5.3/zzq_strings_sum.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zzq-strings-sum
-Version: 0.5.2
+Version: 0.5.3
 Summary: A client for Databus API
 Home-page: UNKNOWN
 Author: zzq
 Author-email: zhaozhiqiang@vikadata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

