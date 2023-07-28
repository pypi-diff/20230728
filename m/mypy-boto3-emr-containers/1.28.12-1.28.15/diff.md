# Comparing `tmp/mypy-boto3-emr-containers-1.28.12.tar.gz` & `tmp/mypy-boto3-emr-containers-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-containers-1.28.12.tar", last modified: Thu Jul 27 05:34:40 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-containers-1.28.15.tar", last modified: Fri Jul 28 20:42:46 2023, max compression
```

## Comparing `mypy-boto3-emr-containers-1.28.12.tar` & `mypy-boto3-emr-containers-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.156515 mypy-boto3-emr-containers-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-07-27 05:34:40.152515 mypy-boto3-emr-containers-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.148515 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18379 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32747 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32706 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.148515 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-07-27 05:34:39.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:34:40.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:39.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:39.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:39.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:39.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:40.156515 mypy-boto3-emr-containers-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.689081 mypy-boto3-emr-containers-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16592 2023-07-28 20:42:46.681081 mypy-boto3-emr-containers-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.673081 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18379 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28645 2023-07-28 20:25:31.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-07-28 20:25:31.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.681081 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16592 2023-07-28 20:42:46.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:42:46.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:46.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:42:46.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:46.689081 mypy-boto3-emr-containers-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/setup.py
```

### Comparing `mypy-boto3-emr-containers-1.28.12/LICENSE` & `mypy-boto3-emr-containers-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.12/PKG-INFO` & `mypy-boto3-emr-containers-1.28.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-containers
-Version: 1.28.12
-Summary: Type annotations for boto3.EMRContainers 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.EMRContainers 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-containers)](https://pepy.tech/project/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
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
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,86 +343,73 @@
 
 `mypy_boto3_emr_containers.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_containers.type_defs import (
     CancelJobRunRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
+    ResponseMetadataTypeDef,
     CertificateTypeDef,
-    CloudWatchMonitoringConfigurationOutputTypeDef,
     CloudWatchMonitoringConfigurationTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
-    EksInfoOutputTypeDef,
     EksInfoTypeDef,
-    ContainerLogRotationConfigurationOutputTypeDef,
     ContainerLogRotationConfigurationTypeDef,
-    CreateJobTemplateResponseTypeDef,
-    CreateManagedEndpointResponseTypeDef,
-    CreateVirtualClusterResponseTypeDef,
     CredentialsTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
-    DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointRequestRequestTypeDef,
-    DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterRequestRequestTypeDef,
-    DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
     DescribeManagedEndpointRequestRequestTypeDef,
     DescribeVirtualClusterRequestRequestTypeDef,
     GetManagedEndpointSessionCredentialsRequestRequestTypeDef,
-    SparkSqlJobDriverOutputTypeDef,
-    SparkSubmitJobDriverOutputTypeDef,
     SparkSqlJobDriverTypeDef,
+    SparkSubmitJobDriverOutputTypeDef,
     SparkSubmitJobDriverTypeDef,
-    RetryPolicyConfigurationOutputTypeDef,
+    RetryPolicyConfigurationTypeDef,
     RetryPolicyExecutionTypeDef,
-    TemplateParameterConfigurationOutputTypeDef,
     TemplateParameterConfigurationTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListJobRunsRequestRequestTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     ListManagedEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
     ListVirtualClustersRequestRequestTypeDef,
-    S3MonitoringConfigurationOutputTypeDef,
     S3MonitoringConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ParametricCloudWatchMonitoringConfigurationOutputTypeDef,
     ParametricCloudWatchMonitoringConfigurationTypeDef,
-    ParametricS3MonitoringConfigurationOutputTypeDef,
     ParametricS3MonitoringConfigurationTypeDef,
-    ResponseMetadataTypeDef,
-    RetryPolicyConfigurationTypeDef,
-    StartJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ContainerInfoOutputTypeDef,
+    CancelJobRunResponseTypeDef,
+    CreateJobTemplateResponseTypeDef,
+    CreateManagedEndpointResponseTypeDef,
+    CreateVirtualClusterResponseTypeDef,
+    DeleteJobTemplateResponseTypeDef,
+    DeleteManagedEndpointResponseTypeDef,
+    DeleteVirtualClusterResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartJobRunResponseTypeDef,
     ContainerInfoTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
     JobDriverOutputTypeDef,
     JobDriverTypeDef,
-    MonitoringConfigurationOutputTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
+    ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
     MonitoringConfigurationTypeDef,
-    ParametricMonitoringConfigurationOutputTypeDef,
     ParametricMonitoringConfigurationTypeDef,
-    ContainerProviderOutputTypeDef,
     ContainerProviderTypeDef,
     ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     ParametricConfigurationOverridesOutputTypeDef,
     ParametricConfigurationOverridesTypeDef,
-    VirtualClusterTypeDef,
     CreateVirtualClusterRequestRequestTypeDef,
+    VirtualClusterTypeDef,
     EndpointTypeDef,
     JobRunTypeDef,
     CreateManagedEndpointRequestRequestTypeDef,
     StartJobRunRequestRequestTypeDef,
     JobTemplateDataOutputTypeDef,
     JobTemplateDataTypeDef,
     DescribeVirtualClusterResponseTypeDef,
```

### Comparing `mypy-boto3-emr-containers-1.28.12/README.md` & `mypy-boto3-emr-containers-1.28.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-containers)](https://pepy.tech/project/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
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
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,86 +311,73 @@
 
 `mypy_boto3_emr_containers.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_containers.type_defs import (
     CancelJobRunRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
+    ResponseMetadataTypeDef,
     CertificateTypeDef,
-    CloudWatchMonitoringConfigurationOutputTypeDef,
     CloudWatchMonitoringConfigurationTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
-    EksInfoOutputTypeDef,
     EksInfoTypeDef,
-    ContainerLogRotationConfigurationOutputTypeDef,
     ContainerLogRotationConfigurationTypeDef,
-    CreateJobTemplateResponseTypeDef,
-    CreateManagedEndpointResponseTypeDef,
-    CreateVirtualClusterResponseTypeDef,
     CredentialsTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
-    DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointRequestRequestTypeDef,
-    DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterRequestRequestTypeDef,
-    DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
     DescribeManagedEndpointRequestRequestTypeDef,
     DescribeVirtualClusterRequestRequestTypeDef,
     GetManagedEndpointSessionCredentialsRequestRequestTypeDef,
-    SparkSqlJobDriverOutputTypeDef,
-    SparkSubmitJobDriverOutputTypeDef,
     SparkSqlJobDriverTypeDef,
+    SparkSubmitJobDriverOutputTypeDef,
     SparkSubmitJobDriverTypeDef,
-    RetryPolicyConfigurationOutputTypeDef,
+    RetryPolicyConfigurationTypeDef,
     RetryPolicyExecutionTypeDef,
-    TemplateParameterConfigurationOutputTypeDef,
     TemplateParameterConfigurationTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListJobRunsRequestRequestTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     ListManagedEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
     ListVirtualClustersRequestRequestTypeDef,
-    S3MonitoringConfigurationOutputTypeDef,
     S3MonitoringConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ParametricCloudWatchMonitoringConfigurationOutputTypeDef,
     ParametricCloudWatchMonitoringConfigurationTypeDef,
-    ParametricS3MonitoringConfigurationOutputTypeDef,
     ParametricS3MonitoringConfigurationTypeDef,
-    ResponseMetadataTypeDef,
-    RetryPolicyConfigurationTypeDef,
-    StartJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ContainerInfoOutputTypeDef,
+    CancelJobRunResponseTypeDef,
+    CreateJobTemplateResponseTypeDef,
+    CreateManagedEndpointResponseTypeDef,
+    CreateVirtualClusterResponseTypeDef,
+    DeleteJobTemplateResponseTypeDef,
+    DeleteManagedEndpointResponseTypeDef,
+    DeleteVirtualClusterResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartJobRunResponseTypeDef,
     ContainerInfoTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
     JobDriverOutputTypeDef,
     JobDriverTypeDef,
-    MonitoringConfigurationOutputTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
+    ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
     MonitoringConfigurationTypeDef,
-    ParametricMonitoringConfigurationOutputTypeDef,
     ParametricMonitoringConfigurationTypeDef,
-    ContainerProviderOutputTypeDef,
     ContainerProviderTypeDef,
     ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     ParametricConfigurationOverridesOutputTypeDef,
     ParametricConfigurationOverridesTypeDef,
-    VirtualClusterTypeDef,
     CreateVirtualClusterRequestRequestTypeDef,
+    VirtualClusterTypeDef,
     EndpointTypeDef,
     JobRunTypeDef,
     CreateManagedEndpointRequestRequestTypeDef,
     StartJobRunRequestRequestTypeDef,
     JobTemplateDataOutputTypeDef,
     JobTemplateDataTypeDef,
     DescribeVirtualClusterResponseTypeDef,
```

### Comparing `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/__init__.py` & `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/__init__.pyi` & `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/__main__.py` & `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRContainers 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.EMRContainers 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers\nOther"
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

### Comparing `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/client.py` & `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/client.pyi` & `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/literals.py` & `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/literals.pyi` & `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/paginator.py` & `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self,
         *,
         virtualClusterId: str,
         createdBefore: Union[datetime, str] = ...,
         createdAfter: Union[datetime, str] = ...,
         name: str = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobrunspaginator)
         """
 
 
@@ -93,15 +93,15 @@
     """
 
     def paginate(
         self,
         *,
         createdAfter: Union[datetime, str] = ...,
         createdBefore: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobtemplatespaginator)
         """
 
 
@@ -115,15 +115,15 @@
         self,
         *,
         virtualClusterId: str,
         createdBefore: Union[datetime, str] = ...,
         createdAfter: Union[datetime, str] = ...,
         types: Sequence[str] = ...,
         states: Sequence[EndpointStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listmanagedendpointspaginator)
         """
 
 
