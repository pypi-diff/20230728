# Comparing `tmp/mypy-boto3-devicefarm-1.28.12.tar.gz` & `tmp/mypy-boto3-devicefarm-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-devicefarm-1.28.12.tar", last modified: Thu Jul 27 05:34:33 2023, max compression
+gzip compressed data, was "mypy-boto3-devicefarm-1.28.15.tar", last modified: Fri Jul 28 20:42:37 2023, max compression
```

## Comparing `mypy-boto3-devicefarm-1.28.12.tar` & `mypy-boto3-devicefarm-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.944535 mypy-boto3-devicefarm-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-07-27 05:34:33.944535 mypy-boto3-devicefarm-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.940535 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57697 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57593 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-27 05:20:08.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-27 05:20:08.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22386 2023-07-27 05:20:08.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    74980 2023-07-27 05:20:10.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    74889 2023-07-27 05:20:09.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.944535 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-07-27 05:34:33.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:33.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:33.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:33.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:33.944535 mypy-boto3-devicefarm-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.720957 mypy-boto3-devicefarm-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24826 2023-07-28 20:42:37.716957 mypy-boto3-devicefarm-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23327 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.716957 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57697 2023-07-28 20:22:47.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57593 2023-07-28 20:22:47.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-28 20:22:47.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-28 20:22:47.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22346 2023-07-28 20:22:47.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22324 2023-07-28 20:22:47.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    74057 2023-07-28 20:22:50.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73966 2023-07-28 20:22:49.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.716957 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24826 2023-07-28 20:42:37.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:37.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:37.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:37.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:37.720957 mypy-boto3-devicefarm-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/setup.py
```

### Comparing `mypy-boto3-devicefarm-1.28.12/LICENSE` & `mypy-boto3-devicefarm-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.12/PKG-INFO` & `mypy-boto3-devicefarm-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devicefarm
-Version: 1.28.12
-Summary: Type annotations for boto3.DeviceFarm 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DeviceFarm 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devicefarm)](https://pepy.tech/project/mypy-boto3-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DeviceFarm 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[boto3.DeviceFarm 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
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
 [mypy-boto3-devicefarm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -428,23 +428,23 @@
 ```python
 from mypy_boto3_devicefarm.type_defs import (
     TrialMinutesTypeDef,
     ArtifactTypeDef,
     CPUTypeDef,
     CountersTypeDef,
     RuleTypeDef,
+    ResponseMetadataTypeDef,
     CreateInstanceProfileRequestRequestTypeDef,
     InstanceProfileTypeDef,
     CreateNetworkProfileRequestRequestTypeDef,
     NetworkProfileTypeDef,
     VpcConfigTypeDef,
     CreateRemoteAccessSessionConfigurationTypeDef,
     TestGridVpcConfigTypeDef,
     CreateTestGridUrlRequestRequestTypeDef,
-    CreateTestGridUrlResultTypeDef,
     CreateUploadRequestRequestTypeDef,
     UploadTypeDef,
     CreateVPCEConfigurationRequestRequestTypeDef,
     VPCEConfigurationTypeDef,
     CustomerArtifactPathsOutputTypeDef,
     CustomerArtifactPathsTypeDef,
     DeleteDevicePoolRequestRequestTypeDef,
@@ -456,109 +456,87 @@
     DeleteTestGridProjectRequestRequestTypeDef,
     DeleteUploadRequestRequestTypeDef,
     DeleteVPCEConfigurationRequestRequestTypeDef,
     DeviceFilterOutputTypeDef,
     DeviceFilterTypeDef,
     DeviceMinutesTypeDef,
     IncompatibilityMessageTypeDef,
-    RuleOutputTypeDef,
     ResolutionTypeDef,
     ExecutionConfigurationTypeDef,
     GetDeviceInstanceRequestRequestTypeDef,
     ScheduleRunTestTypeDef,
     GetDevicePoolRequestRequestTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetNetworkProfileRequestRequestTypeDef,
-    GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetOfferingStatusRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetRemoteAccessSessionRequestRequestTypeDef,
     GetRunRequestRequestTypeDef,
     GetSuiteRequestRequestTypeDef,
     GetTestGridProjectRequestRequestTypeDef,
     GetTestGridSessionRequestRequestTypeDef,
     TestGridSessionTypeDef,
     GetTestRequestRequestTypeDef,
     GetUploadRequestRequestTypeDef,
     GetVPCEConfigurationRequestRequestTypeDef,
     InstallToRemoteAccessSessionRequestRequestTypeDef,
-    ListArtifactsRequestListArtifactsPaginateTypeDef,
     ListArtifactsRequestRequestTypeDef,
-    ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef,
     ListDeviceInstancesRequestRequestTypeDef,
-    ListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
     ListDevicePoolsRequestRequestTypeDef,
-    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListInstanceProfilesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
     ListNetworkProfilesRequestRequestTypeDef,
-    ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef,
     ListOfferingPromotionsRequestRequestTypeDef,
     OfferingPromotionTypeDef,
-    ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef,
     ListOfferingTransactionsRequestRequestTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
-    ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
     ListRemoteAccessSessionsRequestRequestTypeDef,
-    ListRunsRequestListRunsPaginateTypeDef,
     ListRunsRequestRequestTypeDef,
-    ListSamplesRequestListSamplesPaginateTypeDef,
     ListSamplesRequestRequestTypeDef,
     SampleTypeDef,
-    ListSuitesRequestListSuitesPaginateTypeDef,
     ListSuitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     ListTestGridProjectsRequestRequestTypeDef,
     ListTestGridSessionActionsRequestRequestTypeDef,
     TestGridSessionActionTypeDef,
     ListTestGridSessionArtifactsRequestRequestTypeDef,
     TestGridSessionArtifactTypeDef,
     ListTestGridSessionsRequestRequestTypeDef,
-    ListTestsRequestListTestsPaginateTypeDef,
     ListTestsRequestRequestTypeDef,
-    ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
     ListUniqueProblemsRequestRequestTypeDef,
-    ListUploadsRequestListUploadsPaginateTypeDef,
     ListUploadsRequestRequestTypeDef,
-    ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef,
     ListVPCEConfigurationsRequestRequestTypeDef,
-    LocationOutputTypeDef,
     LocationTypeDef,
     MonetaryAmountTypeDef,
-    PaginatorConfigTypeDef,
     ProblemDetailTypeDef,
     VpcConfigOutputTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
-    RadiosOutputTypeDef,
     RadiosTypeDef,
     RenewOfferingRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     StopJobRequestRequestTypeDef,
     StopRemoteAccessSessionRequestRequestTypeDef,
     StopRunRequestRequestTypeDef,
-    TagTypeDef,
     TestGridVpcConfigOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceInstanceRequestRequestTypeDef,
     UpdateInstanceProfileRequestRequestTypeDef,
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateUploadRequestRequestTypeDef,
     UpdateVPCEConfigurationRequestRequestTypeDef,
     AccountSettingsTypeDef,
-    ListArtifactsResultTypeDef,
     CreateDevicePoolRequestRequestTypeDef,
+    DevicePoolTypeDef,
     UpdateDevicePoolRequestRequestTypeDef,
+    CreateTestGridUrlResultTypeDef,
+    ListArtifactsResultTypeDef,
     CreateInstanceProfileResultTypeDef,
     DeviceInstanceTypeDef,
     GetInstanceProfileResultTypeDef,
     ListInstanceProfilesResultTypeDef,
     UpdateInstanceProfileResultTypeDef,
     CreateNetworkProfileResultTypeDef,
     GetNetworkProfileResultTypeDef,
@@ -576,45 +554,63 @@
     UpdateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
     GetVPCEConfigurationResultTypeDef,
     ListVPCEConfigurationsResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
     DeviceSelectionResultTypeDef,
     DeviceSelectionConfigurationTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDevicesRequestRequestTypeDef,
     SuiteTypeDef,
     TestTypeDef,
-    DevicePoolTypeDef,
+    GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef,
+    ListArtifactsRequestListArtifactsPaginateTypeDef,
+    ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef,
+    ListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
+    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
+    ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef,
+    ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
+    ListRunsRequestListRunsPaginateTypeDef,
+    ListSamplesRequestListSamplesPaginateTypeDef,
+    ListSuitesRequestListSuitesPaginateTypeDef,
+    ListTestsRequestListTestsPaginateTypeDef,
+    ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
+    ListUploadsRequestListUploadsPaginateTypeDef,
+    ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef,
     GetTestGridSessionResultTypeDef,
     ListTestGridSessionsResultTypeDef,
     ListOfferingPromotionsResultTypeDef,
     ListSamplesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ListTestGridSessionActionsResultTypeDef,
     ListTestGridSessionArtifactsResultTypeDef,
     RecurringChargeTypeDef,
     ProjectTypeDef,
     ScheduleRunConfigurationTypeDef,
-    TagResourceRequestRequestTypeDef,
     TestGridProjectTypeDef,
     GetAccountSettingsResultTypeDef,
+    CreateDevicePoolResultTypeDef,
+    GetDevicePoolResultTypeDef,
+    ListDevicePoolsResultTypeDef,
+    UpdateDevicePoolResultTypeDef,
     DeviceTypeDef,
     GetDeviceInstanceResultTypeDef,
     ListDeviceInstancesResultTypeDef,
     UpdateDeviceInstanceResultTypeDef,
     RunTypeDef,
     GetSuiteResultTypeDef,
     ListSuitesResultTypeDef,
     GetTestResultTypeDef,
     ListTestsResultTypeDef,
-    CreateDevicePoolResultTypeDef,
-    GetDevicePoolResultTypeDef,
-    ListDevicePoolsResultTypeDef,
-    UpdateDevicePoolResultTypeDef,
     OfferingTypeDef,
     CreateProjectResultTypeDef,
     GetProjectResultTypeDef,
     ListProjectsResultTypeDef,
     UpdateProjectResultTypeDef,
     GetDevicePoolCompatibilityRequestRequestTypeDef,
     ScheduleRunRequestRequestTypeDef,
```

### Comparing `mypy-boto3-devicefarm-1.28.12/README.md` & `mypy-boto3-devicefarm-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devicefarm)](https://pepy.tech/project/mypy-boto3-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DeviceFarm 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[boto3.DeviceFarm 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
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
 [mypy-boto3-devicefarm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -396,23 +396,23 @@
 ```python
 from mypy_boto3_devicefarm.type_defs import (
     TrialMinutesTypeDef,
     ArtifactTypeDef,
     CPUTypeDef,
     CountersTypeDef,
     RuleTypeDef,
+    ResponseMetadataTypeDef,
     CreateInstanceProfileRequestRequestTypeDef,
     InstanceProfileTypeDef,
     CreateNetworkProfileRequestRequestTypeDef,
     NetworkProfileTypeDef,
     VpcConfigTypeDef,
     CreateRemoteAccessSessionConfigurationTypeDef,
     TestGridVpcConfigTypeDef,
     CreateTestGridUrlRequestRequestTypeDef,
-    CreateTestGridUrlResultTypeDef,
     CreateUploadRequestRequestTypeDef,
     UploadTypeDef,
     CreateVPCEConfigurationRequestRequestTypeDef,
     VPCEConfigurationTypeDef,
     CustomerArtifactPathsOutputTypeDef,
     CustomerArtifactPathsTypeDef,
     DeleteDevicePoolRequestRequestTypeDef,
@@ -424,109 +424,87 @@
     DeleteTestGridProjectRequestRequestTypeDef,
     DeleteUploadRequestRequestTypeDef,
     DeleteVPCEConfigurationRequestRequestTypeDef,
     DeviceFilterOutputTypeDef,
     DeviceFilterTypeDef,
     DeviceMinutesTypeDef,
     IncompatibilityMessageTypeDef,
-    RuleOutputTypeDef,
     ResolutionTypeDef,
     ExecutionConfigurationTypeDef,
     GetDeviceInstanceRequestRequestTypeDef,
     ScheduleRunTestTypeDef,
     GetDevicePoolRequestRequestTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetNetworkProfileRequestRequestTypeDef,
-    GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetOfferingStatusRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetRemoteAccessSessionRequestRequestTypeDef,
     GetRunRequestRequestTypeDef,
     GetSuiteRequestRequestTypeDef,
     GetTestGridProjectRequestRequestTypeDef,
     GetTestGridSessionRequestRequestTypeDef,
     TestGridSessionTypeDef,
     GetTestRequestRequestTypeDef,
     GetUploadRequestRequestTypeDef,
     GetVPCEConfigurationRequestRequestTypeDef,
     InstallToRemoteAccessSessionRequestRequestTypeDef,
-    ListArtifactsRequestListArtifactsPaginateTypeDef,
     ListArtifactsRequestRequestTypeDef,
-    ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef,
     ListDeviceInstancesRequestRequestTypeDef,
-    ListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
     ListDevicePoolsRequestRequestTypeDef,
-    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListInstanceProfilesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
     ListNetworkProfilesRequestRequestTypeDef,
-    ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef,
     ListOfferingPromotionsRequestRequestTypeDef,
     OfferingPromotionTypeDef,
-    ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef,
     ListOfferingTransactionsRequestRequestTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
-    ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
     ListRemoteAccessSessionsRequestRequestTypeDef,
-    ListRunsRequestListRunsPaginateTypeDef,
     ListRunsRequestRequestTypeDef,
-    ListSamplesRequestListSamplesPaginateTypeDef,
     ListSamplesRequestRequestTypeDef,
     SampleTypeDef,
-    ListSuitesRequestListSuitesPaginateTypeDef,
     ListSuitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     ListTestGridProjectsRequestRequestTypeDef,
     ListTestGridSessionActionsRequestRequestTypeDef,
     TestGridSessionActionTypeDef,
     ListTestGridSessionArtifactsRequestRequestTypeDef,
     TestGridSessionArtifactTypeDef,
     ListTestGridSessionsRequestRequestTypeDef,
-    ListTestsRequestListTestsPaginateTypeDef,
     ListTestsRequestRequestTypeDef,
-    ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
     ListUniqueProblemsRequestRequestTypeDef,
-    ListUploadsRequestListUploadsPaginateTypeDef,
     ListUploadsRequestRequestTypeDef,
-    ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef,
     ListVPCEConfigurationsRequestRequestTypeDef,
-    LocationOutputTypeDef,
     LocationTypeDef,
     MonetaryAmountTypeDef,
-    PaginatorConfigTypeDef,
     ProblemDetailTypeDef,
     VpcConfigOutputTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
-    RadiosOutputTypeDef,
     RadiosTypeDef,
     RenewOfferingRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     StopJobRequestRequestTypeDef,
     StopRemoteAccessSessionRequestRequestTypeDef,
     StopRunRequestRequestTypeDef,
-    TagTypeDef,
     TestGridVpcConfigOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceInstanceRequestRequestTypeDef,
     UpdateInstanceProfileRequestRequestTypeDef,
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateUploadRequestRequestTypeDef,
     UpdateVPCEConfigurationRequestRequestTypeDef,
     AccountSettingsTypeDef,
-    ListArtifactsResultTypeDef,
     CreateDevicePoolRequestRequestTypeDef,
+    DevicePoolTypeDef,
     UpdateDevicePoolRequestRequestTypeDef,
+    CreateTestGridUrlResultTypeDef,
+    ListArtifactsResultTypeDef,
     CreateInstanceProfileResultTypeDef,
     DeviceInstanceTypeDef,
     GetInstanceProfileResultTypeDef,
     ListInstanceProfilesResultTypeDef,
     UpdateInstanceProfileResultTypeDef,
     CreateNetworkProfileResultTypeDef,
     GetNetworkProfileResultTypeDef,
@@ -544,45 +522,63 @@
     UpdateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
     GetVPCEConfigurationResultTypeDef,
     ListVPCEConfigurationsResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
     DeviceSelectionResultTypeDef,
     DeviceSelectionConfigurationTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDevicesRequestRequestTypeDef,
     SuiteTypeDef,
     TestTypeDef,
-    DevicePoolTypeDef,
+    GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef,
+    ListArtifactsRequestListArtifactsPaginateTypeDef,
+    ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef,
+    ListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
+    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
+    ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef,
+    ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
+    ListRunsRequestListRunsPaginateTypeDef,
+    ListSamplesRequestListSamplesPaginateTypeDef,
+    ListSuitesRequestListSuitesPaginateTypeDef,
+    ListTestsRequestListTestsPaginateTypeDef,
+    ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
+    ListUploadsRequestListUploadsPaginateTypeDef,
+    ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef,
     GetTestGridSessionResultTypeDef,
     ListTestGridSessionsResultTypeDef,
     ListOfferingPromotionsResultTypeDef,
     ListSamplesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ListTestGridSessionActionsResultTypeDef,
     ListTestGridSessionArtifactsResultTypeDef,
     RecurringChargeTypeDef,
     ProjectTypeDef,
     ScheduleRunConfigurationTypeDef,
-    TagResourceRequestRequestTypeDef,
     TestGridProjectTypeDef,
     GetAccountSettingsResultTypeDef,
+    CreateDevicePoolResultTypeDef,
+    GetDevicePoolResultTypeDef,
+    ListDevicePoolsResultTypeDef,
+    UpdateDevicePoolResultTypeDef,
     DeviceTypeDef,
     GetDeviceInstanceResultTypeDef,
     ListDeviceInstancesResultTypeDef,
     UpdateDeviceInstanceResultTypeDef,
     RunTypeDef,
     GetSuiteResultTypeDef,
     ListSuitesResultTypeDef,
     GetTestResultTypeDef,
     ListTestsResultTypeDef,
-    CreateDevicePoolResultTypeDef,
-    GetDevicePoolResultTypeDef,
-    ListDevicePoolsResultTypeDef,
-    UpdateDevicePoolResultTypeDef,
     OfferingTypeDef,
     CreateProjectResultTypeDef,
     GetProjectResultTypeDef,
     ListProjectsResultTypeDef,
     UpdateProjectResultTypeDef,
     GetDevicePoolCompatibilityRequestRequestTypeDef,
     ScheduleRunRequestRequestTypeDef,
```

### Comparing `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/__init__.py` & `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/__init__.pyi` & `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/__main__.py` & `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DeviceFarm 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.DeviceFarm 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm\nOther"
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

### Comparing `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/client.py` & `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/client.pyi` & `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/literals.py` & `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/literals.pyi` & `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/paginator.py` & `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 class GetOfferingStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.GetOfferingStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#getofferingstatuspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetOfferingStatusResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.GetOfferingStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#getofferingstatuspaginator)
         """
 
 
@@ -148,30 +148,30 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: ArtifactCategoryType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListArtifactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListArtifacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listartifactspaginator)
         """
 
 
 class ListDeviceInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDeviceInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdeviceinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeviceInstancesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDeviceInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdeviceinstancespaginator)
         """
 
 
@@ -182,15 +182,15 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: DevicePoolTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevicePoolsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevicePools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicepoolspaginator)
         """
 
 
@@ -201,45 +201,45 @@
     """
 
     def paginate(
         self,
         *,
         arn: str = ...,
         filters: Sequence[DeviceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevicesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicespaginator)
         """
 
 
 class ListInstanceProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListInstanceProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listinstanceprofilespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstanceProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListInstanceProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listinstanceprofilespaginator)
         """
 
 
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listjobspaginator)
         """
 
 
@@ -250,165 +250,165 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: NetworkProfileTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNetworkProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListNetworkProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listnetworkprofilespaginator)
         """
 
 
 class ListOfferingPromotionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingPromotions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingpromotionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOfferingPromotionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingPromotions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingpromotionspaginator)
         """
 
 
 class ListOfferingTransactionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingTransactions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingtransactionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOfferingTransactionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingTransactions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingtransactionspaginator)
         """
 
 
 class ListOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOfferingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingspaginator)
         """
 
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, arn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listprojectspaginator)
         """
 
 
 class ListRemoteAccessSessionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRemoteAccessSessions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listremoteaccesssessionspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRemoteAccessSessionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRemoteAccessSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listremoteaccesssessionspaginator)
         """
 
 
 class ListRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listrunspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRunsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listrunspaginator)
         """
 
 
 class ListSamplesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSamples)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsamplespaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSamplesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSamples.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsamplespaginator)
         """
 
 
 class ListSuitesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSuites)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsuitespaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSuitesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSuites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsuitespaginator)
         """
 
 
 class ListTestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListTests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listtestspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTestsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListTests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listtestspaginator)
         """
 
 
 class ListUniqueProblemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUniqueProblems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listuniqueproblemspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUniqueProblemsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUniqueProblems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listuniqueproblemspaginator)
         """
 
 
@@ -419,28 +419,28 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: UploadTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUploadsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listuploadspaginator)
         """
 
 
 class ListVPCEConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListVPCEConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listvpceconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVPCEConfigurationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListVPCEConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listvpceconfigurationspaginator)
         """
```

### Comparing `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/paginator.pyi` & `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 class GetOfferingStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.GetOfferingStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#getofferingstatuspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetOfferingStatusResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.GetOfferingStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#getofferingstatuspaginator)
         """
 
 class ListArtifactsPaginator(Paginator):
