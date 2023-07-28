# Comparing `tmp/mypy-boto3-emr-serverless-1.28.12.tar.gz` & `tmp/mypy-boto3-emr-serverless-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-serverless-1.28.12.tar", last modified: Thu Jul 27 05:34:40 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-serverless-1.28.15.tar", last modified: Fri Jul 28 20:42:47 2023, max compression
```

## Comparing `mypy-boto3-emr-serverless-1.28.12.tar` & `mypy-boto3-emr-serverless-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.304515 mypy-boto3-emr-serverless-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15581 2023-07-27 05:34:40.304515 mypy-boto3-emr-serverless-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14067 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.304515 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26557 2023-07-27 05:22:04.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26508 2023-07-27 05:22:03.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.304515 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15581 2023-07-27 05:34:40.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:34:40.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:40.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:40.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:40.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:40.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:40.304515 mypy-boto3-emr-serverless-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.081086 mypy-boto3-emr-serverless-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15266 2023-07-28 20:42:47.081086 mypy-boto3-emr-serverless-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.077087 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-28 20:25:32.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-28 20:25:32.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-28 20:25:32.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-07-28 20:25:32.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-28 20:25:32.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-28 20:25:32.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23608 2023-07-28 20:25:33.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23567 2023-07-28 20:25:32.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.081086 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15266 2023-07-28 20:42:46.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:42:46.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:46.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:42:46.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:47.081086 mypy-boto3-emr-serverless-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/setup.py
```

### Comparing `mypy-boto3-emr-serverless-1.28.12/LICENSE` & `mypy-boto3-emr-serverless-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.12/PKG-INFO` & `mypy-boto3-emr-serverless-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.28.12
-Summary: Type annotations for boto3.EMRServerless 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.EMRServerless 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-serverless)](https://pepy.tech/project/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,70 +326,62 @@
 
 `mypy_boto3_emr_serverless.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_serverless.type_defs import (
     ApplicationSummaryTypeDef,
-    AutoStartConfigOutputTypeDef,
-    AutoStopConfigOutputTypeDef,
-    ImageConfigurationTypeDef,
-    MaximumAllowedResourcesOutputTypeDef,
-    NetworkConfigurationOutputTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
+    ImageConfigurationTypeDef,
+    MaximumAllowedResourcesTypeDef,
+    NetworkConfigurationOutputTypeDef,
     CancelJobRunRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
+    ResponseMetadataTypeDef,
     CloudWatchLoggingConfigurationOutputTypeDef,
     CloudWatchLoggingConfigurationTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ImageConfigurationInputTypeDef,
-    MaximumAllowedResourcesTypeDef,
     NetworkConfigurationTypeDef,
-    CreateApplicationResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
     GetJobRunRequestRequestTypeDef,
-    HiveOutputTypeDef,
     HiveTypeDef,
-    WorkerResourceConfigOutputTypeDef,
     WorkerResourceConfigTypeDef,
     SparkSubmitOutputTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
     ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ManagedPersistenceMonitoringConfigurationOutputTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
-    S3MonitoringConfigurationOutputTypeDef,
     S3MonitoringConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
-    StartJobRunResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListApplicationsResponseTypeDef,
     WorkerTypeSpecificationTypeDef,
+    CancelJobRunResponseTypeDef,
+    CreateApplicationResponseTypeDef,
+    GetDashboardForJobRunResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartJobRunResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
-    InitialCapacityConfigOutputTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
     MonitoringConfigurationOutputTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
```

### Comparing `mypy-boto3-emr-serverless-1.28.12/README.md` & `mypy-boto3-emr-serverless-1.28.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-serverless)](https://pepy.tech/project/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -294,70 +294,62 @@
 
 `mypy_boto3_emr_serverless.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_serverless.type_defs import (
     ApplicationSummaryTypeDef,
-    AutoStartConfigOutputTypeDef,
-    AutoStopConfigOutputTypeDef,
-    ImageConfigurationTypeDef,
-    MaximumAllowedResourcesOutputTypeDef,
-    NetworkConfigurationOutputTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
+    ImageConfigurationTypeDef,
+    MaximumAllowedResourcesTypeDef,
+    NetworkConfigurationOutputTypeDef,
     CancelJobRunRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
+    ResponseMetadataTypeDef,
     CloudWatchLoggingConfigurationOutputTypeDef,
     CloudWatchLoggingConfigurationTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ImageConfigurationInputTypeDef,
-    MaximumAllowedResourcesTypeDef,
     NetworkConfigurationTypeDef,
-    CreateApplicationResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
     GetJobRunRequestRequestTypeDef,
-    HiveOutputTypeDef,
     HiveTypeDef,
-    WorkerResourceConfigOutputTypeDef,
     WorkerResourceConfigTypeDef,
     SparkSubmitOutputTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
     ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ManagedPersistenceMonitoringConfigurationOutputTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
-    S3MonitoringConfigurationOutputTypeDef,
     S3MonitoringConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
-    StartJobRunResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListApplicationsResponseTypeDef,
     WorkerTypeSpecificationTypeDef,
+    CancelJobRunResponseTypeDef,
+    CreateApplicationResponseTypeDef,
+    GetDashboardForJobRunResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartJobRunResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
-    InitialCapacityConfigOutputTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
     MonitoringConfigurationOutputTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
```

### Comparing `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/__init__.py` & `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/__init__.pyi` & `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/__main__.py` & `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRServerless 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.EMRServerless 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.15")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/client.py` & `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/client.pyi` & `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/literals.py` & `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/literals.pyi` & `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/paginator.py` & `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         states: Sequence[ApplicationStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
         """
 
 
@@ -73,13 +73,13 @@
     def paginate(
         self,
         *,
         applicationId: str,
         createdAtAfter: Union[datetime, str] = ...,
         createdAtBefore: Union[datetime, str] = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/paginator.pyi` & `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         states: Sequence[ApplicationStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
         """
 
 class ListJobRunsPaginator(Paginator):
@@ -69,13 +69,13 @@
     def paginate(
         self,
         *,
         applicationId: str,
         createdAtAfter: Union[datetime, str] = ...,
         createdAtBefore: Union[datetime, str] = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/type_defs.py` & `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,70 +21,62 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ApplicationSummaryTypeDef",
-    "AutoStartConfigOutputTypeDef",
-    "AutoStopConfigOutputTypeDef",
-    "ImageConfigurationTypeDef",
-    "MaximumAllowedResourcesOutputTypeDef",
-    "NetworkConfigurationOutputTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
+    "ImageConfigurationTypeDef",
+    "MaximumAllowedResourcesTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "CancelJobRunRequestRequestTypeDef",
-    "CancelJobRunResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CloudWatchLoggingConfigurationOutputTypeDef",
     "CloudWatchLoggingConfigurationTypeDef",
     "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ImageConfigurationInputTypeDef",
-    "MaximumAllowedResourcesTypeDef",
     "NetworkConfigurationTypeDef",
-    "CreateApplicationResponseTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
-    "GetDashboardForJobRunResponseTypeDef",
     "GetJobRunRequestRequestTypeDef",
-    "HiveOutputTypeDef",
     "HiveTypeDef",
-    "WorkerResourceConfigOutputTypeDef",
     "WorkerResourceConfigTypeDef",
     "SparkSubmitOutputTypeDef",
     "SparkSubmitTypeDef",
     "JobRunSummaryTypeDef",
     "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ManagedPersistenceMonitoringConfigurationOutputTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
-    "S3MonitoringConfigurationOutputTypeDef",
     "S3MonitoringConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
-    "StartJobRunResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListApplicationsResponseTypeDef",
     "WorkerTypeSpecificationTypeDef",
+    "CancelJobRunResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "GetDashboardForJobRunResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartJobRunResponseTypeDef",
     "WorkerTypeSpecificationInputTypeDef",
-    "InitialCapacityConfigOutputTypeDef",
     "InitialCapacityConfigTypeDef",
     "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "MonitoringConfigurationOutputTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
@@ -120,24 +112,24 @@
 
 class ApplicationSummaryTypeDef(
     _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
 ):
     pass
 
 
-AutoStartConfigOutputTypeDef = TypedDict(
-    "AutoStartConfigOutputTypeDef",
+AutoStartConfigTypeDef = TypedDict(
+    "AutoStartConfigTypeDef",
     {
         "enabled": bool,
     },
     total=False,
 )
 
-AutoStopConfigOutputTypeDef = TypedDict(
-    "AutoStopConfigOutputTypeDef",
+AutoStopConfigTypeDef = TypedDict(
+    "AutoStopConfigTypeDef",
     {
         "enabled": bool,
         "idleTimeoutMinutes": int,
     },
     total=False,
 )
 
@@ -158,76 +150,61 @@
 
 class ImageConfigurationTypeDef(
     _RequiredImageConfigurationTypeDef, _OptionalImageConfigurationTypeDef
 ):
     pass
 
 
-_RequiredMaximumAllowedResourcesOutputTypeDef = TypedDict(
-    "_RequiredMaximumAllowedResourcesOutputTypeDef",
+_RequiredMaximumAllowedResourcesTypeDef = TypedDict(
+    "_RequiredMaximumAllowedResourcesTypeDef",
     {
         "cpu": str,
         "memory": str,
     },
 )
-_OptionalMaximumAllowedResourcesOutputTypeDef = TypedDict(
-    "_OptionalMaximumAllowedResourcesOutputTypeDef",
+_OptionalMaximumAllowedResourcesTypeDef = TypedDict(
+    "_OptionalMaximumAllowedResourcesTypeDef",
     {
         "disk": str,
     },
     total=False,
 )
 
 
-class MaximumAllowedResourcesOutputTypeDef(
-    _RequiredMaximumAllowedResourcesOutputTypeDef, _OptionalMaximumAllowedResourcesOutputTypeDef
+class MaximumAllowedResourcesTypeDef(
+    _RequiredMaximumAllowedResourcesTypeDef, _OptionalMaximumAllowedResourcesTypeDef
 ):
     pass
 
 
 NetworkConfigurationOutputTypeDef = TypedDict(
     "NetworkConfigurationOutputTypeDef",
     {
         "subnetIds": List[str],
         "securityGroupIds": List[str],
     },
     total=False,
 )
 
-AutoStartConfigTypeDef = TypedDict(
-    "AutoStartConfigTypeDef",
-    {
-        "enabled": bool,
-    },
-    total=False,
-)
-
-AutoStopConfigTypeDef = TypedDict(
-    "AutoStopConfigTypeDef",
-    {
-        "enabled": bool,
-        "idleTimeoutMinutes": int,
-    },
-    total=False,
-)
-
 CancelJobRunRequestRequestTypeDef = TypedDict(
     "CancelJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-CancelJobRunResponseTypeDef = TypedDict(
-    "CancelJobRunResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "applicationId": str,
-        "jobRunId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCloudWatchLoggingConfigurationOutputTypeDef = TypedDict(
     "_RequiredCloudWatchLoggingConfigurationOutputTypeDef",
     {
         "enabled": bool,
@@ -322,55 +299,23 @@
     "ImageConfigurationInputTypeDef",
     {
         "imageUri": str,
     },
     total=False,
 )
 
-_RequiredMaximumAllowedResourcesTypeDef = TypedDict(
-    "_RequiredMaximumAllowedResourcesTypeDef",
-    {
-        "cpu": str,
-        "memory": str,
-    },
-)
-_OptionalMaximumAllowedResourcesTypeDef = TypedDict(
-    "_OptionalMaximumAllowedResourcesTypeDef",
-    {
-        "disk": str,
-    },
-    total=False,
-)
-
-
-class MaximumAllowedResourcesTypeDef(
-    _RequiredMaximumAllowedResourcesTypeDef, _OptionalMaximumAllowedResourcesTypeDef
-):
-    pass
-
-
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "subnetIds": Sequence[str],
         "securityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "applicationId": str,
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -385,50 +330,22 @@
     "GetDashboardForJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-GetDashboardForJobRunResponseTypeDef = TypedDict(
-    "GetDashboardForJobRunResponseTypeDef",
-    {
-        "url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetJobRunRequestRequestTypeDef = TypedDict(
     "GetJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-_RequiredHiveOutputTypeDef = TypedDict(
-    "_RequiredHiveOutputTypeDef",
-    {
-        "query": str,
-    },
-)
-_OptionalHiveOutputTypeDef = TypedDict(
-    "_OptionalHiveOutputTypeDef",
-    {
-        "initQueryFile": str,
-        "parameters": str,
-    },
-    total=False,
-)
-
-
-class HiveOutputTypeDef(_RequiredHiveOutputTypeDef, _OptionalHiveOutputTypeDef):
-    pass
-
-
 _RequiredHiveTypeDef = TypedDict(
     "_RequiredHiveTypeDef",
     {
         "query": str,
     },
 )
 _OptionalHiveTypeDef = TypedDict(
@@ -441,36 +358,14 @@
 )
 
 
 class HiveTypeDef(_RequiredHiveTypeDef, _OptionalHiveTypeDef):
     pass
 
 
-_RequiredWorkerResourceConfigOutputTypeDef = TypedDict(
-    "_RequiredWorkerResourceConfigOutputTypeDef",
-    {
-        "cpu": str,
-        "memory": str,
-    },
-)
-_OptionalWorkerResourceConfigOutputTypeDef = TypedDict(
-    "_OptionalWorkerResourceConfigOutputTypeDef",
-    {
-        "disk": str,
-    },
-    total=False,
-)
-
-
-class WorkerResourceConfigOutputTypeDef(
-    _RequiredWorkerResourceConfigOutputTypeDef, _OptionalWorkerResourceConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredWorkerResourceConfigTypeDef = TypedDict(
     "_RequiredWorkerResourceConfigTypeDef",
     {
         "cpu": str,
         "memory": str,
     },
 )
@@ -576,58 +471,34 @@
         "vCPUHour": float,
         "memoryGBHour": float,
         "storageGBHour": float,
     },
     total=False,
 )
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "states": Sequence[ApplicationStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "states": Sequence[ApplicationStateType],
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
-        "states": Sequence[JobRunStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListJobRunsRequestListJobRunsPaginateTypeDef(
-    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
-    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -652,96 +523,39 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ManagedPersistenceMonitoringConfigurationOutputTypeDef = TypedDict(
-    "ManagedPersistenceMonitoringConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-        "encryptionKeyArn": str,
-    },
-    total=False,
-)
-
 ManagedPersistenceMonitoringConfigurationTypeDef = TypedDict(
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     {
         "enabled": bool,
         "encryptionKeyArn": str,
     },
     total=False,
 )
 
-S3MonitoringConfigurationOutputTypeDef = TypedDict(
-    "S3MonitoringConfigurationOutputTypeDef",
-    {
-        "logUri": str,
-        "encryptionKeyArn": str,
-    },
-    total=False,
-)
-
 S3MonitoringConfigurationTypeDef = TypedDict(
     "S3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
         "encryptionKeyArn": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
-    {
-        "applicationId": str,
-        "jobRunId": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopApplicationRequestRequestTypeDef = TypedDict(
     "StopApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -757,59 +571,83 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-ListApplicationsResponseTypeDef = TypedDict(
-    "ListApplicationsResponseTypeDef",
-    {
-        "applications": List[ApplicationSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkerTypeSpecificationTypeDef = TypedDict(
     "WorkerTypeSpecificationTypeDef",
     {
         "imageConfiguration": ImageConfigurationTypeDef,
     },
     total=False,
 )
 
-WorkerTypeSpecificationInputTypeDef = TypedDict(
-    "WorkerTypeSpecificationInputTypeDef",
+CancelJobRunResponseTypeDef = TypedDict(
+    "CancelJobRunResponseTypeDef",
     {
-        "imageConfiguration": ImageConfigurationInputTypeDef,
+        "applicationId": str,
+        "jobRunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "applicationId": str,
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredInitialCapacityConfigOutputTypeDef = TypedDict(
-    "_RequiredInitialCapacityConfigOutputTypeDef",
+GetDashboardForJobRunResponseTypeDef = TypedDict(
+    "GetDashboardForJobRunResponseTypeDef",
     {
-        "workerCount": int,
+        "url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalInitialCapacityConfigOutputTypeDef = TypedDict(
-    "_OptionalInitialCapacityConfigOutputTypeDef",
+
+ListApplicationsResponseTypeDef = TypedDict(
+    "ListApplicationsResponseTypeDef",
     {
-        "workerConfiguration": WorkerResourceConfigOutputTypeDef,
+        "applications": List[ApplicationSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class InitialCapacityConfigOutputTypeDef(
-    _RequiredInitialCapacityConfigOutputTypeDef, _OptionalInitialCapacityConfigOutputTypeDef
-):
-    pass
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
+    {
+        "applicationId": str,
+        "jobRunId": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+WorkerTypeSpecificationInputTypeDef = TypedDict(
+    "WorkerTypeSpecificationInputTypeDef",
+    {
+        "imageConfiguration": ImageConfigurationInputTypeDef,
+    },
+    total=False,
+)
 
 _RequiredInitialCapacityConfigTypeDef = TypedDict(
     "_RequiredInitialCapacityConfigTypeDef",
     {
         "workerCount": int,
     },
 )
@@ -828,15 +666,15 @@
     pass
 
 
 JobDriverOutputTypeDef = TypedDict(
     "JobDriverOutputTypeDef",
     {
         "sparkSubmit": SparkSubmitOutputTypeDef,
-        "hive": HiveOutputTypeDef,
+        "hive": HiveTypeDef,
     },
     total=False,
 )
 
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
@@ -847,24 +685,58 @@
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "jobRuns": List[JobRunSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "states": Sequence[ApplicationStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "createdAtAfter": Union[datetime, str],
+        "createdAtBefore": Union[datetime, str],
+        "states": Sequence[JobRunStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListJobRunsRequestListJobRunsPaginateTypeDef(
+    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
+    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
+):
+    pass
+
+
 MonitoringConfigurationOutputTypeDef = TypedDict(
     "MonitoringConfigurationOutputTypeDef",
     {
-        "s3MonitoringConfiguration": S3MonitoringConfigurationOutputTypeDef,
+        "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "managedPersistenceMonitoringConfiguration": (
-            ManagedPersistenceMonitoringConfigurationOutputTypeDef
+            ManagedPersistenceMonitoringConfigurationTypeDef
         ),
         "cloudWatchLoggingConfiguration": CloudWatchLoggingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 MonitoringConfigurationTypeDef = TypedDict(
@@ -892,19 +764,19 @@
     },
 )
 _OptionalApplicationTypeDef = TypedDict(
     "_OptionalApplicationTypeDef",
     {
         "name": str,
         "stateDetails": str,
-        "initialCapacity": Dict[str, InitialCapacityConfigOutputTypeDef],
-        "maximumCapacity": MaximumAllowedResourcesOutputTypeDef,
+        "initialCapacity": Dict[str, InitialCapacityConfigTypeDef],
+        "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "tags": Dict[str, str],
-        "autoStartConfiguration": AutoStartConfigOutputTypeDef,
-        "autoStopConfiguration": AutoStopConfigOutputTypeDef,
+        "autoStartConfiguration": AutoStartConfigTypeDef,
+        "autoStopConfiguration": AutoStopConfigTypeDef,
         "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationTypeDef,
         "workerTypeSpecifications": Dict[str, WorkerTypeSpecificationTypeDef],
     },
     total=False,
 )
@@ -994,23 +866,23 @@
     total=False,
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJobRunTypeDef = TypedDict(
     "_RequiredJobRunTypeDef",
     {
         "applicationId": str,
@@ -1073,10 +945,10 @@
     pass
 
 
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "jobRun": JobRunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/type_defs.pyi` & `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -20,70 +20,62 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApplicationSummaryTypeDef",
-    "AutoStartConfigOutputTypeDef",
-    "AutoStopConfigOutputTypeDef",
-    "ImageConfigurationTypeDef",
-    "MaximumAllowedResourcesOutputTypeDef",
-    "NetworkConfigurationOutputTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
+    "ImageConfigurationTypeDef",
+    "MaximumAllowedResourcesTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "CancelJobRunRequestRequestTypeDef",
-    "CancelJobRunResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CloudWatchLoggingConfigurationOutputTypeDef",
     "CloudWatchLoggingConfigurationTypeDef",
     "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ImageConfigurationInputTypeDef",
-    "MaximumAllowedResourcesTypeDef",
     "NetworkConfigurationTypeDef",
-    "CreateApplicationResponseTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
-    "GetDashboardForJobRunResponseTypeDef",
     "GetJobRunRequestRequestTypeDef",
-    "HiveOutputTypeDef",
     "HiveTypeDef",
-    "WorkerResourceConfigOutputTypeDef",
     "WorkerResourceConfigTypeDef",
     "SparkSubmitOutputTypeDef",
     "SparkSubmitTypeDef",
     "JobRunSummaryTypeDef",
     "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ManagedPersistenceMonitoringConfigurationOutputTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
-    "S3MonitoringConfigurationOutputTypeDef",
     "S3MonitoringConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
-    "StartJobRunResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListApplicationsResponseTypeDef",
     "WorkerTypeSpecificationTypeDef",
+    "CancelJobRunResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "GetDashboardForJobRunResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartJobRunResponseTypeDef",
     "WorkerTypeSpecificationInputTypeDef",
-    "InitialCapacityConfigOutputTypeDef",
     "InitialCapacityConfigTypeDef",
     "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "MonitoringConfigurationOutputTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
@@ -117,24 +109,24 @@
 )
 
 class ApplicationSummaryTypeDef(
     _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
 ):
     pass
 
-AutoStartConfigOutputTypeDef = TypedDict(
-    "AutoStartConfigOutputTypeDef",
+AutoStartConfigTypeDef = TypedDict(
+    "AutoStartConfigTypeDef",
     {
         "enabled": bool,
     },
     total=False,
 )
 
-AutoStopConfigOutputTypeDef = TypedDict(
-    "AutoStopConfigOutputTypeDef",
+AutoStopConfigTypeDef = TypedDict(
+    "AutoStopConfigTypeDef",
     {
         "enabled": bool,
         "idleTimeoutMinutes": int,
     },
     total=False,
 )
 
@@ -153,74 +145,59 @@
 )
 
 class ImageConfigurationTypeDef(
     _RequiredImageConfigurationTypeDef, _OptionalImageConfigurationTypeDef
 ):
     pass
 
-_RequiredMaximumAllowedResourcesOutputTypeDef = TypedDict(
-    "_RequiredMaximumAllowedResourcesOutputTypeDef",
+_RequiredMaximumAllowedResourcesTypeDef = TypedDict(
+    "_RequiredMaximumAllowedResourcesTypeDef",
     {
         "cpu": str,
         "memory": str,
     },
 )
-_OptionalMaximumAllowedResourcesOutputTypeDef = TypedDict(
-    "_OptionalMaximumAllowedResourcesOutputTypeDef",
+_OptionalMaximumAllowedResourcesTypeDef = TypedDict(
+    "_OptionalMaximumAllowedResourcesTypeDef",
     {
         "disk": str,
     },
     total=False,
 )
 
-class MaximumAllowedResourcesOutputTypeDef(
-    _RequiredMaximumAllowedResourcesOutputTypeDef, _OptionalMaximumAllowedResourcesOutputTypeDef
+class MaximumAllowedResourcesTypeDef(
+    _RequiredMaximumAllowedResourcesTypeDef, _OptionalMaximumAllowedResourcesTypeDef
 ):
     pass
 
 NetworkConfigurationOutputTypeDef = TypedDict(
     "NetworkConfigurationOutputTypeDef",
     {
         "subnetIds": List[str],
         "securityGroupIds": List[str],
     },
     total=False,
 )
 
-AutoStartConfigTypeDef = TypedDict(
-    "AutoStartConfigTypeDef",
-    {
-        "enabled": bool,
-    },
-    total=False,
-)
-
-AutoStopConfigTypeDef = TypedDict(
-    "AutoStopConfigTypeDef",
-    {
-        "enabled": bool,
-        "idleTimeoutMinutes": int,
-    },
-    total=False,
-)
-
 CancelJobRunRequestRequestTypeDef = TypedDict(
     "CancelJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-CancelJobRunResponseTypeDef = TypedDict(
-    "CancelJobRunResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "applicationId": str,
-        "jobRunId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCloudWatchLoggingConfigurationOutputTypeDef = TypedDict(
     "_RequiredCloudWatchLoggingConfigurationOutputTypeDef",
     {
         "enabled": bool,
@@ -307,53 +284,23 @@
     "ImageConfigurationInputTypeDef",
     {
         "imageUri": str,
     },
     total=False,
 )
 
-_RequiredMaximumAllowedResourcesTypeDef = TypedDict(
-    "_RequiredMaximumAllowedResourcesTypeDef",
-    {
-        "cpu": str,
-        "memory": str,
-    },
-)
-_OptionalMaximumAllowedResourcesTypeDef = TypedDict(
-    "_OptionalMaximumAllowedResourcesTypeDef",
-    {
-        "disk": str,
-    },
-    total=False,
-)
-
-class MaximumAllowedResourcesTypeDef(
-    _RequiredMaximumAllowedResourcesTypeDef, _OptionalMaximumAllowedResourcesTypeDef
-):
-    pass
-
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "subnetIds": Sequence[str],
         "securityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "applicationId": str,
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -368,48 +315,22 @@
     "GetDashboardForJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-GetDashboardForJobRunResponseTypeDef = TypedDict(
-    "GetDashboardForJobRunResponseTypeDef",
-    {
-        "url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetJobRunRequestRequestTypeDef = TypedDict(
     "GetJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-_RequiredHiveOutputTypeDef = TypedDict(
-    "_RequiredHiveOutputTypeDef",
-    {
-        "query": str,
-    },
-)
-_OptionalHiveOutputTypeDef = TypedDict(
-    "_OptionalHiveOutputTypeDef",
-    {
-        "initQueryFile": str,
-        "parameters": str,
-    },
-    total=False,
-)
-
-class HiveOutputTypeDef(_RequiredHiveOutputTypeDef, _OptionalHiveOutputTypeDef):
-    pass
-
 _RequiredHiveTypeDef = TypedDict(
     "_RequiredHiveTypeDef",
     {
         "query": str,
     },
 )
 _OptionalHiveTypeDef = TypedDict(
@@ -420,34 +341,14 @@
     },
     total=False,
 )
 
 class HiveTypeDef(_RequiredHiveTypeDef, _OptionalHiveTypeDef):
     pass
 
-_RequiredWorkerResourceConfigOutputTypeDef = TypedDict(
-    "_RequiredWorkerResourceConfigOutputTypeDef",
-    {
-        "cpu": str,
-        "memory": str,
-    },
-)
-_OptionalWorkerResourceConfigOutputTypeDef = TypedDict(
-    "_OptionalWorkerResourceConfigOutputTypeDef",
-    {
-        "disk": str,
-    },
-    total=False,
-)
-
-class WorkerResourceConfigOutputTypeDef(
-    _RequiredWorkerResourceConfigOutputTypeDef, _OptionalWorkerResourceConfigOutputTypeDef
-):
-    pass
-
 _RequiredWorkerResourceConfigTypeDef = TypedDict(
     "_RequiredWorkerResourceConfigTypeDef",
     {
         "cpu": str,
         "memory": str,
     },
 )
@@ -545,56 +446,34 @@
         "vCPUHour": float,
         "memoryGBHour": float,
         "storageGBHour": float,
     },
     total=False,
 )
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "states": Sequence[ApplicationStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "states": Sequence[ApplicationStateType],
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
-        "states": Sequence[JobRunStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListJobRunsRequestListJobRunsPaginateTypeDef(
-    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
-    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
-):
-    pass
-
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -617,163 +496,132 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ManagedPersistenceMonitoringConfigurationOutputTypeDef = TypedDict(
-    "ManagedPersistenceMonitoringConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-        "encryptionKeyArn": str,
-    },
-    total=False,
-)
-
 ManagedPersistenceMonitoringConfigurationTypeDef = TypedDict(
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     {
         "enabled": bool,
         "encryptionKeyArn": str,
     },
     total=False,
 )
 
-S3MonitoringConfigurationOutputTypeDef = TypedDict(
-    "S3MonitoringConfigurationOutputTypeDef",
+S3MonitoringConfigurationTypeDef = TypedDict(
+    "S3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
         "encryptionKeyArn": str,
     },
     total=False,
 )
 
-S3MonitoringConfigurationTypeDef = TypedDict(
-    "S3MonitoringConfigurationTypeDef",
+StartApplicationRequestRequestTypeDef = TypedDict(
+    "StartApplicationRequestRequestTypeDef",
     {
-        "logUri": str,
-        "encryptionKeyArn": str,
+        "applicationId": str,
     },
-    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+StopApplicationRequestRequestTypeDef = TypedDict(
+    "StopApplicationRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "applicationId": str,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "resourceArn": str,
+        "tags": Mapping[str, str],
     },
 )
 
-StartApplicationRequestRequestTypeDef = TypedDict(
-    "StartApplicationRequestRequestTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "applicationId": str,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
+WorkerTypeSpecificationTypeDef = TypedDict(
+    "WorkerTypeSpecificationTypeDef",
     {
-        "applicationId": str,
-        "jobRunId": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "imageConfiguration": ImageConfigurationTypeDef,
     },
+    total=False,
 )
 
-StopApplicationRequestRequestTypeDef = TypedDict(
-    "StopApplicationRequestRequestTypeDef",
+CancelJobRunResponseTypeDef = TypedDict(
+    "CancelJobRunResponseTypeDef",
     {
         "applicationId": str,
+        "jobRunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
     {
-        "resourceArn": str,
-        "tags": Mapping[str, str],
+        "applicationId": str,
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+GetDashboardForJobRunResponseTypeDef = TypedDict(
+    "GetDashboardForJobRunResponseTypeDef",
     {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-WorkerTypeSpecificationTypeDef = TypedDict(
-    "WorkerTypeSpecificationTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "imageConfiguration": ImageConfigurationTypeDef,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-WorkerTypeSpecificationInputTypeDef = TypedDict(
-    "WorkerTypeSpecificationInputTypeDef",
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
     {
-        "imageConfiguration": ImageConfigurationInputTypeDef,
+        "applicationId": str,
+        "jobRunId": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredInitialCapacityConfigOutputTypeDef = TypedDict(
-    "_RequiredInitialCapacityConfigOutputTypeDef",
-    {
-        "workerCount": int,
-    },
-)
-_OptionalInitialCapacityConfigOutputTypeDef = TypedDict(
-    "_OptionalInitialCapacityConfigOutputTypeDef",
+WorkerTypeSpecificationInputTypeDef = TypedDict(
+    "WorkerTypeSpecificationInputTypeDef",
     {
-        "workerConfiguration": WorkerResourceConfigOutputTypeDef,
+        "imageConfiguration": ImageConfigurationInputTypeDef,
     },
     total=False,
 )
 
-class InitialCapacityConfigOutputTypeDef(
-    _RequiredInitialCapacityConfigOutputTypeDef, _OptionalInitialCapacityConfigOutputTypeDef
-):
-    pass
-
 _RequiredInitialCapacityConfigTypeDef = TypedDict(
     "_RequiredInitialCapacityConfigTypeDef",
     {
         "workerCount": int,
     },
 )
 _OptionalInitialCapacityConfigTypeDef = TypedDict(
@@ -789,15 +637,15 @@
 ):
     pass
 
 JobDriverOutputTypeDef = TypedDict(
     "JobDriverOutputTypeDef",
     {
         "sparkSubmit": SparkSubmitOutputTypeDef,
-        "hive": HiveOutputTypeDef,
+        "hive": HiveTypeDef,
     },
     total=False,
 )
 
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
@@ -808,24 +656,56 @@
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "jobRuns": List[JobRunSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "states": Sequence[ApplicationStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "createdAtAfter": Union[datetime, str],
+        "createdAtBefore": Union[datetime, str],
+        "states": Sequence[JobRunStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListJobRunsRequestListJobRunsPaginateTypeDef(
+    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
+    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
+):
+    pass
+
 MonitoringConfigurationOutputTypeDef = TypedDict(
     "MonitoringConfigurationOutputTypeDef",
     {
-        "s3MonitoringConfiguration": S3MonitoringConfigurationOutputTypeDef,
+        "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "managedPersistenceMonitoringConfiguration": (
-            ManagedPersistenceMonitoringConfigurationOutputTypeDef
+            ManagedPersistenceMonitoringConfigurationTypeDef
         ),
         "cloudWatchLoggingConfiguration": CloudWatchLoggingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 MonitoringConfigurationTypeDef = TypedDict(
@@ -853,19 +733,19 @@
     },
 )
 _OptionalApplicationTypeDef = TypedDict(
     "_OptionalApplicationTypeDef",
     {
         "name": str,
         "stateDetails": str,
-        "initialCapacity": Dict[str, InitialCapacityConfigOutputTypeDef],
-        "maximumCapacity": MaximumAllowedResourcesOutputTypeDef,
+        "initialCapacity": Dict[str, InitialCapacityConfigTypeDef],
+        "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "tags": Dict[str, str],
-        "autoStartConfiguration": AutoStartConfigOutputTypeDef,
-        "autoStopConfiguration": AutoStopConfigOutputTypeDef,
+        "autoStartConfiguration": AutoStartConfigTypeDef,
+        "autoStopConfiguration": AutoStopConfigTypeDef,
         "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationTypeDef,
         "workerTypeSpecifications": Dict[str, WorkerTypeSpecificationTypeDef],
     },
     total=False,
 )
@@ -949,23 +829,23 @@
     total=False,
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJobRunTypeDef = TypedDict(
     "_RequiredJobRunTypeDef",
     {
         "applicationId": str,
@@ -1024,10 +904,10 @@
 ):
     pass
 
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "jobRun": JobRunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/PKG-INFO` & `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.28.12
-Summary: Type annotations for boto3.EMRServerless 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.EMRServerless 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-serverless)](https://pepy.tech/project/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,70 +326,62 @@
 
 `mypy_boto3_emr_serverless.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_serverless.type_defs import (
     ApplicationSummaryTypeDef,
-    AutoStartConfigOutputTypeDef,
-    AutoStopConfigOutputTypeDef,
-    ImageConfigurationTypeDef,
-    MaximumAllowedResourcesOutputTypeDef,
-    NetworkConfigurationOutputTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
+    ImageConfigurationTypeDef,
+    MaximumAllowedResourcesTypeDef,
+    NetworkConfigurationOutputTypeDef,
     CancelJobRunRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
+    ResponseMetadataTypeDef,
     CloudWatchLoggingConfigurationOutputTypeDef,
     CloudWatchLoggingConfigurationTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ImageConfigurationInputTypeDef,
-    MaximumAllowedResourcesTypeDef,
     NetworkConfigurationTypeDef,
-    CreateApplicationResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
     GetJobRunRequestRequestTypeDef,
-    HiveOutputTypeDef,
     HiveTypeDef,
-    WorkerResourceConfigOutputTypeDef,
     WorkerResourceConfigTypeDef,
     SparkSubmitOutputTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
     ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ManagedPersistenceMonitoringConfigurationOutputTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
-    S3MonitoringConfigurationOutputTypeDef,
     S3MonitoringConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
-    StartJobRunResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListApplicationsResponseTypeDef,
     WorkerTypeSpecificationTypeDef,
+    CancelJobRunResponseTypeDef,
+    CreateApplicationResponseTypeDef,
+    GetDashboardForJobRunResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartJobRunResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
-    InitialCapacityConfigOutputTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
     MonitoringConfigurationOutputTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
```

### Comparing `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/SOURCES.txt` & `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.12/setup.py` & `mypy-boto3-emr-serverless-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr-serverless",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_emr_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMRServerless 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.EMRServerless 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

