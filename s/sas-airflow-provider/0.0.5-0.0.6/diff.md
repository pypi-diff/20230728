# Comparing `tmp/sas-airflow-provider-0.0.5.tar.gz` & `tmp/sas-airflow-provider-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sas-airflow-provider/sas-airflow-provider/dist/.tmp-9djbkkx6/sas-airflow-provider-0.0.5.tar", last modified: Fri Jul 14 19:48:01 2023, max compression
+gzip compressed data, was "/home/runner/work/sas-airflow-provider/sas-airflow-provider/dist/.tmp-gmcu142n/sas-airflow-provider-0.0.6.tar", last modified: Fri Jul 28 17:39:23 2023, max compression
```

## Comparing `sas-airflow-provider-0.0.5.tar` & `sas-airflow-provider-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/example_sas_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/example_studio_advanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/example_templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/hooks/sas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/sas_create_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/sas_jobexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)    12575 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/sas_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/sas_studioflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/util/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_sas_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_studio_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/hooks/sas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_create_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_jobexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_studioflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/top_level.txt
```

### Comparing `sas-airflow-provider-0.0.5/LICENSE` & `sas-airflow-provider-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.5/PKG-INFO` & `sas-airflow-provider-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sas-airflow-provider
-Version: 0.0.5
+Version: 0.0.6
 Summary: Enables execution of Studio Flows and Jobs from Airflow
 Home-page: https://github.com/sassoftware/sas-airflow-provider
 Author: SAS
 Author-email: andrew.shakinovsky@sas.com
 Project-URL: Bug Tracker, https://github.com/sassoftware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sas-airflow-provider-0.0.5/README.md` & `sas-airflow-provider-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.5/setup.cfg` & `sas-airflow-provider-0.0.6/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sas-airflow-provider
-version = 0.0.5
+version = 0.0.6
 author = SAS
 author_email = andrew.shakinovsky@sas.com
 description = Enables execution of Studio Flows and Jobs from Airflow
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sassoftware/sas-airflow-provider
 project_urls =
```

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/__init__.py` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/example_sas_studio.py` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_sas_studio.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/example_studio_advanced.py` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_studio_advanced.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/example_templating.py` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_templating.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider/hooks/__init__.py` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider/hooks/sas.py` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider/hooks/sas.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/__init__.py` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/sas_create_session.py` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_create_session.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/sas_jobexecution.py` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_jobexecution.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/sas_studio.py` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_studio.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,21 +185,21 @@
                 self.env_vars[x] = v
 
     def _get_pre_code(self):
 
         pre_code = ""
         if self.env_vars:
             self.log.info(f"Adding {len(self.env_vars)} environment variables to code")
-            pre_code = "/** Begin environment variables **/\n"
+            pre_code += "/** Begin environment variables **/\n"
             for k, v in self.env_vars.items():
                 pre_code += f"OPTIONS SET={k}='{v}';\n"
             pre_code += "/** End environment variables **/\n\n"
         if self.macro_vars:
             self.log.info(f"Adding {len(self.macro_vars)} macro variables to code")
-            pre_code = "/** Begin macro variables **/\n"
+            pre_code += "/** Begin macro variables **/\n"
             for k, v in self.macro_vars.items():
                 pre_code += f"%LET {k} = {v};\n"
             pre_code += "/** End macro variables **/\n\n"
         return pre_code
 
     def _generate_object_code(self):
```

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/sas_studioflow.py` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_studioflow.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider/util/__init__.py` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider/util/util.py` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider/util/util.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/PKG-INFO` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sas-airflow-provider
-Version: 0.0.5
+Version: 0.0.6
 Summary: Enables execution of Studio Flows and Jobs from Airflow
 Home-page: https://github.com/sassoftware/sas-airflow-provider
 Author: SAS
 Author-email: andrew.shakinovsky@sas.com
 Project-URL: Bug Tracker, https://github.com/sassoftware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/SOURCES.txt` & `sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

