# Comparing `tmp/mypy-boto3-sms-1.28.12.tar.gz` & `tmp/mypy-boto3-sms-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sms-1.28.12.tar", last modified: Thu Jul 27 11:49:41 2023, max compression
+gzip compressed data, was "mypy-boto3-sms-1.28.15.tar", last modified: Fri Jul 28 20:43:46 2023, max compression
```

## Comparing `mypy-boto3-sms-1.28.12.tar` & `mypy-boto3-sms-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.077315 mypy-boto3-sms-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17464 2023-07-27 11:49:41.077315 mypy-boto3-sms-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.077315 mypy-boto3-sms-1.28.12/mypy_boto3_sms/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25869 2023-07-27 11:47:03.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25822 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-07-27 11:47:03.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-07-27 11:47:03.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-27 11:47:03.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-07-27 11:47:03.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34042 2023-07-27 11:47:04.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34025 2023-07-27 11:47:03.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.077315 mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17464 2023-07-27 11:49:40.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 11:49:40.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:40.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:40.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:40.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:40.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:41.077315 mypy-boto3-sms-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:46.229898 mypy-boto3-sms-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:35.000000 mypy-boto3-sms-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17049 2023-07-28 20:43:46.229898 mypy-boto3-sms-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-07-28 20:39:35.000000 mypy-boto3-sms-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:46.229898 mypy-boto3-sms-1.28.15/mypy_boto3_sms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-28 20:39:35.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-28 20:39:35.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:39:35.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25869 2023-07-28 20:39:35.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25822 2023-07-28 20:39:35.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-07-28 20:39:35.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-07-28 20:39:35.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-28 20:39:35.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-07-28 20:39:35.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:35.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    30477 2023-07-28 20:39:36.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30460 2023-07-28 20:39:36.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:35.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:46.229898 mypy-boto3-sms-1.28.15/mypy_boto3_sms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17049 2023-07-28 20:43:46.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:43:46.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:46.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:46.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:46.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:46.000000 mypy-boto3-sms-1.28.15/mypy_boto3_sms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:46.229898 mypy-boto3-sms-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:39:34.000000 mypy-boto3-sms-1.28.15/setup.py
```

### Comparing `mypy-boto3-sms-1.28.12/LICENSE` & `mypy-boto3-sms-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.12/PKG-INFO` & `mypy-boto3-sms-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sms
-Version: 1.28.12
-Summary: Type annotations for boto3.SMS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SMS 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sms.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sms)](https://pepy.tech/project/mypy-boto3-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
+[boto3.SMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
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
 [mypy-boto3-sms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,24 +358,23 @@
 
 ```python
 from mypy_boto3_sms.type_defs import (
     LaunchDetailsTypeDef,
     ConnectorTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
-    TagOutputTypeDef,
     CreateReplicationJobRequestRequestTypeDef,
     DeleteAppLaunchConfigurationRequestRequestTypeDef,
     DeleteAppReplicationConfigurationRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppValidationConfigurationRequestRequestTypeDef,
     DeleteReplicationJobRequestRequestTypeDef,
     DisassociateConnectorRequestRequestTypeDef,
     GenerateChangeSetRequestRequestTypeDef,
-    S3LocationOutputTypeDef,
+    S3LocationTypeDef,
     GenerateTemplateRequestRequestTypeDef,
     GetAppLaunchConfigurationRequestRequestTypeDef,
     GetAppReplicationConfigurationRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
     GetAppValidationConfigurationRequestRequestTypeDef,
     GetAppValidationOutputRequestRequestTypeDef,
     PaginatorConfigTypeDef,
@@ -384,86 +383,75 @@
     GetReplicationRunsRequestRequestTypeDef,
     VmServerAddressTypeDef,
     ImportAppCatalogRequestRequestTypeDef,
     LaunchAppRequestRequestTypeDef,
     ListAppsRequestRequestTypeDef,
     NotificationContextTypeDef,
     ReplicationRunStageDetailsTypeDef,
-    S3LocationTypeDef,
     ServerReplicationParametersOutputTypeDef,
     ServerReplicationParametersTypeDef,
     StartAppReplicationRequestRequestTypeDef,
     StartOnDemandAppReplicationRequestRequestTypeDef,
     StartOnDemandReplicationRunRequestRequestTypeDef,
     StopAppReplicationRequestRequestTypeDef,
     TerminateAppRequestRequestTypeDef,
     UpdateReplicationJobRequestRequestTypeDef,
-    VmServerAddressOutputTypeDef,
     AppSummaryTypeDef,
     CreateReplicationJobResponseTypeDef,
     GetConnectorsResponseTypeDef,
     StartOnDemandReplicationRunResponseTypeDef,
     GenerateChangeSetResponseTypeDef,
     GenerateTemplateResponseTypeDef,
     SSMOutputTypeDef,
-    SourceOutputTypeDef,
-    UserDataOutputTypeDef,
+    SourceTypeDef,
+    UserDataTypeDef,
     GetConnectorsRequestGetConnectorsPaginateTypeDef,
     GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
     GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
     ListAppsRequestListAppsPaginateTypeDef,
     GetServersRequestGetServersPaginateTypeDef,
     GetServersRequestRequestTypeDef,
     VmServerTypeDef,
     NotifyAppValidationOutputRequestRequestTypeDef,
     ReplicationRunTypeDef,
-    SourceTypeDef,
-    UserDataTypeDef,
-    VmServerOutputTypeDef,
     ListAppsResponseTypeDef,
     AppValidationOutputTypeDef,
-    SSMValidationParametersOutputTypeDef,
-    UserDataValidationParametersOutputTypeDef,
-    ServerTypeDef,
     SSMValidationParametersTypeDef,
     UserDataValidationParametersTypeDef,
+    ServerTypeDef,
     ReplicationJobTypeDef,
-    ServerOutputTypeDef,
-    AppValidationConfigurationOutputTypeDef,
+    AppValidationConfigurationTypeDef,
+    GetServersResponseTypeDef,
+    ServerGroupOutputTypeDef,
     ServerGroupTypeDef,
     ServerLaunchConfigurationTypeDef,
+    ServerReplicationConfigurationOutputTypeDef,
     ServerReplicationConfigurationTypeDef,
-    AppValidationConfigurationTypeDef,
     ServerValidationConfigurationTypeDef,
+    ServerValidationOutputTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
-    GetServersResponseTypeDef,
-    ServerGroupOutputTypeDef,
-    ServerLaunchConfigurationOutputTypeDef,
-    ServerReplicationConfigurationOutputTypeDef,
-    ServerValidationConfigurationOutputTypeDef,
-    ServerValidationOutputTypeDef,
-    CreateAppRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
-    ServerGroupLaunchConfigurationTypeDef,
-    ServerGroupReplicationConfigurationTypeDef,
-    ServerGroupValidationConfigurationTypeDef,
     CreateAppResponseTypeDef,
     GetAppResponseTypeDef,
     UpdateAppResponseTypeDef,
+    CreateAppRequestRequestTypeDef,
+    UpdateAppRequestRequestTypeDef,
     ServerGroupLaunchConfigurationOutputTypeDef,
+    ServerGroupLaunchConfigurationTypeDef,
     ServerGroupReplicationConfigurationOutputTypeDef,
+    ServerGroupReplicationConfigurationTypeDef,
     ServerGroupValidationConfigurationOutputTypeDef,
+    ServerGroupValidationConfigurationTypeDef,
     ValidationOutputTypeDef,
-    PutAppLaunchConfigurationRequestRequestTypeDef,
-    PutAppReplicationConfigurationRequestRequestTypeDef,
-    PutAppValidationConfigurationRequestRequestTypeDef,
     GetAppLaunchConfigurationResponseTypeDef,
+    PutAppLaunchConfigurationRequestRequestTypeDef,
     GetAppReplicationConfigurationResponseTypeDef,
+    PutAppReplicationConfigurationRequestRequestTypeDef,
     GetAppValidationConfigurationResponseTypeDef,
+    PutAppValidationConfigurationRequestRequestTypeDef,
     GetAppValidationOutputResponseTypeDef,
 )
 
 
 def get_structure() -> LaunchDetailsTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sms-1.28.12/README.md` & `mypy-boto3-sms-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sms.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sms)](https://pepy.tech/project/mypy-boto3-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
+[boto3.SMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
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
 [mypy-boto3-sms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,24 +326,23 @@
 
 ```python
 from mypy_boto3_sms.type_defs import (
     LaunchDetailsTypeDef,
     ConnectorTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
-    TagOutputTypeDef,
     CreateReplicationJobRequestRequestTypeDef,
     DeleteAppLaunchConfigurationRequestRequestTypeDef,
     DeleteAppReplicationConfigurationRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppValidationConfigurationRequestRequestTypeDef,
     DeleteReplicationJobRequestRequestTypeDef,
     DisassociateConnectorRequestRequestTypeDef,
     GenerateChangeSetRequestRequestTypeDef,
-    S3LocationOutputTypeDef,
+    S3LocationTypeDef,
     GenerateTemplateRequestRequestTypeDef,
     GetAppLaunchConfigurationRequestRequestTypeDef,
     GetAppReplicationConfigurationRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
     GetAppValidationConfigurationRequestRequestTypeDef,
     GetAppValidationOutputRequestRequestTypeDef,
     PaginatorConfigTypeDef,
@@ -352,86 +351,75 @@
     GetReplicationRunsRequestRequestTypeDef,
     VmServerAddressTypeDef,
     ImportAppCatalogRequestRequestTypeDef,
     LaunchAppRequestRequestTypeDef,
     ListAppsRequestRequestTypeDef,
     NotificationContextTypeDef,
     ReplicationRunStageDetailsTypeDef,
-    S3LocationTypeDef,
     ServerReplicationParametersOutputTypeDef,
     ServerReplicationParametersTypeDef,
     StartAppReplicationRequestRequestTypeDef,
     StartOnDemandAppReplicationRequestRequestTypeDef,
     StartOnDemandReplicationRunRequestRequestTypeDef,
     StopAppReplicationRequestRequestTypeDef,
     TerminateAppRequestRequestTypeDef,
     UpdateReplicationJobRequestRequestTypeDef,
-    VmServerAddressOutputTypeDef,
     AppSummaryTypeDef,
     CreateReplicationJobResponseTypeDef,
     GetConnectorsResponseTypeDef,
     StartOnDemandReplicationRunResponseTypeDef,
     GenerateChangeSetResponseTypeDef,
     GenerateTemplateResponseTypeDef,
     SSMOutputTypeDef,
-    SourceOutputTypeDef,
-    UserDataOutputTypeDef,
+    SourceTypeDef,
+    UserDataTypeDef,
     GetConnectorsRequestGetConnectorsPaginateTypeDef,
     GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
     GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
     ListAppsRequestListAppsPaginateTypeDef,
     GetServersRequestGetServersPaginateTypeDef,
     GetServersRequestRequestTypeDef,
     VmServerTypeDef,
     NotifyAppValidationOutputRequestRequestTypeDef,
     ReplicationRunTypeDef,
-    SourceTypeDef,
-    UserDataTypeDef,
-    VmServerOutputTypeDef,
     ListAppsResponseTypeDef,
     AppValidationOutputTypeDef,
-    SSMValidationParametersOutputTypeDef,
-    UserDataValidationParametersOutputTypeDef,
-    ServerTypeDef,
     SSMValidationParametersTypeDef,
     UserDataValidationParametersTypeDef,
+    ServerTypeDef,
     ReplicationJobTypeDef,
-    ServerOutputTypeDef,
-    AppValidationConfigurationOutputTypeDef,
+    AppValidationConfigurationTypeDef,
+    GetServersResponseTypeDef,
+    ServerGroupOutputTypeDef,
     ServerGroupTypeDef,
     ServerLaunchConfigurationTypeDef,
+    ServerReplicationConfigurationOutputTypeDef,
     ServerReplicationConfigurationTypeDef,
-    AppValidationConfigurationTypeDef,
     ServerValidationConfigurationTypeDef,
+    ServerValidationOutputTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
-    GetServersResponseTypeDef,
-    ServerGroupOutputTypeDef,
-    ServerLaunchConfigurationOutputTypeDef,
-    ServerReplicationConfigurationOutputTypeDef,
-    ServerValidationConfigurationOutputTypeDef,
-    ServerValidationOutputTypeDef,
-    CreateAppRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
-    ServerGroupLaunchConfigurationTypeDef,
-    ServerGroupReplicationConfigurationTypeDef,
-    ServerGroupValidationConfigurationTypeDef,
     CreateAppResponseTypeDef,
     GetAppResponseTypeDef,
     UpdateAppResponseTypeDef,
+    CreateAppRequestRequestTypeDef,
+    UpdateAppRequestRequestTypeDef,
     ServerGroupLaunchConfigurationOutputTypeDef,
+    ServerGroupLaunchConfigurationTypeDef,
     ServerGroupReplicationConfigurationOutputTypeDef,
+    ServerGroupReplicationConfigurationTypeDef,
     ServerGroupValidationConfigurationOutputTypeDef,
+    ServerGroupValidationConfigurationTypeDef,
     ValidationOutputTypeDef,
-    PutAppLaunchConfigurationRequestRequestTypeDef,
-    PutAppReplicationConfigurationRequestRequestTypeDef,
-    PutAppValidationConfigurationRequestRequestTypeDef,
     GetAppLaunchConfigurationResponseTypeDef,
+    PutAppLaunchConfigurationRequestRequestTypeDef,
     GetAppReplicationConfigurationResponseTypeDef,
+    PutAppReplicationConfigurationRequestRequestTypeDef,
     GetAppValidationConfigurationResponseTypeDef,
+    PutAppValidationConfigurationRequestRequestTypeDef,
     GetAppValidationOutputResponseTypeDef,
 )
 
 
 def get_structure() -> LaunchDetailsTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sms-1.28.12/mypy_boto3_sms/__init__.py` & `mypy-boto3-sms-1.28.15/mypy_boto3_sms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.12/mypy_boto3_sms/__init__.pyi` & `mypy-boto3-sms-1.28.15/mypy_boto3_sms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.12/mypy_boto3_sms/__main__.py` & `mypy-boto3-sms-1.28.15/mypy_boto3_sms/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SMS 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.SMS 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS\nOther"
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

### Comparing `mypy-boto3-sms-1.28.12/mypy_boto3_sms/client.py` & `mypy-boto3-sms-1.28.15/mypy_boto3_sms/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.12/mypy_boto3_sms/client.pyi` & `mypy-boto3-sms-1.28.15/mypy_boto3_sms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.12/mypy_boto3_sms/literals.py` & `mypy-boto3-sms-1.28.15/mypy_boto3_sms/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -491,29 +491,8 @@
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "get_connectors", "get_replication_jobs", "get_replication_runs", "get_servers", "list_apps"
 ]
-RegionName = Literal[
-    "af-south-1",
-    "ap-east-1",
-    "ap-northeast-1",
-    "ap-northeast-2",
-    "ap-south-1",
-    "ap-southeast-1",
-    "ap-southeast-2",
-    "ca-central-1",
-    "eu-central-1",
-    "eu-north-1",
-    "eu-south-1",
-    "eu-west-1",
-    "eu-west-2",
-    "eu-west-3",
-    "me-south-1",
-    "sa-east-1",
-    "us-east-1",
-    "us-east-2",
-    "us-west-1",
-    "us-west-2",
-]
+RegionName = Literal["us-west-2"]
```

### Comparing `mypy-boto3-sms-1.28.12/mypy_boto3_sms/literals.pyi` & `mypy-boto3-sms-1.28.15/mypy_boto3_sms/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -489,29 +489,8 @@
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "get_connectors", "get_replication_jobs", "get_replication_runs", "get_servers", "list_apps"
 ]
-RegionName = Literal[
-    "af-south-1",
-    "ap-east-1",
-    "ap-northeast-1",
-    "ap-northeast-2",
-    "ap-south-1",
-    "ap-southeast-1",
-    "ap-southeast-2",
-    "ca-central-1",
-    "eu-central-1",
-    "eu-north-1",
-    "eu-south-1",
-    "eu-west-1",
-    "eu-west-2",
-    "eu-west-3",
-    "me-south-1",
-    "sa-east-1",
-    "us-east-1",
-    "us-east-2",
-    "us-west-1",
-    "us-west-2",
-]
+RegionName = Literal["us-west-2"]
```

### Comparing `mypy-boto3-sms-1.28.12/mypy_boto3_sms/paginator.py` & `mypy-boto3-sms-1.28.15/mypy_boto3_sms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.12/mypy_boto3_sms/paginator.pyi` & `mypy-boto3-sms-1.28.15/mypy_boto3_sms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.12/mypy_boto3_sms/type_defs.py` & `mypy-boto3-sms-1.28.15/mypy_boto3_sms/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,24 +45,23 @@
 
 
 __all__ = (
     "LaunchDetailsTypeDef",
     "ConnectorTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
-    "TagOutputTypeDef",
     "CreateReplicationJobRequestRequestTypeDef",
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     "DeleteAppReplicationConfigurationRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppValidationConfigurationRequestRequestTypeDef",
     "DeleteReplicationJobRequestRequestTypeDef",
     "DisassociateConnectorRequestRequestTypeDef",
     "GenerateChangeSetRequestRequestTypeDef",
-    "S3LocationOutputTypeDef",
+    "S3LocationTypeDef",
     "GenerateTemplateRequestRequestTypeDef",
     "GetAppLaunchConfigurationRequestRequestTypeDef",
     "GetAppReplicationConfigurationRequestRequestTypeDef",
     "GetAppRequestRequestTypeDef",
     "GetAppValidationConfigurationRequestRequestTypeDef",
     "GetAppValidationOutputRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -71,86 +70,75 @@
     "GetReplicationRunsRequestRequestTypeDef",
     "VmServerAddressTypeDef",
     "ImportAppCatalogRequestRequestTypeDef",
     "LaunchAppRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "NotificationContextTypeDef",
     "ReplicationRunStageDetailsTypeDef",
-    "S3LocationTypeDef",
     "ServerReplicationParametersOutputTypeDef",
     "ServerReplicationParametersTypeDef",
     "StartAppReplicationRequestRequestTypeDef",
     "StartOnDemandAppReplicationRequestRequestTypeDef",
     "StartOnDemandReplicationRunRequestRequestTypeDef",
     "StopAppReplicationRequestRequestTypeDef",
     "TerminateAppRequestRequestTypeDef",
     "UpdateReplicationJobRequestRequestTypeDef",
-    "VmServerAddressOutputTypeDef",
     "AppSummaryTypeDef",
     "CreateReplicationJobResponseTypeDef",
     "GetConnectorsResponseTypeDef",
     "StartOnDemandReplicationRunResponseTypeDef",
     "GenerateChangeSetResponseTypeDef",
     "GenerateTemplateResponseTypeDef",
     "SSMOutputTypeDef",
-    "SourceOutputTypeDef",
-    "UserDataOutputTypeDef",
+    "SourceTypeDef",
+    "UserDataTypeDef",
     "GetConnectorsRequestGetConnectorsPaginateTypeDef",
     "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
     "GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
     "ListAppsRequestListAppsPaginateTypeDef",
     "GetServersRequestGetServersPaginateTypeDef",
     "GetServersRequestRequestTypeDef",
     "VmServerTypeDef",
     "NotifyAppValidationOutputRequestRequestTypeDef",
     "ReplicationRunTypeDef",
-    "SourceTypeDef",
-    "UserDataTypeDef",
-    "VmServerOutputTypeDef",
     "ListAppsResponseTypeDef",
     "AppValidationOutputTypeDef",
-    "SSMValidationParametersOutputTypeDef",
-    "UserDataValidationParametersOutputTypeDef",
-    "ServerTypeDef",
     "SSMValidationParametersTypeDef",
     "UserDataValidationParametersTypeDef",
+    "ServerTypeDef",
     "ReplicationJobTypeDef",
-    "ServerOutputTypeDef",
-    "AppValidationConfigurationOutputTypeDef",
+    "AppValidationConfigurationTypeDef",
+    "GetServersResponseTypeDef",
+    "ServerGroupOutputTypeDef",
     "ServerGroupTypeDef",
     "ServerLaunchConfigurationTypeDef",
+    "ServerReplicationConfigurationOutputTypeDef",
     "ServerReplicationConfigurationTypeDef",
-    "AppValidationConfigurationTypeDef",
     "ServerValidationConfigurationTypeDef",
+    "ServerValidationOutputTypeDef",
     "GetReplicationJobsResponseTypeDef",
     "GetReplicationRunsResponseTypeDef",
-    "GetServersResponseTypeDef",
-    "ServerGroupOutputTypeDef",
-    "ServerLaunchConfigurationOutputTypeDef",
-    "ServerReplicationConfigurationOutputTypeDef",
-    "ServerValidationConfigurationOutputTypeDef",
-    "ServerValidationOutputTypeDef",
-    "CreateAppRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
-    "ServerGroupLaunchConfigurationTypeDef",
-    "ServerGroupReplicationConfigurationTypeDef",
-    "ServerGroupValidationConfigurationTypeDef",
     "CreateAppResponseTypeDef",
     "GetAppResponseTypeDef",
     "UpdateAppResponseTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "ServerGroupLaunchConfigurationOutputTypeDef",
+    "ServerGroupLaunchConfigurationTypeDef",
     "ServerGroupReplicationConfigurationOutputTypeDef",
+    "ServerGroupReplicationConfigurationTypeDef",
     "ServerGroupValidationConfigurationOutputTypeDef",
+    "ServerGroupValidationConfigurationTypeDef",
     "ValidationOutputTypeDef",
-    "PutAppLaunchConfigurationRequestRequestTypeDef",
-    "PutAppReplicationConfigurationRequestRequestTypeDef",
-    "PutAppValidationConfigurationRequestRequestTypeDef",
     "GetAppLaunchConfigurationResponseTypeDef",
+    "PutAppLaunchConfigurationRequestRequestTypeDef",
     "GetAppReplicationConfigurationResponseTypeDef",
+    "PutAppReplicationConfigurationRequestRequestTypeDef",
     "GetAppValidationConfigurationResponseTypeDef",
+    "PutAppValidationConfigurationRequestRequestTypeDef",
     "GetAppValidationOutputResponseTypeDef",
 )
 
 LaunchDetailsTypeDef = TypedDict(
     "LaunchDetailsTypeDef",
     {
         "latestLaunchTime": datetime,
@@ -193,23 +181,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-    total=False,
-)
-
 _RequiredCreateReplicationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationJobRequestRequestTypeDef",
     {
         "serverId": str,
         "seedReplicationTime": Union[datetime, str],
     },
 )
@@ -288,16 +267,16 @@
     {
         "appId": str,
         "changesetFormat": OutputFormatType,
     },
     total=False,
 )
 
