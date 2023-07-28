# Comparing `tmp/vdk-smarter-0.1.924312320.tar.gz` & `tmp/vdk-smarter-0.1.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-smarter-0.1.924312320.tar", last modified: Fri Jul  7 11:41:20 2023, max compression
+gzip compressed data, was "vdk-smarter-0.1.948436673.tar", last modified: Fri Jul 28 09:43:51 2023, max compression
```

## Comparing `vdk-smarter-0.1.924312320.tar` & `vdk-smarter-0.1.948436673.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 11:41:20.288820 vdk-smarter-0.1.924312320/
--rw-r--r--   0 root         (0) root         (0)     3304 2023-07-07 11:41:20.288820 vdk-smarter-0.1.924312320/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2733 2023-07-07 11:41:01.000000 vdk-smarter-0.1.924312320/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 11:41:20.288820 vdk-smarter-0.1.924312320/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1322 2023-07-07 11:41:05.000000 vdk-smarter-0.1.924312320/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 11:41:20.288820 vdk-smarter-0.1.924312320/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 11:41:20.288820 vdk-smarter-0.1.924312320/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 11:41:20.288820 vdk-smarter-0.1.924312320/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 11:41:20.288820 vdk-smarter-0.1.924312320/src/vdk/plugin/smarter/
--rw-rw-rw-   0 root         (0) root         (0)     4473 2023-07-07 11:41:01.000000 vdk-smarter-0.1.924312320/src/vdk/plugin/smarter/openai_plugin_entry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 11:41:20.288820 vdk-smarter-0.1.924312320/src/vdk_smarter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3304 2023-07-07 11:41:20.000000 vdk-smarter-0.1.924312320/src/vdk_smarter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      325 2023-07-07 11:41:20.000000 vdk-smarter-0.1.924312320/src/vdk_smarter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 11:41:20.000000 vdk-smarter-0.1.924312320/src/vdk_smarter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-07 11:41:20.000000 vdk-smarter-0.1.924312320/src/vdk_smarter.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-07 11:41:20.000000 vdk-smarter-0.1.924312320/src/vdk_smarter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-07 11:41:20.000000 vdk-smarter-0.1.924312320/src/vdk_smarter.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 11:41:20.288820 vdk-smarter-0.1.924312320/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2017 2023-07-07 11:41:01.000000 vdk-smarter-0.1.924312320/tests/test_sql_review.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:51.197923 vdk-smarter-0.1.948436673/
+-rw-r--r--   0 root         (0) root         (0)     3304 2023-07-28 09:43:51.197923 vdk-smarter-0.1.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2733 2023-07-28 09:43:27.000000 vdk-smarter-0.1.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:43:51.197923 vdk-smarter-0.1.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1322 2023-07-28 09:43:36.000000 vdk-smarter-0.1.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:51.193923 vdk-smarter-0.1.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:51.193923 vdk-smarter-0.1.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:51.193923 vdk-smarter-0.1.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:51.193923 vdk-smarter-0.1.948436673/src/vdk/plugin/smarter/
+-rw-rw-rw-   0 root         (0) root         (0)     4473 2023-07-28 09:43:27.000000 vdk-smarter-0.1.948436673/src/vdk/plugin/smarter/openai_plugin_entry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:51.197923 vdk-smarter-0.1.948436673/src/vdk_smarter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3304 2023-07-28 09:43:51.000000 vdk-smarter-0.1.948436673/src/vdk_smarter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      325 2023-07-28 09:43:51.000000 vdk-smarter-0.1.948436673/src/vdk_smarter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:43:51.000000 vdk-smarter-0.1.948436673/src/vdk_smarter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-28 09:43:51.000000 vdk-smarter-0.1.948436673/src/vdk_smarter.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-28 09:43:51.000000 vdk-smarter-0.1.948436673/src/vdk_smarter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:43:51.000000 vdk-smarter-0.1.948436673/src/vdk_smarter.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:51.197923 vdk-smarter-0.1.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2017 2023-07-28 09:43:27.000000 vdk-smarter-0.1.948436673/tests/test_sql_review.py
```

### Comparing `vdk-smarter-0.1.924312320/PKG-INFO` & `vdk-smarter-0.1.948436673/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-smarter
-Version: 0.1.924312320
+Version: 0.1.948436673
 Summary: Making VDK smarter by employing ML/AI.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-smarter-0.1.924312320/README.md` & `vdk-smarter-0.1.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-smarter-0.1.924312320/setup.py` & `vdk-smarter-0.1.948436673/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.924312320"
+__version__ = "0.1.948436673"
 
 setuptools.setup(
     name="vdk-smarter",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Making VDK smarter by employing ML/AI.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-smarter-0.1.924312320/src/vdk/plugin/smarter/openai_plugin_entry.py` & `vdk-smarter-0.1.948436673/src/vdk/plugin/smarter/openai_plugin_entry.py`

 * *Files identical despite different names*

### Comparing `vdk-smarter-0.1.924312320/src/vdk_smarter.egg-info/PKG-INFO` & `vdk-smarter-0.1.948436673/src/vdk_smarter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-smarter
-Version: 0.1.924312320
+Version: 0.1.948436673
 Summary: Making VDK smarter by employing ML/AI.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-smarter-0.1.924312320/tests/test_sql_review.py` & `vdk-smarter-0.1.948436673/tests/test_sql_review.py`

 * *Files identical despite different names*

