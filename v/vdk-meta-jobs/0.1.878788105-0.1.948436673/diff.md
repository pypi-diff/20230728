# Comparing `tmp/vdk-meta-jobs-0.1.878788105.tar.gz` & `tmp/vdk-meta-jobs-0.1.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-meta-jobs-0.1.878788105.tar", last modified: Thu May 25 10:48:22 2023, max compression
+gzip compressed data, was "vdk-meta-jobs-0.1.948436673.tar", last modified: Fri Jul 28 09:43:42 2023, max compression
```

## Comparing `vdk-meta-jobs-0.1.878788105.tar` & `vdk-meta-jobs-0.1.948436673.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.422975 vdk-meta-jobs-0.1.878788105/
--rw-r--r--   0 root         (0) root         (0)     8391 2023-05-25 10:48:22.422975 vdk-meta-jobs-0.1.878788105/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7818 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 10:48:22.422975 vdk-meta-jobs-0.1.878788105/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1456 2023-05-25 10:48:12.000000 vdk-meta-jobs-0.1.878788105/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.418975 vdk-meta-jobs-0.1.878788105/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.418975 vdk-meta-jobs-0.1.878788105/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.418975 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.418975 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.418975 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/api/
--rw-rw-rw-   0 root         (0) root         (0)     1402 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/api/meta_job.py
--rw-rw-rw-   0 root         (0) root         (0)     9347 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/cached_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     7949 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/dag_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/dags_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2269 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     6713 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     6148 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta_dag.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta_job_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     9346 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/remote_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1743 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/remote_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     2579 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/time_based_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.418975 vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8391 2023-05-25 10:48:22.000000 vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      858 2023-05-25 10:48:22.000000 vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 10:48:22.000000 vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-05-25 10:48:22.000000 vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-25 10:48:22.000000 vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-25 10:48:22.000000 vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.422975 vdk-meta-jobs-0.1.878788105/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2624 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/tests/test_meta_dag.py
--rw-rw-rw-   0 root         (0) root         (0)    15690 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/tests/test_meta_job.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/tests/test_time_based_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2303 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/tests/test_tracking_job_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:42.457878 vdk-meta-jobs-0.1.948436673/
+-rw-r--r--   0 root         (0) root         (0)     8391 2023-07-28 09:43:42.457878 vdk-meta-jobs-0.1.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7818 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:43:42.457878 vdk-meta-jobs-0.1.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2023-07-28 09:43:29.000000 vdk-meta-jobs-0.1.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:42.449878 vdk-meta-jobs-0.1.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:42.449878 vdk-meta-jobs-0.1.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:42.449878 vdk-meta-jobs-0.1.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:42.453878 vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:42.453878 vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1402 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/api/meta_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     9347 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/cached_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7949 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/dag_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/dags_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2269 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     6713 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/meta_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     6148 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/meta_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/meta_job_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     9346 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/remote_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1743 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/remote_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2579 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/time_based_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:42.453878 vdk-meta-jobs-0.1.948436673/src/vdk_meta_jobs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8391 2023-07-28 09:43:42.000000 vdk-meta-jobs-0.1.948436673/src/vdk_meta_jobs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      858 2023-07-28 09:43:42.000000 vdk-meta-jobs-0.1.948436673/src/vdk_meta_jobs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:43:42.000000 vdk-meta-jobs-0.1.948436673/src/vdk_meta_jobs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-28 09:43:42.000000 vdk-meta-jobs-0.1.948436673/src/vdk_meta_jobs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-28 09:43:42.000000 vdk-meta-jobs-0.1.948436673/src/vdk_meta_jobs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:43:42.000000 vdk-meta-jobs-0.1.948436673/src/vdk_meta_jobs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:42.453878 vdk-meta-jobs-0.1.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/tests/test_meta_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)    15690 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/tests/test_meta_job.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/tests/test_time_based_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2303 2023-07-28 09:43:19.000000 vdk-meta-jobs-0.1.948436673/tests/test_tracking_job_executor.py
```

### Comparing `vdk-meta-jobs-0.1.878788105/PKG-INFO` & `vdk-meta-jobs-0.1.948436673/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-meta-jobs
-Version: 0.1.878788105
+Version: 0.1.948436673
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-meta-jobs-0.1.878788105/README.md` & `vdk-meta-jobs-0.1.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/setup.py` & `vdk-meta-jobs-0.1.948436673/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.878788105"
+__version__ = "0.1.948436673"
 
 setuptools.setup(
     name="vdk-meta-jobs",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Express dependecies between data jobs.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/api/meta_job.py` & `vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/api/meta_job.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/cached_data_job_executor.py` & `vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/cached_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/dag_validator.py` & `vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/dag_validator.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/dags_plugin.py` & `vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/dags_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta.py` & `vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/meta.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta_configuration.py` & `vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/meta_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta_dag.py` & `vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/meta_dag.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta_job_runner.py` & `vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/meta_job_runner.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/remote_data_job.py` & `vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/remote_data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/remote_data_job_executor.py` & `vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/remote_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/time_based_queue.py` & `vdk-meta-jobs-0.1.948436673/src/vdk/plugin/meta_jobs/time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/PKG-INFO` & `vdk-meta-jobs-0.1.948436673/src/vdk_meta_jobs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-meta-jobs
-Version: 0.1.878788105
+Version: 0.1.948436673
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/SOURCES.txt` & `vdk-meta-jobs-0.1.948436673/src/vdk_meta_jobs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/tests/test_meta_dag.py` & `vdk-meta-jobs-0.1.948436673/tests/test_meta_dag.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/tests/test_meta_job.py` & `vdk-meta-jobs-0.1.948436673/tests/test_meta_job.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/tests/test_time_based_queue.py` & `vdk-meta-jobs-0.1.948436673/tests/test_time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.878788105/tests/test_tracking_job_executor.py` & `vdk-meta-jobs-0.1.948436673/tests/test_tracking_job_executor.py`

 * *Files identical despite different names*

