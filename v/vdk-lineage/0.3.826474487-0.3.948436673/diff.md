# Comparing `tmp/vdk-lineage-0.3.826474487.tar.gz` & `tmp/vdk-lineage-0.3.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-lineage-0.3.826474487.tar", last modified: Mon Apr  3 15:06:05 2023, max compression
+gzip compressed data, was "vdk-lineage-0.3.948436673.tar", last modified: Fri Jul 28 09:42:44 2023, max compression
```

## Comparing `vdk-lineage-0.3.826474487.tar` & `vdk-lineage-0.3.948436673.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 15:06:05.966601 vdk-lineage-0.3.826474487/
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-03 15:05:54.000000 vdk-lineage-0.3.826474487/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2138 2023-04-03 15:06:05.966601 vdk-lineage-0.3.826474487/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-04-03 15:05:54.000000 vdk-lineage-0.3.826474487/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-03 15:06:05.966601 vdk-lineage-0.3.826474487/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1518 2023-04-03 15:05:57.000000 vdk-lineage-0.3.826474487/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 15:06:05.966601 vdk-lineage-0.3.826474487/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 15:06:05.966601 vdk-lineage-0.3.826474487/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 15:06:05.966601 vdk-lineage-0.3.826474487/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 15:06:05.966601 vdk-lineage-0.3.826474487/src/vdk/plugin/lineage/
--rw-rw-rw-   0 root         (0) root         (0)      974 2023-04-03 15:05:54.000000 vdk-lineage-0.3.826474487/src/vdk/plugin/lineage/openlineage_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2764 2023-04-03 15:05:54.000000 vdk-lineage-0.3.826474487/src/vdk/plugin/lineage/openlineage_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6574 2023-04-03 15:05:54.000000 vdk-lineage-0.3.826474487/src/vdk/plugin/lineage/plugin_lineage.py
--rw-rw-rw-   0 root         (0) root         (0)     3175 2023-04-03 15:05:54.000000 vdk-lineage-0.3.826474487/src/vdk/plugin/lineage/sql_lineage_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 15:06:05.966601 vdk-lineage-0.3.826474487/src/vdk/plugin/marquez/
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-04-03 15:05:54.000000 vdk-lineage-0.3.826474487/src/vdk/plugin/marquez/.env
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 15:06:05.966601 vdk-lineage-0.3.826474487/src/vdk/plugin/marquez/docker/
--rwxrwxrwx   0 root         (0) root         (0)      402 2023-04-03 15:05:54.000000 vdk-lineage-0.3.826474487/src/vdk/plugin/marquez/docker/init-db.sh
--rwxrwxrwx   0 root         (0) root         (0)     5136 2023-04-03 15:05:54.000000 vdk-lineage-0.3.826474487/src/vdk/plugin/marquez/docker/wait-for-it.sh
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-04-03 15:05:54.000000 vdk-lineage-0.3.826474487/src/vdk/plugin/marquez/docker-compose.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-04-03 15:05:54.000000 vdk-lineage-0.3.826474487/src/vdk/plugin/marquez/marquez_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2470 2023-04-03 15:05:54.000000 vdk-lineage-0.3.826474487/src/vdk/plugin/marquez/marquez_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 15:06:05.966601 vdk-lineage-0.3.826474487/src/vdk_lineage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2138 2023-04-03 15:06:05.000000 vdk-lineage-0.3.826474487/src/vdk_lineage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      742 2023-04-03 15:06:05.000000 vdk-lineage-0.3.826474487/src/vdk_lineage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 15:06:05.000000 vdk-lineage-0.3.826474487/src/vdk_lineage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      113 2023-04-03 15:06:05.000000 vdk-lineage-0.3.826474487/src/vdk_lineage.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2023-04-03 15:06:05.000000 vdk-lineage-0.3.826474487/src/vdk_lineage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-03 15:06:05.000000 vdk-lineage-0.3.826474487/src/vdk_lineage.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 15:06:05.966601 vdk-lineage-0.3.826474487/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1887 2023-04-03 15:05:54.000000 vdk-lineage-0.3.826474487/tests/test_plugin_lineage.py
--rw-rw-rw-   0 root         (0) root         (0)     3900 2023-04-03 15:05:54.000000 vdk-lineage-0.3.826474487/tests/test_sql_lineage_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:44.758532 vdk-lineage-0.3.948436673/
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-28 09:42:22.000000 vdk-lineage-0.3.948436673/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-07-28 09:42:44.758532 vdk-lineage-0.3.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-07-28 09:42:22.000000 vdk-lineage-0.3.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:42:44.758532 vdk-lineage-0.3.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2023-07-28 09:42:31.000000 vdk-lineage-0.3.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:44.754532 vdk-lineage-0.3.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:44.754532 vdk-lineage-0.3.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:44.754532 vdk-lineage-0.3.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:44.754532 vdk-lineage-0.3.948436673/src/vdk/plugin/lineage/
+-rw-rw-rw-   0 root         (0) root         (0)      974 2023-07-28 09:42:22.000000 vdk-lineage-0.3.948436673/src/vdk/plugin/lineage/openlineage_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2764 2023-07-28 09:42:22.000000 vdk-lineage-0.3.948436673/src/vdk/plugin/lineage/openlineage_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6574 2023-07-28 09:42:22.000000 vdk-lineage-0.3.948436673/src/vdk/plugin/lineage/plugin_lineage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3175 2023-07-28 09:42:22.000000 vdk-lineage-0.3.948436673/src/vdk/plugin/lineage/sql_lineage_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:44.754532 vdk-lineage-0.3.948436673/src/vdk/plugin/marquez/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-07-28 09:42:22.000000 vdk-lineage-0.3.948436673/src/vdk/plugin/marquez/.env
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:44.758532 vdk-lineage-0.3.948436673/src/vdk/plugin/marquez/docker/
+-rwxrwxrwx   0 root         (0) root         (0)      402 2023-07-28 09:42:22.000000 vdk-lineage-0.3.948436673/src/vdk/plugin/marquez/docker/init-db.sh
+-rwxrwxrwx   0 root         (0) root         (0)     5136 2023-07-28 09:42:22.000000 vdk-lineage-0.3.948436673/src/vdk/plugin/marquez/docker/wait-for-it.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-07-28 09:42:22.000000 vdk-lineage-0.3.948436673/src/vdk/plugin/marquez/docker-compose.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-07-28 09:42:22.000000 vdk-lineage-0.3.948436673/src/vdk/plugin/marquez/marquez_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2470 2023-07-28 09:42:22.000000 vdk-lineage-0.3.948436673/src/vdk/plugin/marquez/marquez_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:44.758532 vdk-lineage-0.3.948436673/src/vdk_lineage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-07-28 09:42:44.000000 vdk-lineage-0.3.948436673/src/vdk_lineage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      742 2023-07-28 09:42:44.000000 vdk-lineage-0.3.948436673/src/vdk_lineage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:44.000000 vdk-lineage-0.3.948436673/src/vdk_lineage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-28 09:42:44.000000 vdk-lineage-0.3.948436673/src/vdk_lineage.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2023-07-28 09:42:44.000000 vdk-lineage-0.3.948436673/src/vdk_lineage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:42:44.000000 vdk-lineage-0.3.948436673/src/vdk_lineage.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:44.758532 vdk-lineage-0.3.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1887 2023-07-28 09:42:22.000000 vdk-lineage-0.3.948436673/tests/test_plugin_lineage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3900 2023-07-28 09:42:22.000000 vdk-lineage-0.3.948436673/tests/test_sql_lineage_parser.py
```

### Comparing `vdk-lineage-0.3.826474487/PKG-INFO` & `vdk-lineage-0.3.948436673/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-lineage
-Version: 0.3.826474487
+Version: 0.3.948436673
 Summary: VDK Lineage plugin collects lineage (input -> job -> output) information and send it to a pre-configured destination.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-lineage-0.3.826474487/README.md` & `vdk-lineage-0.3.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-lineage-0.3.826474487/setup.py` & `vdk-lineage-0.3.948436673/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.3.826474487"