@@ -144,29 +144,29 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: ArtifactCategoryType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListArtifactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListArtifacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listartifactspaginator)
         """
 
 class ListDeviceInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDeviceInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdeviceinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeviceInstancesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDeviceInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdeviceinstancespaginator)
         """
 
 class ListDevicePoolsPaginator(Paginator):
@@ -176,15 +176,15 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: DevicePoolTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevicePoolsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevicePools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicepoolspaginator)
         """
 
 class ListDevicesPaginator(Paginator):
@@ -194,43 +194,43 @@
     """
 
     def paginate(
         self,
         *,
         arn: str = ...,
         filters: Sequence[DeviceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevicesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicespaginator)
         """
 
 class ListInstanceProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListInstanceProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listinstanceprofilespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstanceProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListInstanceProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listinstanceprofilespaginator)
         """
 
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listjobspaginator)
         """
 
 class ListNetworkProfilesPaginator(Paginator):
@@ -240,155 +240,155 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: NetworkProfileTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNetworkProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListNetworkProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listnetworkprofilespaginator)
         """
 
 class ListOfferingPromotionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingPromotions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingpromotionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOfferingPromotionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingPromotions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingpromotionspaginator)
         """
 
 class ListOfferingTransactionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingTransactions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingtransactionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOfferingTransactionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingTransactions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingtransactionspaginator)
         """
 
 class ListOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOfferingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingspaginator)
         """
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, arn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listprojectspaginator)
         """
 
 class ListRemoteAccessSessionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRemoteAccessSessions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listremoteaccesssessionspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRemoteAccessSessionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRemoteAccessSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listremoteaccesssessionspaginator)
         """
 
 class ListRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listrunspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRunsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listrunspaginator)
         """
 
 class ListSamplesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSamples)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsamplespaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSamplesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSamples.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsamplespaginator)
         """
 
 class ListSuitesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSuites)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsuitespaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSuitesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSuites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsuitespaginator)
         """
 
 class ListTestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListTests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listtestspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTestsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListTests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listtestspaginator)
         """
 
 class ListUniqueProblemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUniqueProblems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listuniqueproblemspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUniqueProblemsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUniqueProblems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listuniqueproblemspaginator)
         """
 
 class ListUploadsPaginator(Paginator):
@@ -398,27 +398,27 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: UploadTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUploadsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listuploadspaginator)
         """
 
 class ListVPCEConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListVPCEConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listvpceconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVPCEConfigurationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListVPCEConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listvpceconfigurationspaginator)
         """
