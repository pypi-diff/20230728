# Comparing `tmp/vdk-jobs-troubleshooting-0.2.824443273.tar.gz` & `tmp/vdk-jobs-troubleshooting-0.2.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-jobs-troubleshooting-0.2.824443273.tar", last modified: Fri Mar 31 14:27:04 2023, max compression
+gzip compressed data, was "vdk-jobs-troubleshooting-0.2.948436673.tar", last modified: Fri Jul 28 09:42:41 2023, max compression
```

## Comparing `vdk-jobs-troubleshooting-0.2.824443273.tar` & `vdk-jobs-troubleshooting-0.2.948436673.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:27:04.123496 vdk-jobs-troubleshooting-0.2.824443273/
--rw-r--r--   0 root         (0) root         (0)      671 2023-03-31 14:27:04.123496 vdk-jobs-troubleshooting-0.2.824443273/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-03-31 14:26:49.000000 vdk-jobs-troubleshooting-0.2.824443273/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 14:27:04.123496 vdk-jobs-troubleshooting-0.2.824443273/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-03-31 14:26:53.000000 vdk-jobs-troubleshooting-0.2.824443273/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:27:04.123496 vdk-jobs-troubleshooting-0.2.824443273/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:27:04.123496 vdk-jobs-troubleshooting-0.2.824443273/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:27:04.123496 vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:27:04.123496 vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/jobs_troubleshoot/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:27:04.123496 vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/jobs_troubleshoot/api/
--rw-rw-rw-   0 root         (0) root         (0)     1632 2023-03-31 14:26:49.000000 vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/jobs_troubleshoot/api/troubleshoot_utility.py
--rw-rw-rw-   0 root         (0) root         (0)     2504 2023-03-31 14:26:49.000000 vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/jobs_troubleshoot/jobs_troubleshoot_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1209 2023-03-31 14:26:49.000000 vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/jobs_troubleshoot/troubleshoot_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:27:04.123496 vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/jobs_troubleshoot/troubleshoot_utilities/
--rw-rw-rw-   0 root         (0) root         (0)     2462 2023-03-31 14:26:49.000000 vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/jobs_troubleshoot/troubleshoot_utilities/healthcheck_server.py
--rw-rw-rw-   0 root         (0) root         (0)     2881 2023-03-31 14:26:49.000000 vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/jobs_troubleshoot/troubleshoot_utilities/thread_dump.py
--rw-rw-rw-   0 root         (0) root         (0)     2138 2023-03-31 14:26:49.000000 vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/jobs_troubleshoot/troubleshoot_utilities/utilities_registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:27:04.123496 vdk-jobs-troubleshooting-0.2.824443273/src/vdk_jobs_troubleshooting.egg-info/
--rw-r--r--   0 root         (0) root         (0)      671 2023-03-31 14:27:04.000000 vdk-jobs-troubleshooting-0.2.824443273/src/vdk_jobs_troubleshooting.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      777 2023-03-31 14:27:04.000000 vdk-jobs-troubleshooting-0.2.824443273/src/vdk_jobs_troubleshooting.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:27:04.000000 vdk-jobs-troubleshooting-0.2.824443273/src/vdk_jobs_troubleshooting.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-03-31 14:27:04.000000 vdk-jobs-troubleshooting-0.2.824443273/src/vdk_jobs_troubleshooting.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-31 14:27:04.000000 vdk-jobs-troubleshooting-0.2.824443273/src/vdk_jobs_troubleshooting.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 14:27:04.000000 vdk-jobs-troubleshooting-0.2.824443273/src/vdk_jobs_troubleshooting.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:27:04.123496 vdk-jobs-troubleshooting-0.2.824443273/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-03-31 14:26:49.000000 vdk-jobs-troubleshooting-0.2.824443273/tests/test_utilities_registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.366745 vdk-jobs-troubleshooting-0.2.948436673/
+-rw-r--r--   0 root         (0) root         (0)      671 2023-07-28 09:42:41.366745 vdk-jobs-troubleshooting-0.2.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-28 09:42:17.000000 vdk-jobs-troubleshooting-0.2.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:42:41.366745 vdk-jobs-troubleshooting-0.2.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-07-28 09:42:26.000000 vdk-jobs-troubleshooting-0.2.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.362745 vdk-jobs-troubleshooting-0.2.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.362745 vdk-jobs-troubleshooting-0.2.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.362745 vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.362745 vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/jobs_troubleshoot/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.362745 vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/jobs_troubleshoot/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1632 2023-07-28 09:42:17.000000 vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/jobs_troubleshoot/api/troubleshoot_utility.py
+-rw-rw-rw-   0 root         (0) root         (0)     2504 2023-07-28 09:42:17.000000 vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/jobs_troubleshoot/jobs_troubleshoot_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2023-07-28 09:42:17.000000 vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/jobs_troubleshoot/troubleshoot_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.366745 vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/jobs_troubleshoot/troubleshoot_utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2023-07-28 09:42:17.000000 vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/jobs_troubleshoot/troubleshoot_utilities/healthcheck_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     2881 2023-07-28 09:42:17.000000 vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/jobs_troubleshoot/troubleshoot_utilities/thread_dump.py
+-rw-rw-rw-   0 root         (0) root         (0)     2138 2023-07-28 09:42:17.000000 vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/jobs_troubleshoot/troubleshoot_utilities/utilities_registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.366745 vdk-jobs-troubleshooting-0.2.948436673/src/vdk_jobs_troubleshooting.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      671 2023-07-28 09:42:41.000000 vdk-jobs-troubleshooting-0.2.948436673/src/vdk_jobs_troubleshooting.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      777 2023-07-28 09:42:41.000000 vdk-jobs-troubleshooting-0.2.948436673/src/vdk_jobs_troubleshooting.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:41.000000 vdk-jobs-troubleshooting-0.2.948436673/src/vdk_jobs_troubleshooting.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-28 09:42:41.000000 vdk-jobs-troubleshooting-0.2.948436673/src/vdk_jobs_troubleshooting.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-28 09:42:41.000000 vdk-jobs-troubleshooting-0.2.948436673/src/vdk_jobs_troubleshooting.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:42:41.000000 vdk-jobs-troubleshooting-0.2.948436673/src/vdk_jobs_troubleshooting.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.366745 vdk-jobs-troubleshooting-0.2.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-28 09:42:17.000000 vdk-jobs-troubleshooting-0.2.948436673/tests/test_utilities_registry.py
```

### Comparing `vdk-jobs-troubleshooting-0.2.824443273/PKG-INFO` & `vdk-jobs-troubleshooting-0.2.948436673/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-jobs-troubleshooting
-Version: 0.2.824443273
+Version: 0.2.948436673
 Summary: Versatile Data Kit SDK troubleshooting plugin to assist in troubleshooting deployed data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-jobs-troubleshooting-0.2.824443273/setup.py` & `vdk-jobs-troubleshooting-0.2.948436673/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.824443273"