+__version__ = "0.3.948436673"
 
 setuptools.setup(
     name="vdk-lineage",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="VDK Lineage plugin collects lineage (input -> job -> output) information "
     "and send it to a pre-configured destination.",
```

### Comparing `vdk-lineage-0.3.826474487/src/vdk/plugin/lineage/openlineage_config.py` & `vdk-lineage-0.3.948436673/src/vdk/plugin/lineage/openlineage_config.py`

 * *Files identical despite different names*

### Comparing `vdk-lineage-0.3.826474487/src/vdk/plugin/lineage/openlineage_utils.py` & `vdk-lineage-0.3.948436673/src/vdk/plugin/lineage/openlineage_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-lineage-0.3.826474487/src/vdk/plugin/lineage/plugin_lineage.py` & `vdk-lineage-0.3.948436673/src/vdk/plugin/lineage/plugin_lineage.py`

 * *Files identical despite different names*

### Comparing `vdk-lineage-0.3.826474487/src/vdk/plugin/lineage/sql_lineage_parser.py` & `vdk-lineage-0.3.948436673/src/vdk/plugin/lineage/sql_lineage_parser.py`

 * *Files identical despite different names*

### Comparing `vdk-lineage-0.3.826474487/src/vdk/plugin/marquez/docker/wait-for-it.sh` & `vdk-lineage-0.3.948436673/src/vdk/plugin/marquez/docker/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `vdk-lineage-0.3.826474487/src/vdk/plugin/marquez/docker-compose.yaml` & `vdk-lineage-0.3.948436673/src/vdk/plugin/marquez/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `vdk-lineage-0.3.826474487/src/vdk/plugin/marquez/marquez_plugin.py` & `vdk-lineage-0.3.948436673/src/vdk/plugin/marquez/marquez_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-lineage-0.3.826474487/src/vdk/plugin/marquez/marquez_server.py` & `vdk-lineage-0.3.948436673/src/vdk/plugin/marquez/marquez_server.py`

 * *Files identical despite different names*

### Comparing `vdk-lineage-0.3.826474487/src/vdk_lineage.egg-info/PKG-INFO` & `vdk-lineage-0.3.948436673/src/vdk_lineage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-lineage
-Version: 0.3.826474487
+Version: 0.3.948436673
 Summary: VDK Lineage plugin collects lineage (input -> job -> output) information and send it to a pre-configured destination.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-lineage-0.3.826474487/src/vdk_lineage.egg-info/SOURCES.txt` & `vdk-lineage-0.3.948436673/src/vdk_lineage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-lineage-0.3.826474487/tests/test_plugin_lineage.py` & `vdk-lineage-0.3.948436673/tests/test_plugin_lineage.py`

 * *Files identical despite different names*

### Comparing `vdk-lineage-0.3.826474487/tests/test_sql_lineage_parser.py` & `vdk-lineage-0.3.948436673/tests/test_sql_lineage_parser.py`

 * *Files identical despite different names*