@@ -137,13 +137,13 @@
         self,
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
         createdAfter: Union[datetime, str] = ...,
         createdBefore: Union[datetime, str] = ...,
         states: Sequence[VirtualClusterStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVirtualClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listvirtualclusterspaginator)
         """
```

### Comparing `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/paginator.pyi` & `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         self,
         *,
         virtualClusterId: str,
         createdBefore: Union[datetime, str] = ...,
         createdAfter: Union[datetime, str] = ...,
         name: str = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobrunspaginator)
         """
 
 class ListJobTemplatesPaginator(Paginator):
@@ -88,15 +88,15 @@
     """
 
     def paginate(
         self,
         *,
         createdAfter: Union[datetime, str] = ...,
         createdBefore: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobtemplatespaginator)
         """
 
 class ListManagedEndpointsPaginator(Paginator):
@@ -109,15 +109,15 @@
         self,
         *,
         virtualClusterId: str,
         createdBefore: Union[datetime, str] = ...,
         createdAfter: Union[datetime, str] = ...,
         types: Sequence[str] = ...,
         states: Sequence[EndpointStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listmanagedendpointspaginator)
         """
 
 class ListVirtualClustersPaginator(Paginator):
@@ -130,13 +130,13 @@
         self,
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
         createdAfter: Union[datetime, str] = ...,
         createdBefore: Union[datetime, str] = ...,
         states: Sequence[VirtualClusterStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVirtualClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listvirtualclusterspaginator)
         """
```

### Comparing `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/type_defs.py` & `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -29,89 +29,75 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelJobRunRequestRequestTypeDef",
-    "CancelJobRunResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CertificateTypeDef",
-    "CloudWatchMonitoringConfigurationOutputTypeDef",
     "CloudWatchMonitoringConfigurationTypeDef",
     "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
-    "EksInfoOutputTypeDef",
     "EksInfoTypeDef",
-    "ContainerLogRotationConfigurationOutputTypeDef",
     "ContainerLogRotationConfigurationTypeDef",
-    "CreateJobTemplateResponseTypeDef",
-    "CreateManagedEndpointResponseTypeDef",
-    "CreateVirtualClusterResponseTypeDef",
     "CredentialsTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
-    "DeleteJobTemplateResponseTypeDef",
     "DeleteManagedEndpointRequestRequestTypeDef",
-    "DeleteManagedEndpointResponseTypeDef",
     "DeleteVirtualClusterRequestRequestTypeDef",
-    "DeleteVirtualClusterResponseTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
     "DescribeManagedEndpointRequestRequestTypeDef",
     "DescribeVirtualClusterRequestRequestTypeDef",
     "GetManagedEndpointSessionCredentialsRequestRequestTypeDef",
-    "SparkSqlJobDriverOutputTypeDef",
-    "SparkSubmitJobDriverOutputTypeDef",
     "SparkSqlJobDriverTypeDef",
+    "SparkSubmitJobDriverOutputTypeDef",
     "SparkSubmitJobDriverTypeDef",
-    "RetryPolicyConfigurationOutputTypeDef",
+    "RetryPolicyConfigurationTypeDef",
     "RetryPolicyExecutionTypeDef",
-    "TemplateParameterConfigurationOutputTypeDef",
     "TemplateParameterConfigurationTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListJobRunsRequestRequestTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
-    "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     "ListManagedEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     "ListVirtualClustersRequestRequestTypeDef",
-    "S3MonitoringConfigurationOutputTypeDef",
     "S3MonitoringConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
-    "ParametricCloudWatchMonitoringConfigurationOutputTypeDef",
     "ParametricCloudWatchMonitoringConfigurationTypeDef",
-    "ParametricS3MonitoringConfigurationOutputTypeDef",
     "ParametricS3MonitoringConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
-    "RetryPolicyConfigurationTypeDef",
-    "StartJobRunResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ContainerInfoOutputTypeDef",
+    "CancelJobRunResponseTypeDef",
+    "CreateJobTemplateResponseTypeDef",
+    "CreateManagedEndpointResponseTypeDef",
+    "CreateVirtualClusterResponseTypeDef",
+    "DeleteJobTemplateResponseTypeDef",
+    "DeleteManagedEndpointResponseTypeDef",
+    "DeleteVirtualClusterResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartJobRunResponseTypeDef",
     "ContainerInfoTypeDef",
     "GetManagedEndpointSessionCredentialsResponseTypeDef",
     "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
-    "MonitoringConfigurationOutputTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
+    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     "MonitoringConfigurationTypeDef",
-    "ParametricMonitoringConfigurationOutputTypeDef",
     "ParametricMonitoringConfigurationTypeDef",
-    "ContainerProviderOutputTypeDef",
     "ContainerProviderTypeDef",
     "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
     "ParametricConfigurationOverridesOutputTypeDef",
     "ParametricConfigurationOverridesTypeDef",
-    "VirtualClusterTypeDef",
     "CreateVirtualClusterRequestRequestTypeDef",
+    "VirtualClusterTypeDef",
     "EndpointTypeDef",
     "JobRunTypeDef",
     "CreateManagedEndpointRequestRequestTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "JobTemplateDataOutputTypeDef",
     "JobTemplateDataTypeDef",
     "DescribeVirtualClusterResponseTypeDef",
@@ -130,76 +116,54 @@
     "CancelJobRunRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
     },
 )
 
-CancelJobRunResponseTypeDef = TypedDict(
-    "CancelJobRunResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "id": str,
-        "virtualClusterId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "certificateArn": str,
         "certificateData": str,
     },
     total=False,
 )
 
