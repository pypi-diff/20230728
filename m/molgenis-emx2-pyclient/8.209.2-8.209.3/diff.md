# Comparing `tmp/molgenis_emx2_pyclient-8.209.2.tar.gz` & `tmp/molgenis_emx2_pyclient-8.209.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgenis_emx2_pyclient-8.209.2.tar", last modified: Fri Jul 28 13:01:31 2023, max compression
+gzip compressed data, was "molgenis_emx2_pyclient-8.209.3.tar", last modified: Fri Jul 28 13:59:21 2023, max compression
```

## Comparing `molgenis_emx2_pyclient-8.209.2.tar` & `molgenis_emx2_pyclient-8.209.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:01:31.419379 molgenis_emx2_pyclient-8.209.2/
--rw-r--r--   0 root         (0) root         (0)     7631 2023-07-28 12:50:26.000000 molgenis_emx2_pyclient-8.209.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1342 2023-07-28 13:01:31.419379 molgenis_emx2_pyclient-8.209.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-07-28 12:50:26.000000 molgenis_emx2_pyclient-8.209.2/README.md
--rw-r--r--   0 root         (0) root         (0)      634 2023-07-28 12:50:26.000000 molgenis_emx2_pyclient-8.209.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-28 12:50:26.000000 molgenis_emx2_pyclient-8.209.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 13:01:31.419379 molgenis_emx2_pyclient-8.209.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:01:31.419379 molgenis_emx2_pyclient-8.209.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:01:31.419379 molgenis_emx2_pyclient-8.209.2/src/molgenis_emx2_pyclient/
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-28 12:50:26.000000 molgenis_emx2_pyclient-8.209.2/src/molgenis_emx2_pyclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2781 2023-07-28 12:50:26.000000 molgenis_emx2_pyclient-8.209.2/src/molgenis_emx2_pyclient/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:01:31.419379 molgenis_emx2_pyclient-8.209.2/src/molgenis_emx2_pyclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1342 2023-07-28 13:01:31.000000 molgenis_emx2_pyclient-8.209.2/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      386 2023-07-28 13:01:31.000000 molgenis_emx2_pyclient-8.209.2/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 13:01:31.000000 molgenis_emx2_pyclient-8.209.2/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-28 13:01:31.000000 molgenis_emx2_pyclient-8.209.2/src/molgenis_emx2_pyclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-28 13:01:31.000000 molgenis_emx2_pyclient-8.209.2/src/molgenis_emx2_pyclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-28 12:56:51.000000 molgenis_emx2_pyclient-8.209.2/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:59:21.296408 molgenis_emx2_pyclient-8.209.3/
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-07-28 13:48:55.000000 molgenis_emx2_pyclient-8.209.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-07-28 13:59:21.296408 molgenis_emx2_pyclient-8.209.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-07-28 13:48:55.000000 molgenis_emx2_pyclient-8.209.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-28 13:48:55.000000 molgenis_emx2_pyclient-8.209.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-28 13:48:55.000000 molgenis_emx2_pyclient-8.209.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 13:59:21.296408 molgenis_emx2_pyclient-8.209.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:59:21.296408 molgenis_emx2_pyclient-8.209.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:59:21.296408 molgenis_emx2_pyclient-8.209.3/src/molgenis_emx2_pyclient/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-28 13:48:55.000000 molgenis_emx2_pyclient-8.209.3/src/molgenis_emx2_pyclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2023-07-28 13:48:55.000000 molgenis_emx2_pyclient-8.209.3/src/molgenis_emx2_pyclient/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:59:21.296408 molgenis_emx2_pyclient-8.209.3/src/molgenis_emx2_pyclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-07-28 13:59:21.000000 molgenis_emx2_pyclient-8.209.3/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      386 2023-07-28 13:59:21.000000 molgenis_emx2_pyclient-8.209.3/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 13:59:21.000000 molgenis_emx2_pyclient-8.209.3/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-28 13:59:21.000000 molgenis_emx2_pyclient-8.209.3/src/molgenis_emx2_pyclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-28 13:59:21.000000 molgenis_emx2_pyclient-8.209.3/src/molgenis_emx2_pyclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-28 13:54:48.000000 molgenis_emx2_pyclient-8.209.3/version.txt
```

### Comparing `molgenis_emx2_pyclient-8.209.2/LICENSE` & `molgenis_emx2_pyclient-8.209.3/LICENSE`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.209.2/PKG-INFO` & `molgenis_emx2_pyclient-8.209.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis_emx2_pyclient
-Version: 8.209.2
+Version: 8.209.3
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molgenis_emx2_pyclient-8.209.2/README.md` & `molgenis_emx2_pyclient-8.209.3/README.md`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.209.2/pyproject.toml` & `molgenis_emx2_pyclient-8.209.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.209.2/src/molgenis_emx2_pyclient/client.py` & `molgenis_emx2_pyclient-8.209.3/src/molgenis_emx2_pyclient/client.py`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.209.2/src/molgenis_emx2_pyclient.egg-info/PKG-INFO` & `molgenis_emx2_pyclient-8.209.3/src/molgenis_emx2_pyclient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis-emx2-pyclient
-Version: 8.209.2
+Version: 8.209.3
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

