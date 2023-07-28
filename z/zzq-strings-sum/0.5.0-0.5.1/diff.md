# Comparing `tmp/zzq-strings-sum-0.5.0.tar.gz` & `tmp/zzq-strings-sum-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zzq-strings-sum-0.5.0.tar", last modified: Fri Jul 28 05:05:58 2023, max compression
+gzip compressed data, was "zzq-strings-sum-0.5.1.tar", last modified: Fri Jul 28 05:08:12 2023, max compression
```

## Comparing `zzq-strings-sum-0.5.0.tar` & `zzq-strings-sum-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:05:58.514284 zzq-strings-sum-0.5.0/
--rw-r--r--   0 zzq        (501) staff       (20)      209 2023-07-28 05:05:58.514158 zzq-strings-sum-0.5.0/PKG-INFO
--rw-r--r--   0 zzq        (501) staff       (20)      880 2023-07-28 05:02:28.000000 zzq-strings-sum-0.5.0/README.md
--rw-r--r--   0 zzq        (501) staff       (20)       38 2023-07-28 05:05:58.514329 zzq-strings-sum-0.5.0/setup.cfg
--rw-r--r--   0 zzq        (501) staff       (20)      276 2023-07-28 05:03:16.000000 zzq-strings-sum-0.5.0/setup.py
-drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:05:58.513366 zzq-strings-sum-0.5.0/src/
--rw-r--r--   0 zzq        (501) staff       (20)      220 2023-07-28 05:02:28.000000 zzq-strings-sum-0.5.0/src/__init__.py
--rw-r--r--   0 zzq        (501) staff       (20)     2686 2023-07-28 04:47:09.000000 zzq-strings-sum-0.5.0/src/apitable_databus_client.py
-drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:05:58.513998 zzq-strings-sum-0.5.0/zzq_strings_sum.egg-info/
--rw-r--r--   0 zzq        (501) staff       (20)      209 2023-07-28 05:05:58.000000 zzq-strings-sum-0.5.0/zzq_strings_sum.egg-info/PKG-INFO
--rw-r--r--   0 zzq        (501) staff       (20)      259 2023-07-28 05:05:58.000000 zzq-strings-sum-0.5.0/zzq_strings_sum.egg-info/SOURCES.txt
--rw-r--r--   0 zzq        (501) staff       (20)        1 2023-07-28 05:05:58.000000 zzq-strings-sum-0.5.0/zzq_strings_sum.egg-info/dependency_links.txt
--rw-r--r--   0 zzq        (501) staff       (20)        9 2023-07-28 05:05:58.000000 zzq-strings-sum-0.5.0/zzq_strings_sum.egg-info/requires.txt
--rw-r--r--   0 zzq        (501) staff       (20)        4 2023-07-28 05:05:58.000000 zzq-strings-sum-0.5.0/zzq_strings_sum.egg-info/top_level.txt
+drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:08:12.190397 zzq-strings-sum-0.5.1/
+-rw-r--r--   0 zzq        (501) staff       (20)     1122 2023-07-28 05:08:12.190278 zzq-strings-sum-0.5.1/PKG-INFO
+-rw-r--r--   0 zzq        (501) staff       (20)      880 2023-07-28 05:02:28.000000 zzq-strings-sum-0.5.1/README.md
+-rw-r--r--   0 zzq        (501) staff       (20)       38 2023-07-28 05:08:12.190440 zzq-strings-sum-0.5.1/setup.cfg
+-rw-r--r--   0 zzq        (501) staff       (20)      451 2023-07-28 05:07:37.000000 zzq-strings-sum-0.5.1/setup.py
+drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:08:12.189486 zzq-strings-sum-0.5.1/src/
+-rw-r--r--   0 zzq        (501) staff       (20)      220 2023-07-28 05:02:28.000000 zzq-strings-sum-0.5.1/src/__init__.py
+-rw-r--r--   0 zzq        (501) staff       (20)     2686 2023-07-28 04:47:09.000000 zzq-strings-sum-0.5.1/src/apitable_databus_client.py
+drwxr-xr-x   0 zzq        (501) staff       (20)        0 2023-07-28 05:08:12.190116 zzq-strings-sum-0.5.1/zzq_strings_sum.egg-info/
+-rw-r--r--   0 zzq        (501) staff       (20)     1122 2023-07-28 05:08:12.000000 zzq-strings-sum-0.5.1/zzq_strings_sum.egg-info/PKG-INFO
+-rw-r--r--   0 zzq        (501) staff       (20)      259 2023-07-28 05:08:12.000000 zzq-strings-sum-0.5.1/zzq_strings_sum.egg-info/SOURCES.txt
+-rw-r--r--   0 zzq        (501) staff       (20)        1 2023-07-28 05:08:12.000000 zzq-strings-sum-0.5.1/zzq_strings_sum.egg-info/dependency_links.txt
+-rw-r--r--   0 zzq        (501) staff       (20)        9 2023-07-28 05:08:12.000000 zzq-strings-sum-0.5.1/zzq_strings_sum.egg-info/requires.txt
+-rw-r--r--   0 zzq        (501) staff       (20)        4 2023-07-28 05:08:12.000000 zzq-strings-sum-0.5.1/zzq_strings_sum.egg-info/top_level.txt
```

### Comparing `zzq-strings-sum-0.5.0/README.md` & `zzq-strings-sum-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `zzq-strings-sum-0.5.0/src/apitable_databus_client.py` & `zzq-strings-sum-0.5.1/src/apitable_databus_client.py`

 * *Files identical despite different names*