-_RequiredCloudWatchMonitoringConfigurationOutputTypeDef = TypedDict(
-    "_RequiredCloudWatchMonitoringConfigurationOutputTypeDef",
-    {
-        "logGroupName": str,
-    },
-)
-_OptionalCloudWatchMonitoringConfigurationOutputTypeDef = TypedDict(
-    "_OptionalCloudWatchMonitoringConfigurationOutputTypeDef",
-    {
-        "logStreamNamePrefix": str,
-    },
-    total=False,
-)
-
-
-class CloudWatchMonitoringConfigurationOutputTypeDef(
-    _RequiredCloudWatchMonitoringConfigurationOutputTypeDef,
-    _OptionalCloudWatchMonitoringConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredCloudWatchMonitoringConfigurationTypeDef = TypedDict(
     "_RequiredCloudWatchMonitoringConfigurationTypeDef",
     {
         "logGroupName": str,
     },
 )
 _OptionalCloudWatchMonitoringConfigurationTypeDef = TypedDict(
     "_OptionalCloudWatchMonitoringConfigurationTypeDef",
     {
         "logStreamNamePrefix": str,
     },
     total=False,
 )
 
-
 class CloudWatchMonitoringConfigurationTypeDef(
     _RequiredCloudWatchMonitoringConfigurationTypeDef,
     _OptionalCloudWatchMonitoringConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredConfigurationOutputTypeDef = TypedDict(
     "_RequiredConfigurationOutputTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationOutputTypeDef = TypedDict(
@@ -207,21 +171,19 @@
     {
         "properties": Dict[str, str],
         "configurations": List[Dict[str, Any]],
     },
     total=False,
 )
 
-
 class ConfigurationOutputTypeDef(
     _RequiredConfigurationOutputTypeDef, _OptionalConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationTypeDef = TypedDict(
@@ -229,83 +191,33 @@
     {
         "properties": Mapping[str, str],
         "configurations": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
-
-EksInfoOutputTypeDef = TypedDict(
-    "EksInfoOutputTypeDef",
-    {
-        "namespace": str,
-    },
-    total=False,
-)
-
 EksInfoTypeDef = TypedDict(
     "EksInfoTypeDef",
     {
         "namespace": str,
     },
     total=False,
 )
 
-ContainerLogRotationConfigurationOutputTypeDef = TypedDict(
-    "ContainerLogRotationConfigurationOutputTypeDef",
-    {
-        "rotationSize": str,
-        "maxFilesToKeep": int,
-    },
-)
-
 ContainerLogRotationConfigurationTypeDef = TypedDict(
     "ContainerLogRotationConfigurationTypeDef",
     {
         "rotationSize": str,
         "maxFilesToKeep": int,
     },
 )
 
-CreateJobTemplateResponseTypeDef = TypedDict(
-    "CreateJobTemplateResponseTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "arn": str,
-        "createdAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateManagedEndpointResponseTypeDef = TypedDict(
-    "CreateManagedEndpointResponseTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "arn": str,
-        "virtualClusterId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVirtualClusterResponseTypeDef = TypedDict(
-    "CreateVirtualClusterResponseTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CredentialsTypeDef = TypedDict(
     "CredentialsTypeDef",
     {
         "token": str,
     },
     total=False,
 )
@@ -313,54 +225,29 @@
 DeleteJobTemplateRequestRequestTypeDef = TypedDict(
     "DeleteJobTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-DeleteJobTemplateResponseTypeDef = TypedDict(
-    "DeleteJobTemplateResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteManagedEndpointRequestRequestTypeDef = TypedDict(
     "DeleteManagedEndpointRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
     },
 )
 
-DeleteManagedEndpointResponseTypeDef = TypedDict(
-    "DeleteManagedEndpointResponseTypeDef",
-    {
-        "id": str,
-        "virtualClusterId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteVirtualClusterRequestRequestTypeDef = TypedDict(
     "DeleteVirtualClusterRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-DeleteVirtualClusterResponseTypeDef = TypedDict(
-    "DeleteVirtualClusterResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeJobRunRequestRequestTypeDef = TypedDict(
     "DescribeJobRunRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
     },
 )
@@ -402,24 +289,22 @@
         "durationInSeconds": int,
         "logContext": str,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class GetManagedEndpointSessionCredentialsRequestRequestTypeDef(
     _RequiredGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
     _OptionalGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
 ):
     pass
 
-
-SparkSqlJobDriverOutputTypeDef = TypedDict(
-    "SparkSqlJobDriverOutputTypeDef",
+SparkSqlJobDriverTypeDef = TypedDict(
+    "SparkSqlJobDriverTypeDef",
     {
         "entryPoint": str,
         "sparkSqlParameters": str,
     },
     total=False,
 )
 
@@ -434,30 +319,19 @@
     {
         "entryPointArguments": List[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
-
 class SparkSubmitJobDriverOutputTypeDef(
     _RequiredSparkSubmitJobDriverOutputTypeDef, _OptionalSparkSubmitJobDriverOutputTypeDef
 ):
     pass
 
-
-SparkSqlJobDriverTypeDef = TypedDict(
-    "SparkSqlJobDriverTypeDef",
-    {
-        "entryPoint": str,
-        "sparkSqlParameters": str,
-    },
-    total=False,
-)
-
 _RequiredSparkSubmitJobDriverTypeDef = TypedDict(
     "_RequiredSparkSubmitJobDriverTypeDef",
     {
         "entryPoint": str,
     },
 )
 _OptionalSparkSubmitJobDriverTypeDef = TypedDict(
@@ -465,79 +339,52 @@
     {
         "entryPointArguments": Sequence[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
-
 class SparkSubmitJobDriverTypeDef(
     _RequiredSparkSubmitJobDriverTypeDef, _OptionalSparkSubmitJobDriverTypeDef
 ):
     pass
 
-
-RetryPolicyConfigurationOutputTypeDef = TypedDict(
-    "RetryPolicyConfigurationOutputTypeDef",
+RetryPolicyConfigurationTypeDef = TypedDict(
+    "RetryPolicyConfigurationTypeDef",
     {
         "maxAttempts": int,
     },
 )
 
 RetryPolicyExecutionTypeDef = TypedDict(
     "RetryPolicyExecutionTypeDef",
     {
         "currentAttemptCount": int,
     },
 )
 
-TemplateParameterConfigurationOutputTypeDef = TypedDict(
-    "TemplateParameterConfigurationOutputTypeDef",
-    {
-        "type": TemplateParameterDataTypeType,
-        "defaultValue": str,
-    },
-    total=False,
-)
-
 TemplateParameterConfigurationTypeDef = TypedDict(
     "TemplateParameterConfigurationTypeDef",
     {
         "type": TemplateParameterDataTypeType,
         "defaultValue": str,
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "virtualClusterId": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
-        "name": str,
-        "states": Sequence[JobRunStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
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
         "virtualClusterId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -549,68 +396,30 @@
         "states": Sequence[JobRunStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
-
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
-    "_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
-    {
-        "virtualClusterId": str,
-    },
-)
-_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
-    "_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
-    {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
-        "types": Sequence[str],
-        "states": Sequence[EndpointStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
-    _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
-    _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListManagedEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListManagedEndpointsRequestRequestTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListManagedEndpointsRequestRequestTypeDef = TypedDict(
@@ -622,173 +431,164 @@
         "states": Sequence[EndpointStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListManagedEndpointsRequestRequestTypeDef(
     _RequiredListManagedEndpointsRequestRequestTypeDef,
     _OptionalListManagedEndpointsRequestRequestTypeDef,
 ):
     pass
 
-
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
-ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
-    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
-    {
-        "containerProviderId": str,
-        "containerProviderType": Literal["EKS"],
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "states": Sequence[VirtualClusterStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVirtualClustersRequestRequestTypeDef = TypedDict(
     "ListVirtualClustersRequestRequestTypeDef",
     {
         "containerProviderId": str,
         "containerProviderType": Literal["EKS"],
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
         "states": Sequence[VirtualClusterStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-S3MonitoringConfigurationOutputTypeDef = TypedDict(
-    "S3MonitoringConfigurationOutputTypeDef",
-    {
-        "logUri": str,
-    },
-)
-
 S3MonitoringConfigurationTypeDef = TypedDict(
     "S3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ParametricCloudWatchMonitoringConfigurationTypeDef = TypedDict(
+    "ParametricCloudWatchMonitoringConfigurationTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "logGroupName": str,
+        "logStreamNamePrefix": str,
     },
     total=False,
 )
 
-ParametricCloudWatchMonitoringConfigurationOutputTypeDef = TypedDict(
-    "ParametricCloudWatchMonitoringConfigurationOutputTypeDef",
+ParametricS3MonitoringConfigurationTypeDef = TypedDict(
+    "ParametricS3MonitoringConfigurationTypeDef",
     {
-        "logGroupName": str,
-        "logStreamNamePrefix": str,
+        "logUri": str,
     },
     total=False,
 )
 
-ParametricCloudWatchMonitoringConfigurationTypeDef = TypedDict(
-    "ParametricCloudWatchMonitoringConfigurationTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "logGroupName": str,
-        "logStreamNamePrefix": str,
+        "resourceArn": str,
+        "tags": Mapping[str, str],
     },
-    total=False,
 )
 
-ParametricS3MonitoringConfigurationOutputTypeDef = TypedDict(
-    "ParametricS3MonitoringConfigurationOutputTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "logUri": str,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
-    total=False,
 )
 
-ParametricS3MonitoringConfigurationTypeDef = TypedDict(
-    "ParametricS3MonitoringConfigurationTypeDef",
+CancelJobRunResponseTypeDef = TypedDict(
+    "CancelJobRunResponseTypeDef",
     {
-        "logUri": str,
+        "id": str,
+        "virtualClusterId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateJobTemplateResponseTypeDef = TypedDict(
+    "CreateJobTemplateResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "id": str,
+        "name": str,
+        "arn": str,
+        "createdAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RetryPolicyConfigurationTypeDef = TypedDict(
-    "RetryPolicyConfigurationTypeDef",
+CreateManagedEndpointResponseTypeDef = TypedDict(
+    "CreateManagedEndpointResponseTypeDef",
     {
-        "maxAttempts": int,
+        "id": str,
+        "name": str,
+        "arn": str,
+        "virtualClusterId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
+CreateVirtualClusterResponseTypeDef = TypedDict(
+    "CreateVirtualClusterResponseTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteJobTemplateResponseTypeDef = TypedDict(
+    "DeleteJobTemplateResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteManagedEndpointResponseTypeDef = TypedDict(
+    "DeleteManagedEndpointResponseTypeDef",
+    {
+        "id": str,
         "virtualClusterId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+DeleteVirtualClusterResponseTypeDef = TypedDict(
+    "DeleteVirtualClusterResponseTypeDef",
     {
-        "resourceArn": str,
-        "tags": Mapping[str, str],
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ContainerInfoOutputTypeDef = TypedDict(
-    "ContainerInfoOutputTypeDef",
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
     {
-        "eksInfo": EksInfoOutputTypeDef,
+        "id": str,
+        "name": str,
+        "arn": str,
+        "virtualClusterId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ContainerInfoTypeDef = TypedDict(
     "ContainerInfoTypeDef",
     {
         "eksInfo": EksInfoTypeDef,
     },
@@ -797,102 +597,128 @@
 
 GetManagedEndpointSessionCredentialsResponseTypeDef = TypedDict(
     "GetManagedEndpointSessionCredentialsResponseTypeDef",
     {
         "id": str,
         "credentials": CredentialsTypeDef,
         "expiresAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobDriverOutputTypeDef = TypedDict(
     "JobDriverOutputTypeDef",
     {
         "sparkSubmitJobDriver": SparkSubmitJobDriverOutputTypeDef,
-        "sparkSqlJobDriver": SparkSqlJobDriverOutputTypeDef,
+        "sparkSqlJobDriver": SparkSqlJobDriverTypeDef,
     },
     total=False,
 )
 
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmitJobDriver": SparkSubmitJobDriverTypeDef,
         "sparkSqlJobDriver": SparkSqlJobDriverTypeDef,
     },
     total=False,
 )
 
-MonitoringConfigurationOutputTypeDef = TypedDict(
-    "MonitoringConfigurationOutputTypeDef",
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
     {
-        "persistentAppUI": PersistentAppUIType,
-        "cloudWatchMonitoringConfiguration": CloudWatchMonitoringConfigurationOutputTypeDef,
-        "s3MonitoringConfiguration": S3MonitoringConfigurationOutputTypeDef,
-        "containerLogRotationConfiguration": ContainerLogRotationConfigurationOutputTypeDef,
+        "virtualClusterId": str,
+    },
+)
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "createdBefore": Union[datetime, str],
+        "createdAfter": Union[datetime, str],
+        "name": str,
+        "states": Sequence[JobRunStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-MonitoringConfigurationTypeDef = TypedDict(
-    "MonitoringConfigurationTypeDef",
+class ListJobRunsRequestListJobRunsPaginateTypeDef(
+    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
+    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
+):
+    pass
+
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     {
-        "persistentAppUI": PersistentAppUIType,
-        "cloudWatchMonitoringConfiguration": CloudWatchMonitoringConfigurationTypeDef,
-        "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
-        "containerLogRotationConfiguration": ContainerLogRotationConfigurationTypeDef,
+        "createdAfter": Union[datetime, str],
+        "createdBefore": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ParametricMonitoringConfigurationOutputTypeDef = TypedDict(
-    "ParametricMonitoringConfigurationOutputTypeDef",
+_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
+    "_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     {
-        "persistentAppUI": str,
-        "cloudWatchMonitoringConfiguration": (
-            ParametricCloudWatchMonitoringConfigurationOutputTypeDef
-        ),
-        "s3MonitoringConfiguration": ParametricS3MonitoringConfigurationOutputTypeDef,
+        "virtualClusterId": str,
+    },
+)
+_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
+    "_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
+    {
+        "createdBefore": Union[datetime, str],
+        "createdAfter": Union[datetime, str],
+        "types": Sequence[str],
+        "states": Sequence[EndpointStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ParametricMonitoringConfigurationTypeDef = TypedDict(
-    "ParametricMonitoringConfigurationTypeDef",
+class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
+    _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
+    _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
+):
+    pass
+
+ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
+    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     {
-        "persistentAppUI": str,
-        "cloudWatchMonitoringConfiguration": ParametricCloudWatchMonitoringConfigurationTypeDef,
-        "s3MonitoringConfiguration": ParametricS3MonitoringConfigurationTypeDef,
+        "containerProviderId": str,
+        "containerProviderType": Literal["EKS"],
+        "createdAfter": Union[datetime, str],
+        "createdBefore": Union[datetime, str],
+        "states": Sequence[VirtualClusterStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredContainerProviderOutputTypeDef = TypedDict(
-    "_RequiredContainerProviderOutputTypeDef",
+MonitoringConfigurationTypeDef = TypedDict(
+    "MonitoringConfigurationTypeDef",
     {
-        "type": Literal["EKS"],
-        "id": str,
+        "persistentAppUI": PersistentAppUIType,
+        "cloudWatchMonitoringConfiguration": CloudWatchMonitoringConfigurationTypeDef,
+        "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
+        "containerLogRotationConfiguration": ContainerLogRotationConfigurationTypeDef,
     },
+    total=False,
 )
-_OptionalContainerProviderOutputTypeDef = TypedDict(
-    "_OptionalContainerProviderOutputTypeDef",
+
+ParametricMonitoringConfigurationTypeDef = TypedDict(
+    "ParametricMonitoringConfigurationTypeDef",
     {
-        "info": ContainerInfoOutputTypeDef,
+        "persistentAppUI": str,
+        "cloudWatchMonitoringConfiguration": ParametricCloudWatchMonitoringConfigurationTypeDef,
+        "s3MonitoringConfiguration": ParametricS3MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class ContainerProviderOutputTypeDef(
-    _RequiredContainerProviderOutputTypeDef, _OptionalContainerProviderOutputTypeDef
-):
-    pass
-
-
 _RequiredContainerProviderTypeDef = TypedDict(
     "_RequiredContainerProviderTypeDef",
     {
         "type": Literal["EKS"],
         "id": str,
     },
 )
@@ -900,26 +726,24 @@
     "_OptionalContainerProviderTypeDef",
     {
         "info": ContainerInfoTypeDef,
     },
     total=False,
 )
 
-
 class ContainerProviderTypeDef(
     _RequiredContainerProviderTypeDef, _OptionalContainerProviderTypeDef
 ):
     pass
 
-
 ConfigurationOverridesOutputTypeDef = TypedDict(
     "ConfigurationOverridesOutputTypeDef",
     {
         "applicationConfiguration": List["ConfigurationOutputTypeDef"],
-        "monitoringConfiguration": MonitoringConfigurationOutputTypeDef,
+        "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
 ConfigurationOverridesTypeDef = TypedDict(
     "ConfigurationOverridesTypeDef",
     {
@@ -929,42 +753,28 @@
     total=False,
 )
 
 ParametricConfigurationOverridesOutputTypeDef = TypedDict(
     "ParametricConfigurationOverridesOutputTypeDef",
     {
         "applicationConfiguration": List["ConfigurationOutputTypeDef"],
-        "monitoringConfiguration": ParametricMonitoringConfigurationOutputTypeDef,
+        "monitoringConfiguration": ParametricMonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
 ParametricConfigurationOverridesTypeDef = TypedDict(
     "ParametricConfigurationOverridesTypeDef",
     {
         "applicationConfiguration": Sequence["ConfigurationTypeDef"],
         "monitoringConfiguration": ParametricMonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
-VirtualClusterTypeDef = TypedDict(
-    "VirtualClusterTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "arn": str,
-        "state": VirtualClusterStateType,
-        "containerProvider": ContainerProviderOutputTypeDef,
-        "createdAt": datetime,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredCreateVirtualClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualClusterRequestRequestTypeDef",
     {
         "name": str,
         "containerProvider": ContainerProviderTypeDef,
         "clientToken": str,
     },
@@ -973,21 +783,33 @@
     "_OptionalCreateVirtualClusterRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateVirtualClusterRequestRequestTypeDef(
     _RequiredCreateVirtualClusterRequestRequestTypeDef,
     _OptionalCreateVirtualClusterRequestRequestTypeDef,
 ):
     pass
 
+VirtualClusterTypeDef = TypedDict(
+    "VirtualClusterTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "arn": str,
+        "state": VirtualClusterStateType,
+        "containerProvider": ContainerProviderTypeDef,
+        "createdAt": datetime,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
@@ -1025,15 +847,15 @@
         "jobDriver": JobDriverOutputTypeDef,
         "createdAt": datetime,
         "createdBy": str,
         "finishedAt": datetime,
         "stateDetails": str,
         "failureReason": FailureReasonType,
         "tags": Dict[str, str],
-        "retryPolicyConfiguration": RetryPolicyConfigurationOutputTypeDef,
+        "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
         "retryPolicyExecution": RetryPolicyExecutionTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateManagedEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateManagedEndpointRequestRequestTypeDef",
@@ -1052,22 +874,20 @@
         "certificateArn": str,
         "configurationOverrides": ConfigurationOverridesTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateManagedEndpointRequestRequestTypeDef(
     _RequiredCreateManagedEndpointRequestRequestTypeDef,
     _OptionalCreateManagedEndpointRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "virtualClusterId": str,
         "clientToken": str,
     },
 )
@@ -1083,46 +903,42 @@
         "jobTemplateId": str,
         "jobTemplateParameters": Mapping[str, str],
         "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredJobTemplateDataOutputTypeDef = TypedDict(
     "_RequiredJobTemplateDataOutputTypeDef",
     {
         "executionRoleArn": str,
         "releaseLabel": str,
         "jobDriver": JobDriverOutputTypeDef,
     },
 )
 _OptionalJobTemplateDataOutputTypeDef = TypedDict(
     "_OptionalJobTemplateDataOutputTypeDef",
     {
         "configurationOverrides": ParametricConfigurationOverridesOutputTypeDef,
-        "parameterConfiguration": Dict[str, TemplateParameterConfigurationOutputTypeDef],
+        "parameterConfiguration": Dict[str, TemplateParameterConfigurationTypeDef],
         "jobTags": Dict[str, str],
     },
     total=False,
 )
 
-
 class JobTemplateDataOutputTypeDef(
     _RequiredJobTemplateDataOutputTypeDef, _OptionalJobTemplateDataOutputTypeDef
 ):
     pass
 
-
 _RequiredJobTemplateDataTypeDef = TypedDict(
     "_RequiredJobTemplateDataTypeDef",
     {
         "executionRoleArn": str,
         "releaseLabel": str,
         "jobDriver": JobDriverTypeDef,
     },
@@ -1133,67 +949,65 @@
         "configurationOverrides": ParametricConfigurationOverridesTypeDef,
         "parameterConfiguration": Mapping[str, TemplateParameterConfigurationTypeDef],
         "jobTags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class JobTemplateDataTypeDef(_RequiredJobTemplateDataTypeDef, _OptionalJobTemplateDataTypeDef):
     pass
 
-
 DescribeVirtualClusterResponseTypeDef = TypedDict(
     "DescribeVirtualClusterResponseTypeDef",
     {
         "virtualCluster": VirtualClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualClustersResponseTypeDef = TypedDict(
     "ListVirtualClustersResponseTypeDef",
     {
         "virtualClusters": List[VirtualClusterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeManagedEndpointResponseTypeDef = TypedDict(
     "DescribeManagedEndpointResponseTypeDef",
     {
         "endpoint": EndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListManagedEndpointsResponseTypeDef = TypedDict(
     "ListManagedEndpointsResponseTypeDef",
     {
         "endpoints": List[EndpointTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobRunResponseTypeDef = TypedDict(
     "DescribeJobRunResponseTypeDef",
     {
         "jobRun": JobRunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "jobRuns": List[JobRunTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJobTemplateTypeDef = TypedDict(
     "_RequiredJobTemplateTypeDef",
     {
         "jobTemplateData": JobTemplateDataOutputTypeDef,
@@ -1210,19 +1024,17 @@
         "tags": Dict[str, str],
         "kmsKeyArn": str,
         "decryptionError": str,
     },
     total=False,
 )
 
-
 class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
     pass
 
-
 _RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobTemplateRequestRequestTypeDef",
     {
         "name": str,
         "clientToken": str,
         "jobTemplateData": JobTemplateDataTypeDef,
     },
@@ -1232,30 +1044,28 @@
     {
         "tags": Mapping[str, str],
         "kmsKeyArn": str,
     },
     total=False,
 )
 
-
 class CreateJobTemplateRequestRequestTypeDef(
     _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
     pass
 
-
 DescribeJobTemplateResponseTypeDef = TypedDict(
     "DescribeJobTemplateResponseTypeDef",
     {
         "jobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "templates": List[JobTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/type_defs.pyi` & `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,88 +29,76 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CancelJobRunRequestRequestTypeDef",
-    "CancelJobRunResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CertificateTypeDef",
-    "CloudWatchMonitoringConfigurationOutputTypeDef",
     "CloudWatchMonitoringConfigurationTypeDef",
     "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
-    "EksInfoOutputTypeDef",
     "EksInfoTypeDef",
-    "ContainerLogRotationConfigurationOutputTypeDef",
     "ContainerLogRotationConfigurationTypeDef",
-    "CreateJobTemplateResponseTypeDef",
-    "CreateManagedEndpointResponseTypeDef",
-    "CreateVirtualClusterResponseTypeDef",
     "CredentialsTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
-    "DeleteJobTemplateResponseTypeDef",
     "DeleteManagedEndpointRequestRequestTypeDef",
-    "DeleteManagedEndpointResponseTypeDef",
     "DeleteVirtualClusterRequestRequestTypeDef",
-    "DeleteVirtualClusterResponseTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
     "DescribeManagedEndpointRequestRequestTypeDef",
     "DescribeVirtualClusterRequestRequestTypeDef",
     "GetManagedEndpointSessionCredentialsRequestRequestTypeDef",
-    "SparkSqlJobDriverOutputTypeDef",
-    "SparkSubmitJobDriverOutputTypeDef",
     "SparkSqlJobDriverTypeDef",
+    "SparkSubmitJobDriverOutputTypeDef",
     "SparkSubmitJobDriverTypeDef",
-    "RetryPolicyConfigurationOutputTypeDef",
+    "RetryPolicyConfigurationTypeDef",
     "RetryPolicyExecutionTypeDef",
-    "TemplateParameterConfigurationOutputTypeDef",
     "TemplateParameterConfigurationTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListJobRunsRequestRequestTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
-    "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     "ListManagedEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     "ListVirtualClustersRequestRequestTypeDef",
-    "S3MonitoringConfigurationOutputTypeDef",
     "S3MonitoringConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
-    "ParametricCloudWatchMonitoringConfigurationOutputTypeDef",
     "ParametricCloudWatchMonitoringConfigurationTypeDef",
-    "ParametricS3MonitoringConfigurationOutputTypeDef",
     "ParametricS3MonitoringConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
-    "RetryPolicyConfigurationTypeDef",
-    "StartJobRunResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ContainerInfoOutputTypeDef",
+    "CancelJobRunResponseTypeDef",
+    "CreateJobTemplateResponseTypeDef",
+    "CreateManagedEndpointResponseTypeDef",
+    "CreateVirtualClusterResponseTypeDef",
+    "DeleteJobTemplateResponseTypeDef",
+    "DeleteManagedEndpointResponseTypeDef",
+    "DeleteVirtualClusterResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartJobRunResponseTypeDef",
     "ContainerInfoTypeDef",
     "GetManagedEndpointSessionCredentialsResponseTypeDef",
     "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
-    "MonitoringConfigurationOutputTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
+    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     "MonitoringConfigurationTypeDef",
-    "ParametricMonitoringConfigurationOutputTypeDef",
     "ParametricMonitoringConfigurationTypeDef",
-    "ContainerProviderOutputTypeDef",
     "ContainerProviderTypeDef",
     "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
     "ParametricConfigurationOverridesOutputTypeDef",
     "ParametricConfigurationOverridesTypeDef",
-    "VirtualClusterTypeDef",
     "CreateVirtualClusterRequestRequestTypeDef",
+    "VirtualClusterTypeDef",
     "EndpointTypeDef",
     "JobRunTypeDef",
     "CreateManagedEndpointRequestRequestTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "JobTemplateDataOutputTypeDef",
     "JobTemplateDataTypeDef",
     "DescribeVirtualClusterResponseTypeDef",
@@ -129,72 +117,56 @@
     "CancelJobRunRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
     },
 )
 
-CancelJobRunResponseTypeDef = TypedDict(
-    "CancelJobRunResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "id": str,
-        "virtualClusterId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "certificateArn": str,
         "certificateData": str,
     },
     total=False,
 )
 
-_RequiredCloudWatchMonitoringConfigurationOutputTypeDef = TypedDict(
-    "_RequiredCloudWatchMonitoringConfigurationOutputTypeDef",
-    {
-        "logGroupName": str,
-    },
-)
-_OptionalCloudWatchMonitoringConfigurationOutputTypeDef = TypedDict(
-    "_OptionalCloudWatchMonitoringConfigurationOutputTypeDef",
-    {
-        "logStreamNamePrefix": str,
-    },
-    total=False,
-)
-
-class CloudWatchMonitoringConfigurationOutputTypeDef(
-    _RequiredCloudWatchMonitoringConfigurationOutputTypeDef,
-    _OptionalCloudWatchMonitoringConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredCloudWatchMonitoringConfigurationTypeDef = TypedDict(
     "_RequiredCloudWatchMonitoringConfigurationTypeDef",
     {
         "logGroupName": str,
     },
 )
 _OptionalCloudWatchMonitoringConfigurationTypeDef = TypedDict(
     "_OptionalCloudWatchMonitoringConfigurationTypeDef",
     {
         "logStreamNamePrefix": str,
     },
     total=False,
 )
 
+
 class CloudWatchMonitoringConfigurationTypeDef(
     _RequiredCloudWatchMonitoringConfigurationTypeDef,
     _OptionalCloudWatchMonitoringConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredConfigurationOutputTypeDef = TypedDict(
     "_RequiredConfigurationOutputTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationOutputTypeDef = TypedDict(
@@ -202,19 +174,21 @@
     {
         "properties": Dict[str, str],
         "configurations": List[Dict[str, Any]],
     },
     total=False,
 )
 
+
 class ConfigurationOutputTypeDef(
     _RequiredConfigurationOutputTypeDef, _OptionalConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationTypeDef = TypedDict(
@@ -222,81 +196,35 @@
     {
         "properties": Mapping[str, str],
         "configurations": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
+
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
-EksInfoOutputTypeDef = TypedDict(
-    "EksInfoOutputTypeDef",
-    {
-        "namespace": str,
-    },
-    total=False,
-)
 
 EksInfoTypeDef = TypedDict(
     "EksInfoTypeDef",
     {
         "namespace": str,
     },
     total=False,
 )
 
-ContainerLogRotationConfigurationOutputTypeDef = TypedDict(
-    "ContainerLogRotationConfigurationOutputTypeDef",
-    {
-        "rotationSize": str,
-        "maxFilesToKeep": int,
-    },
-)
-
 ContainerLogRotationConfigurationTypeDef = TypedDict(
     "ContainerLogRotationConfigurationTypeDef",
     {
         "rotationSize": str,
         "maxFilesToKeep": int,
     },
 )
 
-CreateJobTemplateResponseTypeDef = TypedDict(
-    "CreateJobTemplateResponseTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "arn": str,
-        "createdAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateManagedEndpointResponseTypeDef = TypedDict(
-    "CreateManagedEndpointResponseTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "arn": str,
-        "virtualClusterId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVirtualClusterResponseTypeDef = TypedDict(
-    "CreateVirtualClusterResponseTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CredentialsTypeDef = TypedDict(
     "CredentialsTypeDef",
     {
         "token": str,
     },
     total=False,
 )
@@ -304,54 +232,29 @@
 DeleteJobTemplateRequestRequestTypeDef = TypedDict(
     "DeleteJobTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-DeleteJobTemplateResponseTypeDef = TypedDict(
-    "DeleteJobTemplateResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteManagedEndpointRequestRequestTypeDef = TypedDict(
     "DeleteManagedEndpointRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
     },
 )
 
-DeleteManagedEndpointResponseTypeDef = TypedDict(
-    "DeleteManagedEndpointResponseTypeDef",
-    {
-        "id": str,
-        "virtualClusterId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteVirtualClusterRequestRequestTypeDef = TypedDict(
     "DeleteVirtualClusterRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-DeleteVirtualClusterResponseTypeDef = TypedDict(
-    "DeleteVirtualClusterResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeJobRunRequestRequestTypeDef = TypedDict(
     "DescribeJobRunRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
     },
 )
@@ -393,22 +296,24 @@
         "durationInSeconds": int,
         "logContext": str,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class GetManagedEndpointSessionCredentialsRequestRequestTypeDef(
     _RequiredGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
     _OptionalGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
 ):
     pass
 
-SparkSqlJobDriverOutputTypeDef = TypedDict(
-    "SparkSqlJobDriverOutputTypeDef",
+
+SparkSqlJobDriverTypeDef = TypedDict(
+    "SparkSqlJobDriverTypeDef",
     {
         "entryPoint": str,
         "sparkSqlParameters": str,
     },
     total=False,
 )
 
@@ -423,27 +328,20 @@
     {
         "entryPointArguments": List[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
+
 class SparkSubmitJobDriverOutputTypeDef(
     _RequiredSparkSubmitJobDriverOutputTypeDef, _OptionalSparkSubmitJobDriverOutputTypeDef
 ):
     pass
 
-SparkSqlJobDriverTypeDef = TypedDict(
-    "SparkSqlJobDriverTypeDef",
-    {
-        "entryPoint": str,
-        "sparkSqlParameters": str,
-    },
-    total=False,
-)
 
 _RequiredSparkSubmitJobDriverTypeDef = TypedDict(
     "_RequiredSparkSubmitJobDriverTypeDef",
     {
         "entryPoint": str,
     },
 )
@@ -452,75 +350,54 @@
     {
         "entryPointArguments": Sequence[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
+
 class SparkSubmitJobDriverTypeDef(
     _RequiredSparkSubmitJobDriverTypeDef, _OptionalSparkSubmitJobDriverTypeDef
 ):
     pass
 
-RetryPolicyConfigurationOutputTypeDef = TypedDict(
-    "RetryPolicyConfigurationOutputTypeDef",
+
+RetryPolicyConfigurationTypeDef = TypedDict(
+    "RetryPolicyConfigurationTypeDef",
     {
         "maxAttempts": int,
     },
 )
 
 RetryPolicyExecutionTypeDef = TypedDict(
     "RetryPolicyExecutionTypeDef",
     {
         "currentAttemptCount": int,
     },
 )
 
-TemplateParameterConfigurationOutputTypeDef = TypedDict(
-    "TemplateParameterConfigurationOutputTypeDef",
-    {
-        "type": TemplateParameterDataTypeType,
-        "defaultValue": str,
-    },
-    total=False,
-)
-
 TemplateParameterConfigurationTypeDef = TypedDict(
     "TemplateParameterConfigurationTypeDef",
     {
         "type": TemplateParameterDataTypeType,
         "defaultValue": str,
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "virtualClusterId": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
-        "name": str,
-        "states": Sequence[JobRunStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListJobRunsRequestListJobRunsPaginateTypeDef(
-    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
-    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
-):
-    pass
-
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -532,64 +409,32 @@
         "states": Sequence[JobRunStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
-    "_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
-    {
-        "virtualClusterId": str,
-    },
-)
-_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
-    "_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
-    {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
-        "types": Sequence[str],
-        "states": Sequence[EndpointStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
-    _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
-    _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
-):
-    pass
-
 _RequiredListManagedEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListManagedEndpointsRequestRequestTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListManagedEndpointsRequestRequestTypeDef = TypedDict(
@@ -601,171 +446,166 @@
         "states": Sequence[EndpointStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListManagedEndpointsRequestRequestTypeDef(
     _RequiredListManagedEndpointsRequestRequestTypeDef,
     _OptionalListManagedEndpointsRequestRequestTypeDef,
 ):
     pass
 
+
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
-ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
-    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
-    {
-        "containerProviderId": str,
-        "containerProviderType": Literal["EKS"],
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "states": Sequence[VirtualClusterStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVirtualClustersRequestRequestTypeDef = TypedDict(
     "ListVirtualClustersRequestRequestTypeDef",
     {
         "containerProviderId": str,
         "containerProviderType": Literal["EKS"],
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
         "states": Sequence[VirtualClusterStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-S3MonitoringConfigurationOutputTypeDef = TypedDict(
-    "S3MonitoringConfigurationOutputTypeDef",
-    {
-        "logUri": str,
-    },
-)
-
 S3MonitoringConfigurationTypeDef = TypedDict(
     "S3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ParametricCloudWatchMonitoringConfigurationTypeDef = TypedDict(
+    "ParametricCloudWatchMonitoringConfigurationTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "logGroupName": str,
+        "logStreamNamePrefix": str,
     },
     total=False,
 )
 
-ParametricCloudWatchMonitoringConfigurationOutputTypeDef = TypedDict(
-    "ParametricCloudWatchMonitoringConfigurationOutputTypeDef",
+ParametricS3MonitoringConfigurationTypeDef = TypedDict(
+    "ParametricS3MonitoringConfigurationTypeDef",
     {
-        "logGroupName": str,
-        "logStreamNamePrefix": str,
+        "logUri": str,
     },
     total=False,
 )
 
-ParametricCloudWatchMonitoringConfigurationTypeDef = TypedDict(
-    "ParametricCloudWatchMonitoringConfigurationTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "logGroupName": str,
-        "logStreamNamePrefix": str,
+        "resourceArn": str,
+        "tags": Mapping[str, str],
     },
-    total=False,
 )
 
-ParametricS3MonitoringConfigurationOutputTypeDef = TypedDict(
-    "ParametricS3MonitoringConfigurationOutputTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "logUri": str,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
-    total=False,
 )
 
-ParametricS3MonitoringConfigurationTypeDef = TypedDict(
-    "ParametricS3MonitoringConfigurationTypeDef",
+CancelJobRunResponseTypeDef = TypedDict(
+    "CancelJobRunResponseTypeDef",
     {
-        "logUri": str,
+        "id": str,
+        "virtualClusterId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateJobTemplateResponseTypeDef = TypedDict(
+    "CreateJobTemplateResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "id": str,
+        "name": str,
+        "arn": str,
+        "createdAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RetryPolicyConfigurationTypeDef = TypedDict(
-    "RetryPolicyConfigurationTypeDef",
+CreateManagedEndpointResponseTypeDef = TypedDict(
+    "CreateManagedEndpointResponseTypeDef",
     {
-        "maxAttempts": int,
+        "id": str,
+        "name": str,
+        "arn": str,
+        "virtualClusterId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
+CreateVirtualClusterResponseTypeDef = TypedDict(
+    "CreateVirtualClusterResponseTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteJobTemplateResponseTypeDef = TypedDict(
+    "DeleteJobTemplateResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteManagedEndpointResponseTypeDef = TypedDict(
+    "DeleteManagedEndpointResponseTypeDef",
+    {
+        "id": str,
         "virtualClusterId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+DeleteVirtualClusterResponseTypeDef = TypedDict(
+    "DeleteVirtualClusterResponseTypeDef",
     {
-        "resourceArn": str,
-        "tags": Mapping[str, str],
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ContainerInfoOutputTypeDef = TypedDict(
-    "ContainerInfoOutputTypeDef",
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
     {
-        "eksInfo": EksInfoOutputTypeDef,
+        "id": str,
+        "name": str,
+        "arn": str,
+        "virtualClusterId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ContainerInfoTypeDef = TypedDict(
     "ContainerInfoTypeDef",
     {
         "eksInfo": EksInfoTypeDef,
     },
@@ -774,100 +614,132 @@
 
 GetManagedEndpointSessionCredentialsResponseTypeDef = TypedDict(
     "GetManagedEndpointSessionCredentialsResponseTypeDef",
     {
         "id": str,
         "credentials": CredentialsTypeDef,
         "expiresAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobDriverOutputTypeDef = TypedDict(
     "JobDriverOutputTypeDef",
     {
         "sparkSubmitJobDriver": SparkSubmitJobDriverOutputTypeDef,
-        "sparkSqlJobDriver": SparkSqlJobDriverOutputTypeDef,
+        "sparkSqlJobDriver": SparkSqlJobDriverTypeDef,
     },
     total=False,
 )
 
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmitJobDriver": SparkSubmitJobDriverTypeDef,
         "sparkSqlJobDriver": SparkSqlJobDriverTypeDef,
     },
     total=False,
 )
 
-MonitoringConfigurationOutputTypeDef = TypedDict(
-    "MonitoringConfigurationOutputTypeDef",
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
     {
-        "persistentAppUI": PersistentAppUIType,
-        "cloudWatchMonitoringConfiguration": CloudWatchMonitoringConfigurationOutputTypeDef,
-        "s3MonitoringConfiguration": S3MonitoringConfigurationOutputTypeDef,
-        "containerLogRotationConfiguration": ContainerLogRotationConfigurationOutputTypeDef,
+        "virtualClusterId": str,
+    },
+)
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "createdBefore": Union[datetime, str],
+        "createdAfter": Union[datetime, str],
+        "name": str,
+        "states": Sequence[JobRunStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-MonitoringConfigurationTypeDef = TypedDict(
-    "MonitoringConfigurationTypeDef",
+
+class ListJobRunsRequestListJobRunsPaginateTypeDef(
+    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
+    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
+):
+    pass
+
+
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     {
-        "persistentAppUI": PersistentAppUIType,
-        "cloudWatchMonitoringConfiguration": CloudWatchMonitoringConfigurationTypeDef,
-        "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
-        "containerLogRotationConfiguration": ContainerLogRotationConfigurationTypeDef,
+        "createdAfter": Union[datetime, str],
+        "createdBefore": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ParametricMonitoringConfigurationOutputTypeDef = TypedDict(
-    "ParametricMonitoringConfigurationOutputTypeDef",
+_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
+    "_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     {
-        "persistentAppUI": str,
-        "cloudWatchMonitoringConfiguration": (
-            ParametricCloudWatchMonitoringConfigurationOutputTypeDef
-        ),
-        "s3MonitoringConfiguration": ParametricS3MonitoringConfigurationOutputTypeDef,
+        "virtualClusterId": str,
+    },
+)
+_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
+    "_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
+    {
+        "createdBefore": Union[datetime, str],
+        "createdAfter": Union[datetime, str],
+        "types": Sequence[str],
+        "states": Sequence[EndpointStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ParametricMonitoringConfigurationTypeDef = TypedDict(
-    "ParametricMonitoringConfigurationTypeDef",
+
+class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
+    _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
+    _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
+):
+    pass
+
+
+ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
+    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     {
-        "persistentAppUI": str,
-        "cloudWatchMonitoringConfiguration": ParametricCloudWatchMonitoringConfigurationTypeDef,
-        "s3MonitoringConfiguration": ParametricS3MonitoringConfigurationTypeDef,
+        "containerProviderId": str,
+        "containerProviderType": Literal["EKS"],
+        "createdAfter": Union[datetime, str],
+        "createdBefore": Union[datetime, str],
+        "states": Sequence[VirtualClusterStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredContainerProviderOutputTypeDef = TypedDict(
-    "_RequiredContainerProviderOutputTypeDef",
+MonitoringConfigurationTypeDef = TypedDict(
+    "MonitoringConfigurationTypeDef",
     {
-        "type": Literal["EKS"],
-        "id": str,
+        "persistentAppUI": PersistentAppUIType,
+        "cloudWatchMonitoringConfiguration": CloudWatchMonitoringConfigurationTypeDef,
+        "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
+        "containerLogRotationConfiguration": ContainerLogRotationConfigurationTypeDef,
     },
+    total=False,
 )
-_OptionalContainerProviderOutputTypeDef = TypedDict(
-    "_OptionalContainerProviderOutputTypeDef",
+
+ParametricMonitoringConfigurationTypeDef = TypedDict(
+    "ParametricMonitoringConfigurationTypeDef",
     {
-        "info": ContainerInfoOutputTypeDef,
+        "persistentAppUI": str,
+        "cloudWatchMonitoringConfiguration": ParametricCloudWatchMonitoringConfigurationTypeDef,
+        "s3MonitoringConfiguration": ParametricS3MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
-class ContainerProviderOutputTypeDef(
-    _RequiredContainerProviderOutputTypeDef, _OptionalContainerProviderOutputTypeDef
-):
-    pass
-
 _RequiredContainerProviderTypeDef = TypedDict(
     "_RequiredContainerProviderTypeDef",
     {
         "type": Literal["EKS"],
         "id": str,
     },
 )
@@ -875,24 +747,26 @@
     "_OptionalContainerProviderTypeDef",
     {
         "info": ContainerInfoTypeDef,
     },
     total=False,
 )
 
+
 class ContainerProviderTypeDef(
     _RequiredContainerProviderTypeDef, _OptionalContainerProviderTypeDef
 ):
     pass
 
+
 ConfigurationOverridesOutputTypeDef = TypedDict(
     "ConfigurationOverridesOutputTypeDef",
     {
         "applicationConfiguration": List["ConfigurationOutputTypeDef"],
-        "monitoringConfiguration": MonitoringConfigurationOutputTypeDef,
+        "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
 ConfigurationOverridesTypeDef = TypedDict(
     "ConfigurationOverridesTypeDef",
     {
@@ -902,42 +776,28 @@
     total=False,
 )
 
 ParametricConfigurationOverridesOutputTypeDef = TypedDict(
     "ParametricConfigurationOverridesOutputTypeDef",
     {
         "applicationConfiguration": List["ConfigurationOutputTypeDef"],
-        "monitoringConfiguration": ParametricMonitoringConfigurationOutputTypeDef,
+        "monitoringConfiguration": ParametricMonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
 ParametricConfigurationOverridesTypeDef = TypedDict(
     "ParametricConfigurationOverridesTypeDef",
     {
         "applicationConfiguration": Sequence["ConfigurationTypeDef"],
         "monitoringConfiguration": ParametricMonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
-VirtualClusterTypeDef = TypedDict(
-    "VirtualClusterTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "arn": str,
-        "state": VirtualClusterStateType,
-        "containerProvider": ContainerProviderOutputTypeDef,
-        "createdAt": datetime,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredCreateVirtualClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualClusterRequestRequestTypeDef",
     {
         "name": str,
         "containerProvider": ContainerProviderTypeDef,
         "clientToken": str,
     },
@@ -946,20 +806,36 @@
     "_OptionalCreateVirtualClusterRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateVirtualClusterRequestRequestTypeDef(
     _RequiredCreateVirtualClusterRequestRequestTypeDef,
     _OptionalCreateVirtualClusterRequestRequestTypeDef,
 ):
     pass
 
+
+VirtualClusterTypeDef = TypedDict(
+    "VirtualClusterTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "arn": str,
+        "state": VirtualClusterStateType,
+        "containerProvider": ContainerProviderTypeDef,
+        "createdAt": datetime,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "virtualClusterId": str,
@@ -996,15 +872,15 @@
         "jobDriver": JobDriverOutputTypeDef,
         "createdAt": datetime,
         "createdBy": str,
         "finishedAt": datetime,
         "stateDetails": str,
         "failureReason": FailureReasonType,
         "tags": Dict[str, str],
-        "retryPolicyConfiguration": RetryPolicyConfigurationOutputTypeDef,
+        "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
         "retryPolicyExecution": RetryPolicyExecutionTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateManagedEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateManagedEndpointRequestRequestTypeDef",
@@ -1023,20 +899,22 @@
         "certificateArn": str,
         "configurationOverrides": ConfigurationOverridesTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateManagedEndpointRequestRequestTypeDef(
     _RequiredCreateManagedEndpointRequestRequestTypeDef,
     _OptionalCreateManagedEndpointRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "virtualClusterId": str,
         "clientToken": str,
     },
 )
@@ -1052,42 +930,46 @@
         "jobTemplateId": str,
         "jobTemplateParameters": Mapping[str, str],
         "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredJobTemplateDataOutputTypeDef = TypedDict(
     "_RequiredJobTemplateDataOutputTypeDef",
     {
         "executionRoleArn": str,
         "releaseLabel": str,
         "jobDriver": JobDriverOutputTypeDef,
     },
 )
 _OptionalJobTemplateDataOutputTypeDef = TypedDict(
     "_OptionalJobTemplateDataOutputTypeDef",
     {
         "configurationOverrides": ParametricConfigurationOverridesOutputTypeDef,
-        "parameterConfiguration": Dict[str, TemplateParameterConfigurationOutputTypeDef],
+        "parameterConfiguration": Dict[str, TemplateParameterConfigurationTypeDef],
         "jobTags": Dict[str, str],
     },
     total=False,
 )
 
+
 class JobTemplateDataOutputTypeDef(
     _RequiredJobTemplateDataOutputTypeDef, _OptionalJobTemplateDataOutputTypeDef
 ):
     pass
 
+
 _RequiredJobTemplateDataTypeDef = TypedDict(
     "_RequiredJobTemplateDataTypeDef",
     {
         "executionRoleArn": str,
         "releaseLabel": str,
         "jobDriver": JobDriverTypeDef,
     },
@@ -1098,65 +980,67 @@
         "configurationOverrides": ParametricConfigurationOverridesTypeDef,
         "parameterConfiguration": Mapping[str, TemplateParameterConfigurationTypeDef],
         "jobTags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class JobTemplateDataTypeDef(_RequiredJobTemplateDataTypeDef, _OptionalJobTemplateDataTypeDef):
     pass
 
+
 DescribeVirtualClusterResponseTypeDef = TypedDict(
     "DescribeVirtualClusterResponseTypeDef",
     {
         "virtualCluster": VirtualClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualClustersResponseTypeDef = TypedDict(
     "ListVirtualClustersResponseTypeDef",
     {
         "virtualClusters": List[VirtualClusterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeManagedEndpointResponseTypeDef = TypedDict(
     "DescribeManagedEndpointResponseTypeDef",
     {
         "endpoint": EndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListManagedEndpointsResponseTypeDef = TypedDict(
     "ListManagedEndpointsResponseTypeDef",
     {
         "endpoints": List[EndpointTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobRunResponseTypeDef = TypedDict(
     "DescribeJobRunResponseTypeDef",
     {
         "jobRun": JobRunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "jobRuns": List[JobRunTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJobTemplateTypeDef = TypedDict(
     "_RequiredJobTemplateTypeDef",
     {
         "jobTemplateData": JobTemplateDataOutputTypeDef,
@@ -1173,17 +1057,19 @@
         "tags": Dict[str, str],
         "kmsKeyArn": str,
         "decryptionError": str,
     },
     total=False,
 )
 
+
 class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
     pass
 
+
 _RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobTemplateRequestRequestTypeDef",
     {
         "name": str,
         "clientToken": str,
         "jobTemplateData": JobTemplateDataTypeDef,
     },
@@ -1193,28 +1079,30 @@
     {
         "tags": Mapping[str, str],
         "kmsKeyArn": str,
     },
     total=False,
 )
 
+
 class CreateJobTemplateRequestRequestTypeDef(
     _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
     pass
 
+
 DescribeJobTemplateResponseTypeDef = TypedDict(
     "DescribeJobTemplateResponseTypeDef",
     {
         "jobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "templates": List[JobTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/PKG-INFO` & `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-containers
-Version: 1.28.12
-Summary: Type annotations for boto3.EMRContainers 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.EMRContainers 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-containers)](https://pepy.tech/project/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
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
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,86 +343,73 @@
 
 `mypy_boto3_emr_containers.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_containers.type_defs import (
     CancelJobRunRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
+    ResponseMetadataTypeDef,
     CertificateTypeDef,
-    CloudWatchMonitoringConfigurationOutputTypeDef,
     CloudWatchMonitoringConfigurationTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
-    EksInfoOutputTypeDef,
     EksInfoTypeDef,
-    ContainerLogRotationConfigurationOutputTypeDef,
     ContainerLogRotationConfigurationTypeDef,
-    CreateJobTemplateResponseTypeDef,
-    CreateManagedEndpointResponseTypeDef,
-    CreateVirtualClusterResponseTypeDef,
     CredentialsTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
-    DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointRequestRequestTypeDef,
-    DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterRequestRequestTypeDef,
-    DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
     DescribeManagedEndpointRequestRequestTypeDef,
     DescribeVirtualClusterRequestRequestTypeDef,
     GetManagedEndpointSessionCredentialsRequestRequestTypeDef,
-    SparkSqlJobDriverOutputTypeDef,
-    SparkSubmitJobDriverOutputTypeDef,
     SparkSqlJobDriverTypeDef,
+    SparkSubmitJobDriverOutputTypeDef,
     SparkSubmitJobDriverTypeDef,
-    RetryPolicyConfigurationOutputTypeDef,
+    RetryPolicyConfigurationTypeDef,
     RetryPolicyExecutionTypeDef,
-    TemplateParameterConfigurationOutputTypeDef,
     TemplateParameterConfigurationTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListJobRunsRequestRequestTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     ListManagedEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
     ListVirtualClustersRequestRequestTypeDef,
-    S3MonitoringConfigurationOutputTypeDef,
     S3MonitoringConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ParametricCloudWatchMonitoringConfigurationOutputTypeDef,
     ParametricCloudWatchMonitoringConfigurationTypeDef,
-    ParametricS3MonitoringConfigurationOutputTypeDef,
     ParametricS3MonitoringConfigurationTypeDef,
-    ResponseMetadataTypeDef,
-    RetryPolicyConfigurationTypeDef,
-    StartJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ContainerInfoOutputTypeDef,
+    CancelJobRunResponseTypeDef,
+    CreateJobTemplateResponseTypeDef,
+    CreateManagedEndpointResponseTypeDef,
+    CreateVirtualClusterResponseTypeDef,
+    DeleteJobTemplateResponseTypeDef,
+    DeleteManagedEndpointResponseTypeDef,
+    DeleteVirtualClusterResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartJobRunResponseTypeDef,
     ContainerInfoTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
     JobDriverOutputTypeDef,
     JobDriverTypeDef,
-    MonitoringConfigurationOutputTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
+    ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
     MonitoringConfigurationTypeDef,
-    ParametricMonitoringConfigurationOutputTypeDef,
     ParametricMonitoringConfigurationTypeDef,
-    ContainerProviderOutputTypeDef,
     ContainerProviderTypeDef,
     ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     ParametricConfigurationOverridesOutputTypeDef,
     ParametricConfigurationOverridesTypeDef,
-    VirtualClusterTypeDef,
     CreateVirtualClusterRequestRequestTypeDef,
+    VirtualClusterTypeDef,
     EndpointTypeDef,
     JobRunTypeDef,
     CreateManagedEndpointRequestRequestTypeDef,
     StartJobRunRequestRequestTypeDef,
     JobTemplateDataOutputTypeDef,
     JobTemplateDataTypeDef,
     DescribeVirtualClusterResponseTypeDef,
```

### Comparing `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/SOURCES.txt` & `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.12/setup.py` & `mypy-boto3-emr-containers-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr-containers",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_emr_containers"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMRContainers 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.EMRContainers 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