```

### Comparing `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/type_defs.py` & `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,23 +55,23 @@
 
 __all__ = (
     "TrialMinutesTypeDef",
     "ArtifactTypeDef",
     "CPUTypeDef",
     "CountersTypeDef",
     "RuleTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateInstanceProfileRequestRequestTypeDef",
     "InstanceProfileTypeDef",
     "CreateNetworkProfileRequestRequestTypeDef",
     "NetworkProfileTypeDef",
     "VpcConfigTypeDef",
     "CreateRemoteAccessSessionConfigurationTypeDef",
     "TestGridVpcConfigTypeDef",
     "CreateTestGridUrlRequestRequestTypeDef",
-    "CreateTestGridUrlResultTypeDef",
     "CreateUploadRequestRequestTypeDef",
     "UploadTypeDef",
     "CreateVPCEConfigurationRequestRequestTypeDef",
     "VPCEConfigurationTypeDef",
     "CustomerArtifactPathsOutputTypeDef",
     "CustomerArtifactPathsTypeDef",
     "DeleteDevicePoolRequestRequestTypeDef",
@@ -83,109 +83,87 @@
     "DeleteTestGridProjectRequestRequestTypeDef",
     "DeleteUploadRequestRequestTypeDef",
     "DeleteVPCEConfigurationRequestRequestTypeDef",
     "DeviceFilterOutputTypeDef",
     "DeviceFilterTypeDef",
     "DeviceMinutesTypeDef",
     "IncompatibilityMessageTypeDef",
-    "RuleOutputTypeDef",
     "ResolutionTypeDef",
     "ExecutionConfigurationTypeDef",
     "GetDeviceInstanceRequestRequestTypeDef",
     "ScheduleRunTestTypeDef",
     "GetDevicePoolRequestRequestTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetInstanceProfileRequestRequestTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetNetworkProfileRequestRequestTypeDef",
-    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetOfferingStatusRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetRemoteAccessSessionRequestRequestTypeDef",
     "GetRunRequestRequestTypeDef",
     "GetSuiteRequestRequestTypeDef",
     "GetTestGridProjectRequestRequestTypeDef",
     "GetTestGridSessionRequestRequestTypeDef",
     "TestGridSessionTypeDef",
     "GetTestRequestRequestTypeDef",
     "GetUploadRequestRequestTypeDef",
     "GetVPCEConfigurationRequestRequestTypeDef",
     "InstallToRemoteAccessSessionRequestRequestTypeDef",
-    "ListArtifactsRequestListArtifactsPaginateTypeDef",
     "ListArtifactsRequestRequestTypeDef",
-    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
     "ListDeviceInstancesRequestRequestTypeDef",
-    "ListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
     "ListDevicePoolsRequestRequestTypeDef",
-    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     "ListInstanceProfilesRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
     "ListNetworkProfilesRequestRequestTypeDef",
-    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
     "ListOfferingPromotionsRequestRequestTypeDef",
     "OfferingPromotionTypeDef",
-    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
     "ListOfferingTransactionsRequestRequestTypeDef",
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListOfferingsRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
-    "ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
     "ListRemoteAccessSessionsRequestRequestTypeDef",
-    "ListRunsRequestListRunsPaginateTypeDef",
     "ListRunsRequestRequestTypeDef",
-    "ListSamplesRequestListSamplesPaginateTypeDef",
     "ListSamplesRequestRequestTypeDef",
     "SampleTypeDef",
-    "ListSuitesRequestListSuitesPaginateTypeDef",
     "ListSuitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "ListTestGridProjectsRequestRequestTypeDef",
     "ListTestGridSessionActionsRequestRequestTypeDef",
     "TestGridSessionActionTypeDef",
     "ListTestGridSessionArtifactsRequestRequestTypeDef",
     "TestGridSessionArtifactTypeDef",
     "ListTestGridSessionsRequestRequestTypeDef",
-    "ListTestsRequestListTestsPaginateTypeDef",
     "ListTestsRequestRequestTypeDef",
-    "ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
     "ListUniqueProblemsRequestRequestTypeDef",
-    "ListUploadsRequestListUploadsPaginateTypeDef",
     "ListUploadsRequestRequestTypeDef",
-    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
     "ListVPCEConfigurationsRequestRequestTypeDef",
-    "LocationOutputTypeDef",
     "LocationTypeDef",
     "MonetaryAmountTypeDef",
-    "PaginatorConfigTypeDef",
     "ProblemDetailTypeDef",
     "VpcConfigOutputTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
-    "RadiosOutputTypeDef",
     "RadiosTypeDef",
     "RenewOfferingRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StopJobRequestRequestTypeDef",
     "StopRemoteAccessSessionRequestRequestTypeDef",
     "StopRunRequestRequestTypeDef",
-    "TagTypeDef",
     "TestGridVpcConfigOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceInstanceRequestRequestTypeDef",
     "UpdateInstanceProfileRequestRequestTypeDef",
     "UpdateNetworkProfileRequestRequestTypeDef",
     "UpdateUploadRequestRequestTypeDef",
     "UpdateVPCEConfigurationRequestRequestTypeDef",
     "AccountSettingsTypeDef",
-    "ListArtifactsResultTypeDef",
     "CreateDevicePoolRequestRequestTypeDef",
+    "DevicePoolTypeDef",
     "UpdateDevicePoolRequestRequestTypeDef",
+    "CreateTestGridUrlResultTypeDef",
+    "ListArtifactsResultTypeDef",
     "CreateInstanceProfileResultTypeDef",
     "DeviceInstanceTypeDef",
     "GetInstanceProfileResultTypeDef",
     "ListInstanceProfilesResultTypeDef",
     "UpdateInstanceProfileResultTypeDef",
     "CreateNetworkProfileResultTypeDef",
     "GetNetworkProfileResultTypeDef",
@@ -203,45 +181,63 @@
     "UpdateUploadResultTypeDef",
     "CreateVPCEConfigurationResultTypeDef",
     "GetVPCEConfigurationResultTypeDef",
     "ListVPCEConfigurationsResultTypeDef",
     "UpdateVPCEConfigurationResultTypeDef",
     "DeviceSelectionResultTypeDef",
     "DeviceSelectionConfigurationTypeDef",
-    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "SuiteTypeDef",
     "TestTypeDef",
-    "DevicePoolTypeDef",
+    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
+    "ListArtifactsRequestListArtifactsPaginateTypeDef",
+    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
+    "ListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
+    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
+    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
+    "ListRunsRequestListRunsPaginateTypeDef",
+    "ListSamplesRequestListSamplesPaginateTypeDef",
+    "ListSuitesRequestListSuitesPaginateTypeDef",
+    "ListTestsRequestListTestsPaginateTypeDef",
+    "ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
+    "ListUploadsRequestListUploadsPaginateTypeDef",
+    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
     "GetTestGridSessionResultTypeDef",
     "ListTestGridSessionsResultTypeDef",
     "ListOfferingPromotionsResultTypeDef",
     "ListSamplesResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ListTestGridSessionActionsResultTypeDef",
     "ListTestGridSessionArtifactsResultTypeDef",
     "RecurringChargeTypeDef",
     "ProjectTypeDef",
     "ScheduleRunConfigurationTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "TestGridProjectTypeDef",
     "GetAccountSettingsResultTypeDef",
+    "CreateDevicePoolResultTypeDef",
+    "GetDevicePoolResultTypeDef",
+    "ListDevicePoolsResultTypeDef",
+    "UpdateDevicePoolResultTypeDef",
     "DeviceTypeDef",
     "GetDeviceInstanceResultTypeDef",
     "ListDeviceInstancesResultTypeDef",
     "UpdateDeviceInstanceResultTypeDef",
     "RunTypeDef",
     "GetSuiteResultTypeDef",
     "ListSuitesResultTypeDef",
     "GetTestResultTypeDef",
     "ListTestsResultTypeDef",
-    "CreateDevicePoolResultTypeDef",
-    "GetDevicePoolResultTypeDef",
-    "ListDevicePoolsResultTypeDef",
-    "UpdateDevicePoolResultTypeDef",
     "OfferingTypeDef",
     "CreateProjectResultTypeDef",
     "GetProjectResultTypeDef",
     "ListProjectsResultTypeDef",
     "UpdateProjectResultTypeDef",
     "GetDevicePoolCompatibilityRequestRequestTypeDef",
     "ScheduleRunRequestRequestTypeDef",
@@ -329,14 +325,25 @@
         "attribute": DeviceAttributeType,
         "operator": RuleOperatorType,
         "value": str,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredCreateInstanceProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInstanceProfileRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateInstanceProfileRequestRequestTypeDef = TypedDict(
@@ -453,23 +460,14 @@
     "CreateTestGridUrlRequestRequestTypeDef",
     {
         "projectArn": str,
         "expiresInSeconds": int,
     },
 )
 
-CreateTestGridUrlResultTypeDef = TypedDict(
-    "CreateTestGridUrlResultTypeDef",
-    {
-        "url": str,
-        "expires": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUploadRequestRequestTypeDef",
     {
         "projectArn": str,
         "name": str,
         "type": UploadTypeType,
     },
@@ -658,24 +656,14 @@
     {
         "message": str,
         "type": DeviceAttributeType,
     },
     total=False,
 )
 
-RuleOutputTypeDef = TypedDict(
-    "RuleOutputTypeDef",
-    {
-        "attribute": DeviceAttributeType,
-        "operator": RuleOperatorType,
-        "value": str,
-    },
-    total=False,
-)
-
 ResolutionTypeDef = TypedDict(
     "ResolutionTypeDef",
     {
         "width": int,
         "height": int,
     },
     total=False,
@@ -753,18 +741,20 @@
 GetNetworkProfileRequestRequestTypeDef = TypedDict(
     "GetNetworkProfileRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef = TypedDict(
-    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetOfferingStatusRequestRequestTypeDef = TypedDict(
     "GetOfferingStatusRequestRequestTypeDef",
     {
@@ -856,37 +846,14 @@
     "InstallToRemoteAccessSessionRequestRequestTypeDef",
     {
         "remoteAccessSessionArn": str,
         "appArn": str,
     },
 )
 
-_RequiredListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
-    "_RequiredListArtifactsRequestListArtifactsPaginateTypeDef",
-    {
-        "arn": str,
-        "type": ArtifactCategoryType,
-    },
-)
-_OptionalListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
-    "_OptionalListArtifactsRequestListArtifactsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListArtifactsRequestListArtifactsPaginateTypeDef(
-    _RequiredListArtifactsRequestListArtifactsPaginateTypeDef,
-    _OptionalListArtifactsRequestListArtifactsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListArtifactsRequestRequestTypeDef = TypedDict(
     "_RequiredListArtifactsRequestRequestTypeDef",
     {
         "arn": str,
         "type": ArtifactCategoryType,
     },
 )
@@ -901,54 +868,23 @@
 
 class ListArtifactsRequestRequestTypeDef(
     _RequiredListArtifactsRequestRequestTypeDef, _OptionalListArtifactsRequestRequestTypeDef
 ):
     pass
 
 
-ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef = TypedDict(
-    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDeviceInstancesRequestRequestTypeDef = TypedDict(
     "ListDeviceInstancesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
-    "_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
-    "_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
-    {
-        "type": DevicePoolTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDevicePoolsRequestListDevicePoolsPaginateTypeDef(
-    _RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
-    _OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDevicePoolsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevicePoolsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListDevicePoolsRequestRequestTypeDef = TypedDict(
@@ -963,52 +899,23 @@
 
 class ListDevicePoolsRequestRequestTypeDef(
     _RequiredListDevicePoolsRequestRequestTypeDef, _OptionalListDevicePoolsRequestRequestTypeDef
 ):
     pass
 
 
-ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
-    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInstanceProfilesRequestRequestTypeDef = TypedDict(
     "ListInstanceProfilesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "_RequiredListJobsRequestListJobsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "_OptionalListJobsRequestListJobsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListJobsRequestListJobsPaginateTypeDef(
-    _RequiredListJobsRequestListJobsPaginateTypeDef, _OptionalListJobsRequestListJobsPaginateTypeDef
-):
-    pass
-
-
 _RequiredListJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListJobsRequestRequestTypeDef = TypedDict(
@@ -1022,37 +929,14 @@
 
 class ListJobsRequestRequestTypeDef(
     _RequiredListJobsRequestRequestTypeDef, _OptionalListJobsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
-    "_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
-    "_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
-    {
-        "type": NetworkProfileTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef(
-    _RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
-    _OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListNetworkProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListNetworkProfilesRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListNetworkProfilesRequestRequestTypeDef = TypedDict(
@@ -1068,22 +952,14 @@
 class ListNetworkProfilesRequestRequestTypeDef(
     _RequiredListNetworkProfilesRequestRequestTypeDef,
     _OptionalListNetworkProfilesRequestRequestTypeDef,
 ):
     pass
 
 
-ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef = TypedDict(
-    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOfferingPromotionsRequestRequestTypeDef = TypedDict(
     "ListOfferingPromotionsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -1093,86 +969,39 @@
     {
         "id": str,
         "description": str,
     },
     total=False,
 )
 
-ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef = TypedDict(
-    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOfferingTransactionsRequestRequestTypeDef = TypedDict(
     "ListOfferingTransactionsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "arn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "arn": str,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
-    "_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
-    "_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef(
-    _RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
-    _OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRemoteAccessSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListRemoteAccessSessionsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListRemoteAccessSessionsRequestRequestTypeDef = TypedDict(
@@ -1187,35 +1016,14 @@
 class ListRemoteAccessSessionsRequestRequestTypeDef(
     _RequiredListRemoteAccessSessionsRequestRequestTypeDef,
     _OptionalListRemoteAccessSessionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListRunsRequestListRunsPaginateTypeDef = TypedDict(
-    "_RequiredListRunsRequestListRunsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListRunsRequestListRunsPaginateTypeDef = TypedDict(
-    "_OptionalListRunsRequestListRunsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRunsRequestListRunsPaginateTypeDef(
-    _RequiredListRunsRequestListRunsPaginateTypeDef, _OptionalListRunsRequestListRunsPaginateTypeDef
-):
-    pass
-
-
 _RequiredListRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListRunsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListRunsRequestRequestTypeDef = TypedDict(
@@ -1229,36 +1037,14 @@
 
 class ListRunsRequestRequestTypeDef(
     _RequiredListRunsRequestRequestTypeDef, _OptionalListRunsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
-    "_RequiredListSamplesRequestListSamplesPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
-    "_OptionalListSamplesRequestListSamplesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSamplesRequestListSamplesPaginateTypeDef(
-    _RequiredListSamplesRequestListSamplesPaginateTypeDef,
-    _OptionalListSamplesRequestListSamplesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSamplesRequestRequestTypeDef = TypedDict(
     "_RequiredListSamplesRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListSamplesRequestRequestTypeDef = TypedDict(
@@ -1282,36 +1068,14 @@
         "arn": str,
         "type": SampleTypeType,
         "url": str,
     },
     total=False,
 )
 
-_RequiredListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
-    "_RequiredListSuitesRequestListSuitesPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
-    "_OptionalListSuitesRequestListSuitesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSuitesRequestListSuitesPaginateTypeDef(
-    _RequiredListSuitesRequestListSuitesPaginateTypeDef,
-    _OptionalListSuitesRequestListSuitesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSuitesRequestRequestTypeDef = TypedDict(
     "_RequiredListSuitesRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListSuitesRequestRequestTypeDef = TypedDict(
@@ -1332,16 +1096,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 ListTestGridProjectsRequestRequestTypeDef = TypedDict(
@@ -1446,36 +1210,14 @@
 class ListTestGridSessionsRequestRequestTypeDef(
     _RequiredListTestGridSessionsRequestRequestTypeDef,
     _OptionalListTestGridSessionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListTestsRequestListTestsPaginateTypeDef = TypedDict(
-    "_RequiredListTestsRequestListTestsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListTestsRequestListTestsPaginateTypeDef = TypedDict(
-    "_OptionalListTestsRequestListTestsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTestsRequestListTestsPaginateTypeDef(
-    _RequiredListTestsRequestListTestsPaginateTypeDef,
-    _OptionalListTestsRequestListTestsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTestsRequestRequestTypeDef = TypedDict(
     "_RequiredListTestsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListTestsRequestRequestTypeDef = TypedDict(
@@ -1489,36 +1231,14 @@
 
 class ListTestsRequestRequestTypeDef(
     _RequiredListTestsRequestRequestTypeDef, _OptionalListTestsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
-    "_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
-    "_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef(
-    _RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
-    _OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUniqueProblemsRequestRequestTypeDef = TypedDict(
     "_RequiredListUniqueProblemsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListUniqueProblemsRequestRequestTypeDef = TypedDict(
@@ -1533,37 +1253,14 @@
 class ListUniqueProblemsRequestRequestTypeDef(
     _RequiredListUniqueProblemsRequestRequestTypeDef,
     _OptionalListUniqueProblemsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListUploadsRequestListUploadsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListUploadsRequestListUploadsPaginateTypeDef",
-    {
-        "type": UploadTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUploadsRequestListUploadsPaginateTypeDef(
-    _RequiredListUploadsRequestListUploadsPaginateTypeDef,
-    _OptionalListUploadsRequestListUploadsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUploadsRequestRequestTypeDef = TypedDict(
     "_RequiredListUploadsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListUploadsRequestRequestTypeDef = TypedDict(
@@ -1578,39 +1275,23 @@
 
 class ListUploadsRequestRequestTypeDef(
     _RequiredListUploadsRequestRequestTypeDef, _OptionalListUploadsRequestRequestTypeDef
 ):
     pass
 
 
-ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef = TypedDict(
-    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVPCEConfigurationsRequestRequestTypeDef = TypedDict(
     "ListVPCEConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-LocationOutputTypeDef = TypedDict(
-    "LocationOutputTypeDef",
-    {
-        "latitude": float,
-        "longitude": float,
-    },
-)
-
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "latitude": float,
         "longitude": float,
     },
 )
@@ -1620,24 +1301,14 @@
     {
         "amount": float,
         "currencyCode": Literal["USD"],
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
 ProblemDetailTypeDef = TypedDict(
     "ProblemDetailTypeDef",
     {
         "arn": str,
         "name": str,
     },
     total=False,
@@ -1670,25 +1341,14 @@
 
 class PurchaseOfferingRequestRequestTypeDef(
     _RequiredPurchaseOfferingRequestRequestTypeDef, _OptionalPurchaseOfferingRequestRequestTypeDef
 ):
     pass
 
 
-RadiosOutputTypeDef = TypedDict(
-    "RadiosOutputTypeDef",
-    {
-        "wifi": bool,
-        "bluetooth": bool,
-        "nfc": bool,
-        "gps": bool,
-    },
-    total=False,
-)
-
 RadiosTypeDef = TypedDict(
     "RadiosTypeDef",
     {
         "wifi": bool,
         "bluetooth": bool,
         "nfc": bool,
         "gps": bool,
@@ -1700,25 +1360,14 @@
     "RenewOfferingRequestRequestTypeDef",
     {
         "offeringId": str,
         "quantity": int,
     },
 )
 
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
 StopJobRequestRequestTypeDef = TypedDict(
     "StopJobRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -1732,22 +1381,14 @@
 StopRunRequestRequestTypeDef = TypedDict(
     "StopRunRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 TestGridVpcConfigOutputTypeDef = TypedDict(
     "TestGridVpcConfigOutputTypeDef",
     {
         "securityGroupIds": List[str],
         "subnetIds": List[str],
         "vpcId": str,
     },
@@ -1901,23 +1542,14 @@
         "maxSlots": Dict[str, int],
         "defaultJobTimeoutMinutes": int,
         "skipAppResign": bool,
     },
     total=False,
 )
 
-ListArtifactsResultTypeDef = TypedDict(
-    "ListArtifactsResultTypeDef",
-    {
-        "artifacts": List[ArtifactTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateDevicePoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevicePoolRequestRequestTypeDef",
     {
         "projectArn": str,
         "name": str,
         "rules": Sequence[RuleTypeDef],
     },
@@ -1934,14 +1566,27 @@
 
 class CreateDevicePoolRequestRequestTypeDef(
     _RequiredCreateDevicePoolRequestRequestTypeDef, _OptionalCreateDevicePoolRequestRequestTypeDef
 ):
     pass
 
 
+DevicePoolTypeDef = TypedDict(
+    "DevicePoolTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "description": str,
+        "type": DevicePoolTypeType,
+        "rules": List[RuleTypeDef],
+        "maxDevices": int,
+    },
+    total=False,
+)
+
 _RequiredUpdateDevicePoolRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDevicePoolRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateDevicePoolRequestRequestTypeDef = TypedDict(
@@ -1959,19 +1604,37 @@
 
 class UpdateDevicePoolRequestRequestTypeDef(
     _RequiredUpdateDevicePoolRequestRequestTypeDef, _OptionalUpdateDevicePoolRequestRequestTypeDef
 ):
     pass
 
 
+CreateTestGridUrlResultTypeDef = TypedDict(
+    "CreateTestGridUrlResultTypeDef",
+    {
+        "url": str,
+        "expires": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListArtifactsResultTypeDef = TypedDict(
+    "ListArtifactsResultTypeDef",
+    {
+        "artifacts": List[ArtifactTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateInstanceProfileResultTypeDef = TypedDict(
     "CreateInstanceProfileResultTypeDef",
     {
         "instanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceInstanceTypeDef = TypedDict(
     "DeviceInstanceTypeDef",
     {
         "arn": str,
@@ -1984,65 +1647,65 @@
     total=False,
 )
 
 GetInstanceProfileResultTypeDef = TypedDict(
     "GetInstanceProfileResultTypeDef",
     {
         "instanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInstanceProfilesResultTypeDef = TypedDict(
     "ListInstanceProfilesResultTypeDef",
     {
         "instanceProfiles": List[InstanceProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInstanceProfileResultTypeDef = TypedDict(
     "UpdateInstanceProfileResultTypeDef",
     {
         "instanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateNetworkProfileResultTypeDef = TypedDict(
     "CreateNetworkProfileResultTypeDef",
     {
         "networkProfile": NetworkProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkProfileResultTypeDef = TypedDict(
     "GetNetworkProfileResultTypeDef",
     {
         "networkProfile": NetworkProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNetworkProfilesResultTypeDef = TypedDict(
     "ListNetworkProfilesResultTypeDef",
     {
         "networkProfiles": List[NetworkProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNetworkProfileResultTypeDef = TypedDict(
     "UpdateNetworkProfileResultTypeDef",
     {
         "networkProfile": NetworkProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "name": str,
@@ -2166,81 +1829,81 @@
     pass
 
 
 CreateUploadResultTypeDef = TypedDict(
     "CreateUploadResultTypeDef",
     {
         "upload": UploadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUploadResultTypeDef = TypedDict(
     "GetUploadResultTypeDef",
     {
         "upload": UploadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstallToRemoteAccessSessionResultTypeDef = TypedDict(
     "InstallToRemoteAccessSessionResultTypeDef",
     {
         "appUpload": UploadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUploadsResultTypeDef = TypedDict(
     "ListUploadsResultTypeDef",
     {
         "uploads": List[UploadTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUploadResultTypeDef = TypedDict(
     "UpdateUploadResultTypeDef",
     {
         "upload": UploadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVPCEConfigurationResultTypeDef = TypedDict(
     "CreateVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVPCEConfigurationResultTypeDef = TypedDict(
     "GetVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVPCEConfigurationsResultTypeDef = TypedDict(
     "ListVPCEConfigurationsResultTypeDef",
     {
         "vpceConfigurations": List[VPCEConfigurationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVPCEConfigurationResultTypeDef = TypedDict(
     "UpdateVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceSelectionResultTypeDef = TypedDict(
     "DeviceSelectionResultTypeDef",
     {
         "filters": List[DeviceFilterOutputTypeDef],
@@ -2254,24 +1917,14 @@
     "DeviceSelectionConfigurationTypeDef",
     {
         "filters": Sequence[DeviceFilterTypeDef],
         "maxDevices": int,
     },
 )
 
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    {
-        "arn": str,
-        "filters": Sequence[DeviceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDevicesRequestRequestTypeDef = TypedDict(
     "ListDevicesRequestRequestTypeDef",
     {
         "arn": str,
         "nextToken": str,
         "filters": Sequence[DeviceFilterTypeDef],
     },
@@ -2310,85 +1963,399 @@
         "counters": CountersTypeDef,
         "message": str,
         "deviceMinutes": DeviceMinutesTypeDef,
     },
     total=False,
 )
 
-DevicePoolTypeDef = TypedDict(
-    "DevicePoolTypeDef",
+GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef = TypedDict(
+    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
+    "_RequiredListArtifactsRequestListArtifactsPaginateTypeDef",
     {
         "arn": str,
-        "name": str,
-        "description": str,
+        "type": ArtifactCategoryType,
+    },
+)
+_OptionalListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
+    "_OptionalListArtifactsRequestListArtifactsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListArtifactsRequestListArtifactsPaginateTypeDef(
+    _RequiredListArtifactsRequestListArtifactsPaginateTypeDef,
+    _OptionalListArtifactsRequestListArtifactsPaginateTypeDef,
+):
+    pass
+
+
+ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef = TypedDict(
+    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
+    "_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
+    "_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
+    {
         "type": DevicePoolTypeType,
-        "rules": List[RuleOutputTypeDef],
-        "maxDevices": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDevicePoolsRequestListDevicePoolsPaginateTypeDef(
+    _RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
+    _OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
+):
+    pass
+
+
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "arn": str,
+        "filters": Sequence[DeviceFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
+    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "_RequiredListJobsRequestListJobsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "_OptionalListJobsRequestListJobsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListJobsRequestListJobsPaginateTypeDef(
+    _RequiredListJobsRequestListJobsPaginateTypeDef, _OptionalListJobsRequestListJobsPaginateTypeDef
+):
+    pass
+
+
+_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
+    "_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
+    "_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
+    {
+        "type": NetworkProfileTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef(
+    _RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
+    _OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
+):
+    pass
+
+
+ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef = TypedDict(
+    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef = TypedDict(
+    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "arn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef(
+    _RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
+    _OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRunsRequestListRunsPaginateTypeDef = TypedDict(
+    "_RequiredListRunsRequestListRunsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListRunsRequestListRunsPaginateTypeDef = TypedDict(
+    "_OptionalListRunsRequestListRunsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRunsRequestListRunsPaginateTypeDef(
+    _RequiredListRunsRequestListRunsPaginateTypeDef, _OptionalListRunsRequestListRunsPaginateTypeDef
+):
+    pass
+
+
+_RequiredListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
+    "_RequiredListSamplesRequestListSamplesPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
+    "_OptionalListSamplesRequestListSamplesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSamplesRequestListSamplesPaginateTypeDef(
+    _RequiredListSamplesRequestListSamplesPaginateTypeDef,
+    _OptionalListSamplesRequestListSamplesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
+    "_RequiredListSuitesRequestListSuitesPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
+    "_OptionalListSuitesRequestListSuitesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSuitesRequestListSuitesPaginateTypeDef(
+    _RequiredListSuitesRequestListSuitesPaginateTypeDef,
+    _OptionalListSuitesRequestListSuitesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTestsRequestListTestsPaginateTypeDef = TypedDict(
+    "_RequiredListTestsRequestListTestsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListTestsRequestListTestsPaginateTypeDef = TypedDict(
+    "_OptionalListTestsRequestListTestsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTestsRequestListTestsPaginateTypeDef(
+    _RequiredListTestsRequestListTestsPaginateTypeDef,
+    _OptionalListTestsRequestListTestsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
+    "_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
+    "_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef(
+    _RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
+    _OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListUploadsRequestListUploadsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListUploadsRequestListUploadsPaginateTypeDef",
+    {
+        "type": UploadTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUploadsRequestListUploadsPaginateTypeDef(
+    _RequiredListUploadsRequestListUploadsPaginateTypeDef,
+    _OptionalListUploadsRequestListUploadsPaginateTypeDef,
+):
+    pass
+
+
+ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef = TypedDict(
+    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetTestGridSessionResultTypeDef = TypedDict(
     "GetTestGridSessionResultTypeDef",
     {
         "testGridSession": TestGridSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTestGridSessionsResultTypeDef = TypedDict(
     "ListTestGridSessionsResultTypeDef",
     {
         "testGridSessions": List[TestGridSessionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOfferingPromotionsResultTypeDef = TypedDict(
     "ListOfferingPromotionsResultTypeDef",
     {
         "offeringPromotions": List[OfferingPromotionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSamplesResultTypeDef = TypedDict(
     "ListSamplesResultTypeDef",
     {
         "samples": List[SampleTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 ListTestGridSessionActionsResultTypeDef = TypedDict(
     "ListTestGridSessionActionsResultTypeDef",
     {
         "actions": List[TestGridSessionActionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTestGridSessionArtifactsResultTypeDef = TypedDict(
     "ListTestGridSessionArtifactsResultTypeDef",
     {
         "artifacts": List[TestGridSessionArtifactTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "cost": MonetaryAmountTypeDef,
@@ -2421,22 +2388,14 @@
         "radios": RadiosTypeDef,
         "auxiliaryApps": Sequence[str],
         "billingMethod": BillingMethodType,
     },
     total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
 TestGridProjectTypeDef = TypedDict(
     "TestGridProjectTypeDef",
     {
         "arn": str,
         "name": str,
         "description": str,
         "vpcConfig": TestGridVpcConfigOutputTypeDef,
@@ -2445,15 +2404,48 @@
     total=False,
 )
 
 GetAccountSettingsResultTypeDef = TypedDict(
     "GetAccountSettingsResultTypeDef",
     {
         "accountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDevicePoolResultTypeDef = TypedDict(
+    "CreateDevicePoolResultTypeDef",
+    {
+        "devicePool": DevicePoolTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDevicePoolResultTypeDef = TypedDict(
+    "GetDevicePoolResultTypeDef",
+    {
+        "devicePool": DevicePoolTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDevicePoolsResultTypeDef = TypedDict(
+    "ListDevicePoolsResultTypeDef",
+    {
+        "devicePools": List[DevicePoolTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDevicePoolResultTypeDef = TypedDict(
+    "UpdateDevicePoolResultTypeDef",
+    {
+        "devicePool": DevicePoolTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
         "arn": str,
@@ -2481,32 +2473,32 @@
     total=False,
 )
 
 GetDeviceInstanceResultTypeDef = TypedDict(
     "GetDeviceInstanceResultTypeDef",
     {
         "deviceInstance": DeviceInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeviceInstancesResultTypeDef = TypedDict(
     "ListDeviceInstancesResultTypeDef",
     {
         "deviceInstances": List[DeviceInstanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDeviceInstanceResultTypeDef = TypedDict(
     "UpdateDeviceInstanceResultTypeDef",
     {
         "deviceInstance": DeviceInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RunTypeDef = TypedDict(
     "RunTypeDef",
     {
         "arn": str,
@@ -2529,90 +2521,57 @@
         "resultCode": ExecutionResultCodeType,
         "seed": int,
         "appUpload": str,
         "eventCount": int,
         "jobTimeoutMinutes": int,
         "devicePoolArn": str,
         "locale": str,
-        "radios": RadiosOutputTypeDef,
-        "location": LocationOutputTypeDef,
+        "radios": RadiosTypeDef,
+        "location": LocationTypeDef,
         "customerArtifactPaths": CustomerArtifactPathsOutputTypeDef,
         "webUrl": str,
         "skipAppResign": bool,
         "testSpecArn": str,
         "deviceSelectionResult": DeviceSelectionResultTypeDef,
         "vpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
 
 GetSuiteResultTypeDef = TypedDict(
     "GetSuiteResultTypeDef",
     {
         "suite": SuiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSuitesResultTypeDef = TypedDict(
     "ListSuitesResultTypeDef",
     {
         "suites": List[SuiteTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTestResultTypeDef = TypedDict(
     "GetTestResultTypeDef",
     {
         "test": TestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTestsResultTypeDef = TypedDict(
     "ListTestsResultTypeDef",
     {
         "tests": List[TestTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDevicePoolResultTypeDef = TypedDict(
-    "CreateDevicePoolResultTypeDef",
-    {
-        "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDevicePoolResultTypeDef = TypedDict(
-    "GetDevicePoolResultTypeDef",
-    {
-        "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDevicePoolsResultTypeDef = TypedDict(
-    "ListDevicePoolsResultTypeDef",
-    {
-        "devicePools": List[DevicePoolTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDevicePoolResultTypeDef = TypedDict(
-    "UpdateDevicePoolResultTypeDef",
-    {
-        "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "id": str,
@@ -2624,40 +2583,40 @@
     total=False,
 )
 
 CreateProjectResultTypeDef = TypedDict(
     "CreateProjectResultTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProjectResultTypeDef = TypedDict(
     "GetProjectResultTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProjectsResultTypeDef = TypedDict(
     "ListProjectsResultTypeDef",
     {
         "projects": List[ProjectTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProjectResultTypeDef = TypedDict(
     "UpdateProjectResultTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetDevicePoolCompatibilityRequestRequestTypeDef = TypedDict(
     "_RequiredGetDevicePoolCompatibilityRequestRequestTypeDef",
     {
         "devicePoolArn": str,
@@ -2709,40 +2668,40 @@
     pass
 
 
 CreateTestGridProjectResultTypeDef = TypedDict(
     "CreateTestGridProjectResultTypeDef",
     {
         "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTestGridProjectResultTypeDef = TypedDict(
     "GetTestGridProjectResultTypeDef",
     {
         "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTestGridProjectsResultTypeDef = TypedDict(
     "ListTestGridProjectsResultTypeDef",
     {
         "testGridProjects": List[TestGridProjectTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTestGridProjectResultTypeDef = TypedDict(
     "UpdateTestGridProjectResultTypeDef",
     {
         "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DevicePoolCompatibilityResultTypeDef = TypedDict(
     "DevicePoolCompatibilityResultTypeDef",
     {
         "device": DeviceTypeDef,
@@ -2752,15 +2711,15 @@
     total=False,
 )
 
 GetDeviceResultTypeDef = TypedDict(
     "GetDeviceResultTypeDef",
     {
         "device": DeviceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "arn": str,
@@ -2783,15 +2742,15 @@
 )
 
 ListDevicesResultTypeDef = TypedDict(
     "ListDevicesResultTypeDef",
     {
         "devices": List[DeviceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProblemTypeDef = TypedDict(
     "ProblemTypeDef",
     {
         "run": ProblemDetailTypeDef,
@@ -2834,49 +2793,49 @@
     total=False,
 )
 
 GetRunResultTypeDef = TypedDict(
     "GetRunResultTypeDef",
     {
         "run": RunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRunsResultTypeDef = TypedDict(
     "ListRunsResultTypeDef",
     {
         "runs": List[RunTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScheduleRunResultTypeDef = TypedDict(
     "ScheduleRunResultTypeDef",
     {
         "run": RunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopRunResultTypeDef = TypedDict(
     "StopRunResultTypeDef",
     {
         "run": RunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOfferingsResultTypeDef = TypedDict(
     "ListOfferingsResultTypeDef",
     {
         "offerings": List[OfferingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OfferingStatusTypeDef = TypedDict(
     "OfferingStatusTypeDef",
     {
         "type": OfferingTransactionTypeType,
@@ -2888,40 +2847,40 @@
 )
 
 GetDevicePoolCompatibilityResultTypeDef = TypedDict(
     "GetDevicePoolCompatibilityResultTypeDef",
     {
         "compatibleDevices": List[DevicePoolCompatibilityResultTypeDef],
         "incompatibleDevices": List[DevicePoolCompatibilityResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobResultTypeDef = TypedDict(
     "GetJobResultTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "jobs": List[JobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopJobResultTypeDef = TypedDict(
     "StopJobResultTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UniqueProblemTypeDef = TypedDict(
     "UniqueProblemTypeDef",
     {
         "message": str,
@@ -2930,50 +2889,50 @@
     total=False,
 )
 
 CreateRemoteAccessSessionResultTypeDef = TypedDict(
     "CreateRemoteAccessSessionResultTypeDef",
     {
         "remoteAccessSession": RemoteAccessSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRemoteAccessSessionResultTypeDef = TypedDict(
     "GetRemoteAccessSessionResultTypeDef",
     {
         "remoteAccessSession": RemoteAccessSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRemoteAccessSessionsResultTypeDef = TypedDict(
     "ListRemoteAccessSessionsResultTypeDef",
     {
         "remoteAccessSessions": List[RemoteAccessSessionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopRemoteAccessSessionResultTypeDef = TypedDict(
     "StopRemoteAccessSessionResultTypeDef",
     {
         "remoteAccessSession": RemoteAccessSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOfferingStatusResultTypeDef = TypedDict(
     "GetOfferingStatusResultTypeDef",
     {
         "current": Dict[str, OfferingStatusTypeDef],
         "nextPeriod": Dict[str, OfferingStatusTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OfferingTransactionTypeDef = TypedDict(
     "OfferingTransactionTypeDef",
     {
         "offeringStatus": OfferingStatusTypeDef,
@@ -2986,35 +2945,35 @@
 )
 
 ListUniqueProblemsResultTypeDef = TypedDict(
     "ListUniqueProblemsResultTypeDef",
     {
         "uniqueProblems": Dict[ExecutionResultType, List[UniqueProblemTypeDef]],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOfferingTransactionsResultTypeDef = TypedDict(
     "ListOfferingTransactionsResultTypeDef",
     {
         "offeringTransactions": List[OfferingTransactionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PurchaseOfferingResultTypeDef = TypedDict(
     "PurchaseOfferingResultTypeDef",
     {
         "offeringTransaction": OfferingTransactionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RenewOfferingResultTypeDef = TypedDict(
     "RenewOfferingResultTypeDef",
     {
         "offeringTransaction": OfferingTransactionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/type_defs.pyi` & `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -54,23 +54,23 @@
 
 __all__ = (
     "TrialMinutesTypeDef",
     "ArtifactTypeDef",
     "CPUTypeDef",
     "CountersTypeDef",
     "RuleTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateInstanceProfileRequestRequestTypeDef",
     "InstanceProfileTypeDef",
     "CreateNetworkProfileRequestRequestTypeDef",
     "NetworkProfileTypeDef",
     "VpcConfigTypeDef",
     "CreateRemoteAccessSessionConfigurationTypeDef",
     "TestGridVpcConfigTypeDef",
     "CreateTestGridUrlRequestRequestTypeDef",
-    "CreateTestGridUrlResultTypeDef",
     "CreateUploadRequestRequestTypeDef",
     "UploadTypeDef",
     "CreateVPCEConfigurationRequestRequestTypeDef",
     "VPCEConfigurationTypeDef",
     "CustomerArtifactPathsOutputTypeDef",
     "CustomerArtifactPathsTypeDef",
     "DeleteDevicePoolRequestRequestTypeDef",
@@ -82,109 +82,87 @@
     "DeleteTestGridProjectRequestRequestTypeDef",
     "DeleteUploadRequestRequestTypeDef",
     "DeleteVPCEConfigurationRequestRequestTypeDef",
     "DeviceFilterOutputTypeDef",
     "DeviceFilterTypeDef",
     "DeviceMinutesTypeDef",
     "IncompatibilityMessageTypeDef",
-    "RuleOutputTypeDef",
     "ResolutionTypeDef",
     "ExecutionConfigurationTypeDef",
     "GetDeviceInstanceRequestRequestTypeDef",
     "ScheduleRunTestTypeDef",
     "GetDevicePoolRequestRequestTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetInstanceProfileRequestRequestTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetNetworkProfileRequestRequestTypeDef",
-    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetOfferingStatusRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetRemoteAccessSessionRequestRequestTypeDef",
     "GetRunRequestRequestTypeDef",
     "GetSuiteRequestRequestTypeDef",
     "GetTestGridProjectRequestRequestTypeDef",
     "GetTestGridSessionRequestRequestTypeDef",
     "TestGridSessionTypeDef",
     "GetTestRequestRequestTypeDef",
     "GetUploadRequestRequestTypeDef",
     "GetVPCEConfigurationRequestRequestTypeDef",
     "InstallToRemoteAccessSessionRequestRequestTypeDef",
-    "ListArtifactsRequestListArtifactsPaginateTypeDef",
     "ListArtifactsRequestRequestTypeDef",
-    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
     "ListDeviceInstancesRequestRequestTypeDef",
-    "ListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
     "ListDevicePoolsRequestRequestTypeDef",
-    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     "ListInstanceProfilesRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
     "ListNetworkProfilesRequestRequestTypeDef",
-    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
     "ListOfferingPromotionsRequestRequestTypeDef",
     "OfferingPromotionTypeDef",
-    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
     "ListOfferingTransactionsRequestRequestTypeDef",
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListOfferingsRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
-    "ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
     "ListRemoteAccessSessionsRequestRequestTypeDef",
-    "ListRunsRequestListRunsPaginateTypeDef",
     "ListRunsRequestRequestTypeDef",
-    "ListSamplesRequestListSamplesPaginateTypeDef",
     "ListSamplesRequestRequestTypeDef",
     "SampleTypeDef",
-    "ListSuitesRequestListSuitesPaginateTypeDef",
     "ListSuitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "ListTestGridProjectsRequestRequestTypeDef",
     "ListTestGridSessionActionsRequestRequestTypeDef",
     "TestGridSessionActionTypeDef",
     "ListTestGridSessionArtifactsRequestRequestTypeDef",
     "TestGridSessionArtifactTypeDef",
     "ListTestGridSessionsRequestRequestTypeDef",
-    "ListTestsRequestListTestsPaginateTypeDef",
     "ListTestsRequestRequestTypeDef",
-    "ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
     "ListUniqueProblemsRequestRequestTypeDef",
-    "ListUploadsRequestListUploadsPaginateTypeDef",
     "ListUploadsRequestRequestTypeDef",
-    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
     "ListVPCEConfigurationsRequestRequestTypeDef",
-    "LocationOutputTypeDef",
     "LocationTypeDef",
     "MonetaryAmountTypeDef",
-    "PaginatorConfigTypeDef",
     "ProblemDetailTypeDef",
     "VpcConfigOutputTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
-    "RadiosOutputTypeDef",
     "RadiosTypeDef",
     "RenewOfferingRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StopJobRequestRequestTypeDef",
     "StopRemoteAccessSessionRequestRequestTypeDef",
     "StopRunRequestRequestTypeDef",
-    "TagTypeDef",
     "TestGridVpcConfigOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceInstanceRequestRequestTypeDef",
     "UpdateInstanceProfileRequestRequestTypeDef",
     "UpdateNetworkProfileRequestRequestTypeDef",
     "UpdateUploadRequestRequestTypeDef",
     "UpdateVPCEConfigurationRequestRequestTypeDef",
     "AccountSettingsTypeDef",
-    "ListArtifactsResultTypeDef",
     "CreateDevicePoolRequestRequestTypeDef",
+    "DevicePoolTypeDef",
     "UpdateDevicePoolRequestRequestTypeDef",
+    "CreateTestGridUrlResultTypeDef",
+    "ListArtifactsResultTypeDef",
     "CreateInstanceProfileResultTypeDef",
     "DeviceInstanceTypeDef",
     "GetInstanceProfileResultTypeDef",
     "ListInstanceProfilesResultTypeDef",
     "UpdateInstanceProfileResultTypeDef",
     "CreateNetworkProfileResultTypeDef",
     "GetNetworkProfileResultTypeDef",
@@ -202,45 +180,63 @@
     "UpdateUploadResultTypeDef",
     "CreateVPCEConfigurationResultTypeDef",
     "GetVPCEConfigurationResultTypeDef",
     "ListVPCEConfigurationsResultTypeDef",
     "UpdateVPCEConfigurationResultTypeDef",
     "DeviceSelectionResultTypeDef",
     "DeviceSelectionConfigurationTypeDef",
-    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "SuiteTypeDef",
     "TestTypeDef",
-    "DevicePoolTypeDef",
+    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
+    "ListArtifactsRequestListArtifactsPaginateTypeDef",
+    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
+    "ListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
+    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
+    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
+    "ListRunsRequestListRunsPaginateTypeDef",
+    "ListSamplesRequestListSamplesPaginateTypeDef",
+    "ListSuitesRequestListSuitesPaginateTypeDef",
+    "ListTestsRequestListTestsPaginateTypeDef",
+    "ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
+    "ListUploadsRequestListUploadsPaginateTypeDef",
+    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
     "GetTestGridSessionResultTypeDef",
     "ListTestGridSessionsResultTypeDef",
     "ListOfferingPromotionsResultTypeDef",
     "ListSamplesResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ListTestGridSessionActionsResultTypeDef",
     "ListTestGridSessionArtifactsResultTypeDef",
     "RecurringChargeTypeDef",
     "ProjectTypeDef",
     "ScheduleRunConfigurationTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "TestGridProjectTypeDef",
     "GetAccountSettingsResultTypeDef",
+    "CreateDevicePoolResultTypeDef",
+    "GetDevicePoolResultTypeDef",
+    "ListDevicePoolsResultTypeDef",
+    "UpdateDevicePoolResultTypeDef",
     "DeviceTypeDef",
     "GetDeviceInstanceResultTypeDef",
     "ListDeviceInstancesResultTypeDef",
     "UpdateDeviceInstanceResultTypeDef",
     "RunTypeDef",
     "GetSuiteResultTypeDef",
     "ListSuitesResultTypeDef",
     "GetTestResultTypeDef",
     "ListTestsResultTypeDef",
-    "CreateDevicePoolResultTypeDef",
-    "GetDevicePoolResultTypeDef",
-    "ListDevicePoolsResultTypeDef",
-    "UpdateDevicePoolResultTypeDef",
     "OfferingTypeDef",
     "CreateProjectResultTypeDef",
     "GetProjectResultTypeDef",
     "ListProjectsResultTypeDef",
     "UpdateProjectResultTypeDef",
     "GetDevicePoolCompatibilityRequestRequestTypeDef",
     "ScheduleRunRequestRequestTypeDef",
@@ -328,14 +324,25 @@
         "attribute": DeviceAttributeType,
         "operator": RuleOperatorType,
         "value": str,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredCreateInstanceProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInstanceProfileRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateInstanceProfileRequestRequestTypeDef = TypedDict(
@@ -448,23 +455,14 @@
     "CreateTestGridUrlRequestRequestTypeDef",
     {
         "projectArn": str,
         "expiresInSeconds": int,
     },
 )
 
-CreateTestGridUrlResultTypeDef = TypedDict(
-    "CreateTestGridUrlResultTypeDef",
-    {
-        "url": str,
-        "expires": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUploadRequestRequestTypeDef",
     {
         "projectArn": str,
         "name": str,
         "type": UploadTypeType,
     },
@@ -649,24 +647,14 @@
     {
         "message": str,
         "type": DeviceAttributeType,
     },
     total=False,
 )
 
-RuleOutputTypeDef = TypedDict(
-    "RuleOutputTypeDef",
-    {
-        "attribute": DeviceAttributeType,
-        "operator": RuleOperatorType,
-        "value": str,
-    },
-    total=False,
-)
-
 ResolutionTypeDef = TypedDict(
     "ResolutionTypeDef",
     {
         "width": int,
         "height": int,
     },
     total=False,
@@ -742,18 +730,20 @@
 GetNetworkProfileRequestRequestTypeDef = TypedDict(
     "GetNetworkProfileRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef = TypedDict(
-    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetOfferingStatusRequestRequestTypeDef = TypedDict(
     "GetOfferingStatusRequestRequestTypeDef",
     {
@@ -845,35 +835,14 @@
     "InstallToRemoteAccessSessionRequestRequestTypeDef",
     {
         "remoteAccessSessionArn": str,
         "appArn": str,
     },
 )
 
-_RequiredListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
-    "_RequiredListArtifactsRequestListArtifactsPaginateTypeDef",
-    {
-        "arn": str,
-        "type": ArtifactCategoryType,
-    },
-)
-_OptionalListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
-    "_OptionalListArtifactsRequestListArtifactsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListArtifactsRequestListArtifactsPaginateTypeDef(
-    _RequiredListArtifactsRequestListArtifactsPaginateTypeDef,
-    _OptionalListArtifactsRequestListArtifactsPaginateTypeDef,
-):
-    pass
-
 _RequiredListArtifactsRequestRequestTypeDef = TypedDict(
     "_RequiredListArtifactsRequestRequestTypeDef",
     {
         "arn": str,
         "type": ArtifactCategoryType,
     },
 )
@@ -886,52 +855,23 @@
 )
 
 class ListArtifactsRequestRequestTypeDef(
     _RequiredListArtifactsRequestRequestTypeDef, _OptionalListArtifactsRequestRequestTypeDef
 ):
     pass
 
-ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef = TypedDict(
-    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDeviceInstancesRequestRequestTypeDef = TypedDict(
     "ListDeviceInstancesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
-    "_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
-    "_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
-    {
-        "type": DevicePoolTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDevicePoolsRequestListDevicePoolsPaginateTypeDef(
-    _RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
-    _OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDevicePoolsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevicePoolsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListDevicePoolsRequestRequestTypeDef = TypedDict(
@@ -944,50 +884,23 @@
 )
 
 class ListDevicePoolsRequestRequestTypeDef(
     _RequiredListDevicePoolsRequestRequestTypeDef, _OptionalListDevicePoolsRequestRequestTypeDef
 ):
     pass
 
-ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
-    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInstanceProfilesRequestRequestTypeDef = TypedDict(
     "ListInstanceProfilesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "_RequiredListJobsRequestListJobsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "_OptionalListJobsRequestListJobsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListJobsRequestListJobsPaginateTypeDef(
-    _RequiredListJobsRequestListJobsPaginateTypeDef, _OptionalListJobsRequestListJobsPaginateTypeDef
-):
-    pass
-
 _RequiredListJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListJobsRequestRequestTypeDef = TypedDict(
@@ -999,35 +912,14 @@
 )
 
 class ListJobsRequestRequestTypeDef(
     _RequiredListJobsRequestRequestTypeDef, _OptionalListJobsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
-    "_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
-    "_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
-    {
-        "type": NetworkProfileTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef(
-    _RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
-    _OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
-):
-    pass
-
 _RequiredListNetworkProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListNetworkProfilesRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListNetworkProfilesRequestRequestTypeDef = TypedDict(
@@ -1041,22 +933,14 @@
 
 class ListNetworkProfilesRequestRequestTypeDef(
     _RequiredListNetworkProfilesRequestRequestTypeDef,
     _OptionalListNetworkProfilesRequestRequestTypeDef,
 ):
     pass
 
-ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef = TypedDict(
-    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOfferingPromotionsRequestRequestTypeDef = TypedDict(
     "ListOfferingPromotionsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -1066,84 +950,39 @@
     {
         "id": str,
         "description": str,
     },
     total=False,
 )
 
-ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef = TypedDict(
-    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOfferingTransactionsRequestRequestTypeDef = TypedDict(
     "ListOfferingTransactionsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "arn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "arn": str,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
-    "_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
-    "_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef(
-    _RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
-    _OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListRemoteAccessSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListRemoteAccessSessionsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListRemoteAccessSessionsRequestRequestTypeDef = TypedDict(
@@ -1156,33 +995,14 @@
 
 class ListRemoteAccessSessionsRequestRequestTypeDef(
     _RequiredListRemoteAccessSessionsRequestRequestTypeDef,
     _OptionalListRemoteAccessSessionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListRunsRequestListRunsPaginateTypeDef = TypedDict(
-    "_RequiredListRunsRequestListRunsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListRunsRequestListRunsPaginateTypeDef = TypedDict(
-    "_OptionalListRunsRequestListRunsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRunsRequestListRunsPaginateTypeDef(
-    _RequiredListRunsRequestListRunsPaginateTypeDef, _OptionalListRunsRequestListRunsPaginateTypeDef
-):
-    pass
-
 _RequiredListRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListRunsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListRunsRequestRequestTypeDef = TypedDict(
@@ -1194,34 +1014,14 @@
 )
 
 class ListRunsRequestRequestTypeDef(
     _RequiredListRunsRequestRequestTypeDef, _OptionalListRunsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
-    "_RequiredListSamplesRequestListSamplesPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
-    "_OptionalListSamplesRequestListSamplesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSamplesRequestListSamplesPaginateTypeDef(
-    _RequiredListSamplesRequestListSamplesPaginateTypeDef,
-    _OptionalListSamplesRequestListSamplesPaginateTypeDef,
-):
-    pass
-
 _RequiredListSamplesRequestRequestTypeDef = TypedDict(
     "_RequiredListSamplesRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListSamplesRequestRequestTypeDef = TypedDict(
@@ -1243,34 +1043,14 @@
         "arn": str,
         "type": SampleTypeType,
         "url": str,
     },
     total=False,
 )
 
-_RequiredListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
-    "_RequiredListSuitesRequestListSuitesPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
-    "_OptionalListSuitesRequestListSuitesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSuitesRequestListSuitesPaginateTypeDef(
-    _RequiredListSuitesRequestListSuitesPaginateTypeDef,
-    _OptionalListSuitesRequestListSuitesPaginateTypeDef,
-):
-    pass
-
 _RequiredListSuitesRequestRequestTypeDef = TypedDict(
     "_RequiredListSuitesRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListSuitesRequestRequestTypeDef = TypedDict(
@@ -1289,16 +1069,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 ListTestGridProjectsRequestRequestTypeDef = TypedDict(
@@ -1397,34 +1177,14 @@
 
 class ListTestGridSessionsRequestRequestTypeDef(
     _RequiredListTestGridSessionsRequestRequestTypeDef,
     _OptionalListTestGridSessionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListTestsRequestListTestsPaginateTypeDef = TypedDict(
-    "_RequiredListTestsRequestListTestsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListTestsRequestListTestsPaginateTypeDef = TypedDict(
-    "_OptionalListTestsRequestListTestsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTestsRequestListTestsPaginateTypeDef(
-    _RequiredListTestsRequestListTestsPaginateTypeDef,
-    _OptionalListTestsRequestListTestsPaginateTypeDef,
-):
-    pass
-
 _RequiredListTestsRequestRequestTypeDef = TypedDict(
     "_RequiredListTestsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListTestsRequestRequestTypeDef = TypedDict(
@@ -1436,34 +1196,14 @@
 )
 
 class ListTestsRequestRequestTypeDef(
     _RequiredListTestsRequestRequestTypeDef, _OptionalListTestsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
-    "_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
-    "_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef(
-    _RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
-    _OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
-):
-    pass
-
 _RequiredListUniqueProblemsRequestRequestTypeDef = TypedDict(
     "_RequiredListUniqueProblemsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListUniqueProblemsRequestRequestTypeDef = TypedDict(
@@ -1476,35 +1216,14 @@
 
 class ListUniqueProblemsRequestRequestTypeDef(
     _RequiredListUniqueProblemsRequestRequestTypeDef,
     _OptionalListUniqueProblemsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListUploadsRequestListUploadsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListUploadsRequestListUploadsPaginateTypeDef",
-    {
-        "type": UploadTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUploadsRequestListUploadsPaginateTypeDef(
-    _RequiredListUploadsRequestListUploadsPaginateTypeDef,
-    _OptionalListUploadsRequestListUploadsPaginateTypeDef,
-):
-    pass
-
 _RequiredListUploadsRequestRequestTypeDef = TypedDict(
     "_RequiredListUploadsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListUploadsRequestRequestTypeDef = TypedDict(
@@ -1517,39 +1236,23 @@
 )
 
 class ListUploadsRequestRequestTypeDef(
     _RequiredListUploadsRequestRequestTypeDef, _OptionalListUploadsRequestRequestTypeDef
 ):
     pass
 
-ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef = TypedDict(
-    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVPCEConfigurationsRequestRequestTypeDef = TypedDict(
     "ListVPCEConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-LocationOutputTypeDef = TypedDict(
-    "LocationOutputTypeDef",
-    {
-        "latitude": float,
-        "longitude": float,
-    },
-)
-
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "latitude": float,
         "longitude": float,
     },
 )
@@ -1559,24 +1262,14 @@
     {
         "amount": float,
         "currencyCode": Literal["USD"],
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
 ProblemDetailTypeDef = TypedDict(
     "ProblemDetailTypeDef",
     {
         "arn": str,
         "name": str,
     },
     total=False,
@@ -1607,25 +1300,14 @@
 )
 
 class PurchaseOfferingRequestRequestTypeDef(
     _RequiredPurchaseOfferingRequestRequestTypeDef, _OptionalPurchaseOfferingRequestRequestTypeDef
 ):
     pass
 
-RadiosOutputTypeDef = TypedDict(
-    "RadiosOutputTypeDef",
-    {
-        "wifi": bool,
-        "bluetooth": bool,
-        "nfc": bool,
-        "gps": bool,
-    },
-    total=False,
-)
-
 RadiosTypeDef = TypedDict(
     "RadiosTypeDef",
     {
         "wifi": bool,
         "bluetooth": bool,
         "nfc": bool,
         "gps": bool,
@@ -1637,25 +1319,14 @@
     "RenewOfferingRequestRequestTypeDef",
     {
         "offeringId": str,
         "quantity": int,
     },
 )
 
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
 StopJobRequestRequestTypeDef = TypedDict(
     "StopJobRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -1669,22 +1340,14 @@
 StopRunRequestRequestTypeDef = TypedDict(
     "StopRunRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 TestGridVpcConfigOutputTypeDef = TypedDict(
     "TestGridVpcConfigOutputTypeDef",
     {
         "securityGroupIds": List[str],
         "subnetIds": List[str],
         "vpcId": str,
     },
@@ -1828,23 +1491,14 @@
         "maxSlots": Dict[str, int],
         "defaultJobTimeoutMinutes": int,
         "skipAppResign": bool,
     },
     total=False,
 )
 
-ListArtifactsResultTypeDef = TypedDict(
-    "ListArtifactsResultTypeDef",
-    {
-        "artifacts": List[ArtifactTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateDevicePoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevicePoolRequestRequestTypeDef",
     {
         "projectArn": str,
         "name": str,
         "rules": Sequence[RuleTypeDef],
     },
@@ -1859,14 +1513,27 @@
 )
 
 class CreateDevicePoolRequestRequestTypeDef(
     _RequiredCreateDevicePoolRequestRequestTypeDef, _OptionalCreateDevicePoolRequestRequestTypeDef
 ):
     pass
 
+DevicePoolTypeDef = TypedDict(
+    "DevicePoolTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "description": str,
+        "type": DevicePoolTypeType,
+        "rules": List[RuleTypeDef],
+        "maxDevices": int,
+    },
+    total=False,
+)
+
 _RequiredUpdateDevicePoolRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDevicePoolRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateDevicePoolRequestRequestTypeDef = TypedDict(
@@ -1882,19 +1549,37 @@
 )
 
 class UpdateDevicePoolRequestRequestTypeDef(
     _RequiredUpdateDevicePoolRequestRequestTypeDef, _OptionalUpdateDevicePoolRequestRequestTypeDef
 ):
     pass
 
+CreateTestGridUrlResultTypeDef = TypedDict(
+    "CreateTestGridUrlResultTypeDef",
+    {
+        "url": str,
+        "expires": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListArtifactsResultTypeDef = TypedDict(
+    "ListArtifactsResultTypeDef",
+    {
+        "artifacts": List[ArtifactTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateInstanceProfileResultTypeDef = TypedDict(
     "CreateInstanceProfileResultTypeDef",
     {
         "instanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceInstanceTypeDef = TypedDict(
     "DeviceInstanceTypeDef",
     {
         "arn": str,
@@ -1907,65 +1592,65 @@
     total=False,
 )
 
 GetInstanceProfileResultTypeDef = TypedDict(
     "GetInstanceProfileResultTypeDef",
     {
         "instanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInstanceProfilesResultTypeDef = TypedDict(
     "ListInstanceProfilesResultTypeDef",
     {
         "instanceProfiles": List[InstanceProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInstanceProfileResultTypeDef = TypedDict(
     "UpdateInstanceProfileResultTypeDef",
     {
         "instanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateNetworkProfileResultTypeDef = TypedDict(
     "CreateNetworkProfileResultTypeDef",
     {
         "networkProfile": NetworkProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkProfileResultTypeDef = TypedDict(
     "GetNetworkProfileResultTypeDef",
     {
         "networkProfile": NetworkProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNetworkProfilesResultTypeDef = TypedDict(
     "ListNetworkProfilesResultTypeDef",
     {
         "networkProfiles": List[NetworkProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNetworkProfileResultTypeDef = TypedDict(
     "UpdateNetworkProfileResultTypeDef",
     {
         "networkProfile": NetworkProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "name": str,
@@ -2079,81 +1764,81 @@
 ):
     pass
 
 CreateUploadResultTypeDef = TypedDict(
     "CreateUploadResultTypeDef",
     {
         "upload": UploadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUploadResultTypeDef = TypedDict(
     "GetUploadResultTypeDef",
     {
         "upload": UploadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstallToRemoteAccessSessionResultTypeDef = TypedDict(
     "InstallToRemoteAccessSessionResultTypeDef",
     {
         "appUpload": UploadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUploadsResultTypeDef = TypedDict(
     "ListUploadsResultTypeDef",
     {
         "uploads": List[UploadTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUploadResultTypeDef = TypedDict(
     "UpdateUploadResultTypeDef",
     {
         "upload": UploadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVPCEConfigurationResultTypeDef = TypedDict(
     "CreateVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVPCEConfigurationResultTypeDef = TypedDict(
     "GetVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVPCEConfigurationsResultTypeDef = TypedDict(
     "ListVPCEConfigurationsResultTypeDef",
     {
         "vpceConfigurations": List[VPCEConfigurationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVPCEConfigurationResultTypeDef = TypedDict(
     "UpdateVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceSelectionResultTypeDef = TypedDict(
     "DeviceSelectionResultTypeDef",
     {
         "filters": List[DeviceFilterOutputTypeDef],
@@ -2167,24 +1852,14 @@
     "DeviceSelectionConfigurationTypeDef",
     {
         "filters": Sequence[DeviceFilterTypeDef],
         "maxDevices": int,
     },
 )
 
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    {
-        "arn": str,
-        "filters": Sequence[DeviceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDevicesRequestRequestTypeDef = TypedDict(
     "ListDevicesRequestRequestTypeDef",
     {
         "arn": str,
         "nextToken": str,
         "filters": Sequence[DeviceFilterTypeDef],
     },
@@ -2223,85 +1898,377 @@
         "counters": CountersTypeDef,
         "message": str,
         "deviceMinutes": DeviceMinutesTypeDef,
     },
     total=False,
 )
 
-DevicePoolTypeDef = TypedDict(
-    "DevicePoolTypeDef",
+GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef = TypedDict(
+    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
+    "_RequiredListArtifactsRequestListArtifactsPaginateTypeDef",
     {
         "arn": str,
-        "name": str,
-        "description": str,
+        "type": ArtifactCategoryType,
+    },
+)
+_OptionalListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
+    "_OptionalListArtifactsRequestListArtifactsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListArtifactsRequestListArtifactsPaginateTypeDef(
+    _RequiredListArtifactsRequestListArtifactsPaginateTypeDef,
+    _OptionalListArtifactsRequestListArtifactsPaginateTypeDef,
+):
+    pass
+
+ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef = TypedDict(
+    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
+    "_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
+    "_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
+    {
         "type": DevicePoolTypeType,
-        "rules": List[RuleOutputTypeDef],
-        "maxDevices": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDevicePoolsRequestListDevicePoolsPaginateTypeDef(
+    _RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
+    _OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
+):
+    pass
+
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "arn": str,
+        "filters": Sequence[DeviceFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
+    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "_RequiredListJobsRequestListJobsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "_OptionalListJobsRequestListJobsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListJobsRequestListJobsPaginateTypeDef(
+    _RequiredListJobsRequestListJobsPaginateTypeDef, _OptionalListJobsRequestListJobsPaginateTypeDef
+):
+    pass
+
+_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
+    "_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
+    "_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
+    {
+        "type": NetworkProfileTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef(
+    _RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
+    _OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
+):
+    pass
+
+ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef = TypedDict(
+    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef = TypedDict(
+    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "arn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef(
+    _RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
+    _OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListRunsRequestListRunsPaginateTypeDef = TypedDict(
+    "_RequiredListRunsRequestListRunsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListRunsRequestListRunsPaginateTypeDef = TypedDict(
+    "_OptionalListRunsRequestListRunsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRunsRequestListRunsPaginateTypeDef(
+    _RequiredListRunsRequestListRunsPaginateTypeDef, _OptionalListRunsRequestListRunsPaginateTypeDef
+):
+    pass
+
+_RequiredListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
+    "_RequiredListSamplesRequestListSamplesPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
+    "_OptionalListSamplesRequestListSamplesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSamplesRequestListSamplesPaginateTypeDef(
+    _RequiredListSamplesRequestListSamplesPaginateTypeDef,
+    _OptionalListSamplesRequestListSamplesPaginateTypeDef,
+):
+    pass
+
+_RequiredListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
+    "_RequiredListSuitesRequestListSuitesPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
+    "_OptionalListSuitesRequestListSuitesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSuitesRequestListSuitesPaginateTypeDef(
+    _RequiredListSuitesRequestListSuitesPaginateTypeDef,
+    _OptionalListSuitesRequestListSuitesPaginateTypeDef,
+):
+    pass
+
+_RequiredListTestsRequestListTestsPaginateTypeDef = TypedDict(
+    "_RequiredListTestsRequestListTestsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListTestsRequestListTestsPaginateTypeDef = TypedDict(
+    "_OptionalListTestsRequestListTestsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTestsRequestListTestsPaginateTypeDef(
+    _RequiredListTestsRequestListTestsPaginateTypeDef,
+    _OptionalListTestsRequestListTestsPaginateTypeDef,
+):
+    pass
+
+_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
+    "_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
+    "_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef(
+    _RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
+    _OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
+):
+    pass
+
+_RequiredListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListUploadsRequestListUploadsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListUploadsRequestListUploadsPaginateTypeDef",
+    {
+        "type": UploadTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUploadsRequestListUploadsPaginateTypeDef(
+    _RequiredListUploadsRequestListUploadsPaginateTypeDef,
+    _OptionalListUploadsRequestListUploadsPaginateTypeDef,
+):
+    pass
+
+ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef = TypedDict(
+    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetTestGridSessionResultTypeDef = TypedDict(
     "GetTestGridSessionResultTypeDef",
     {
         "testGridSession": TestGridSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTestGridSessionsResultTypeDef = TypedDict(
     "ListTestGridSessionsResultTypeDef",
     {
         "testGridSessions": List[TestGridSessionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOfferingPromotionsResultTypeDef = TypedDict(
     "ListOfferingPromotionsResultTypeDef",
     {
         "offeringPromotions": List[OfferingPromotionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSamplesResultTypeDef = TypedDict(
     "ListSamplesResultTypeDef",
     {
         "samples": List[SampleTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 ListTestGridSessionActionsResultTypeDef = TypedDict(
     "ListTestGridSessionActionsResultTypeDef",
     {
         "actions": List[TestGridSessionActionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTestGridSessionArtifactsResultTypeDef = TypedDict(
     "ListTestGridSessionArtifactsResultTypeDef",
     {
         "artifacts": List[TestGridSessionArtifactTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "cost": MonetaryAmountTypeDef,
@@ -2334,22 +2301,14 @@
         "radios": RadiosTypeDef,
         "auxiliaryApps": Sequence[str],
         "billingMethod": BillingMethodType,
     },
     total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
 TestGridProjectTypeDef = TypedDict(
     "TestGridProjectTypeDef",
     {
         "arn": str,
         "name": str,
         "description": str,
         "vpcConfig": TestGridVpcConfigOutputTypeDef,
@@ -2358,15 +2317,48 @@
     total=False,
 )
 
 GetAccountSettingsResultTypeDef = TypedDict(
     "GetAccountSettingsResultTypeDef",
     {
         "accountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDevicePoolResultTypeDef = TypedDict(
+    "CreateDevicePoolResultTypeDef",
+    {
+        "devicePool": DevicePoolTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDevicePoolResultTypeDef = TypedDict(
+    "GetDevicePoolResultTypeDef",
+    {
+        "devicePool": DevicePoolTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDevicePoolsResultTypeDef = TypedDict(
+    "ListDevicePoolsResultTypeDef",
+    {
+        "devicePools": List[DevicePoolTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDevicePoolResultTypeDef = TypedDict(
+    "UpdateDevicePoolResultTypeDef",
+    {
+        "devicePool": DevicePoolTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
         "arn": str,
@@ -2394,32 +2386,32 @@
     total=False,
 )
 
 GetDeviceInstanceResultTypeDef = TypedDict(
     "GetDeviceInstanceResultTypeDef",
     {
         "deviceInstance": DeviceInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeviceInstancesResultTypeDef = TypedDict(
     "ListDeviceInstancesResultTypeDef",
     {
         "deviceInstances": List[DeviceInstanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDeviceInstanceResultTypeDef = TypedDict(
     "UpdateDeviceInstanceResultTypeDef",
     {
         "deviceInstance": DeviceInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RunTypeDef = TypedDict(
     "RunTypeDef",
     {
         "arn": str,
@@ -2442,90 +2434,57 @@
         "resultCode": ExecutionResultCodeType,
         "seed": int,
         "appUpload": str,
         "eventCount": int,
         "jobTimeoutMinutes": int,
         "devicePoolArn": str,
         "locale": str,
-        "radios": RadiosOutputTypeDef,
-        "location": LocationOutputTypeDef,
+        "radios": RadiosTypeDef,
+        "location": LocationTypeDef,
         "customerArtifactPaths": CustomerArtifactPathsOutputTypeDef,
         "webUrl": str,
         "skipAppResign": bool,
         "testSpecArn": str,
         "deviceSelectionResult": DeviceSelectionResultTypeDef,
         "vpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
 
 GetSuiteResultTypeDef = TypedDict(
     "GetSuiteResultTypeDef",
     {
         "suite": SuiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSuitesResultTypeDef = TypedDict(
     "ListSuitesResultTypeDef",
     {
         "suites": List[SuiteTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTestResultTypeDef = TypedDict(
     "GetTestResultTypeDef",
     {
         "test": TestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTestsResultTypeDef = TypedDict(
     "ListTestsResultTypeDef",
     {
         "tests": List[TestTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDevicePoolResultTypeDef = TypedDict(
-    "CreateDevicePoolResultTypeDef",
-    {
-        "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDevicePoolResultTypeDef = TypedDict(
-    "GetDevicePoolResultTypeDef",
-    {
-        "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDevicePoolsResultTypeDef = TypedDict(
-    "ListDevicePoolsResultTypeDef",
-    {
-        "devicePools": List[DevicePoolTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDevicePoolResultTypeDef = TypedDict(
-    "UpdateDevicePoolResultTypeDef",
-    {
-        "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "id": str,
@@ -2537,40 +2496,40 @@
     total=False,
 )
 
 CreateProjectResultTypeDef = TypedDict(
     "CreateProjectResultTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProjectResultTypeDef = TypedDict(
     "GetProjectResultTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProjectsResultTypeDef = TypedDict(
     "ListProjectsResultTypeDef",
     {
         "projects": List[ProjectTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProjectResultTypeDef = TypedDict(
     "UpdateProjectResultTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetDevicePoolCompatibilityRequestRequestTypeDef = TypedDict(
     "_RequiredGetDevicePoolCompatibilityRequestRequestTypeDef",
     {
         "devicePoolArn": str,
@@ -2618,40 +2577,40 @@
 ):
     pass
 
 CreateTestGridProjectResultTypeDef = TypedDict(
     "CreateTestGridProjectResultTypeDef",
     {
         "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTestGridProjectResultTypeDef = TypedDict(
     "GetTestGridProjectResultTypeDef",
     {
         "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTestGridProjectsResultTypeDef = TypedDict(
     "ListTestGridProjectsResultTypeDef",
     {
         "testGridProjects": List[TestGridProjectTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTestGridProjectResultTypeDef = TypedDict(
     "UpdateTestGridProjectResultTypeDef",
     {
         "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DevicePoolCompatibilityResultTypeDef = TypedDict(
     "DevicePoolCompatibilityResultTypeDef",
     {
         "device": DeviceTypeDef,
@@ -2661,15 +2620,15 @@
     total=False,
 )
 
 GetDeviceResultTypeDef = TypedDict(
     "GetDeviceResultTypeDef",
     {
         "device": DeviceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "arn": str,
@@ -2692,15 +2651,15 @@
 )
 
 ListDevicesResultTypeDef = TypedDict(
     "ListDevicesResultTypeDef",
     {
         "devices": List[DeviceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProblemTypeDef = TypedDict(
     "ProblemTypeDef",
     {
         "run": ProblemDetailTypeDef,
@@ -2743,49 +2702,49 @@
     total=False,
 )
 
 GetRunResultTypeDef = TypedDict(
     "GetRunResultTypeDef",
     {
         "run": RunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRunsResultTypeDef = TypedDict(
     "ListRunsResultTypeDef",
     {
         "runs": List[RunTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScheduleRunResultTypeDef = TypedDict(
     "ScheduleRunResultTypeDef",
     {
         "run": RunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopRunResultTypeDef = TypedDict(
     "StopRunResultTypeDef",
     {
         "run": RunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOfferingsResultTypeDef = TypedDict(
     "ListOfferingsResultTypeDef",
     {
         "offerings": List[OfferingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OfferingStatusTypeDef = TypedDict(
     "OfferingStatusTypeDef",
     {
         "type": OfferingTransactionTypeType,
@@ -2797,40 +2756,40 @@
 )
 
 GetDevicePoolCompatibilityResultTypeDef = TypedDict(
     "GetDevicePoolCompatibilityResultTypeDef",
     {
         "compatibleDevices": List[DevicePoolCompatibilityResultTypeDef],
         "incompatibleDevices": List[DevicePoolCompatibilityResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobResultTypeDef = TypedDict(
     "GetJobResultTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "jobs": List[JobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopJobResultTypeDef = TypedDict(
     "StopJobResultTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UniqueProblemTypeDef = TypedDict(
     "UniqueProblemTypeDef",
     {
         "message": str,
@@ -2839,50 +2798,50 @@
     total=False,
 )
 
 CreateRemoteAccessSessionResultTypeDef = TypedDict(
     "CreateRemoteAccessSessionResultTypeDef",
     {
         "remoteAccessSession": RemoteAccessSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRemoteAccessSessionResultTypeDef = TypedDict(
     "GetRemoteAccessSessionResultTypeDef",
     {
         "remoteAccessSession": RemoteAccessSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRemoteAccessSessionsResultTypeDef = TypedDict(
     "ListRemoteAccessSessionsResultTypeDef",
     {
         "remoteAccessSessions": List[RemoteAccessSessionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopRemoteAccessSessionResultTypeDef = TypedDict(
     "StopRemoteAccessSessionResultTypeDef",
     {
         "remoteAccessSession": RemoteAccessSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOfferingStatusResultTypeDef = TypedDict(
     "GetOfferingStatusResultTypeDef",
     {
         "current": Dict[str, OfferingStatusTypeDef],
         "nextPeriod": Dict[str, OfferingStatusTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OfferingTransactionTypeDef = TypedDict(
     "OfferingTransactionTypeDef",
     {
         "offeringStatus": OfferingStatusTypeDef,
@@ -2895,35 +2854,35 @@
 )
 
 ListUniqueProblemsResultTypeDef = TypedDict(
     "ListUniqueProblemsResultTypeDef",
     {
         "uniqueProblems": Dict[ExecutionResultType, List[UniqueProblemTypeDef]],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOfferingTransactionsResultTypeDef = TypedDict(
     "ListOfferingTransactionsResultTypeDef",
     {
         "offeringTransactions": List[OfferingTransactionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PurchaseOfferingResultTypeDef = TypedDict(
     "PurchaseOfferingResultTypeDef",
     {
         "offeringTransaction": OfferingTransactionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RenewOfferingResultTypeDef = TypedDict(
     "RenewOfferingResultTypeDef",
     {
         "offeringTransaction": OfferingTransactionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/PKG-INFO` & `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devicefarm
-Version: 1.28.12
-Summary: Type annotations for boto3.DeviceFarm 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DeviceFarm 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devicefarm)](https://pepy.tech/project/mypy-boto3-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DeviceFarm 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[boto3.DeviceFarm 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
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
 [mypy-boto3-devicefarm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -428,23 +428,23 @@
 ```python
 from mypy_boto3_devicefarm.type_defs import (
     TrialMinutesTypeDef,
     ArtifactTypeDef,
     CPUTypeDef,
     CountersTypeDef,
     RuleTypeDef,
+    ResponseMetadataTypeDef,
     CreateInstanceProfileRequestRequestTypeDef,
     InstanceProfileTypeDef,
     CreateNetworkProfileRequestRequestTypeDef,
     NetworkProfileTypeDef,
     VpcConfigTypeDef,
     CreateRemoteAccessSessionConfigurationTypeDef,
     TestGridVpcConfigTypeDef,
     CreateTestGridUrlRequestRequestTypeDef,
-    CreateTestGridUrlResultTypeDef,
     CreateUploadRequestRequestTypeDef,
     UploadTypeDef,
     CreateVPCEConfigurationRequestRequestTypeDef,
     VPCEConfigurationTypeDef,
     CustomerArtifactPathsOutputTypeDef,
     CustomerArtifactPathsTypeDef,
     DeleteDevicePoolRequestRequestTypeDef,
@@ -456,109 +456,87 @@
     DeleteTestGridProjectRequestRequestTypeDef,
     DeleteUploadRequestRequestTypeDef,
     DeleteVPCEConfigurationRequestRequestTypeDef,
     DeviceFilterOutputTypeDef,
     DeviceFilterTypeDef,
     DeviceMinutesTypeDef,
     IncompatibilityMessageTypeDef,
-    RuleOutputTypeDef,
     ResolutionTypeDef,
     ExecutionConfigurationTypeDef,
     GetDeviceInstanceRequestRequestTypeDef,
     ScheduleRunTestTypeDef,
     GetDevicePoolRequestRequestTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetNetworkProfileRequestRequestTypeDef,
-    GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetOfferingStatusRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetRemoteAccessSessionRequestRequestTypeDef,
     GetRunRequestRequestTypeDef,
     GetSuiteRequestRequestTypeDef,
     GetTestGridProjectRequestRequestTypeDef,
     GetTestGridSessionRequestRequestTypeDef,
     TestGridSessionTypeDef,
     GetTestRequestRequestTypeDef,
     GetUploadRequestRequestTypeDef,
     GetVPCEConfigurationRequestRequestTypeDef,
     InstallToRemoteAccessSessionRequestRequestTypeDef,
-    ListArtifactsRequestListArtifactsPaginateTypeDef,
     ListArtifactsRequestRequestTypeDef,
-    ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef,
     ListDeviceInstancesRequestRequestTypeDef,
-    ListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
     ListDevicePoolsRequestRequestTypeDef,
-    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListInstanceProfilesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
     ListNetworkProfilesRequestRequestTypeDef,
-    ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef,
     ListOfferingPromotionsRequestRequestTypeDef,
     OfferingPromotionTypeDef,
-    ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef,
     ListOfferingTransactionsRequestRequestTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
-    ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
     ListRemoteAccessSessionsRequestRequestTypeDef,
-    ListRunsRequestListRunsPaginateTypeDef,
     ListRunsRequestRequestTypeDef,
-    ListSamplesRequestListSamplesPaginateTypeDef,
     ListSamplesRequestRequestTypeDef,
     SampleTypeDef,
-    ListSuitesRequestListSuitesPaginateTypeDef,
     ListSuitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     ListTestGridProjectsRequestRequestTypeDef,
     ListTestGridSessionActionsRequestRequestTypeDef,
     TestGridSessionActionTypeDef,
     ListTestGridSessionArtifactsRequestRequestTypeDef,
     TestGridSessionArtifactTypeDef,
     ListTestGridSessionsRequestRequestTypeDef,
-    ListTestsRequestListTestsPaginateTypeDef,
     ListTestsRequestRequestTypeDef,
-    ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
     ListUniqueProblemsRequestRequestTypeDef,
-    ListUploadsRequestListUploadsPaginateTypeDef,
     ListUploadsRequestRequestTypeDef,
-    ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef,
     ListVPCEConfigurationsRequestRequestTypeDef,
-    LocationOutputTypeDef,
     LocationTypeDef,
     MonetaryAmountTypeDef,
-    PaginatorConfigTypeDef,
     ProblemDetailTypeDef,
     VpcConfigOutputTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
-    RadiosOutputTypeDef,
     RadiosTypeDef,
     RenewOfferingRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     StopJobRequestRequestTypeDef,
     StopRemoteAccessSessionRequestRequestTypeDef,
     StopRunRequestRequestTypeDef,
-    TagTypeDef,
     TestGridVpcConfigOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceInstanceRequestRequestTypeDef,
     UpdateInstanceProfileRequestRequestTypeDef,
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateUploadRequestRequestTypeDef,
     UpdateVPCEConfigurationRequestRequestTypeDef,
     AccountSettingsTypeDef,
-    ListArtifactsResultTypeDef,
     CreateDevicePoolRequestRequestTypeDef,
+    DevicePoolTypeDef,
     UpdateDevicePoolRequestRequestTypeDef,
+    CreateTestGridUrlResultTypeDef,
+    ListArtifactsResultTypeDef,
     CreateInstanceProfileResultTypeDef,
     DeviceInstanceTypeDef,
     GetInstanceProfileResultTypeDef,
     ListInstanceProfilesResultTypeDef,
     UpdateInstanceProfileResultTypeDef,
     CreateNetworkProfileResultTypeDef,
     GetNetworkProfileResultTypeDef,
@@ -576,45 +554,63 @@
     UpdateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
     GetVPCEConfigurationResultTypeDef,
     ListVPCEConfigurationsResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
     DeviceSelectionResultTypeDef,
     DeviceSelectionConfigurationTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDevicesRequestRequestTypeDef,
     SuiteTypeDef,
     TestTypeDef,
-    DevicePoolTypeDef,
+    GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef,
+    ListArtifactsRequestListArtifactsPaginateTypeDef,
+    ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef,
+    ListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
+    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
+    ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef,
+    ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
+    ListRunsRequestListRunsPaginateTypeDef,
+    ListSamplesRequestListSamplesPaginateTypeDef,
+    ListSuitesRequestListSuitesPaginateTypeDef,
+    ListTestsRequestListTestsPaginateTypeDef,
+    ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
+    ListUploadsRequestListUploadsPaginateTypeDef,
+    ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef,
     GetTestGridSessionResultTypeDef,
     ListTestGridSessionsResultTypeDef,
     ListOfferingPromotionsResultTypeDef,
     ListSamplesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ListTestGridSessionActionsResultTypeDef,
     ListTestGridSessionArtifactsResultTypeDef,
     RecurringChargeTypeDef,
     ProjectTypeDef,
     ScheduleRunConfigurationTypeDef,
-    TagResourceRequestRequestTypeDef,
     TestGridProjectTypeDef,
     GetAccountSettingsResultTypeDef,
+    CreateDevicePoolResultTypeDef,
+    GetDevicePoolResultTypeDef,
+    ListDevicePoolsResultTypeDef,
+    UpdateDevicePoolResultTypeDef,
     DeviceTypeDef,
     GetDeviceInstanceResultTypeDef,
     ListDeviceInstancesResultTypeDef,
     UpdateDeviceInstanceResultTypeDef,
     RunTypeDef,
     GetSuiteResultTypeDef,
     ListSuitesResultTypeDef,
     GetTestResultTypeDef,
     ListTestsResultTypeDef,
-    CreateDevicePoolResultTypeDef,
-    GetDevicePoolResultTypeDef,
-    ListDevicePoolsResultTypeDef,
-    UpdateDevicePoolResultTypeDef,
     OfferingTypeDef,
     CreateProjectResultTypeDef,
     GetProjectResultTypeDef,
     ListProjectsResultTypeDef,
     UpdateProjectResultTypeDef,
     GetDevicePoolCompatibilityRequestRequestTypeDef,
     ScheduleRunRequestRequestTypeDef,
```

### Comparing `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/SOURCES.txt` & `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.12/setup.py` & `mypy-boto3-devicefarm-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-devicefarm",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_devicefarm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DeviceFarm 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.DeviceFarm 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

