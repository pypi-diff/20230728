# Comparing `tmp/tsbs-0.0.1.tar.gz` & `tmp/tsbs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsbs-0.0.1.tar", last modified: Fri Jul 28 00:40:45 2023, max compression
+gzip compressed data, was "tsbs-0.0.2.tar", last modified: Fri Jul 28 00:58:52 2023, max compression
```

## Comparing `tsbs-0.0.1.tar` & `tsbs-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 rajat.ghosh   (502) staff       (20)        0 2023-07-28 00:40:45.989807 tsbs-0.0.1/
--rw-r--r--   0 rajat.ghosh   (502) staff       (20)    35129 2023-07-27 23:32:42.000000 tsbs-0.0.1/LICENSE
--rw-r--r--   0 rajat.ghosh   (502) staff       (20)      999 2023-07-28 00:40:45.989351 tsbs-0.0.1/PKG-INFO
--rw-r--r--   0 rajat.ghosh   (502) staff       (20)      636 2023-07-28 00:11:10.000000 tsbs-0.0.1/README.md
--rw-r--r--   0 rajat.ghosh   (502) staff       (20)      342 2023-07-28 00:40:18.000000 tsbs-0.0.1/pyproject.toml
--rw-r--r--   0 rajat.ghosh   (502) staff       (20)       38 2023-07-28 00:40:45.989954 tsbs-0.0.1/setup.cfg
-drwxr-xr-x   0 rajat.ghosh   (502) staff       (20)        0 2023-07-28 00:40:45.982989 tsbs-0.0.1/src/
-drwxr-xr-x   0 rajat.ghosh   (502) staff       (20)        0 2023-07-28 00:40:45.987305 tsbs-0.0.1/src/tsbs.egg-info/
--rw-r--r--   0 rajat.ghosh   (502) staff       (20)      999 2023-07-28 00:40:45.000000 tsbs-0.0.1/src/tsbs.egg-info/PKG-INFO
--rw-r--r--   0 rajat.ghosh   (502) staff       (20)      218 2023-07-28 00:40:45.000000 tsbs-0.0.1/src/tsbs.egg-info/SOURCES.txt
--rw-r--r--   0 rajat.ghosh   (502) staff       (20)        1 2023-07-28 00:40:45.000000 tsbs-0.0.1/src/tsbs.egg-info/dependency_links.txt
--rw-r--r--   0 rajat.ghosh   (502) staff       (20)       13 2023-07-28 00:40:45.000000 tsbs-0.0.1/src/tsbs.egg-info/top_level.txt
-drwxr-xr-x   0 rajat.ghosh   (502) staff       (20)        0 2023-07-28 00:40:45.988632 tsbs-0.0.1/src/tsbs_rghosh8/
--rw-r--r--   0 rajat.ghosh   (502) staff       (20)        0 2023-07-27 21:59:55.000000 tsbs-0.0.1/src/tsbs_rghosh8/__init__.py
--rw-r--r--   0 rajat.ghosh   (502) staff       (20)     9778 2023-07-27 23:36:39.000000 tsbs-0.0.1/src/tsbs_rghosh8/baseline.py
+drwxr-xr-x   0 rajat.ghosh   (502) staff       (20)        0 2023-07-28 00:58:52.466986 tsbs-0.0.2/
+-rw-r--r--   0 rajat.ghosh   (502) staff       (20)    35129 2023-07-27 23:32:42.000000 tsbs-0.0.2/LICENSE
+-rw-r--r--   0 rajat.ghosh   (502) staff       (20)      999 2023-07-28 00:58:52.466564 tsbs-0.0.2/PKG-INFO
+-rw-r--r--   0 rajat.ghosh   (502) staff       (20)      636 2023-07-28 00:11:10.000000 tsbs-0.0.2/README.md
+-rw-r--r--   0 rajat.ghosh   (502) staff       (20)      342 2023-07-28 00:54:44.000000 tsbs-0.0.2/pyproject.toml
+-rw-r--r--   0 rajat.ghosh   (502) staff       (20)       38 2023-07-28 00:58:52.467160 tsbs-0.0.2/setup.cfg
+drwxr-xr-x   0 rajat.ghosh   (502) staff       (20)        0 2023-07-28 00:58:52.461717 tsbs-0.0.2/src/
+-rw-r--r--   0 rajat.ghosh   (502) staff       (20)        0 2023-07-28 00:57:01.000000 tsbs-0.0.2/src/__init__.py
+drwxr-xr-x   0 rajat.ghosh   (502) staff       (20)        0 2023-07-28 00:58:52.464211 tsbs-0.0.2/src/tsbs.egg-info/
+-rw-r--r--   0 rajat.ghosh   (502) staff       (20)      999 2023-07-28 00:58:52.000000 tsbs-0.0.2/src/tsbs.egg-info/PKG-INFO
+-rw-r--r--   0 rajat.ghosh   (502) staff       (20)      234 2023-07-28 00:58:52.000000 tsbs-0.0.2/src/tsbs.egg-info/SOURCES.txt
+-rw-r--r--   0 rajat.ghosh   (502) staff       (20)        1 2023-07-28 00:58:52.000000 tsbs-0.0.2/src/tsbs.egg-info/dependency_links.txt
+-rw-r--r--   0 rajat.ghosh   (502) staff       (20)       22 2023-07-28 00:58:52.000000 tsbs-0.0.2/src/tsbs.egg-info/top_level.txt
+drwxr-xr-x   0 rajat.ghosh   (502) staff       (20)        0 2023-07-28 00:58:52.465341 tsbs-0.0.2/src/tsbs_rghosh8/
+-rw-r--r--   0 rajat.ghosh   (502) staff       (20)        0 2023-07-27 21:59:55.000000 tsbs-0.0.2/src/tsbs_rghosh8/__init__.py
+-rw-r--r--   0 rajat.ghosh   (502) staff       (20)     9778 2023-07-27 23:36:39.000000 tsbs-0.0.2/src/tsbs_rghosh8/baseline.py
```

### Comparing `tsbs-0.0.1/LICENSE` & `tsbs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tsbs-0.0.1/PKG-INFO` & `tsbs-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsbs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Time Series Baseline
 Author-email: Rajat Ghosh <rajat.ghosh11@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `tsbs-0.0.1/README.md` & `tsbs-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tsbs-0.0.1/src/tsbs.egg-info/PKG-INFO` & `tsbs-0.0.2/src/tsbs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsbs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Time Series Baseline
 Author-email: Rajat Ghosh <rajat.ghosh11@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `tsbs-0.0.1/src/tsbs_rghosh8/baseline.py` & `tsbs-0.0.2/src/tsbs_rghosh8/baseline.py`

 * *Files identical despite different names*

