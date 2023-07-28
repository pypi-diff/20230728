# Comparing `tmp/mypy-boto3-robomaker-1.28.12.tar.gz` & `tmp/mypy-boto3-robomaker-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-robomaker-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
+gzip compressed data, was "mypy-boto3-robomaker-1.28.15.tar", last modified: Fri Jul 28 20:43:35 2023, max compression
```

## Comparing `mypy-boto3-robomaker-1.28.12.tar` & `mypy-boto3-robomaker-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.421214 mypy-boto3-robomaker-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-07-27 11:49:30.421214 mypy-boto3-robomaker-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.421214 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42233 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42158 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-07-27 11:44:44.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-07-27 11:44:44.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-07-27 11:44:44.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-07-27 11:44:47.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    72951 2023-07-27 11:44:45.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.421214 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-07-27 11:49:30.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 11:49:30.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:30.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 11:49:30.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.421214 mypy-boto3-robomaker-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:35.113746 mypy-boto3-robomaker-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22084 2023-07-28 20:43:35.113746 mypy-boto3-robomaker-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20589 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:35.113746 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42233 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42158 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-07-28 20:37:03.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-07-28 20:37:03.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-07-28 20:37:03.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-07-28 20:37:03.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68764 2023-07-28 20:37:05.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68697 2023-07-28 20:37:04.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:35.113746 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22084 2023-07-28 20:43:34.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:43:34.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:34.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:34.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:34.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:43:34.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:35.113746 mypy-boto3-robomaker-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/setup.py
```

### Comparing `mypy-boto3-robomaker-1.28.12/LICENSE` & `mypy-boto3-robomaker-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.12/PKG-INFO` & `mypy-boto3-robomaker-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-robomaker
-Version: 1.28.12
-Summary: Type annotations for boto3.RoboMaker 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.RoboMaker 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-robomaker)](https://pepy.tech/project/mypy-boto3-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RoboMaker 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[boto3.RoboMaker 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [mypy-boto3-robomaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -391,58 +391,48 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_robomaker.type_defs import (
     BatchDeleteWorldsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     BatchDescribeSimulationJobRequestRequestTypeDef,
-    BatchPolicyOutputTypeDef,
     BatchPolicyTypeDef,
     CancelDeploymentJobRequestRequestTypeDef,
     CancelSimulationJobBatchRequestRequestTypeDef,
     CancelSimulationJobRequestRequestTypeDef,
     CancelWorldExportJobRequestRequestTypeDef,
     CancelWorldGenerationJobRequestRequestTypeDef,
-    ComputeOutputTypeDef,
     ComputeResponseTypeDef,
     ComputeTypeDef,
     CreateFleetRequestRequestTypeDef,
     EnvironmentTypeDef,
     RobotSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
-    EnvironmentOutputTypeDef,
-    RobotSoftwareSuiteOutputTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
-    RenderingEngineOutputTypeDef,
-    SimulationSoftwareSuiteOutputTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
     DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
-    LoggingConfigOutputTypeDef,
-    OutputLocationOutputTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
-    WorldCountOutputTypeDef,
     TemplateLocationTypeDef,
     DataSourceConfigOutputTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
     DeploymentLaunchConfigOutputTypeDef,
     DeploymentLaunchConfigTypeDef,
-    S3ObjectOutputTypeDef,
     S3ObjectTypeDef,
     DeregisterRobotRequestRequestTypeDef,
     DescribeDeploymentJobRequestRequestTypeDef,
     DescribeFleetRequestRequestTypeDef,
     RobotTypeDef,
     DescribeRobotApplicationRequestRequestTypeDef,
     DescribeRobotRequestRequestTypeDef,
@@ -461,24 +451,20 @@
     GetWorldTemplateBodyRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     SimulationJobBatchSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWorldTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     WorldSummaryTypeDef,
-    PortMappingOutputTypeDef,
     PortMappingTypeDef,
     ProgressDetailTypeDef,
     RegisterRobotRequestRequestTypeDef,
     RestartSimulationJobRequestRequestTypeDef,
-    ToolOutputTypeDef,
-    UploadConfigurationOutputTypeDef,
     ToolTypeDef,
     UploadConfigurationTypeDef,
-    WorldConfigOutputTypeDef,
     WorldConfigTypeDef,
     VPCConfigOutputTypeDef,
     SyncDeploymentJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchDeleteWorldsResponseTypeDef,
     CreateFleetResponseTypeDef,
@@ -488,41 +474,40 @@
     DescribeRobotResponseTypeDef,
     DescribeWorldResponseTypeDef,
     DescribeWorldTemplateResponseTypeDef,
     GetWorldTemplateBodyResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     RegisterRobotResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
+    RobotApplicationSummaryTypeDef,
     CreateRobotApplicationRequestRequestTypeDef,
     UpdateRobotApplicationRequestRequestTypeDef,
-    RobotApplicationSummaryTypeDef,
     CreateRobotApplicationResponseTypeDef,
     CreateRobotApplicationVersionResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
     UpdateRobotApplicationResponseTypeDef,
     CreateSimulationApplicationRequestRequestTypeDef,
-    UpdateSimulationApplicationRequestRequestTypeDef,
     CreateSimulationApplicationResponseTypeDef,
     CreateSimulationApplicationVersionResponseTypeDef,
     DescribeSimulationApplicationResponseTypeDef,
     SimulationApplicationSummaryTypeDef,
+    UpdateSimulationApplicationRequestRequestTypeDef,
     UpdateSimulationApplicationResponseTypeDef,
     CreateWorldExportJobRequestRequestTypeDef,
     CreateWorldExportJobResponseTypeDef,
     DescribeWorldExportJobResponseTypeDef,
     WorldExportJobSummaryTypeDef,
     CreateWorldGenerationJobRequestRequestTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     WorldGenerationJobSummaryTypeDef,
     CreateWorldTemplateRequestRequestTypeDef,
     UpdateWorldTemplateRequestRequestTypeDef,
     DataSourceTypeDef,
     DeploymentApplicationConfigOutputTypeDef,
     DeploymentApplicationConfigTypeDef,
-    DeploymentConfigOutputTypeDef,
     DeploymentConfigTypeDef,
     DescribeFleetResponseTypeDef,
     ListRobotsResponseTypeDef,
     ListSimulationJobsResponseTypeDef,
     FailureSummaryTypeDef,
     ListDeploymentJobsRequestRequestTypeDef,
     ListFleetsRequestRequestTypeDef,
@@ -552,18 +537,18 @@
     PortForwardingConfigOutputTypeDef,
     PortForwardingConfigTypeDef,
     RobotDeploymentTypeDef,
     ListRobotApplicationsResponseTypeDef,
     ListSimulationApplicationsResponseTypeDef,
     ListWorldExportJobsResponseTypeDef,
     ListWorldGenerationJobsResponseTypeDef,
+    CreateDeploymentJobRequestRequestTypeDef,
     CreateDeploymentJobResponseTypeDef,
     DeploymentJobTypeDef,
     SyncDeploymentJobResponseTypeDef,
-    CreateDeploymentJobRequestRequestTypeDef,
     FinishedWorldsSummaryTypeDef,
     LaunchConfigOutputTypeDef,
     LaunchConfigTypeDef,
     DescribeDeploymentJobResponseTypeDef,
     ListDeploymentJobsResponseTypeDef,
     DescribeWorldGenerationJobResponseTypeDef,
     RobotApplicationConfigOutputTypeDef,
```

### Comparing `mypy-boto3-robomaker-1.28.12/README.md` & `mypy-boto3-robomaker-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-robomaker)](https://pepy.tech/project/mypy-boto3-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RoboMaker 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[boto3.RoboMaker 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [mypy-boto3-robomaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,58 +359,48 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_robomaker.type_defs import (
     BatchDeleteWorldsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     BatchDescribeSimulationJobRequestRequestTypeDef,
-    BatchPolicyOutputTypeDef,
     BatchPolicyTypeDef,
     CancelDeploymentJobRequestRequestTypeDef,
     CancelSimulationJobBatchRequestRequestTypeDef,
     CancelSimulationJobRequestRequestTypeDef,
     CancelWorldExportJobRequestRequestTypeDef,
     CancelWorldGenerationJobRequestRequestTypeDef,
-    ComputeOutputTypeDef,
     ComputeResponseTypeDef,
     ComputeTypeDef,
     CreateFleetRequestRequestTypeDef,
     EnvironmentTypeDef,
     RobotSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
-    EnvironmentOutputTypeDef,
-    RobotSoftwareSuiteOutputTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
-    RenderingEngineOutputTypeDef,
-    SimulationSoftwareSuiteOutputTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
     DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
-    LoggingConfigOutputTypeDef,
-    OutputLocationOutputTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
-    WorldCountOutputTypeDef,
     TemplateLocationTypeDef,
     DataSourceConfigOutputTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
     DeploymentLaunchConfigOutputTypeDef,
     DeploymentLaunchConfigTypeDef,
-    S3ObjectOutputTypeDef,
     S3ObjectTypeDef,
     DeregisterRobotRequestRequestTypeDef,
     DescribeDeploymentJobRequestRequestTypeDef,
     DescribeFleetRequestRequestTypeDef,
     RobotTypeDef,
     DescribeRobotApplicationRequestRequestTypeDef,
     DescribeRobotRequestRequestTypeDef,
@@ -429,24 +419,20 @@
     GetWorldTemplateBodyRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     SimulationJobBatchSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWorldTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     WorldSummaryTypeDef,
-    PortMappingOutputTypeDef,
     PortMappingTypeDef,
     ProgressDetailTypeDef,
     RegisterRobotRequestRequestTypeDef,
     RestartSimulationJobRequestRequestTypeDef,
-    ToolOutputTypeDef,
-    UploadConfigurationOutputTypeDef,
     ToolTypeDef,
     UploadConfigurationTypeDef,
-    WorldConfigOutputTypeDef,
     WorldConfigTypeDef,
     VPCConfigOutputTypeDef,
     SyncDeploymentJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchDeleteWorldsResponseTypeDef,
     CreateFleetResponseTypeDef,
@@ -456,41 +442,40 @@
     DescribeRobotResponseTypeDef,
     DescribeWorldResponseTypeDef,
     DescribeWorldTemplateResponseTypeDef,
     GetWorldTemplateBodyResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     RegisterRobotResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
+    RobotApplicationSummaryTypeDef,
     CreateRobotApplicationRequestRequestTypeDef,
     UpdateRobotApplicationRequestRequestTypeDef,
-    RobotApplicationSummaryTypeDef,
     CreateRobotApplicationResponseTypeDef,
     CreateRobotApplicationVersionResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
     UpdateRobotApplicationResponseTypeDef,
     CreateSimulationApplicationRequestRequestTypeDef,
-    UpdateSimulationApplicationRequestRequestTypeDef,
     CreateSimulationApplicationResponseTypeDef,
     CreateSimulationApplicationVersionResponseTypeDef,
     DescribeSimulationApplicationResponseTypeDef,
     SimulationApplicationSummaryTypeDef,
+    UpdateSimulationApplicationRequestRequestTypeDef,
     UpdateSimulationApplicationResponseTypeDef,
     CreateWorldExportJobRequestRequestTypeDef,
     CreateWorldExportJobResponseTypeDef,
     DescribeWorldExportJobResponseTypeDef,
     WorldExportJobSummaryTypeDef,
     CreateWorldGenerationJobRequestRequestTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     WorldGenerationJobSummaryTypeDef,
     CreateWorldTemplateRequestRequestTypeDef,
     UpdateWorldTemplateRequestRequestTypeDef,
     DataSourceTypeDef,
     DeploymentApplicationConfigOutputTypeDef,
     DeploymentApplicationConfigTypeDef,
-    DeploymentConfigOutputTypeDef,
     DeploymentConfigTypeDef,
     DescribeFleetResponseTypeDef,
     ListRobotsResponseTypeDef,
     ListSimulationJobsResponseTypeDef,
     FailureSummaryTypeDef,
     ListDeploymentJobsRequestRequestTypeDef,
     ListFleetsRequestRequestTypeDef,
@@ -520,18 +505,18 @@
     PortForwardingConfigOutputTypeDef,
     PortForwardingConfigTypeDef,
     RobotDeploymentTypeDef,
     ListRobotApplicationsResponseTypeDef,
     ListSimulationApplicationsResponseTypeDef,
     ListWorldExportJobsResponseTypeDef,
     ListWorldGenerationJobsResponseTypeDef,
+    CreateDeploymentJobRequestRequestTypeDef,
     CreateDeploymentJobResponseTypeDef,
     DeploymentJobTypeDef,
     SyncDeploymentJobResponseTypeDef,
-    CreateDeploymentJobRequestRequestTypeDef,
     FinishedWorldsSummaryTypeDef,
     LaunchConfigOutputTypeDef,
     LaunchConfigTypeDef,
     DescribeDeploymentJobResponseTypeDef,
     ListDeploymentJobsResponseTypeDef,
     DescribeWorldGenerationJobResponseTypeDef,
     RobotApplicationConfigOutputTypeDef,
```

### Comparing `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/__init__.py` & `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/__init__.pyi` & `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/__main__.py` & `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RoboMaker 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.RoboMaker 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker\nOther"
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

### Comparing `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/client.py` & `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/client.pyi` & `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/literals.py` & `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/literals.pyi` & `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/paginator.py` & `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/paginator.pyi` & `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/type_defs.py` & `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,58 +48,48 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BatchDeleteWorldsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDescribeSimulationJobRequestRequestTypeDef",
-    "BatchPolicyOutputTypeDef",
     "BatchPolicyTypeDef",
     "CancelDeploymentJobRequestRequestTypeDef",
     "CancelSimulationJobBatchRequestRequestTypeDef",
     "CancelSimulationJobRequestRequestTypeDef",
     "CancelWorldExportJobRequestRequestTypeDef",
     "CancelWorldGenerationJobRequestRequestTypeDef",
-    "ComputeOutputTypeDef",
     "ComputeResponseTypeDef",
     "ComputeTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "EnvironmentTypeDef",
     "RobotSoftwareSuiteTypeDef",
     "SourceConfigTypeDef",
-    "EnvironmentOutputTypeDef",
-    "RobotSoftwareSuiteOutputTypeDef",
     "SourceTypeDef",
     "CreateRobotApplicationVersionRequestRequestTypeDef",
     "CreateRobotRequestRequestTypeDef",
     "RenderingEngineTypeDef",
     "SimulationSoftwareSuiteTypeDef",
-    "RenderingEngineOutputTypeDef",
-    "SimulationSoftwareSuiteOutputTypeDef",
     "CreateSimulationApplicationVersionRequestRequestTypeDef",
     "DataSourceConfigTypeDef",
     "LoggingConfigTypeDef",
     "OutputLocationTypeDef",
     "VPCConfigTypeDef",
-    "LoggingConfigOutputTypeDef",
-    "OutputLocationOutputTypeDef",
     "VPCConfigResponseTypeDef",
     "WorldCountTypeDef",
-    "WorldCountOutputTypeDef",
     "TemplateLocationTypeDef",
     "DataSourceConfigOutputTypeDef",
     "S3KeyOutputTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteRobotApplicationRequestRequestTypeDef",
     "DeleteRobotRequestRequestTypeDef",
     "DeleteSimulationApplicationRequestRequestTypeDef",
     "DeleteWorldTemplateRequestRequestTypeDef",
     "DeploymentLaunchConfigOutputTypeDef",
     "DeploymentLaunchConfigTypeDef",
-    "S3ObjectOutputTypeDef",
     "S3ObjectTypeDef",
     "DeregisterRobotRequestRequestTypeDef",
     "DescribeDeploymentJobRequestRequestTypeDef",
     "DescribeFleetRequestRequestTypeDef",
     "RobotTypeDef",
     "DescribeRobotApplicationRequestRequestTypeDef",
     "DescribeRobotRequestRequestTypeDef",
@@ -118,24 +108,20 @@
     "GetWorldTemplateBodyRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "SimulationJobBatchSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorldTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "WorldSummaryTypeDef",
-    "PortMappingOutputTypeDef",
     "PortMappingTypeDef",
     "ProgressDetailTypeDef",
     "RegisterRobotRequestRequestTypeDef",
     "RestartSimulationJobRequestRequestTypeDef",
-    "ToolOutputTypeDef",
-    "UploadConfigurationOutputTypeDef",
     "ToolTypeDef",
     "UploadConfigurationTypeDef",
-    "WorldConfigOutputTypeDef",
     "WorldConfigTypeDef",
     "VPCConfigOutputTypeDef",
     "SyncDeploymentJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchDeleteWorldsResponseTypeDef",
     "CreateFleetResponseTypeDef",
@@ -145,41 +131,40 @@
     "DescribeRobotResponseTypeDef",
     "DescribeWorldResponseTypeDef",
     "DescribeWorldTemplateResponseTypeDef",
     "GetWorldTemplateBodyResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RegisterRobotResponseTypeDef",
     "UpdateWorldTemplateResponseTypeDef",
+    "RobotApplicationSummaryTypeDef",
     "CreateRobotApplicationRequestRequestTypeDef",
     "UpdateRobotApplicationRequestRequestTypeDef",
-    "RobotApplicationSummaryTypeDef",
     "CreateRobotApplicationResponseTypeDef",
     "CreateRobotApplicationVersionResponseTypeDef",
     "DescribeRobotApplicationResponseTypeDef",
     "UpdateRobotApplicationResponseTypeDef",
     "CreateSimulationApplicationRequestRequestTypeDef",
-    "UpdateSimulationApplicationRequestRequestTypeDef",
     "CreateSimulationApplicationResponseTypeDef",
     "CreateSimulationApplicationVersionResponseTypeDef",
     "DescribeSimulationApplicationResponseTypeDef",
     "SimulationApplicationSummaryTypeDef",
+    "UpdateSimulationApplicationRequestRequestTypeDef",
     "UpdateSimulationApplicationResponseTypeDef",
     "CreateWorldExportJobRequestRequestTypeDef",
     "CreateWorldExportJobResponseTypeDef",
     "DescribeWorldExportJobResponseTypeDef",
     "WorldExportJobSummaryTypeDef",
     "CreateWorldGenerationJobRequestRequestTypeDef",
     "CreateWorldGenerationJobResponseTypeDef",
     "WorldGenerationJobSummaryTypeDef",
     "CreateWorldTemplateRequestRequestTypeDef",
     "UpdateWorldTemplateRequestRequestTypeDef",
     "DataSourceTypeDef",
     "DeploymentApplicationConfigOutputTypeDef",
     "DeploymentApplicationConfigTypeDef",
-    "DeploymentConfigOutputTypeDef",
     "DeploymentConfigTypeDef",
     "DescribeFleetResponseTypeDef",
     "ListRobotsResponseTypeDef",
     "ListSimulationJobsResponseTypeDef",
     "FailureSummaryTypeDef",
     "ListDeploymentJobsRequestRequestTypeDef",
     "ListFleetsRequestRequestTypeDef",
@@ -209,18 +194,18 @@
     "PortForwardingConfigOutputTypeDef",
     "PortForwardingConfigTypeDef",
     "RobotDeploymentTypeDef",
     "ListRobotApplicationsResponseTypeDef",
     "ListSimulationApplicationsResponseTypeDef",
     "ListWorldExportJobsResponseTypeDef",
     "ListWorldGenerationJobsResponseTypeDef",
+    "CreateDeploymentJobRequestRequestTypeDef",
     "CreateDeploymentJobResponseTypeDef",
     "DeploymentJobTypeDef",
     "SyncDeploymentJobResponseTypeDef",
-    "CreateDeploymentJobRequestRequestTypeDef",
     "FinishedWorldsSummaryTypeDef",
     "LaunchConfigOutputTypeDef",
     "LaunchConfigTypeDef",
     "DescribeDeploymentJobResponseTypeDef",
     "ListDeploymentJobsResponseTypeDef",
     "DescribeWorldGenerationJobResponseTypeDef",
     "RobotApplicationConfigOutputTypeDef",
@@ -261,23 +246,14 @@
 BatchDescribeSimulationJobRequestRequestTypeDef = TypedDict(
     "BatchDescribeSimulationJobRequestRequestTypeDef",
     {
         "jobs": Sequence[str],
     },
 )
 
-BatchPolicyOutputTypeDef = TypedDict(
-    "BatchPolicyOutputTypeDef",
-    {
-        "timeoutInSeconds": int,
-        "maxConcurrency": int,
-    },
-    total=False,
-)
-
 BatchPolicyTypeDef = TypedDict(
     "BatchPolicyTypeDef",
     {
         "timeoutInSeconds": int,
         "maxConcurrency": int,
     },
     total=False,
@@ -314,24 +290,14 @@
 CancelWorldGenerationJobRequestRequestTypeDef = TypedDict(
     "CancelWorldGenerationJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
-ComputeOutputTypeDef = TypedDict(
-    "ComputeOutputTypeDef",
-    {
-        "simulationUnitLimit": int,
-        "computeType": ComputeTypeType,
-        "gpuUnitLimit": int,
-    },
-    total=False,
-)
-
 ComputeResponseTypeDef = TypedDict(
     "ComputeResponseTypeDef",
     {
         "simulationUnitLimit": int,
         "computeType": ComputeTypeType,
         "gpuUnitLimit": int,
     },
@@ -392,31 +358,14 @@
         "s3Bucket": str,
         "s3Key": str,
         "architecture": ArchitectureType,
     },
     total=False,
 )
 
-EnvironmentOutputTypeDef = TypedDict(
-    "EnvironmentOutputTypeDef",
-    {
-        "uri": str,
-    },
-    total=False,
-)
-
-RobotSoftwareSuiteOutputTypeDef = TypedDict(
-    "RobotSoftwareSuiteOutputTypeDef",
-    {
-        "name": RobotSoftwareSuiteTypeType,
-        "version": RobotSoftwareSuiteVersionTypeType,
-    },
-    total=False,
-)
-
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
         "etag": str,
         "architecture": ArchitectureType,
@@ -485,32 +434,14 @@
     {
         "name": SimulationSoftwareSuiteTypeType,
         "version": str,
     },
     total=False,
 )
 
-RenderingEngineOutputTypeDef = TypedDict(
-    "RenderingEngineOutputTypeDef",
-    {
-        "name": Literal["OGRE"],
-        "version": str,
-    },
-    total=False,
-)
-
-SimulationSoftwareSuiteOutputTypeDef = TypedDict(
-    "SimulationSoftwareSuiteOutputTypeDef",
-    {
-        "name": SimulationSoftwareSuiteTypeType,
-        "version": str,
-    },
-    total=False,
-)
-
 _RequiredCreateSimulationApplicationVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSimulationApplicationVersionRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalCreateSimulationApplicationVersionRequestRequestTypeDef = TypedDict(
@@ -586,31 +517,14 @@
 )
 
 
 class VPCConfigTypeDef(_RequiredVPCConfigTypeDef, _OptionalVPCConfigTypeDef):
     pass
 
 
-LoggingConfigOutputTypeDef = TypedDict(
-    "LoggingConfigOutputTypeDef",
-    {
-        "recordAllRosTopics": bool,
-    },
-    total=False,
-)
-
-OutputLocationOutputTypeDef = TypedDict(
-    "OutputLocationOutputTypeDef",
-    {
-        "s3Bucket": str,
-        "s3Prefix": str,
-    },
-    total=False,
-)
-
 VPCConfigResponseTypeDef = TypedDict(
     "VPCConfigResponseTypeDef",
     {
         "subnets": List[str],
         "securityGroups": List[str],
         "vpcId": str,
         "assignPublicIp": bool,
@@ -623,23 +537,14 @@
     {
         "floorplanCount": int,
         "interiorCountPerFloorplan": int,
     },
     total=False,
 )
 
-WorldCountOutputTypeDef = TypedDict(
-    "WorldCountOutputTypeDef",
-    {
-        "floorplanCount": int,
-        "interiorCountPerFloorplan": int,
-    },
-    total=False,
-)
-
 TemplateLocationTypeDef = TypedDict(
     "TemplateLocationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
@@ -786,34 +691,14 @@
 
 class DeploymentLaunchConfigTypeDef(
     _RequiredDeploymentLaunchConfigTypeDef, _OptionalDeploymentLaunchConfigTypeDef
 ):
     pass
 
 
-_RequiredS3ObjectOutputTypeDef = TypedDict(
-    "_RequiredS3ObjectOutputTypeDef",
-    {
-        "bucket": str,
-        "key": str,
-    },
-)
-_OptionalS3ObjectOutputTypeDef = TypedDict(
-    "_OptionalS3ObjectOutputTypeDef",
-    {
-        "etag": str,
-    },
-    total=False,
-)
-
-
-class S3ObjectOutputTypeDef(_RequiredS3ObjectOutputTypeDef, _OptionalS3ObjectOutputTypeDef):
-    pass
-
-
 _RequiredS3ObjectTypeDef = TypedDict(
     "_RequiredS3ObjectTypeDef",
     {
         "bucket": str,
         "key": str,
     },
 )
@@ -1086,36 +971,14 @@
         "createdAt": datetime,
         "generationJob": str,
         "template": str,
     },
     total=False,
 )
 
-_RequiredPortMappingOutputTypeDef = TypedDict(
-    "_RequiredPortMappingOutputTypeDef",
-    {
-        "jobPort": int,
-        "applicationPort": int,
-    },
-)
-_OptionalPortMappingOutputTypeDef = TypedDict(
-    "_OptionalPortMappingOutputTypeDef",
-    {
-        "enableOnPublicIp": bool,
-    },
-    total=False,
-)
-
-
-class PortMappingOutputTypeDef(
-    _RequiredPortMappingOutputTypeDef, _OptionalPortMappingOutputTypeDef
-):
-    pass
-
-
 _RequiredPortMappingTypeDef = TypedDict(
     "_RequiredPortMappingTypeDef",
     {
         "jobPort": int,
         "applicationPort": int,
     },
 )
@@ -1154,45 +1017,14 @@
 RestartSimulationJobRequestRequestTypeDef = TypedDict(
     "RestartSimulationJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
-_RequiredToolOutputTypeDef = TypedDict(
-    "_RequiredToolOutputTypeDef",
-    {
-        "name": str,
-        "command": str,
-    },
-)
-_OptionalToolOutputTypeDef = TypedDict(
-    "_OptionalToolOutputTypeDef",
-    {
-        "streamUI": bool,
-        "streamOutputToCloudWatch": bool,
-        "exitBehavior": ExitBehaviorType,
-    },
-    total=False,
-)
-
-
-class ToolOutputTypeDef(_RequiredToolOutputTypeDef, _OptionalToolOutputTypeDef):
-    pass
-
-
-UploadConfigurationOutputTypeDef = TypedDict(
-    "UploadConfigurationOutputTypeDef",
-    {
-        "name": str,
-        "path": str,
-        "uploadBehavior": UploadBehaviorType,
-    },
-)
-
 _RequiredToolTypeDef = TypedDict(
     "_RequiredToolTypeDef",
     {
         "name": str,
         "command": str,
     },
 )
@@ -1216,22 +1048,14 @@
     {
         "name": str,
         "path": str,
         "uploadBehavior": UploadBehaviorType,
     },
 )
 
-WorldConfigOutputTypeDef = TypedDict(
-    "WorldConfigOutputTypeDef",
-    {
-        "world": str,
-    },
-    total=False,
-)
-
 WorldConfigTypeDef = TypedDict(
     "WorldConfigTypeDef",
     {
         "world": str,
     },
     total=False,
 )
@@ -1409,14 +1233,26 @@
         "name": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RobotApplicationSummaryTypeDef = TypedDict(
+    "RobotApplicationSummaryTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "version": str,
+        "lastUpdatedAt": datetime,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateRobotApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRobotApplicationRequestRequestTypeDef",
     {
         "name": str,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
     },
 )
@@ -1459,85 +1295,73 @@
 class UpdateRobotApplicationRequestRequestTypeDef(
     _RequiredUpdateRobotApplicationRequestRequestTypeDef,
     _OptionalUpdateRobotApplicationRequestRequestTypeDef,
 ):
     pass
 
 
-RobotApplicationSummaryTypeDef = TypedDict(
-    "RobotApplicationSummaryTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "version": str,
-        "lastUpdatedAt": datetime,
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
-    },
-    total=False,
-)
-
 CreateRobotApplicationResponseTypeDef = TypedDict(
     "CreateRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRobotApplicationVersionResponseTypeDef = TypedDict(
     "CreateRobotApplicationVersionResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRobotApplicationResponseTypeDef = TypedDict(
     "DescribeRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "imageDigest": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRobotApplicationResponseTypeDef = TypedDict(
     "UpdateRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSimulationApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSimulationApplicationRequestRequestTypeDef",
     {
@@ -1561,121 +1385,121 @@
 class CreateSimulationApplicationRequestRequestTypeDef(
     _RequiredCreateSimulationApplicationRequestRequestTypeDef,
     _OptionalCreateSimulationApplicationRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSimulationApplicationRequestRequestTypeDef",
-    {
-        "application": str,
-        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
-    },
-)
-_OptionalUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSimulationApplicationRequestRequestTypeDef",
-    {
-        "sources": Sequence[SourceConfigTypeDef],
-        "renderingEngine": RenderingEngineTypeDef,
-        "currentRevisionId": str,
-        "environment": EnvironmentTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateSimulationApplicationRequestRequestTypeDef(
-    _RequiredUpdateSimulationApplicationRequestRequestTypeDef,
-    _OptionalUpdateSimulationApplicationRequestRequestTypeDef,
-):
-    pass
-
-
 CreateSimulationApplicationResponseTypeDef = TypedDict(
     "CreateSimulationApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
-        "renderingEngine": RenderingEngineOutputTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSimulationApplicationVersionResponseTypeDef = TypedDict(
     "CreateSimulationApplicationVersionResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
-        "renderingEngine": RenderingEngineOutputTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSimulationApplicationResponseTypeDef = TypedDict(
     "DescribeSimulationApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
-        "renderingEngine": RenderingEngineOutputTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "renderingEngine": RenderingEngineTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "imageDigest": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SimulationApplicationSummaryTypeDef = TypedDict(
     "SimulationApplicationSummaryTypeDef",
     {
         "name": str,
         "arn": str,
         "version": str,
         "lastUpdatedAt": datetime,
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
-        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
     },
     total=False,
 )
 
+_RequiredUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSimulationApplicationRequestRequestTypeDef",
+    {
+        "application": str,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+    },
+)
+_OptionalUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSimulationApplicationRequestRequestTypeDef",
+    {
+        "sources": Sequence[SourceConfigTypeDef],
+        "renderingEngine": RenderingEngineTypeDef,
+        "currentRevisionId": str,
+        "environment": EnvironmentTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateSimulationApplicationRequestRequestTypeDef(
+    _RequiredUpdateSimulationApplicationRequestRequestTypeDef,
+    _OptionalUpdateSimulationApplicationRequestRequestTypeDef,
+):
+    pass
+
+
 UpdateSimulationApplicationResponseTypeDef = TypedDict(
     "UpdateSimulationApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
-        "renderingEngine": RenderingEngineOutputTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWorldExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorldExportJobRequestRequestTypeDef",
     {
@@ -1705,15 +1529,15 @@
     "CreateWorldExportJobResponseTypeDef",
     {
         "arn": str,
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldExportJobErrorCodeType,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationOutputTypeDef,
+        "outputLocation": OutputLocationTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorldExportJobResponseTypeDef = TypedDict(
@@ -1722,29 +1546,29 @@
         "arn": str,
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldExportJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
         "worlds": List[str],
-        "outputLocation": OutputLocationOutputTypeDef,
+        "outputLocation": OutputLocationTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorldExportJobSummaryTypeDef = TypedDict(
     "WorldExportJobSummaryTypeDef",
     {
         "arn": str,
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "worlds": List[str],
-        "outputLocation": OutputLocationOutputTypeDef,
+        "outputLocation": OutputLocationTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateWorldGenerationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorldGenerationJobRequestRequestTypeDef",
     {
@@ -1775,29 +1599,29 @@
     {
         "arn": str,
         "status": WorldGenerationJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldGenerationJobErrorCodeType,
         "clientRequestToken": str,
         "template": str,
-        "worldCount": WorldCountOutputTypeDef,
+        "worldCount": WorldCountTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorldGenerationJobSummaryTypeDef = TypedDict(
     "WorldGenerationJobSummaryTypeDef",
     {
         "arn": str,
         "template": str,
         "createdAt": datetime,
         "status": WorldGenerationJobStatusType,
-        "worldCount": WorldCountOutputTypeDef,
+        "worldCount": WorldCountTypeDef,
         "succeededWorldCount": int,
         "failedWorldCount": int,
     },
     total=False,
 )
 
 CreateWorldTemplateRequestRequestTypeDef = TypedDict(
@@ -1862,25 +1686,14 @@
     {
         "application": str,
         "applicationVersion": str,
         "launchConfig": DeploymentLaunchConfigTypeDef,
     },
 )
 
-DeploymentConfigOutputTypeDef = TypedDict(
-    "DeploymentConfigOutputTypeDef",
-    {
-        "concurrentDeploymentPercentage": int,
-        "failureThresholdPercentage": int,
-        "robotDeploymentTimeoutInSeconds": int,
-        "downloadConditionFile": S3ObjectOutputTypeDef,
-    },
-    total=False,
-)
-
 DeploymentConfigTypeDef = TypedDict(
     "DeploymentConfigTypeDef",
     {
         "concurrentDeploymentPercentage": int,
         "failureThresholdPercentage": int,
         "robotDeploymentTimeoutInSeconds": int,
         "downloadConditionFile": S3ObjectTypeDef,
@@ -2167,15 +1980,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PortForwardingConfigOutputTypeDef = TypedDict(
     "PortForwardingConfigOutputTypeDef",
     {
-        "portMappings": List[PortMappingOutputTypeDef],
+        "portMappings": List[PortMappingTypeDef],
     },
     total=False,
 )
 
 PortForwardingConfigTypeDef = TypedDict(
     "PortForwardingConfigTypeDef",
     {
@@ -2230,85 +2043,85 @@
     {
         "worldGenerationJobSummaries": List[WorldGenerationJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "fleet": str,
+        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigTypeDef],
+    },
+)
+_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "deploymentConfig": DeploymentConfigTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateDeploymentJobRequestRequestTypeDef(
+    _RequiredCreateDeploymentJobRequestRequestTypeDef,
+    _OptionalCreateDeploymentJobRequestRequestTypeDef,
+):
+    pass
+
+
 CreateDeploymentJobResponseTypeDef = TypedDict(
     "CreateDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
-        "deploymentConfig": DeploymentConfigOutputTypeDef,
+        "deploymentConfig": DeploymentConfigTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentJobTypeDef = TypedDict(
     "DeploymentJobTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
-        "deploymentConfig": DeploymentConfigOutputTypeDef,
+        "deploymentConfig": DeploymentConfigTypeDef,
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
     },
     total=False,
 )
 
 SyncDeploymentJobResponseTypeDef = TypedDict(
     "SyncDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentConfig": DeploymentConfigOutputTypeDef,
+        "deploymentConfig": DeploymentConfigTypeDef,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-        "fleet": str,
-        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigTypeDef],
-    },
-)
-_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "deploymentConfig": DeploymentConfigTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateDeploymentJobRequestRequestTypeDef(
-    _RequiredCreateDeploymentJobRequestRequestTypeDef,
-    _OptionalCreateDeploymentJobRequestRequestTypeDef,
-):
-    pass
-
-
 FinishedWorldsSummaryTypeDef = TypedDict(
     "FinishedWorldsSummaryTypeDef",
     {
         "finishedCount": int,
         "succeededWorlds": List[str],
         "failureSummary": FailureSummaryTypeDef,
     },
@@ -2343,15 +2156,15 @@
 
 DescribeDeploymentJobResponseTypeDef = TypedDict(
     "DescribeDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentConfig": DeploymentConfigOutputTypeDef,
+        "deploymentConfig": DeploymentConfigTypeDef,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "robotDeploymentSummary": List[RobotDeploymentTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2373,15 +2186,15 @@
         "arn": str,
         "status": WorldGenerationJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldGenerationJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
         "template": str,
-        "worldCount": WorldCountOutputTypeDef,
+        "worldCount": WorldCountTypeDef,
         "finishedWorldsSummary": FinishedWorldsSummaryTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2392,17 +2205,17 @@
         "launchConfig": LaunchConfigOutputTypeDef,
     },
 )
 _OptionalRobotApplicationConfigOutputTypeDef = TypedDict(
     "_OptionalRobotApplicationConfigOutputTypeDef",
     {
         "applicationVersion": str,
-        "uploadConfigurations": List[UploadConfigurationOutputTypeDef],
+        "uploadConfigurations": List[UploadConfigurationTypeDef],
         "useDefaultUploadConfigurations": bool,
-        "tools": List[ToolOutputTypeDef],
+        "tools": List[ToolTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
 
 class RobotApplicationConfigOutputTypeDef(
@@ -2418,18 +2231,18 @@
         "launchConfig": LaunchConfigOutputTypeDef,
     },
 )
 _OptionalSimulationApplicationConfigOutputTypeDef = TypedDict(
     "_OptionalSimulationApplicationConfigOutputTypeDef",
     {
         "applicationVersion": str,
-        "uploadConfigurations": List[UploadConfigurationOutputTypeDef],
-        "worldConfigs": List[WorldConfigOutputTypeDef],
+        "uploadConfigurations": List[UploadConfigurationTypeDef],
+        "worldConfigs": List[WorldConfigTypeDef],
         "useDefaultUploadConfigurations": bool,
-        "tools": List[ToolOutputTypeDef],
+        "tools": List[ToolTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
 
 class SimulationApplicationConfigOutputTypeDef(
@@ -2498,16 +2311,16 @@
         "arn": str,
         "status": SimulationJobStatusType,
         "lastStartedAt": datetime,
         "lastUpdatedAt": datetime,
         "failureBehavior": FailureBehaviorType,
         "failureCode": SimulationJobErrorCodeType,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationOutputTypeDef,
-        "loggingConfig": LoggingConfigOutputTypeDef,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
         "robotApplications": List[RobotApplicationConfigOutputTypeDef],
         "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
@@ -2525,16 +2338,16 @@
         "status": SimulationJobStatusType,
         "lastStartedAt": datetime,
         "lastUpdatedAt": datetime,
         "failureBehavior": FailureBehaviorType,
         "failureCode": SimulationJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationOutputTypeDef,
-        "loggingConfig": LoggingConfigOutputTypeDef,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
         "robotApplications": List[RobotApplicationConfigOutputTypeDef],
         "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
@@ -2550,24 +2363,24 @@
     {
         "maxJobDurationInSeconds": int,
     },
 )
 _OptionalSimulationJobRequestOutputTypeDef = TypedDict(
     "_OptionalSimulationJobRequestOutputTypeDef",
     {
-        "outputLocation": OutputLocationOutputTypeDef,
-        "loggingConfig": LoggingConfigOutputTypeDef,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
         "iamRole": str,
         "failureBehavior": FailureBehaviorType,
         "useDefaultApplications": bool,
         "robotApplications": List[RobotApplicationConfigOutputTypeDef],
         "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceConfigOutputTypeDef],
         "vpcConfig": VPCConfigOutputTypeDef,
-        "compute": ComputeOutputTypeDef,
+        "compute": ComputeTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
 class SimulationJobRequestOutputTypeDef(
@@ -2584,16 +2397,16 @@
         "status": SimulationJobStatusType,
         "lastStartedAt": datetime,
         "lastUpdatedAt": datetime,
         "failureBehavior": FailureBehaviorType,
         "failureCode": SimulationJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationOutputTypeDef,
-        "loggingConfig": LoggingConfigOutputTypeDef,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
         "robotApplications": List[RobotApplicationConfigOutputTypeDef],
         "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
@@ -2715,15 +2528,15 @@
     "DescribeSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "lastUpdatedAt": datetime,
         "createdAt": datetime,
         "clientRequestToken": str,
-        "batchPolicy": BatchPolicyOutputTypeDef,
+        "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
         "pendingRequests": List[SimulationJobRequestOutputTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2733,15 +2546,15 @@
 StartSimulationJobBatchResponseTypeDef = TypedDict(
     "StartSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "createdAt": datetime,
         "clientRequestToken": str,
-        "batchPolicy": BatchPolicyOutputTypeDef,
+        "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
         "pendingRequests": List[SimulationJobRequestOutputTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/type_defs.pyi` & `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -47,58 +47,48 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BatchDeleteWorldsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDescribeSimulationJobRequestRequestTypeDef",
-    "BatchPolicyOutputTypeDef",
     "BatchPolicyTypeDef",
     "CancelDeploymentJobRequestRequestTypeDef",
     "CancelSimulationJobBatchRequestRequestTypeDef",
     "CancelSimulationJobRequestRequestTypeDef",
     "CancelWorldExportJobRequestRequestTypeDef",
     "CancelWorldGenerationJobRequestRequestTypeDef",
-    "ComputeOutputTypeDef",
     "ComputeResponseTypeDef",
     "ComputeTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "EnvironmentTypeDef",
     "RobotSoftwareSuiteTypeDef",
     "SourceConfigTypeDef",
-    "EnvironmentOutputTypeDef",
-    "RobotSoftwareSuiteOutputTypeDef",
     "SourceTypeDef",
     "CreateRobotApplicationVersionRequestRequestTypeDef",
     "CreateRobotRequestRequestTypeDef",
     "RenderingEngineTypeDef",
     "SimulationSoftwareSuiteTypeDef",
-    "RenderingEngineOutputTypeDef",
-    "SimulationSoftwareSuiteOutputTypeDef",
     "CreateSimulationApplicationVersionRequestRequestTypeDef",
     "DataSourceConfigTypeDef",
     "LoggingConfigTypeDef",
     "OutputLocationTypeDef",
     "VPCConfigTypeDef",
-    "LoggingConfigOutputTypeDef",
-    "OutputLocationOutputTypeDef",
     "VPCConfigResponseTypeDef",
     "WorldCountTypeDef",
-    "WorldCountOutputTypeDef",
     "TemplateLocationTypeDef",
     "DataSourceConfigOutputTypeDef",
     "S3KeyOutputTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteRobotApplicationRequestRequestTypeDef",
     "DeleteRobotRequestRequestTypeDef",
     "DeleteSimulationApplicationRequestRequestTypeDef",
     "DeleteWorldTemplateRequestRequestTypeDef",
     "DeploymentLaunchConfigOutputTypeDef",
     "DeploymentLaunchConfigTypeDef",
-    "S3ObjectOutputTypeDef",
     "S3ObjectTypeDef",
     "DeregisterRobotRequestRequestTypeDef",
     "DescribeDeploymentJobRequestRequestTypeDef",
     "DescribeFleetRequestRequestTypeDef",
     "RobotTypeDef",
     "DescribeRobotApplicationRequestRequestTypeDef",
     "DescribeRobotRequestRequestTypeDef",
@@ -117,24 +107,20 @@
     "GetWorldTemplateBodyRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "SimulationJobBatchSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorldTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "WorldSummaryTypeDef",
-    "PortMappingOutputTypeDef",
     "PortMappingTypeDef",
     "ProgressDetailTypeDef",
     "RegisterRobotRequestRequestTypeDef",
     "RestartSimulationJobRequestRequestTypeDef",
-    "ToolOutputTypeDef",
-    "UploadConfigurationOutputTypeDef",
     "ToolTypeDef",
     "UploadConfigurationTypeDef",
-    "WorldConfigOutputTypeDef",
     "WorldConfigTypeDef",
     "VPCConfigOutputTypeDef",
     "SyncDeploymentJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchDeleteWorldsResponseTypeDef",
     "CreateFleetResponseTypeDef",
@@ -144,41 +130,40 @@
     "DescribeRobotResponseTypeDef",
     "DescribeWorldResponseTypeDef",
     "DescribeWorldTemplateResponseTypeDef",
     "GetWorldTemplateBodyResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RegisterRobotResponseTypeDef",
     "UpdateWorldTemplateResponseTypeDef",
+    "RobotApplicationSummaryTypeDef",
     "CreateRobotApplicationRequestRequestTypeDef",
     "UpdateRobotApplicationRequestRequestTypeDef",
-    "RobotApplicationSummaryTypeDef",
     "CreateRobotApplicationResponseTypeDef",
     "CreateRobotApplicationVersionResponseTypeDef",
     "DescribeRobotApplicationResponseTypeDef",
     "UpdateRobotApplicationResponseTypeDef",
     "CreateSimulationApplicationRequestRequestTypeDef",
-    "UpdateSimulationApplicationRequestRequestTypeDef",
     "CreateSimulationApplicationResponseTypeDef",
     "CreateSimulationApplicationVersionResponseTypeDef",
     "DescribeSimulationApplicationResponseTypeDef",
     "SimulationApplicationSummaryTypeDef",
+    "UpdateSimulationApplicationRequestRequestTypeDef",
     "UpdateSimulationApplicationResponseTypeDef",
     "CreateWorldExportJobRequestRequestTypeDef",
     "CreateWorldExportJobResponseTypeDef",
     "DescribeWorldExportJobResponseTypeDef",
     "WorldExportJobSummaryTypeDef",
     "CreateWorldGenerationJobRequestRequestTypeDef",
     "CreateWorldGenerationJobResponseTypeDef",
     "WorldGenerationJobSummaryTypeDef",
     "CreateWorldTemplateRequestRequestTypeDef",
     "UpdateWorldTemplateRequestRequestTypeDef",
     "DataSourceTypeDef",
     "DeploymentApplicationConfigOutputTypeDef",
     "DeploymentApplicationConfigTypeDef",
-    "DeploymentConfigOutputTypeDef",
     "DeploymentConfigTypeDef",
     "DescribeFleetResponseTypeDef",
     "ListRobotsResponseTypeDef",
     "ListSimulationJobsResponseTypeDef",
     "FailureSummaryTypeDef",
     "ListDeploymentJobsRequestRequestTypeDef",
     "ListFleetsRequestRequestTypeDef",
@@ -208,18 +193,18 @@
     "PortForwardingConfigOutputTypeDef",
     "PortForwardingConfigTypeDef",
     "RobotDeploymentTypeDef",
     "ListRobotApplicationsResponseTypeDef",
     "ListSimulationApplicationsResponseTypeDef",
     "ListWorldExportJobsResponseTypeDef",
     "ListWorldGenerationJobsResponseTypeDef",
+    "CreateDeploymentJobRequestRequestTypeDef",
     "CreateDeploymentJobResponseTypeDef",
     "DeploymentJobTypeDef",
     "SyncDeploymentJobResponseTypeDef",
-    "CreateDeploymentJobRequestRequestTypeDef",
     "FinishedWorldsSummaryTypeDef",
     "LaunchConfigOutputTypeDef",
     "LaunchConfigTypeDef",
     "DescribeDeploymentJobResponseTypeDef",
     "ListDeploymentJobsResponseTypeDef",
     "DescribeWorldGenerationJobResponseTypeDef",
     "RobotApplicationConfigOutputTypeDef",
@@ -260,23 +245,14 @@
 BatchDescribeSimulationJobRequestRequestTypeDef = TypedDict(
     "BatchDescribeSimulationJobRequestRequestTypeDef",
     {
         "jobs": Sequence[str],
     },
 )
 
-BatchPolicyOutputTypeDef = TypedDict(
-    "BatchPolicyOutputTypeDef",
-    {
-        "timeoutInSeconds": int,
-        "maxConcurrency": int,
-    },
-    total=False,
-)
-
 BatchPolicyTypeDef = TypedDict(
     "BatchPolicyTypeDef",
     {
         "timeoutInSeconds": int,
         "maxConcurrency": int,
     },
     total=False,
@@ -313,24 +289,14 @@
 CancelWorldGenerationJobRequestRequestTypeDef = TypedDict(
     "CancelWorldGenerationJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
-ComputeOutputTypeDef = TypedDict(
-    "ComputeOutputTypeDef",
-    {
-        "simulationUnitLimit": int,
-        "computeType": ComputeTypeType,
-        "gpuUnitLimit": int,
-    },
-    total=False,
-)
-
 ComputeResponseTypeDef = TypedDict(
     "ComputeResponseTypeDef",
     {
         "simulationUnitLimit": int,
         "computeType": ComputeTypeType,
         "gpuUnitLimit": int,
     },
@@ -389,31 +355,14 @@
         "s3Bucket": str,
         "s3Key": str,
         "architecture": ArchitectureType,
     },
     total=False,
 )
 
-EnvironmentOutputTypeDef = TypedDict(
-    "EnvironmentOutputTypeDef",
-    {
-        "uri": str,
-    },
-    total=False,
-)
-
-RobotSoftwareSuiteOutputTypeDef = TypedDict(
-    "RobotSoftwareSuiteOutputTypeDef",
-    {
-        "name": RobotSoftwareSuiteTypeType,
-        "version": RobotSoftwareSuiteVersionTypeType,
-    },
-    total=False,
-)
-
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
         "etag": str,
         "architecture": ArchitectureType,
@@ -478,32 +427,14 @@
     {
         "name": SimulationSoftwareSuiteTypeType,
         "version": str,
     },
     total=False,
 )
 
-RenderingEngineOutputTypeDef = TypedDict(
-    "RenderingEngineOutputTypeDef",
-    {
-        "name": Literal["OGRE"],
-        "version": str,
-    },
-    total=False,
-)
-
-SimulationSoftwareSuiteOutputTypeDef = TypedDict(
-    "SimulationSoftwareSuiteOutputTypeDef",
-    {
-        "name": SimulationSoftwareSuiteTypeType,
-        "version": str,
-    },
-    total=False,
-)
-
 _RequiredCreateSimulationApplicationVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSimulationApplicationVersionRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalCreateSimulationApplicationVersionRequestRequestTypeDef = TypedDict(
@@ -573,31 +504,14 @@
     },
     total=False,
 )
 
 class VPCConfigTypeDef(_RequiredVPCConfigTypeDef, _OptionalVPCConfigTypeDef):
     pass
 
-LoggingConfigOutputTypeDef = TypedDict(
-    "LoggingConfigOutputTypeDef",
-    {
-        "recordAllRosTopics": bool,
-    },
-    total=False,
-)
-
-OutputLocationOutputTypeDef = TypedDict(
-    "OutputLocationOutputTypeDef",
-    {
-        "s3Bucket": str,
-        "s3Prefix": str,
-    },
-    total=False,
-)
-
 VPCConfigResponseTypeDef = TypedDict(
     "VPCConfigResponseTypeDef",
     {
         "subnets": List[str],
         "securityGroups": List[str],
         "vpcId": str,
         "assignPublicIp": bool,
@@ -610,23 +524,14 @@
     {
         "floorplanCount": int,
         "interiorCountPerFloorplan": int,
     },
     total=False,
 )
 
-WorldCountOutputTypeDef = TypedDict(
-    "WorldCountOutputTypeDef",
-    {
-        "floorplanCount": int,
-        "interiorCountPerFloorplan": int,
-    },
-    total=False,
-)
-
 TemplateLocationTypeDef = TypedDict(
     "TemplateLocationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
@@ -763,32 +668,14 @@
 )
 
 class DeploymentLaunchConfigTypeDef(
     _RequiredDeploymentLaunchConfigTypeDef, _OptionalDeploymentLaunchConfigTypeDef
 ):
     pass
 
-_RequiredS3ObjectOutputTypeDef = TypedDict(
-    "_RequiredS3ObjectOutputTypeDef",
-    {
-        "bucket": str,
-        "key": str,
-    },
-)
-_OptionalS3ObjectOutputTypeDef = TypedDict(
-    "_OptionalS3ObjectOutputTypeDef",
-    {
-        "etag": str,
-    },
-    total=False,
-)
-
-class S3ObjectOutputTypeDef(_RequiredS3ObjectOutputTypeDef, _OptionalS3ObjectOutputTypeDef):
-    pass
-
 _RequiredS3ObjectTypeDef = TypedDict(
     "_RequiredS3ObjectTypeDef",
     {
         "bucket": str,
         "key": str,
     },
 )
@@ -1055,34 +942,14 @@
         "createdAt": datetime,
         "generationJob": str,
         "template": str,
     },
     total=False,
 )
 
-_RequiredPortMappingOutputTypeDef = TypedDict(
-    "_RequiredPortMappingOutputTypeDef",
-    {
-        "jobPort": int,
-        "applicationPort": int,
-    },
-)
-_OptionalPortMappingOutputTypeDef = TypedDict(
-    "_OptionalPortMappingOutputTypeDef",
-    {
-        "enableOnPublicIp": bool,
-    },
-    total=False,
-)
-
-class PortMappingOutputTypeDef(
-    _RequiredPortMappingOutputTypeDef, _OptionalPortMappingOutputTypeDef
-):
-    pass
-
 _RequiredPortMappingTypeDef = TypedDict(
     "_RequiredPortMappingTypeDef",
     {
         "jobPort": int,
         "applicationPort": int,
     },
 )
@@ -1119,43 +986,14 @@
 RestartSimulationJobRequestRequestTypeDef = TypedDict(
     "RestartSimulationJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
-_RequiredToolOutputTypeDef = TypedDict(
-    "_RequiredToolOutputTypeDef",
-    {
-        "name": str,
-        "command": str,
-    },
-)
-_OptionalToolOutputTypeDef = TypedDict(
-    "_OptionalToolOutputTypeDef",
-    {
-        "streamUI": bool,
-        "streamOutputToCloudWatch": bool,
-        "exitBehavior": ExitBehaviorType,
-    },
-    total=False,
-)
-
-class ToolOutputTypeDef(_RequiredToolOutputTypeDef, _OptionalToolOutputTypeDef):
-    pass
-
-UploadConfigurationOutputTypeDef = TypedDict(
-    "UploadConfigurationOutputTypeDef",
-    {
-        "name": str,
-        "path": str,
-        "uploadBehavior": UploadBehaviorType,
-    },
-)
-
 _RequiredToolTypeDef = TypedDict(
     "_RequiredToolTypeDef",
     {
         "name": str,
         "command": str,
     },
 )
@@ -1177,22 +1015,14 @@
     {
         "name": str,
         "path": str,
         "uploadBehavior": UploadBehaviorType,
     },
 )
 
-WorldConfigOutputTypeDef = TypedDict(
-    "WorldConfigOutputTypeDef",
-    {
-        "world": str,
-    },
-    total=False,
-)
-
 WorldConfigTypeDef = TypedDict(
     "WorldConfigTypeDef",
     {
         "world": str,
     },
     total=False,
 )
@@ -1368,14 +1198,26 @@
         "name": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RobotApplicationSummaryTypeDef = TypedDict(
+    "RobotApplicationSummaryTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "version": str,
+        "lastUpdatedAt": datetime,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateRobotApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRobotApplicationRequestRequestTypeDef",
     {
         "name": str,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
     },
 )
@@ -1414,85 +1256,73 @@
 
 class UpdateRobotApplicationRequestRequestTypeDef(
     _RequiredUpdateRobotApplicationRequestRequestTypeDef,
     _OptionalUpdateRobotApplicationRequestRequestTypeDef,
 ):
     pass
 
-RobotApplicationSummaryTypeDef = TypedDict(
-    "RobotApplicationSummaryTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "version": str,
-        "lastUpdatedAt": datetime,
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
-    },
-    total=False,
-)
-
 CreateRobotApplicationResponseTypeDef = TypedDict(
     "CreateRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRobotApplicationVersionResponseTypeDef = TypedDict(
     "CreateRobotApplicationVersionResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRobotApplicationResponseTypeDef = TypedDict(
     "DescribeRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "imageDigest": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRobotApplicationResponseTypeDef = TypedDict(
     "UpdateRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSimulationApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSimulationApplicationRequestRequestTypeDef",
     {
@@ -1514,119 +1344,119 @@
 
 class CreateSimulationApplicationRequestRequestTypeDef(
     _RequiredCreateSimulationApplicationRequestRequestTypeDef,
     _OptionalCreateSimulationApplicationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSimulationApplicationRequestRequestTypeDef",
-    {
-        "application": str,
-        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
-    },
-)
-_OptionalUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSimulationApplicationRequestRequestTypeDef",
-    {
-        "sources": Sequence[SourceConfigTypeDef],
-        "renderingEngine": RenderingEngineTypeDef,
-        "currentRevisionId": str,
-        "environment": EnvironmentTypeDef,
-    },
-    total=False,
-)
-
-class UpdateSimulationApplicationRequestRequestTypeDef(
-    _RequiredUpdateSimulationApplicationRequestRequestTypeDef,
-    _OptionalUpdateSimulationApplicationRequestRequestTypeDef,
-):
-    pass
-
 CreateSimulationApplicationResponseTypeDef = TypedDict(
     "CreateSimulationApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
-        "renderingEngine": RenderingEngineOutputTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSimulationApplicationVersionResponseTypeDef = TypedDict(
     "CreateSimulationApplicationVersionResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
-        "renderingEngine": RenderingEngineOutputTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSimulationApplicationResponseTypeDef = TypedDict(
     "DescribeSimulationApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
-        "renderingEngine": RenderingEngineOutputTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "renderingEngine": RenderingEngineTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "imageDigest": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SimulationApplicationSummaryTypeDef = TypedDict(
     "SimulationApplicationSummaryTypeDef",
     {
         "name": str,
         "arn": str,
         "version": str,
         "lastUpdatedAt": datetime,
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
-        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
     },
     total=False,
 )
 
+_RequiredUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSimulationApplicationRequestRequestTypeDef",
+    {
+        "application": str,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+    },
+)
+_OptionalUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSimulationApplicationRequestRequestTypeDef",
+    {
+        "sources": Sequence[SourceConfigTypeDef],
+        "renderingEngine": RenderingEngineTypeDef,
+        "currentRevisionId": str,
+        "environment": EnvironmentTypeDef,
+    },
+    total=False,
+)
+
+class UpdateSimulationApplicationRequestRequestTypeDef(
+    _RequiredUpdateSimulationApplicationRequestRequestTypeDef,
+    _OptionalUpdateSimulationApplicationRequestRequestTypeDef,
+):
+    pass
+
 UpdateSimulationApplicationResponseTypeDef = TypedDict(
     "UpdateSimulationApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
-        "renderingEngine": RenderingEngineOutputTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWorldExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorldExportJobRequestRequestTypeDef",
     {
@@ -1654,15 +1484,15 @@
     "CreateWorldExportJobResponseTypeDef",
     {
         "arn": str,
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldExportJobErrorCodeType,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationOutputTypeDef,
+        "outputLocation": OutputLocationTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorldExportJobResponseTypeDef = TypedDict(
@@ -1671,29 +1501,29 @@
         "arn": str,
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldExportJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
         "worlds": List[str],
-        "outputLocation": OutputLocationOutputTypeDef,
+        "outputLocation": OutputLocationTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorldExportJobSummaryTypeDef = TypedDict(
     "WorldExportJobSummaryTypeDef",
     {
         "arn": str,
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "worlds": List[str],
-        "outputLocation": OutputLocationOutputTypeDef,
+        "outputLocation": OutputLocationTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateWorldGenerationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorldGenerationJobRequestRequestTypeDef",
     {
@@ -1722,29 +1552,29 @@
     {
         "arn": str,
         "status": WorldGenerationJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldGenerationJobErrorCodeType,
         "clientRequestToken": str,
         "template": str,
-        "worldCount": WorldCountOutputTypeDef,
+        "worldCount": WorldCountTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorldGenerationJobSummaryTypeDef = TypedDict(
     "WorldGenerationJobSummaryTypeDef",
     {
         "arn": str,
         "template": str,
         "createdAt": datetime,
         "status": WorldGenerationJobStatusType,
-        "worldCount": WorldCountOutputTypeDef,
+        "worldCount": WorldCountTypeDef,
         "succeededWorldCount": int,
         "failedWorldCount": int,
     },
     total=False,
 )
 
 CreateWorldTemplateRequestRequestTypeDef = TypedDict(
@@ -1807,25 +1637,14 @@
     {
         "application": str,
         "applicationVersion": str,
         "launchConfig": DeploymentLaunchConfigTypeDef,
     },
 )
 
-DeploymentConfigOutputTypeDef = TypedDict(
-    "DeploymentConfigOutputTypeDef",
-    {
-        "concurrentDeploymentPercentage": int,
-        "failureThresholdPercentage": int,
-        "robotDeploymentTimeoutInSeconds": int,
-        "downloadConditionFile": S3ObjectOutputTypeDef,
-    },
-    total=False,
-)
-
 DeploymentConfigTypeDef = TypedDict(
     "DeploymentConfigTypeDef",
     {
         "concurrentDeploymentPercentage": int,
         "failureThresholdPercentage": int,
         "robotDeploymentTimeoutInSeconds": int,
         "downloadConditionFile": S3ObjectTypeDef,
@@ -2112,15 +1931,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PortForwardingConfigOutputTypeDef = TypedDict(
     "PortForwardingConfigOutputTypeDef",
     {
-        "portMappings": List[PortMappingOutputTypeDef],
+        "portMappings": List[PortMappingTypeDef],
     },
     total=False,
 )
 
 PortForwardingConfigTypeDef = TypedDict(
     "PortForwardingConfigTypeDef",
     {
@@ -2175,83 +1994,83 @@
     {
         "worldGenerationJobSummaries": List[WorldGenerationJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "fleet": str,
+        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigTypeDef],
+    },
+)
+_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "deploymentConfig": DeploymentConfigTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateDeploymentJobRequestRequestTypeDef(
+    _RequiredCreateDeploymentJobRequestRequestTypeDef,
+    _OptionalCreateDeploymentJobRequestRequestTypeDef,
+):
+    pass
+
 CreateDeploymentJobResponseTypeDef = TypedDict(
     "CreateDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
-        "deploymentConfig": DeploymentConfigOutputTypeDef,
+        "deploymentConfig": DeploymentConfigTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentJobTypeDef = TypedDict(
     "DeploymentJobTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
-        "deploymentConfig": DeploymentConfigOutputTypeDef,
+        "deploymentConfig": DeploymentConfigTypeDef,
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
     },
     total=False,
 )
 
 SyncDeploymentJobResponseTypeDef = TypedDict(
     "SyncDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentConfig": DeploymentConfigOutputTypeDef,
+        "deploymentConfig": DeploymentConfigTypeDef,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-        "fleet": str,
-        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigTypeDef],
-    },
-)
-_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "deploymentConfig": DeploymentConfigTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateDeploymentJobRequestRequestTypeDef(
-    _RequiredCreateDeploymentJobRequestRequestTypeDef,
-    _OptionalCreateDeploymentJobRequestRequestTypeDef,
-):
-    pass
-
 FinishedWorldsSummaryTypeDef = TypedDict(
     "FinishedWorldsSummaryTypeDef",
     {
         "finishedCount": int,
         "succeededWorlds": List[str],
         "failureSummary": FailureSummaryTypeDef,
     },
@@ -2286,15 +2105,15 @@
 
 DescribeDeploymentJobResponseTypeDef = TypedDict(
     "DescribeDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentConfig": DeploymentConfigOutputTypeDef,
+        "deploymentConfig": DeploymentConfigTypeDef,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "robotDeploymentSummary": List[RobotDeploymentTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2316,15 +2135,15 @@
         "arn": str,
         "status": WorldGenerationJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldGenerationJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
         "template": str,
-        "worldCount": WorldCountOutputTypeDef,
+        "worldCount": WorldCountTypeDef,
         "finishedWorldsSummary": FinishedWorldsSummaryTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2335,17 +2154,17 @@
         "launchConfig": LaunchConfigOutputTypeDef,
     },
 )
 _OptionalRobotApplicationConfigOutputTypeDef = TypedDict(
     "_OptionalRobotApplicationConfigOutputTypeDef",
     {
         "applicationVersion": str,
-        "uploadConfigurations": List[UploadConfigurationOutputTypeDef],
+        "uploadConfigurations": List[UploadConfigurationTypeDef],
         "useDefaultUploadConfigurations": bool,
-        "tools": List[ToolOutputTypeDef],
+        "tools": List[ToolTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
 class RobotApplicationConfigOutputTypeDef(
     _RequiredRobotApplicationConfigOutputTypeDef, _OptionalRobotApplicationConfigOutputTypeDef
@@ -2359,18 +2178,18 @@
         "launchConfig": LaunchConfigOutputTypeDef,
     },
 )
 _OptionalSimulationApplicationConfigOutputTypeDef = TypedDict(
     "_OptionalSimulationApplicationConfigOutputTypeDef",
     {
         "applicationVersion": str,
-        "uploadConfigurations": List[UploadConfigurationOutputTypeDef],
-        "worldConfigs": List[WorldConfigOutputTypeDef],
+        "uploadConfigurations": List[UploadConfigurationTypeDef],
+        "worldConfigs": List[WorldConfigTypeDef],
         "useDefaultUploadConfigurations": bool,
-        "tools": List[ToolOutputTypeDef],
+        "tools": List[ToolTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
 class SimulationApplicationConfigOutputTypeDef(
     _RequiredSimulationApplicationConfigOutputTypeDef,
@@ -2433,16 +2252,16 @@
         "arn": str,
         "status": SimulationJobStatusType,
         "lastStartedAt": datetime,
         "lastUpdatedAt": datetime,
         "failureBehavior": FailureBehaviorType,
         "failureCode": SimulationJobErrorCodeType,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationOutputTypeDef,
-        "loggingConfig": LoggingConfigOutputTypeDef,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
         "robotApplications": List[RobotApplicationConfigOutputTypeDef],
         "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
@@ -2460,16 +2279,16 @@
         "status": SimulationJobStatusType,
         "lastStartedAt": datetime,
         "lastUpdatedAt": datetime,
         "failureBehavior": FailureBehaviorType,
         "failureCode": SimulationJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationOutputTypeDef,
-        "loggingConfig": LoggingConfigOutputTypeDef,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
         "robotApplications": List[RobotApplicationConfigOutputTypeDef],
         "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
@@ -2485,24 +2304,24 @@
     {
         "maxJobDurationInSeconds": int,
     },
 )
 _OptionalSimulationJobRequestOutputTypeDef = TypedDict(
     "_OptionalSimulationJobRequestOutputTypeDef",
     {
-        "outputLocation": OutputLocationOutputTypeDef,
-        "loggingConfig": LoggingConfigOutputTypeDef,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
         "iamRole": str,
         "failureBehavior": FailureBehaviorType,
         "useDefaultApplications": bool,
         "robotApplications": List[RobotApplicationConfigOutputTypeDef],
         "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceConfigOutputTypeDef],
         "vpcConfig": VPCConfigOutputTypeDef,
-        "compute": ComputeOutputTypeDef,
+        "compute": ComputeTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 class SimulationJobRequestOutputTypeDef(
     _RequiredSimulationJobRequestOutputTypeDef, _OptionalSimulationJobRequestOutputTypeDef
@@ -2517,16 +2336,16 @@
         "status": SimulationJobStatusType,
         "lastStartedAt": datetime,
         "lastUpdatedAt": datetime,
         "failureBehavior": FailureBehaviorType,
         "failureCode": SimulationJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationOutputTypeDef,
-        "loggingConfig": LoggingConfigOutputTypeDef,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
         "robotApplications": List[RobotApplicationConfigOutputTypeDef],
         "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
@@ -2642,15 +2461,15 @@
     "DescribeSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "lastUpdatedAt": datetime,
         "createdAt": datetime,
         "clientRequestToken": str,
-        "batchPolicy": BatchPolicyOutputTypeDef,
+        "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
         "pendingRequests": List[SimulationJobRequestOutputTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2660,15 +2479,15 @@
 StartSimulationJobBatchResponseTypeDef = TypedDict(
     "StartSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "createdAt": datetime,
         "clientRequestToken": str,
-        "batchPolicy": BatchPolicyOutputTypeDef,
+        "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
         "pendingRequests": List[SimulationJobRequestOutputTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/PKG-INFO` & `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-robomaker
-Version: 1.28.12
-Summary: Type annotations for boto3.RoboMaker 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.RoboMaker 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-robomaker)](https://pepy.tech/project/mypy-boto3-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RoboMaker 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[boto3.RoboMaker 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [mypy-boto3-robomaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -391,58 +391,48 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_robomaker.type_defs import (
     BatchDeleteWorldsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     BatchDescribeSimulationJobRequestRequestTypeDef,
-    BatchPolicyOutputTypeDef,
     BatchPolicyTypeDef,
     CancelDeploymentJobRequestRequestTypeDef,
     CancelSimulationJobBatchRequestRequestTypeDef,
     CancelSimulationJobRequestRequestTypeDef,
     CancelWorldExportJobRequestRequestTypeDef,
     CancelWorldGenerationJobRequestRequestTypeDef,
-    ComputeOutputTypeDef,
     ComputeResponseTypeDef,
     ComputeTypeDef,
     CreateFleetRequestRequestTypeDef,
     EnvironmentTypeDef,
     RobotSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
-    EnvironmentOutputTypeDef,
-    RobotSoftwareSuiteOutputTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
-    RenderingEngineOutputTypeDef,
-    SimulationSoftwareSuiteOutputTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
     DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
-    LoggingConfigOutputTypeDef,
-    OutputLocationOutputTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
-    WorldCountOutputTypeDef,
     TemplateLocationTypeDef,
     DataSourceConfigOutputTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
     DeploymentLaunchConfigOutputTypeDef,
     DeploymentLaunchConfigTypeDef,
-    S3ObjectOutputTypeDef,
     S3ObjectTypeDef,
     DeregisterRobotRequestRequestTypeDef,
     DescribeDeploymentJobRequestRequestTypeDef,
     DescribeFleetRequestRequestTypeDef,
     RobotTypeDef,
     DescribeRobotApplicationRequestRequestTypeDef,
     DescribeRobotRequestRequestTypeDef,
@@ -461,24 +451,20 @@
     GetWorldTemplateBodyRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     SimulationJobBatchSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWorldTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     WorldSummaryTypeDef,
-    PortMappingOutputTypeDef,
     PortMappingTypeDef,
     ProgressDetailTypeDef,
     RegisterRobotRequestRequestTypeDef,
     RestartSimulationJobRequestRequestTypeDef,
-    ToolOutputTypeDef,
-    UploadConfigurationOutputTypeDef,
     ToolTypeDef,
     UploadConfigurationTypeDef,
-    WorldConfigOutputTypeDef,
     WorldConfigTypeDef,
     VPCConfigOutputTypeDef,
     SyncDeploymentJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchDeleteWorldsResponseTypeDef,
     CreateFleetResponseTypeDef,
@@ -488,41 +474,40 @@
     DescribeRobotResponseTypeDef,
     DescribeWorldResponseTypeDef,
     DescribeWorldTemplateResponseTypeDef,
     GetWorldTemplateBodyResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     RegisterRobotResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
+    RobotApplicationSummaryTypeDef,
     CreateRobotApplicationRequestRequestTypeDef,
     UpdateRobotApplicationRequestRequestTypeDef,
-    RobotApplicationSummaryTypeDef,
     CreateRobotApplicationResponseTypeDef,
     CreateRobotApplicationVersionResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
     UpdateRobotApplicationResponseTypeDef,
     CreateSimulationApplicationRequestRequestTypeDef,
-    UpdateSimulationApplicationRequestRequestTypeDef,
     CreateSimulationApplicationResponseTypeDef,
     CreateSimulationApplicationVersionResponseTypeDef,
     DescribeSimulationApplicationResponseTypeDef,
     SimulationApplicationSummaryTypeDef,
+    UpdateSimulationApplicationRequestRequestTypeDef,
     UpdateSimulationApplicationResponseTypeDef,
     CreateWorldExportJobRequestRequestTypeDef,
     CreateWorldExportJobResponseTypeDef,
     DescribeWorldExportJobResponseTypeDef,
     WorldExportJobSummaryTypeDef,
     CreateWorldGenerationJobRequestRequestTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     WorldGenerationJobSummaryTypeDef,
     CreateWorldTemplateRequestRequestTypeDef,
     UpdateWorldTemplateRequestRequestTypeDef,
     DataSourceTypeDef,
     DeploymentApplicationConfigOutputTypeDef,
     DeploymentApplicationConfigTypeDef,
-    DeploymentConfigOutputTypeDef,
     DeploymentConfigTypeDef,
     DescribeFleetResponseTypeDef,
     ListRobotsResponseTypeDef,
     ListSimulationJobsResponseTypeDef,
     FailureSummaryTypeDef,
     ListDeploymentJobsRequestRequestTypeDef,
     ListFleetsRequestRequestTypeDef,
@@ -552,18 +537,18 @@
     PortForwardingConfigOutputTypeDef,
     PortForwardingConfigTypeDef,
     RobotDeploymentTypeDef,
     ListRobotApplicationsResponseTypeDef,
     ListSimulationApplicationsResponseTypeDef,
     ListWorldExportJobsResponseTypeDef,
     ListWorldGenerationJobsResponseTypeDef,
+    CreateDeploymentJobRequestRequestTypeDef,
     CreateDeploymentJobResponseTypeDef,
     DeploymentJobTypeDef,
     SyncDeploymentJobResponseTypeDef,
-    CreateDeploymentJobRequestRequestTypeDef,
     FinishedWorldsSummaryTypeDef,
     LaunchConfigOutputTypeDef,
     LaunchConfigTypeDef,
     DescribeDeploymentJobResponseTypeDef,
     ListDeploymentJobsResponseTypeDef,
     DescribeWorldGenerationJobResponseTypeDef,
     RobotApplicationConfigOutputTypeDef,
```

### Comparing `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/SOURCES.txt` & `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.12/setup.py` & `mypy-boto3-robomaker-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-robomaker",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_robomaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RoboMaker 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.RoboMaker 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