+__version__ = "0.2.948436673"
 
 setuptools.setup(
     name="vdk-jobs-troubleshooting",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK troubleshooting plugin to assist in troubleshooting deployed data jobs.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/jobs_troubleshoot/api/troubleshoot_utility.py` & `vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/jobs_troubleshoot/api/troubleshoot_utility.py`

 * *Files identical despite different names*

### Comparing `vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/jobs_troubleshoot/jobs_troubleshoot_plugin.py` & `vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/jobs_troubleshoot/jobs_troubleshoot_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/jobs_troubleshoot/troubleshoot_configuration.py` & `vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/jobs_troubleshoot/troubleshoot_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/jobs_troubleshoot/troubleshoot_utilities/healthcheck_server.py` & `vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/jobs_troubleshoot/troubleshoot_utilities/healthcheck_server.py`

 * *Files identical despite different names*

### Comparing `vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/jobs_troubleshoot/troubleshoot_utilities/thread_dump.py` & `vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/jobs_troubleshoot/troubleshoot_utilities/thread_dump.py`

 * *Files identical despite different names*

### Comparing `vdk-jobs-troubleshooting-0.2.824443273/src/vdk/plugin/jobs_troubleshoot/troubleshoot_utilities/utilities_registry.py` & `vdk-jobs-troubleshooting-0.2.948436673/src/vdk/plugin/jobs_troubleshoot/troubleshoot_utilities/utilities_registry.py`

 * *Files identical despite different names*

### Comparing `vdk-jobs-troubleshooting-0.2.824443273/src/vdk_jobs_troubleshooting.egg-info/PKG-INFO` & `vdk-jobs-troubleshooting-0.2.948436673/src/vdk_jobs_troubleshooting.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-jobs-troubleshooting
-Version: 0.2.824443273
+Version: 0.2.948436673
 Summary: Versatile Data Kit SDK troubleshooting plugin to assist in troubleshooting deployed data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-jobs-troubleshooting-0.2.824443273/src/vdk_jobs_troubleshooting.egg-info/SOURCES.txt` & `vdk-jobs-troubleshooting-0.2.948436673/src/vdk_jobs_troubleshooting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-jobs-troubleshooting-0.2.824443273/tests/test_utilities_registry.py` & `vdk-jobs-troubleshooting-0.2.948436673/tests/test_utilities_registry.py`

 * *Files identical despite different names*