-S3LocationOutputTypeDef = TypedDict(
-    "S3LocationOutputTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
     },
     total=False,
 )
 
@@ -450,23 +429,14 @@
     {
         "stage": str,
         "stageProgress": str,
     },
     total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
-    {
-        "bucket": str,
-        "key": str,
-    },
-    total=False,
-)
-
 ServerReplicationParametersOutputTypeDef = TypedDict(
     "ServerReplicationParametersOutputTypeDef",
     {
         "seedTime": datetime,
         "frequency": int,
         "runOnce": bool,
         "licenseType": LicenseTypeType,
@@ -584,23 +554,14 @@
 class UpdateReplicationJobRequestRequestTypeDef(
     _RequiredUpdateReplicationJobRequestRequestTypeDef,
     _OptionalUpdateReplicationJobRequestRequestTypeDef,
 ):
     pass
 
 
-VmServerAddressOutputTypeDef = TypedDict(
-    "VmServerAddressOutputTypeDef",
-    {
-        "vmManagerId": str,
-        "vmId": str,
-    },
-    total=False,
-)
-
 AppSummaryTypeDef = TypedDict(
     "AppSummaryTypeDef",
     {
         "appId": str,
         "importedAppId": str,
         "name": str,
         "description": str,
@@ -647,47 +608,47 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GenerateChangeSetResponseTypeDef = TypedDict(
     "GenerateChangeSetResponseTypeDef",
     {
-        "s3Location": S3LocationOutputTypeDef,
+        "s3Location": S3LocationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GenerateTemplateResponseTypeDef = TypedDict(
     "GenerateTemplateResponseTypeDef",
     {
-        "s3Location": S3LocationOutputTypeDef,
+        "s3Location": S3LocationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SSMOutputTypeDef = TypedDict(
     "SSMOutputTypeDef",
     {
-        "s3Location": S3LocationOutputTypeDef,
+        "s3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
-SourceOutputTypeDef = TypedDict(
-    "SourceOutputTypeDef",
+SourceTypeDef = TypedDict(
+    "SourceTypeDef",
     {
-        "s3Location": S3LocationOutputTypeDef,
+        "s3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
-UserDataOutputTypeDef = TypedDict(
-    "UserDataOutputTypeDef",
+UserDataTypeDef = TypedDict(
+    "UserDataTypeDef",
     {
-        "s3Location": S3LocationOutputTypeDef,
+        "s3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
 GetConnectorsRequestGetConnectorsPaginateTypeDef = TypedDict(
     "GetConnectorsRequestGetConnectorsPaginateTypeDef",
     {
@@ -803,42 +764,14 @@
         "description": str,
         "encrypted": bool,
         "kmsKeyId": str,
     },
     total=False,
 )
 
-SourceTypeDef = TypedDict(
-    "SourceTypeDef",
-    {
-        "s3Location": S3LocationTypeDef,
-    },
-    total=False,
-)
-
-UserDataTypeDef = TypedDict(
-    "UserDataTypeDef",
-    {
-        "s3Location": S3LocationTypeDef,
-    },
-    total=False,
-)
-
-VmServerOutputTypeDef = TypedDict(
-    "VmServerOutputTypeDef",
-    {
-        "vmServerAddress": VmServerAddressOutputTypeDef,
-        "vmName": str,
-        "vmManagerName": str,
-        "vmManagerType": VmManagerTypeType,
-        "vmPath": str,
-    },
-    total=False,
-)
-
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "apps": List[AppSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -848,31 +781,31 @@
     "AppValidationOutputTypeDef",
     {
         "ssmOutput": SSMOutputTypeDef,
     },
     total=False,
 )
 
-SSMValidationParametersOutputTypeDef = TypedDict(
-    "SSMValidationParametersOutputTypeDef",
+SSMValidationParametersTypeDef = TypedDict(
+    "SSMValidationParametersTypeDef",
     {
-        "source": SourceOutputTypeDef,
+        "source": SourceTypeDef,
         "instanceId": str,
         "scriptType": ScriptTypeType,
         "command": str,
         "executionTimeoutSeconds": int,
         "outputS3BucketName": str,
     },
     total=False,
 )
 
-UserDataValidationParametersOutputTypeDef = TypedDict(
-    "UserDataValidationParametersOutputTypeDef",
+UserDataValidationParametersTypeDef = TypedDict(
+    "UserDataValidationParametersTypeDef",
     {
-        "source": SourceOutputTypeDef,
+        "source": SourceTypeDef,
         "scriptType": ScriptTypeType,
     },
     total=False,
 )
 
 ServerTypeDef = TypedDict(
     "ServerTypeDef",
@@ -882,43 +815,21 @@
         "vmServer": VmServerTypeDef,
         "replicationJobId": str,
         "replicationJobTerminated": bool,
     },
     total=False,
 )
 
-SSMValidationParametersTypeDef = TypedDict(
-    "SSMValidationParametersTypeDef",
-    {
-        "source": SourceTypeDef,
-        "instanceId": str,
-        "scriptType": ScriptTypeType,
-        "command": str,
-        "executionTimeoutSeconds": int,
-        "outputS3BucketName": str,
-    },
-    total=False,
-)
-
-UserDataValidationParametersTypeDef = TypedDict(
-    "UserDataValidationParametersTypeDef",
-    {
-        "source": SourceTypeDef,
-        "scriptType": ScriptTypeType,
-    },
-    total=False,
-)
-
 ReplicationJobTypeDef = TypedDict(
     "ReplicationJobTypeDef",
     {
         "replicationJobId": str,
         "serverId": str,
         "serverType": Literal["VIRTUAL_MACHINE"],
-        "vmServer": VmServerOutputTypeDef,
+        "vmServer": VmServerTypeDef,
         "seedReplicationTime": datetime,
         "frequency": int,
         "runOnce": bool,
         "nextReplicationRunStartTime": datetime,
         "licenseType": LicenseTypeType,
         "roleName": str,
         "latestAmiId": str,
@@ -929,33 +840,42 @@
         "encrypted": bool,
         "kmsKeyId": str,
         "replicationRunList": List[ReplicationRunTypeDef],
     },
     total=False,
 )
 
-ServerOutputTypeDef = TypedDict(
-    "ServerOutputTypeDef",
+AppValidationConfigurationTypeDef = TypedDict(
+    "AppValidationConfigurationTypeDef",
     {
-        "serverId": str,
-        "serverType": Literal["VIRTUAL_MACHINE"],
-        "vmServer": VmServerOutputTypeDef,
-        "replicationJobId": str,
-        "replicationJobTerminated": bool,
+        "validationId": str,
+        "name": str,
+        "appValidationStrategy": Literal["SSM"],
+        "ssmValidationParameters": SSMValidationParametersTypeDef,
     },
     total=False,
 )
 
-AppValidationConfigurationOutputTypeDef = TypedDict(
-    "AppValidationConfigurationOutputTypeDef",
+GetServersResponseTypeDef = TypedDict(
+    "GetServersResponseTypeDef",
     {
-        "validationId": str,
+        "lastModifiedOn": datetime,
+        "serverCatalogStatus": ServerCatalogStatusType,
+        "serverList": List[ServerTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ServerGroupOutputTypeDef = TypedDict(
+    "ServerGroupOutputTypeDef",
+    {
+        "serverGroupId": str,
         "name": str,
-        "appValidationStrategy": Literal["SSM"],
-        "ssmValidationParameters": SSMValidationParametersOutputTypeDef,
+        "serverList": List[ServerTypeDef],
     },
     total=False,
 )
 
 ServerGroupTypeDef = TypedDict(
     "ServerGroupTypeDef",
     {
@@ -981,30 +901,28 @@
         "iamInstanceProfileName": str,
         "configureScript": S3LocationTypeDef,
         "configureScriptType": ScriptTypeType,
     },
     total=False,
 )
 
-ServerReplicationConfigurationTypeDef = TypedDict(
-    "ServerReplicationConfigurationTypeDef",
+ServerReplicationConfigurationOutputTypeDef = TypedDict(
+    "ServerReplicationConfigurationOutputTypeDef",
     {
         "server": ServerTypeDef,
-        "serverReplicationParameters": ServerReplicationParametersTypeDef,
+        "serverReplicationParameters": ServerReplicationParametersOutputTypeDef,
     },
     total=False,
 )
 
-AppValidationConfigurationTypeDef = TypedDict(
-    "AppValidationConfigurationTypeDef",
+ServerReplicationConfigurationTypeDef = TypedDict(
+    "ServerReplicationConfigurationTypeDef",
     {
-        "validationId": str,
-        "name": str,
-        "appValidationStrategy": Literal["SSM"],
-        "ssmValidationParameters": SSMValidationParametersTypeDef,
+        "server": ServerTypeDef,
+        "serverReplicationParameters": ServerReplicationParametersTypeDef,
     },
     total=False,
 )
 
 ServerValidationConfigurationTypeDef = TypedDict(
     "ServerValidationConfigurationTypeDef",
     {
@@ -1013,14 +931,22 @@
         "name": str,
         "serverValidationStrategy": Literal["USERDATA"],
         "userDataValidationParameters": UserDataValidationParametersTypeDef,
     },
     total=False,
 )
 
+ServerValidationOutputTypeDef = TypedDict(
+    "ServerValidationOutputTypeDef",
+    {
+        "server": ServerTypeDef,
+    },
+    total=False,
+)
+
 GetReplicationJobsResponseTypeDef = TypedDict(
     "GetReplicationJobsResponseTypeDef",
     {
         "replicationJobList": List[ReplicationJobTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1032,81 +958,42 @@
         "replicationJob": ReplicationJobTypeDef,
         "replicationRunList": List[ReplicationRunTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetServersResponseTypeDef = TypedDict(
-    "GetServersResponseTypeDef",
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
     {
-        "lastModifiedOn": datetime,
-        "serverCatalogStatus": ServerCatalogStatusType,
-        "serverList": List[ServerOutputTypeDef],
-        "nextToken": str,
+        "appSummary": AppSummaryTypeDef,
+        "serverGroups": List[ServerGroupOutputTypeDef],
+        "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ServerGroupOutputTypeDef = TypedDict(
-    "ServerGroupOutputTypeDef",
-    {
-        "serverGroupId": str,
-        "name": str,
-        "serverList": List[ServerOutputTypeDef],
-    },
-    total=False,
-)
-
-ServerLaunchConfigurationOutputTypeDef = TypedDict(
-    "ServerLaunchConfigurationOutputTypeDef",
-    {
-        "server": ServerOutputTypeDef,
-        "logicalId": str,
-        "vpc": str,
-        "subnet": str,
-        "securityGroup": str,
-        "ec2KeyName": str,
-        "userData": UserDataOutputTypeDef,
-        "instanceType": str,
-        "associatePublicIpAddress": bool,
-        "iamInstanceProfileName": str,
-        "configureScript": S3LocationOutputTypeDef,
-        "configureScriptType": ScriptTypeType,
-    },
-    total=False,
-)
-
-ServerReplicationConfigurationOutputTypeDef = TypedDict(
-    "ServerReplicationConfigurationOutputTypeDef",
-    {
-        "server": ServerOutputTypeDef,
-        "serverReplicationParameters": ServerReplicationParametersOutputTypeDef,
-    },
-    total=False,
-)
-
-ServerValidationConfigurationOutputTypeDef = TypedDict(
-    "ServerValidationConfigurationOutputTypeDef",
+GetAppResponseTypeDef = TypedDict(
+    "GetAppResponseTypeDef",
     {
-        "server": ServerOutputTypeDef,
-        "validationId": str,
-        "name": str,
-        "serverValidationStrategy": Literal["USERDATA"],
-        "userDataValidationParameters": UserDataValidationParametersOutputTypeDef,
+        "appSummary": AppSummaryTypeDef,
+        "serverGroups": List[ServerGroupOutputTypeDef],
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ServerValidationOutputTypeDef = TypedDict(
-    "ServerValidationOutputTypeDef",
+UpdateAppResponseTypeDef = TypedDict(
+    "UpdateAppResponseTypeDef",
     {
-        "server": ServerOutputTypeDef,
+        "appSummary": AppSummaryTypeDef,
+        "serverGroups": List[ServerGroupOutputTypeDef],
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 CreateAppRequestRequestTypeDef = TypedDict(
     "CreateAppRequestRequestTypeDef",
     {
         "name": str,
         "description": str,
@@ -1127,96 +1014,66 @@
         "roleName": str,
         "serverGroups": Sequence[ServerGroupTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-ServerGroupLaunchConfigurationTypeDef = TypedDict(
-    "ServerGroupLaunchConfigurationTypeDef",
+ServerGroupLaunchConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupLaunchConfigurationOutputTypeDef",
     {
         "serverGroupId": str,
         "launchOrder": int,
-        "serverLaunchConfigurations": Sequence[ServerLaunchConfigurationTypeDef],
+        "serverLaunchConfigurations": List[ServerLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
-ServerGroupReplicationConfigurationTypeDef = TypedDict(
-    "ServerGroupReplicationConfigurationTypeDef",
+ServerGroupLaunchConfigurationTypeDef = TypedDict(
+    "ServerGroupLaunchConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverReplicationConfigurations": Sequence[ServerReplicationConfigurationTypeDef],
+        "launchOrder": int,
+        "serverLaunchConfigurations": Sequence[ServerLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
-ServerGroupValidationConfigurationTypeDef = TypedDict(
-    "ServerGroupValidationConfigurationTypeDef",
+ServerGroupReplicationConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupReplicationConfigurationOutputTypeDef",
     {
         "serverGroupId": str,
-        "serverValidationConfigurations": Sequence[ServerValidationConfigurationTypeDef],
+        "serverReplicationConfigurations": List[ServerReplicationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
-    {
-        "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupOutputTypeDef],
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAppResponseTypeDef = TypedDict(
-    "GetAppResponseTypeDef",
-    {
-        "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupOutputTypeDef],
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAppResponseTypeDef = TypedDict(
-    "UpdateAppResponseTypeDef",
-    {
-        "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupOutputTypeDef],
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ServerGroupLaunchConfigurationOutputTypeDef = TypedDict(
-    "ServerGroupLaunchConfigurationOutputTypeDef",
+ServerGroupReplicationConfigurationTypeDef = TypedDict(
+    "ServerGroupReplicationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "launchOrder": int,
-        "serverLaunchConfigurations": List[ServerLaunchConfigurationOutputTypeDef],
+        "serverReplicationConfigurations": Sequence[ServerReplicationConfigurationTypeDef],
     },
     total=False,
 )
 
-ServerGroupReplicationConfigurationOutputTypeDef = TypedDict(
-    "ServerGroupReplicationConfigurationOutputTypeDef",
+ServerGroupValidationConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupValidationConfigurationOutputTypeDef",
     {
         "serverGroupId": str,
-        "serverReplicationConfigurations": List[ServerReplicationConfigurationOutputTypeDef],
+        "serverValidationConfigurations": List[ServerValidationConfigurationTypeDef],
     },
     total=False,
 )
 
-ServerGroupValidationConfigurationOutputTypeDef = TypedDict(
-    "ServerGroupValidationConfigurationOutputTypeDef",
+ServerGroupValidationConfigurationTypeDef = TypedDict(
+    "ServerGroupValidationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverValidationConfigurations": List[ServerValidationConfigurationOutputTypeDef],
+        "serverValidationConfigurations": Sequence[ServerValidationConfigurationTypeDef],
     },
     total=False,
 )
 
 ValidationOutputTypeDef = TypedDict(
     "ValidationOutputTypeDef",
     {
@@ -1227,36 +1084,68 @@
         "latestValidationTime": datetime,
         "appValidationOutput": AppValidationOutputTypeDef,
         "serverValidationOutput": ServerValidationOutputTypeDef,
     },
     total=False,
 )
 
+GetAppLaunchConfigurationResponseTypeDef = TypedDict(
+    "GetAppLaunchConfigurationResponseTypeDef",
+    {
+        "appId": str,
+        "roleName": str,
+        "autoLaunch": bool,
+        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
         "roleName": str,
         "autoLaunch": bool,
         "serverGroupLaunchConfigurations": Sequence[ServerGroupLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
+GetAppReplicationConfigurationResponseTypeDef = TypedDict(
+    "GetAppReplicationConfigurationResponseTypeDef",
+    {
+        "serverGroupReplicationConfigurations": List[
+            ServerGroupReplicationConfigurationOutputTypeDef
+        ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppReplicationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
         "serverGroupReplicationConfigurations": Sequence[
             ServerGroupReplicationConfigurationTypeDef
         ],
     },
     total=False,
 )
 
+GetAppValidationConfigurationResponseTypeDef = TypedDict(
+    "GetAppValidationConfigurationResponseTypeDef",
+    {
+        "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
+        "serverGroupValidationConfigurations": List[
+            ServerGroupValidationConfigurationOutputTypeDef
+        ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 _OptionalPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
@@ -1272,46 +1161,14 @@
 class PutAppValidationConfigurationRequestRequestTypeDef(
     _RequiredPutAppValidationConfigurationRequestRequestTypeDef,
     _OptionalPutAppValidationConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-GetAppLaunchConfigurationResponseTypeDef = TypedDict(
-    "GetAppLaunchConfigurationResponseTypeDef",
-    {
-        "appId": str,
-        "roleName": str,
-        "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAppReplicationConfigurationResponseTypeDef = TypedDict(
-    "GetAppReplicationConfigurationResponseTypeDef",
-    {
-        "serverGroupReplicationConfigurations": List[
-            ServerGroupReplicationConfigurationOutputTypeDef
-        ],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAppValidationConfigurationResponseTypeDef = TypedDict(
-    "GetAppValidationConfigurationResponseTypeDef",
-    {
-        "appValidationConfigurations": List[AppValidationConfigurationOutputTypeDef],
-        "serverGroupValidationConfigurations": List[
-            ServerGroupValidationConfigurationOutputTypeDef
-        ],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetAppValidationOutputResponseTypeDef = TypedDict(
     "GetAppValidationOutputResponseTypeDef",
     {
         "validationOutputList": List[ValidationOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-sms-1.28.12/mypy_boto3_sms/type_defs.pyi` & `mypy-boto3-sms-1.28.15/mypy_boto3_sms/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -44,24 +44,23 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "LaunchDetailsTypeDef",
     "ConnectorTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
-    "TagOutputTypeDef",
     "CreateReplicationJobRequestRequestTypeDef",
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     "DeleteAppReplicationConfigurationRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppValidationConfigurationRequestRequestTypeDef",
     "DeleteReplicationJobRequestRequestTypeDef",
     "DisassociateConnectorRequestRequestTypeDef",
     "GenerateChangeSetRequestRequestTypeDef",
-    "S3LocationOutputTypeDef",
+    "S3LocationTypeDef",
     "GenerateTemplateRequestRequestTypeDef",
     "GetAppLaunchConfigurationRequestRequestTypeDef",
     "GetAppReplicationConfigurationRequestRequestTypeDef",
     "GetAppRequestRequestTypeDef",
     "GetAppValidationConfigurationRequestRequestTypeDef",
     "GetAppValidationOutputRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -70,86 +69,75 @@
     "GetReplicationRunsRequestRequestTypeDef",
     "VmServerAddressTypeDef",
     "ImportAppCatalogRequestRequestTypeDef",
     "LaunchAppRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "NotificationContextTypeDef",
     "ReplicationRunStageDetailsTypeDef",
-    "S3LocationTypeDef",
     "ServerReplicationParametersOutputTypeDef",
     "ServerReplicationParametersTypeDef",
     "StartAppReplicationRequestRequestTypeDef",
     "StartOnDemandAppReplicationRequestRequestTypeDef",
     "StartOnDemandReplicationRunRequestRequestTypeDef",
     "StopAppReplicationRequestRequestTypeDef",
     "TerminateAppRequestRequestTypeDef",
     "UpdateReplicationJobRequestRequestTypeDef",
-    "VmServerAddressOutputTypeDef",
     "AppSummaryTypeDef",
     "CreateReplicationJobResponseTypeDef",
     "GetConnectorsResponseTypeDef",
     "StartOnDemandReplicationRunResponseTypeDef",
     "GenerateChangeSetResponseTypeDef",
     "GenerateTemplateResponseTypeDef",
     "SSMOutputTypeDef",
-    "SourceOutputTypeDef",
-    "UserDataOutputTypeDef",
+    "SourceTypeDef",
+    "UserDataTypeDef",
     "GetConnectorsRequestGetConnectorsPaginateTypeDef",
     "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
     "GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
     "ListAppsRequestListAppsPaginateTypeDef",
     "GetServersRequestGetServersPaginateTypeDef",
     "GetServersRequestRequestTypeDef",
     "VmServerTypeDef",
     "NotifyAppValidationOutputRequestRequestTypeDef",
     "ReplicationRunTypeDef",
-    "SourceTypeDef",
-    "UserDataTypeDef",
-    "VmServerOutputTypeDef",
     "ListAppsResponseTypeDef",
     "AppValidationOutputTypeDef",
-    "SSMValidationParametersOutputTypeDef",
-    "UserDataValidationParametersOutputTypeDef",
-    "ServerTypeDef",
     "SSMValidationParametersTypeDef",
     "UserDataValidationParametersTypeDef",
+    "ServerTypeDef",
     "ReplicationJobTypeDef",
-    "ServerOutputTypeDef",
-    "AppValidationConfigurationOutputTypeDef",
+    "AppValidationConfigurationTypeDef",
+    "GetServersResponseTypeDef",
+    "ServerGroupOutputTypeDef",
     "ServerGroupTypeDef",
     "ServerLaunchConfigurationTypeDef",
+    "ServerReplicationConfigurationOutputTypeDef",
     "ServerReplicationConfigurationTypeDef",
-    "AppValidationConfigurationTypeDef",
     "ServerValidationConfigurationTypeDef",
+    "ServerValidationOutputTypeDef",
     "GetReplicationJobsResponseTypeDef",
     "GetReplicationRunsResponseTypeDef",
-    "GetServersResponseTypeDef",
-    "ServerGroupOutputTypeDef",
-    "ServerLaunchConfigurationOutputTypeDef",
-    "ServerReplicationConfigurationOutputTypeDef",
-    "ServerValidationConfigurationOutputTypeDef",
-    "ServerValidationOutputTypeDef",
-    "CreateAppRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
-    "ServerGroupLaunchConfigurationTypeDef",
-    "ServerGroupReplicationConfigurationTypeDef",
-    "ServerGroupValidationConfigurationTypeDef",
     "CreateAppResponseTypeDef",
     "GetAppResponseTypeDef",
     "UpdateAppResponseTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "ServerGroupLaunchConfigurationOutputTypeDef",
+    "ServerGroupLaunchConfigurationTypeDef",
     "ServerGroupReplicationConfigurationOutputTypeDef",
+    "ServerGroupReplicationConfigurationTypeDef",
     "ServerGroupValidationConfigurationOutputTypeDef",
+    "ServerGroupValidationConfigurationTypeDef",
     "ValidationOutputTypeDef",
-    "PutAppLaunchConfigurationRequestRequestTypeDef",
-    "PutAppReplicationConfigurationRequestRequestTypeDef",
-    "PutAppValidationConfigurationRequestRequestTypeDef",
     "GetAppLaunchConfigurationResponseTypeDef",
+    "PutAppLaunchConfigurationRequestRequestTypeDef",
     "GetAppReplicationConfigurationResponseTypeDef",
+    "PutAppReplicationConfigurationRequestRequestTypeDef",
     "GetAppValidationConfigurationResponseTypeDef",
+    "PutAppValidationConfigurationRequestRequestTypeDef",
     "GetAppValidationOutputResponseTypeDef",
 )
 
 LaunchDetailsTypeDef = TypedDict(
     "LaunchDetailsTypeDef",
     {
         "latestLaunchTime": datetime,
@@ -192,23 +180,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-    total=False,
-)
-
 _RequiredCreateReplicationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationJobRequestRequestTypeDef",
     {
         "serverId": str,
         "seedReplicationTime": Union[datetime, str],
     },
 )
@@ -285,16 +264,16 @@
     {
         "appId": str,
         "changesetFormat": OutputFormatType,
     },
     total=False,
 )
 
-S3LocationOutputTypeDef = TypedDict(
-    "S3LocationOutputTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
     },
     total=False,
 )
 
@@ -445,23 +424,14 @@
     {
         "stage": str,
         "stageProgress": str,
     },
     total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
-    {
-        "bucket": str,
-        "key": str,
-    },
-    total=False,
-)
-
 ServerReplicationParametersOutputTypeDef = TypedDict(
     "ServerReplicationParametersOutputTypeDef",
     {
         "seedTime": datetime,
         "frequency": int,
         "runOnce": bool,
         "licenseType": LicenseTypeType,
@@ -573,23 +543,14 @@
 
 class UpdateReplicationJobRequestRequestTypeDef(
     _RequiredUpdateReplicationJobRequestRequestTypeDef,
     _OptionalUpdateReplicationJobRequestRequestTypeDef,
 ):
     pass
 
-VmServerAddressOutputTypeDef = TypedDict(
-    "VmServerAddressOutputTypeDef",
-    {
-        "vmManagerId": str,
-        "vmId": str,
-    },
-    total=False,
-)
-
 AppSummaryTypeDef = TypedDict(
     "AppSummaryTypeDef",
     {
         "appId": str,
         "importedAppId": str,
         "name": str,
         "description": str,
@@ -636,47 +597,47 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GenerateChangeSetResponseTypeDef = TypedDict(
     "GenerateChangeSetResponseTypeDef",
     {
-        "s3Location": S3LocationOutputTypeDef,
+        "s3Location": S3LocationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GenerateTemplateResponseTypeDef = TypedDict(
     "GenerateTemplateResponseTypeDef",
     {
-        "s3Location": S3LocationOutputTypeDef,
+        "s3Location": S3LocationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SSMOutputTypeDef = TypedDict(
     "SSMOutputTypeDef",
     {
-        "s3Location": S3LocationOutputTypeDef,
+        "s3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
-SourceOutputTypeDef = TypedDict(
-    "SourceOutputTypeDef",
+SourceTypeDef = TypedDict(
+    "SourceTypeDef",
     {
-        "s3Location": S3LocationOutputTypeDef,
+        "s3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
-UserDataOutputTypeDef = TypedDict(
-    "UserDataOutputTypeDef",
+UserDataTypeDef = TypedDict(
+    "UserDataTypeDef",
     {
-        "s3Location": S3LocationOutputTypeDef,
+        "s3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
 GetConnectorsRequestGetConnectorsPaginateTypeDef = TypedDict(
     "GetConnectorsRequestGetConnectorsPaginateTypeDef",
     {
@@ -788,42 +749,14 @@
         "description": str,
         "encrypted": bool,
         "kmsKeyId": str,
     },
     total=False,
 )
 
-SourceTypeDef = TypedDict(
-    "SourceTypeDef",
-    {
-        "s3Location": S3LocationTypeDef,
-    },
-    total=False,
-)
-
-UserDataTypeDef = TypedDict(
-    "UserDataTypeDef",
-    {
-        "s3Location": S3LocationTypeDef,
-    },
-    total=False,
-)
-
-VmServerOutputTypeDef = TypedDict(
-    "VmServerOutputTypeDef",
-    {
-        "vmServerAddress": VmServerAddressOutputTypeDef,
-        "vmName": str,
-        "vmManagerName": str,
-        "vmManagerType": VmManagerTypeType,
-        "vmPath": str,
-    },
-    total=False,
-)
-
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "apps": List[AppSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -833,31 +766,31 @@
     "AppValidationOutputTypeDef",
     {
         "ssmOutput": SSMOutputTypeDef,
     },
     total=False,
 )
 
-SSMValidationParametersOutputTypeDef = TypedDict(
-    "SSMValidationParametersOutputTypeDef",
+SSMValidationParametersTypeDef = TypedDict(
+    "SSMValidationParametersTypeDef",
     {
-        "source": SourceOutputTypeDef,
+        "source": SourceTypeDef,
         "instanceId": str,
         "scriptType": ScriptTypeType,
         "command": str,
         "executionTimeoutSeconds": int,
         "outputS3BucketName": str,
     },
     total=False,
 )
 
-UserDataValidationParametersOutputTypeDef = TypedDict(
-    "UserDataValidationParametersOutputTypeDef",
+UserDataValidationParametersTypeDef = TypedDict(
+    "UserDataValidationParametersTypeDef",
     {
-        "source": SourceOutputTypeDef,
+        "source": SourceTypeDef,
         "scriptType": ScriptTypeType,
     },
     total=False,
 )
 
 ServerTypeDef = TypedDict(
     "ServerTypeDef",
@@ -867,43 +800,21 @@
         "vmServer": VmServerTypeDef,
         "replicationJobId": str,
         "replicationJobTerminated": bool,
     },
     total=False,
 )
 
-SSMValidationParametersTypeDef = TypedDict(
-    "SSMValidationParametersTypeDef",
-    {
-        "source": SourceTypeDef,
-        "instanceId": str,
-        "scriptType": ScriptTypeType,
-        "command": str,
-        "executionTimeoutSeconds": int,
-        "outputS3BucketName": str,
-    },
-    total=False,
-)
-
-UserDataValidationParametersTypeDef = TypedDict(
-    "UserDataValidationParametersTypeDef",
-    {
-        "source": SourceTypeDef,
-        "scriptType": ScriptTypeType,
-    },
-    total=False,
-)
-
 ReplicationJobTypeDef = TypedDict(
     "ReplicationJobTypeDef",
     {
         "replicationJobId": str,
         "serverId": str,
         "serverType": Literal["VIRTUAL_MACHINE"],
-        "vmServer": VmServerOutputTypeDef,
+        "vmServer": VmServerTypeDef,
         "seedReplicationTime": datetime,
         "frequency": int,
         "runOnce": bool,
         "nextReplicationRunStartTime": datetime,
         "licenseType": LicenseTypeType,
         "roleName": str,
         "latestAmiId": str,
@@ -914,33 +825,42 @@
         "encrypted": bool,
         "kmsKeyId": str,
         "replicationRunList": List[ReplicationRunTypeDef],
     },
     total=False,
 )
 
-ServerOutputTypeDef = TypedDict(
-    "ServerOutputTypeDef",
+AppValidationConfigurationTypeDef = TypedDict(
+    "AppValidationConfigurationTypeDef",
     {
-        "serverId": str,
-        "serverType": Literal["VIRTUAL_MACHINE"],
-        "vmServer": VmServerOutputTypeDef,
-        "replicationJobId": str,
-        "replicationJobTerminated": bool,
+        "validationId": str,
+        "name": str,
+        "appValidationStrategy": Literal["SSM"],
+        "ssmValidationParameters": SSMValidationParametersTypeDef,
     },
     total=False,
 )
 
-AppValidationConfigurationOutputTypeDef = TypedDict(
-    "AppValidationConfigurationOutputTypeDef",
+GetServersResponseTypeDef = TypedDict(
+    "GetServersResponseTypeDef",
     {
-        "validationId": str,
+        "lastModifiedOn": datetime,
+        "serverCatalogStatus": ServerCatalogStatusType,
+        "serverList": List[ServerTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ServerGroupOutputTypeDef = TypedDict(
+    "ServerGroupOutputTypeDef",
+    {
+        "serverGroupId": str,
         "name": str,
-        "appValidationStrategy": Literal["SSM"],
-        "ssmValidationParameters": SSMValidationParametersOutputTypeDef,
+        "serverList": List[ServerTypeDef],
     },
     total=False,
 )
 
 ServerGroupTypeDef = TypedDict(
     "ServerGroupTypeDef",
     {
@@ -966,30 +886,28 @@
         "iamInstanceProfileName": str,
         "configureScript": S3LocationTypeDef,
         "configureScriptType": ScriptTypeType,
     },
     total=False,
 )
 
-ServerReplicationConfigurationTypeDef = TypedDict(
-    "ServerReplicationConfigurationTypeDef",
+ServerReplicationConfigurationOutputTypeDef = TypedDict(
+    "ServerReplicationConfigurationOutputTypeDef",
     {
         "server": ServerTypeDef,
-        "serverReplicationParameters": ServerReplicationParametersTypeDef,
+        "serverReplicationParameters": ServerReplicationParametersOutputTypeDef,
     },
     total=False,
 )
 
-AppValidationConfigurationTypeDef = TypedDict(
-    "AppValidationConfigurationTypeDef",
+ServerReplicationConfigurationTypeDef = TypedDict(
+    "ServerReplicationConfigurationTypeDef",
     {
-        "validationId": str,
-        "name": str,
-        "appValidationStrategy": Literal["SSM"],
-        "ssmValidationParameters": SSMValidationParametersTypeDef,
+        "server": ServerTypeDef,
+        "serverReplicationParameters": ServerReplicationParametersTypeDef,
     },
     total=False,
 )
 
 ServerValidationConfigurationTypeDef = TypedDict(
     "ServerValidationConfigurationTypeDef",
     {
@@ -998,14 +916,22 @@
         "name": str,
         "serverValidationStrategy": Literal["USERDATA"],
         "userDataValidationParameters": UserDataValidationParametersTypeDef,
     },
     total=False,
 )
 
+ServerValidationOutputTypeDef = TypedDict(
+    "ServerValidationOutputTypeDef",
+    {
+        "server": ServerTypeDef,
+    },
+    total=False,
+)
+
 GetReplicationJobsResponseTypeDef = TypedDict(
     "GetReplicationJobsResponseTypeDef",
     {
         "replicationJobList": List[ReplicationJobTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1017,81 +943,42 @@
         "replicationJob": ReplicationJobTypeDef,
         "replicationRunList": List[ReplicationRunTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetServersResponseTypeDef = TypedDict(
-    "GetServersResponseTypeDef",
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
     {
-        "lastModifiedOn": datetime,
-        "serverCatalogStatus": ServerCatalogStatusType,
-        "serverList": List[ServerOutputTypeDef],
-        "nextToken": str,
+        "appSummary": AppSummaryTypeDef,
+        "serverGroups": List[ServerGroupOutputTypeDef],
+        "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ServerGroupOutputTypeDef = TypedDict(
-    "ServerGroupOutputTypeDef",
-    {
-        "serverGroupId": str,
-        "name": str,
-        "serverList": List[ServerOutputTypeDef],
-    },
-    total=False,
-)
-
-ServerLaunchConfigurationOutputTypeDef = TypedDict(
-    "ServerLaunchConfigurationOutputTypeDef",
-    {
-        "server": ServerOutputTypeDef,
-        "logicalId": str,
-        "vpc": str,
-        "subnet": str,
-        "securityGroup": str,
-        "ec2KeyName": str,
-        "userData": UserDataOutputTypeDef,
-        "instanceType": str,
-        "associatePublicIpAddress": bool,
-        "iamInstanceProfileName": str,
-        "configureScript": S3LocationOutputTypeDef,
-        "configureScriptType": ScriptTypeType,
-    },
-    total=False,
-)
-
-ServerReplicationConfigurationOutputTypeDef = TypedDict(
-    "ServerReplicationConfigurationOutputTypeDef",
-    {
-        "server": ServerOutputTypeDef,
-        "serverReplicationParameters": ServerReplicationParametersOutputTypeDef,
-    },
-    total=False,
-)
-
-ServerValidationConfigurationOutputTypeDef = TypedDict(
-    "ServerValidationConfigurationOutputTypeDef",
+GetAppResponseTypeDef = TypedDict(
+    "GetAppResponseTypeDef",
     {
-        "server": ServerOutputTypeDef,
-        "validationId": str,
-        "name": str,
-        "serverValidationStrategy": Literal["USERDATA"],
-        "userDataValidationParameters": UserDataValidationParametersOutputTypeDef,
+        "appSummary": AppSummaryTypeDef,
+        "serverGroups": List[ServerGroupOutputTypeDef],
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ServerValidationOutputTypeDef = TypedDict(
-    "ServerValidationOutputTypeDef",
+UpdateAppResponseTypeDef = TypedDict(
+    "UpdateAppResponseTypeDef",
     {
-        "server": ServerOutputTypeDef,
+        "appSummary": AppSummaryTypeDef,
+        "serverGroups": List[ServerGroupOutputTypeDef],
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 CreateAppRequestRequestTypeDef = TypedDict(
     "CreateAppRequestRequestTypeDef",
     {
         "name": str,
         "description": str,
@@ -1112,96 +999,66 @@
         "roleName": str,
         "serverGroups": Sequence[ServerGroupTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-ServerGroupLaunchConfigurationTypeDef = TypedDict(
-    "ServerGroupLaunchConfigurationTypeDef",
+ServerGroupLaunchConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupLaunchConfigurationOutputTypeDef",
     {
         "serverGroupId": str,
         "launchOrder": int,
-        "serverLaunchConfigurations": Sequence[ServerLaunchConfigurationTypeDef],
+        "serverLaunchConfigurations": List[ServerLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
-ServerGroupReplicationConfigurationTypeDef = TypedDict(
-    "ServerGroupReplicationConfigurationTypeDef",
+ServerGroupLaunchConfigurationTypeDef = TypedDict(
+    "ServerGroupLaunchConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverReplicationConfigurations": Sequence[ServerReplicationConfigurationTypeDef],
+        "launchOrder": int,
+        "serverLaunchConfigurations": Sequence[ServerLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
-ServerGroupValidationConfigurationTypeDef = TypedDict(
-    "ServerGroupValidationConfigurationTypeDef",
+ServerGroupReplicationConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupReplicationConfigurationOutputTypeDef",
     {
         "serverGroupId": str,
-        "serverValidationConfigurations": Sequence[ServerValidationConfigurationTypeDef],
+        "serverReplicationConfigurations": List[ServerReplicationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
-    {
-        "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupOutputTypeDef],
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAppResponseTypeDef = TypedDict(
-    "GetAppResponseTypeDef",
-    {
-        "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupOutputTypeDef],
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAppResponseTypeDef = TypedDict(
-    "UpdateAppResponseTypeDef",
-    {
-        "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupOutputTypeDef],
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ServerGroupLaunchConfigurationOutputTypeDef = TypedDict(
-    "ServerGroupLaunchConfigurationOutputTypeDef",
+ServerGroupReplicationConfigurationTypeDef = TypedDict(
+    "ServerGroupReplicationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "launchOrder": int,
-        "serverLaunchConfigurations": List[ServerLaunchConfigurationOutputTypeDef],
+        "serverReplicationConfigurations": Sequence[ServerReplicationConfigurationTypeDef],
     },
     total=False,
 )
 
-ServerGroupReplicationConfigurationOutputTypeDef = TypedDict(
-    "ServerGroupReplicationConfigurationOutputTypeDef",
+ServerGroupValidationConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupValidationConfigurationOutputTypeDef",
     {
         "serverGroupId": str,
-        "serverReplicationConfigurations": List[ServerReplicationConfigurationOutputTypeDef],
+        "serverValidationConfigurations": List[ServerValidationConfigurationTypeDef],
     },
     total=False,
 )
 
-ServerGroupValidationConfigurationOutputTypeDef = TypedDict(
-    "ServerGroupValidationConfigurationOutputTypeDef",
+ServerGroupValidationConfigurationTypeDef = TypedDict(
+    "ServerGroupValidationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverValidationConfigurations": List[ServerValidationConfigurationOutputTypeDef],
+        "serverValidationConfigurations": Sequence[ServerValidationConfigurationTypeDef],
     },
     total=False,
 )
 
 ValidationOutputTypeDef = TypedDict(
     "ValidationOutputTypeDef",
     {
@@ -1212,36 +1069,68 @@
         "latestValidationTime": datetime,
         "appValidationOutput": AppValidationOutputTypeDef,
         "serverValidationOutput": ServerValidationOutputTypeDef,
     },
     total=False,
 )
 
+GetAppLaunchConfigurationResponseTypeDef = TypedDict(
+    "GetAppLaunchConfigurationResponseTypeDef",
+    {
+        "appId": str,
+        "roleName": str,
+        "autoLaunch": bool,
+        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
         "roleName": str,
         "autoLaunch": bool,
         "serverGroupLaunchConfigurations": Sequence[ServerGroupLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
+GetAppReplicationConfigurationResponseTypeDef = TypedDict(
+    "GetAppReplicationConfigurationResponseTypeDef",
+    {
+        "serverGroupReplicationConfigurations": List[
+            ServerGroupReplicationConfigurationOutputTypeDef
+        ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppReplicationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
         "serverGroupReplicationConfigurations": Sequence[
             ServerGroupReplicationConfigurationTypeDef
         ],
     },
     total=False,
 )
 
+GetAppValidationConfigurationResponseTypeDef = TypedDict(
+    "GetAppValidationConfigurationResponseTypeDef",
+    {
+        "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
+        "serverGroupValidationConfigurations": List[
+            ServerGroupValidationConfigurationOutputTypeDef
+        ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 _OptionalPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
@@ -1255,46 +1144,14 @@
 
 class PutAppValidationConfigurationRequestRequestTypeDef(
     _RequiredPutAppValidationConfigurationRequestRequestTypeDef,
     _OptionalPutAppValidationConfigurationRequestRequestTypeDef,
 ):
     pass
 
-GetAppLaunchConfigurationResponseTypeDef = TypedDict(
-    "GetAppLaunchConfigurationResponseTypeDef",
-    {
-        "appId": str,
-        "roleName": str,
-        "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAppReplicationConfigurationResponseTypeDef = TypedDict(
-    "GetAppReplicationConfigurationResponseTypeDef",
-    {
-        "serverGroupReplicationConfigurations": List[
-            ServerGroupReplicationConfigurationOutputTypeDef
-        ],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAppValidationConfigurationResponseTypeDef = TypedDict(
-    "GetAppValidationConfigurationResponseTypeDef",
-    {
-        "appValidationConfigurations": List[AppValidationConfigurationOutputTypeDef],
-        "serverGroupValidationConfigurations": List[
-            ServerGroupValidationConfigurationOutputTypeDef
-        ],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetAppValidationOutputResponseTypeDef = TypedDict(
     "GetAppValidationOutputResponseTypeDef",
     {
         "validationOutputList": List[ValidationOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/PKG-INFO` & `mypy-boto3-sms-1.28.15/mypy_boto3_sms.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sms
-Version: 1.28.12
-Summary: Type annotations for boto3.SMS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SMS 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sms.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sms)](https://pepy.tech/project/mypy-boto3-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
+[boto3.SMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
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
 [mypy-boto3-sms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,24 +358,23 @@
 
 ```python
 from mypy_boto3_sms.type_defs import (
     LaunchDetailsTypeDef,
     ConnectorTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
-    TagOutputTypeDef,
     CreateReplicationJobRequestRequestTypeDef,
     DeleteAppLaunchConfigurationRequestRequestTypeDef,
     DeleteAppReplicationConfigurationRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppValidationConfigurationRequestRequestTypeDef,
     DeleteReplicationJobRequestRequestTypeDef,
     DisassociateConnectorRequestRequestTypeDef,
     GenerateChangeSetRequestRequestTypeDef,
-    S3LocationOutputTypeDef,
+    S3LocationTypeDef,
     GenerateTemplateRequestRequestTypeDef,
     GetAppLaunchConfigurationRequestRequestTypeDef,
     GetAppReplicationConfigurationRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
     GetAppValidationConfigurationRequestRequestTypeDef,
     GetAppValidationOutputRequestRequestTypeDef,
     PaginatorConfigTypeDef,
@@ -384,86 +383,75 @@
     GetReplicationRunsRequestRequestTypeDef,
     VmServerAddressTypeDef,
     ImportAppCatalogRequestRequestTypeDef,
     LaunchAppRequestRequestTypeDef,
     ListAppsRequestRequestTypeDef,
     NotificationContextTypeDef,
     ReplicationRunStageDetailsTypeDef,
-    S3LocationTypeDef,
     ServerReplicationParametersOutputTypeDef,
     ServerReplicationParametersTypeDef,
     StartAppReplicationRequestRequestTypeDef,
     StartOnDemandAppReplicationRequestRequestTypeDef,
     StartOnDemandReplicationRunRequestRequestTypeDef,
     StopAppReplicationRequestRequestTypeDef,
     TerminateAppRequestRequestTypeDef,
     UpdateReplicationJobRequestRequestTypeDef,
-    VmServerAddressOutputTypeDef,
     AppSummaryTypeDef,
     CreateReplicationJobResponseTypeDef,
     GetConnectorsResponseTypeDef,
     StartOnDemandReplicationRunResponseTypeDef,
     GenerateChangeSetResponseTypeDef,
     GenerateTemplateResponseTypeDef,
     SSMOutputTypeDef,
-    SourceOutputTypeDef,
-    UserDataOutputTypeDef,
+    SourceTypeDef,
+    UserDataTypeDef,
     GetConnectorsRequestGetConnectorsPaginateTypeDef,
     GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
     GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
     ListAppsRequestListAppsPaginateTypeDef,
     GetServersRequestGetServersPaginateTypeDef,
     GetServersRequestRequestTypeDef,
     VmServerTypeDef,
     NotifyAppValidationOutputRequestRequestTypeDef,
     ReplicationRunTypeDef,
-    SourceTypeDef,
-    UserDataTypeDef,
-    VmServerOutputTypeDef,
     ListAppsResponseTypeDef,
     AppValidationOutputTypeDef,
-    SSMValidationParametersOutputTypeDef,
-    UserDataValidationParametersOutputTypeDef,
-    ServerTypeDef,
     SSMValidationParametersTypeDef,
     UserDataValidationParametersTypeDef,
+    ServerTypeDef,
     ReplicationJobTypeDef,
-    ServerOutputTypeDef,
-    AppValidationConfigurationOutputTypeDef,
+    AppValidationConfigurationTypeDef,
+    GetServersResponseTypeDef,
+    ServerGroupOutputTypeDef,
     ServerGroupTypeDef,
     ServerLaunchConfigurationTypeDef,
+    ServerReplicationConfigurationOutputTypeDef,
     ServerReplicationConfigurationTypeDef,
-    AppValidationConfigurationTypeDef,
     ServerValidationConfigurationTypeDef,
+    ServerValidationOutputTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
-    GetServersResponseTypeDef,
-    ServerGroupOutputTypeDef,
-    ServerLaunchConfigurationOutputTypeDef,
-    ServerReplicationConfigurationOutputTypeDef,
-    ServerValidationConfigurationOutputTypeDef,
-    ServerValidationOutputTypeDef,
-    CreateAppRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
-    ServerGroupLaunchConfigurationTypeDef,
-    ServerGroupReplicationConfigurationTypeDef,
-    ServerGroupValidationConfigurationTypeDef,
     CreateAppResponseTypeDef,
     GetAppResponseTypeDef,
     UpdateAppResponseTypeDef,
+    CreateAppRequestRequestTypeDef,
+    UpdateAppRequestRequestTypeDef,
     ServerGroupLaunchConfigurationOutputTypeDef,
+    ServerGroupLaunchConfigurationTypeDef,
     ServerGroupReplicationConfigurationOutputTypeDef,
+    ServerGroupReplicationConfigurationTypeDef,
     ServerGroupValidationConfigurationOutputTypeDef,
+    ServerGroupValidationConfigurationTypeDef,
     ValidationOutputTypeDef,
-    PutAppLaunchConfigurationRequestRequestTypeDef,
-    PutAppReplicationConfigurationRequestRequestTypeDef,
-    PutAppValidationConfigurationRequestRequestTypeDef,
     GetAppLaunchConfigurationResponseTypeDef,
+    PutAppLaunchConfigurationRequestRequestTypeDef,
     GetAppReplicationConfigurationResponseTypeDef,
+    PutAppReplicationConfigurationRequestRequestTypeDef,
     GetAppValidationConfigurationResponseTypeDef,
+    PutAppValidationConfigurationRequestRequestTypeDef,
     GetAppValidationOutputResponseTypeDef,
 )
 
 
 def get_structure() -> LaunchDetailsTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/SOURCES.txt` & `mypy-boto3-sms-1.28.15/mypy_boto3_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.12/setup.py` & `mypy-boto3-sms-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sms",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_sms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SMS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.SMS 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

