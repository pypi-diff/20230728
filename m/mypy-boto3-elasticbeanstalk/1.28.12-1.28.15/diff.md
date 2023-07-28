# Comparing `tmp/mypy-boto3-elasticbeanstalk-1.28.12.tar.gz` & `tmp/mypy-boto3-elasticbeanstalk-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elasticbeanstalk-1.28.12.tar", last modified: Thu Jul 27 05:34:38 2023, max compression
+gzip compressed data, was "mypy-boto3-elasticbeanstalk-1.28.15.tar", last modified: Fri Jul 28 20:42:43 2023, max compression
```

## Comparing `mypy-boto3-elasticbeanstalk-1.28.12.tar` & `mypy-boto3-elasticbeanstalk-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.732520 mypy-boto3-elasticbeanstalk-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21767 2023-07-27 05:34:38.732520 mypy-boto3-elasticbeanstalk-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20244 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.732520 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42742 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42680 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55546 2023-07-27 05:21:49.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55503 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.732520 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21767 2023-07-27 05:34:38.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-27 05:34:38.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:38.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:38.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:38.732520 mypy-boto3-elasticbeanstalk-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.977044 mypy-boto3-elasticbeanstalk-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:11.000000 mypy-boto3-elasticbeanstalk-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21415 2023-07-28 20:42:43.977044 mypy-boto3-elasticbeanstalk-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19892 2023-07-28 20:25:11.000000 mypy-boto3-elasticbeanstalk-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.961043 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-28 20:25:11.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-28 20:25:11.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 20:25:11.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42686 2023-07-28 20:25:12.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42624 2023-07-28 20:25:11.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-28 20:25:12.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-28 20:25:12.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-07-28 20:25:12.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-07-28 20:25:12.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:11.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52740 2023-07-28 20:25:14.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52701 2023-07-28 20:25:13.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:11.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-07-28 20:25:12.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-28 20:25:12.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.977044 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21415 2023-07-28 20:42:43.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-28 20:42:43.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:43.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:42:43.000000 mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:43.977044 mypy-boto3-elasticbeanstalk-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-28 20:25:11.000000 mypy-boto3-elasticbeanstalk-1.28.15/setup.py
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/LICENSE` & `mypy-boto3-elasticbeanstalk-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/PKG-INFO` & `mypy-boto3-elasticbeanstalk-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticbeanstalk
-Version: 1.28.12
-Summary: Type annotations for boto3.ElasticBeanstalk 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ElasticBeanstalk 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticbeanstalk)](https://pepy.tech/project/mypy-boto3-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticBeanstalk 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[boto3.ElasticBeanstalk 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [mypy-boto3-elasticbeanstalk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -395,123 +395,116 @@
 
 `mypy_boto3_elasticbeanstalk.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticbeanstalk.type_defs import (
     AbortEnvironmentUpdateMessageRequestTypeDef,
+    ResponseMetadataTypeDef,
     LatencyTypeDef,
     StatusCodesTypeDef,
-    S3LocationOutputTypeDef,
-    SourceBuildInformationOutputTypeDef,
-    MaxAgeRuleOutputTypeDef,
-    MaxCountRuleOutputTypeDef,
+    S3LocationTypeDef,
+    SourceBuildInformationTypeDef,
     MaxAgeRuleTypeDef,
     MaxCountRuleTypeDef,
     ApplyEnvironmentManagedActionRequestRequestTypeDef,
-    ApplyEnvironmentManagedActionResultTypeDef,
     AssociateEnvironmentOperationsRoleMessageRequestTypeDef,
     AutoScalingGroupTypeDef,
     BuildConfigurationTypeDef,
     BuilderTypeDef,
     CPUUtilizationTypeDef,
     CheckDNSAvailabilityMessageRequestTypeDef,
-    CheckDNSAvailabilityResultMessageTypeDef,
     ComposeEnvironmentsMessageRequestTypeDef,
     OptionRestrictionRegexTypeDef,
-    ConfigurationOptionSettingOutputTypeDef,
     ConfigurationOptionSettingTypeDef,
     ValidationMessageTypeDef,
     TagTypeDef,
-    S3LocationTypeDef,
-    SourceBuildInformationTypeDef,
     SourceConfigurationTypeDef,
     EnvironmentTierTypeDef,
     OptionSpecificationTypeDef,
     PlatformSummaryTypeDef,
-    CreateStorageLocationResultMessageTypeDef,
     CustomAmiTypeDef,
     DeleteApplicationMessageRequestTypeDef,
     DeleteApplicationVersionMessageRequestTypeDef,
     DeleteConfigurationTemplateMessageRequestTypeDef,
     DeleteEnvironmentConfigurationMessageRequestTypeDef,
     DeletePlatformVersionRequestRequestTypeDef,
     DeploymentTypeDef,
-    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeApplicationVersionsMessageRequestTypeDef,
     DescribeApplicationsMessageRequestTypeDef,
     DescribeConfigurationSettingsMessageRequestTypeDef,
     DescribeEnvironmentHealthRequestRequestTypeDef,
     InstanceHealthSummaryTypeDef,
-    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef,
     ManagedActionHistoryItemTypeDef,
     DescribeEnvironmentManagedActionsRequestRequestTypeDef,
     ManagedActionTypeDef,
     DescribeEnvironmentResourcesMessageRequestTypeDef,
-    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeEnvironmentsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeInstancesHealthRequestRequestTypeDef,
     DescribePlatformVersionRequestRequestTypeDef,
     DisassociateEnvironmentOperationsRoleMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnvironmentLinkTypeDef,
-    EnvironmentTierOutputTypeDef,
     EnvironmentInfoDescriptionTypeDef,
     InstanceTypeDef,
     LaunchConfigurationTypeDef,
     LaunchTemplateTypeDef,
     LoadBalancerTypeDef,
     QueueTypeDef,
     TriggerTypeDef,
     EventDescriptionTypeDef,
     SolutionStackDescriptionTypeDef,
     SearchFilterTypeDef,
     PlatformBranchSummaryTypeDef,
     PlatformFilterTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ListenerTypeDef,
-    PaginatorConfigTypeDef,
     PlatformFrameworkTypeDef,
     PlatformProgrammingLanguageTypeDef,
     RebuildEnvironmentMessageRequestTypeDef,
     RequestEnvironmentInfoMessageRequestTypeDef,
     ResourceQuotaTypeDef,
-    TagOutputTypeDef,
-    ResponseMetadataTypeDef,
     RestartAppServerMessageRequestTypeDef,
     RetrieveEnvironmentInfoMessageRequestTypeDef,
     SwapEnvironmentCNAMEsMessageRequestTypeDef,
     TerminateEnvironmentMessageRequestTypeDef,
     UpdateApplicationMessageRequestTypeDef,
     UpdateApplicationVersionMessageRequestTypeDef,
+    ApplyEnvironmentManagedActionResultTypeDef,
+    CheckDNSAvailabilityResultMessageTypeDef,
+    CreateStorageLocationResultMessageTypeDef,
+    EmptyResponseMetadataTypeDef,
     ApplicationMetricsTypeDef,
     ApplicationVersionDescriptionTypeDef,
-    ApplicationVersionLifecycleConfigOutputTypeDef,
     ApplicationVersionLifecycleConfigTypeDef,
     SystemStatusTypeDef,
     ConfigurationOptionDescriptionTypeDef,
-    ConfigurationSettingsDescriptionResponseMetadataTypeDef,
+    ConfigurationSettingsDescriptionResponseTypeDef,
     ConfigurationSettingsDescriptionTypeDef,
     ValidateConfigurationSettingsMessageRequestTypeDef,
     ConfigurationSettingsValidationMessagesTypeDef,
-    UpdateTagsForResourceMessageRequestTypeDef,
-    CreatePlatformVersionRequestRequestTypeDef,
     CreateApplicationVersionMessageRequestTypeDef,
+    CreatePlatformVersionRequestRequestTypeDef,
+    ResourceTagsDescriptionMessageTypeDef,
+    UpdateTagsForResourceMessageRequestTypeDef,
     CreateConfigurationTemplateMessageRequestTypeDef,
     CreateEnvironmentMessageRequestTypeDef,
     DescribeConfigurationOptionsMessageRequestTypeDef,
     UpdateConfigurationTemplateMessageRequestTypeDef,
     UpdateEnvironmentMessageRequestTypeDef,
     CreatePlatformVersionResultTypeDef,
     DeletePlatformVersionResultTypeDef,
     ListPlatformVersionsResultTypeDef,
+    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
+    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
+    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
     DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     EnvironmentResourceDescriptionTypeDef,
@@ -520,33 +513,31 @@
     ListPlatformBranchesRequestRequestTypeDef,
     ListPlatformBranchesResultTypeDef,
     ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef,
     ListPlatformVersionsRequestRequestTypeDef,
     LoadBalancerDescriptionTypeDef,
     PlatformDescriptionTypeDef,
     ResourceQuotasTypeDef,
-    ResourceTagsDescriptionMessageTypeDef,
     DescribeEnvironmentHealthResultTypeDef,
     ApplicationVersionDescriptionMessageTypeDef,
     ApplicationVersionDescriptionsMessageTypeDef,
-    ApplicationResourceLifecycleConfigOutputTypeDef,
     ApplicationResourceLifecycleConfigTypeDef,
     SingleInstanceHealthTypeDef,
     ConfigurationOptionsDescriptionTypeDef,
     ConfigurationSettingsDescriptionsTypeDef,
     EnvironmentResourceDescriptionsMessageTypeDef,
     EnvironmentResourcesDescriptionTypeDef,
     DescribePlatformVersionResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     ApplicationDescriptionTypeDef,
     ApplicationResourceLifecycleDescriptionMessageTypeDef,
     CreateApplicationMessageRequestTypeDef,
     UpdateApplicationResourceLifecycleMessageRequestTypeDef,
     DescribeInstancesHealthResultTypeDef,
-    EnvironmentDescriptionResponseMetadataTypeDef,
+    EnvironmentDescriptionResponseTypeDef,
     EnvironmentDescriptionTypeDef,
     ApplicationDescriptionMessageTypeDef,
     ApplicationDescriptionsMessageTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
 )
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/README.md` & `mypy-boto3-elasticbeanstalk-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticbeanstalk)](https://pepy.tech/project/mypy-boto3-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticBeanstalk 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[boto3.ElasticBeanstalk 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [mypy-boto3-elasticbeanstalk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,123 +363,116 @@
 
 `mypy_boto3_elasticbeanstalk.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticbeanstalk.type_defs import (
     AbortEnvironmentUpdateMessageRequestTypeDef,
+    ResponseMetadataTypeDef,
     LatencyTypeDef,
     StatusCodesTypeDef,
-    S3LocationOutputTypeDef,
-    SourceBuildInformationOutputTypeDef,
-    MaxAgeRuleOutputTypeDef,
-    MaxCountRuleOutputTypeDef,
+    S3LocationTypeDef,
+    SourceBuildInformationTypeDef,
     MaxAgeRuleTypeDef,
     MaxCountRuleTypeDef,
     ApplyEnvironmentManagedActionRequestRequestTypeDef,
-    ApplyEnvironmentManagedActionResultTypeDef,
     AssociateEnvironmentOperationsRoleMessageRequestTypeDef,
     AutoScalingGroupTypeDef,
     BuildConfigurationTypeDef,
     BuilderTypeDef,
     CPUUtilizationTypeDef,
     CheckDNSAvailabilityMessageRequestTypeDef,
-    CheckDNSAvailabilityResultMessageTypeDef,
     ComposeEnvironmentsMessageRequestTypeDef,
     OptionRestrictionRegexTypeDef,
-    ConfigurationOptionSettingOutputTypeDef,
     ConfigurationOptionSettingTypeDef,
     ValidationMessageTypeDef,
     TagTypeDef,
-    S3LocationTypeDef,
-    SourceBuildInformationTypeDef,
     SourceConfigurationTypeDef,
     EnvironmentTierTypeDef,
     OptionSpecificationTypeDef,
     PlatformSummaryTypeDef,
-    CreateStorageLocationResultMessageTypeDef,
     CustomAmiTypeDef,
     DeleteApplicationMessageRequestTypeDef,
     DeleteApplicationVersionMessageRequestTypeDef,
     DeleteConfigurationTemplateMessageRequestTypeDef,
     DeleteEnvironmentConfigurationMessageRequestTypeDef,
     DeletePlatformVersionRequestRequestTypeDef,
     DeploymentTypeDef,
-    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeApplicationVersionsMessageRequestTypeDef,
     DescribeApplicationsMessageRequestTypeDef,
     DescribeConfigurationSettingsMessageRequestTypeDef,
     DescribeEnvironmentHealthRequestRequestTypeDef,
     InstanceHealthSummaryTypeDef,
-    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef,
     ManagedActionHistoryItemTypeDef,
     DescribeEnvironmentManagedActionsRequestRequestTypeDef,
     ManagedActionTypeDef,
     DescribeEnvironmentResourcesMessageRequestTypeDef,
-    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeEnvironmentsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeInstancesHealthRequestRequestTypeDef,
     DescribePlatformVersionRequestRequestTypeDef,
     DisassociateEnvironmentOperationsRoleMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnvironmentLinkTypeDef,
-    EnvironmentTierOutputTypeDef,
     EnvironmentInfoDescriptionTypeDef,
     InstanceTypeDef,
     LaunchConfigurationTypeDef,
     LaunchTemplateTypeDef,
     LoadBalancerTypeDef,
     QueueTypeDef,
     TriggerTypeDef,
     EventDescriptionTypeDef,
     SolutionStackDescriptionTypeDef,
     SearchFilterTypeDef,
     PlatformBranchSummaryTypeDef,
     PlatformFilterTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ListenerTypeDef,
-    PaginatorConfigTypeDef,
     PlatformFrameworkTypeDef,
     PlatformProgrammingLanguageTypeDef,
     RebuildEnvironmentMessageRequestTypeDef,
     RequestEnvironmentInfoMessageRequestTypeDef,
     ResourceQuotaTypeDef,
-    TagOutputTypeDef,
-    ResponseMetadataTypeDef,
     RestartAppServerMessageRequestTypeDef,
     RetrieveEnvironmentInfoMessageRequestTypeDef,
     SwapEnvironmentCNAMEsMessageRequestTypeDef,
     TerminateEnvironmentMessageRequestTypeDef,
     UpdateApplicationMessageRequestTypeDef,
     UpdateApplicationVersionMessageRequestTypeDef,
+    ApplyEnvironmentManagedActionResultTypeDef,
+    CheckDNSAvailabilityResultMessageTypeDef,
+    CreateStorageLocationResultMessageTypeDef,
+    EmptyResponseMetadataTypeDef,
     ApplicationMetricsTypeDef,
     ApplicationVersionDescriptionTypeDef,
-    ApplicationVersionLifecycleConfigOutputTypeDef,
     ApplicationVersionLifecycleConfigTypeDef,
     SystemStatusTypeDef,
     ConfigurationOptionDescriptionTypeDef,
-    ConfigurationSettingsDescriptionResponseMetadataTypeDef,
+    ConfigurationSettingsDescriptionResponseTypeDef,
     ConfigurationSettingsDescriptionTypeDef,
     ValidateConfigurationSettingsMessageRequestTypeDef,
     ConfigurationSettingsValidationMessagesTypeDef,
-    UpdateTagsForResourceMessageRequestTypeDef,
-    CreatePlatformVersionRequestRequestTypeDef,
     CreateApplicationVersionMessageRequestTypeDef,
+    CreatePlatformVersionRequestRequestTypeDef,
+    ResourceTagsDescriptionMessageTypeDef,
+    UpdateTagsForResourceMessageRequestTypeDef,
     CreateConfigurationTemplateMessageRequestTypeDef,
     CreateEnvironmentMessageRequestTypeDef,
     DescribeConfigurationOptionsMessageRequestTypeDef,
     UpdateConfigurationTemplateMessageRequestTypeDef,
     UpdateEnvironmentMessageRequestTypeDef,
     CreatePlatformVersionResultTypeDef,
     DeletePlatformVersionResultTypeDef,
     ListPlatformVersionsResultTypeDef,
+    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
+    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
+    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
     DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     EnvironmentResourceDescriptionTypeDef,
@@ -488,33 +481,31 @@
     ListPlatformBranchesRequestRequestTypeDef,
     ListPlatformBranchesResultTypeDef,
     ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef,
     ListPlatformVersionsRequestRequestTypeDef,
     LoadBalancerDescriptionTypeDef,
     PlatformDescriptionTypeDef,
     ResourceQuotasTypeDef,
-    ResourceTagsDescriptionMessageTypeDef,
     DescribeEnvironmentHealthResultTypeDef,
     ApplicationVersionDescriptionMessageTypeDef,
     ApplicationVersionDescriptionsMessageTypeDef,
-    ApplicationResourceLifecycleConfigOutputTypeDef,
     ApplicationResourceLifecycleConfigTypeDef,
     SingleInstanceHealthTypeDef,
     ConfigurationOptionsDescriptionTypeDef,
     ConfigurationSettingsDescriptionsTypeDef,
     EnvironmentResourceDescriptionsMessageTypeDef,
     EnvironmentResourcesDescriptionTypeDef,
     DescribePlatformVersionResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     ApplicationDescriptionTypeDef,
     ApplicationResourceLifecycleDescriptionMessageTypeDef,
     CreateApplicationMessageRequestTypeDef,
     UpdateApplicationResourceLifecycleMessageRequestTypeDef,
     DescribeInstancesHealthResultTypeDef,
-    EnvironmentDescriptionResponseMetadataTypeDef,
+    EnvironmentDescriptionResponseTypeDef,
     EnvironmentDescriptionTypeDef,
     ApplicationDescriptionMessageTypeDef,
     ApplicationDescriptionsMessageTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
 )
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/__init__.py` & `mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/__init__.pyi` & `mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/__main__.py` & `mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticBeanstalk 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ElasticBeanstalk 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk\nOther"
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

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/client.py` & `mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,28 +41,28 @@
     ApplicationVersionDescriptionMessageTypeDef,
     ApplicationVersionDescriptionsMessageTypeDef,
     ApplyEnvironmentManagedActionResultTypeDef,
     BuildConfigurationTypeDef,
     CheckDNSAvailabilityResultMessageTypeDef,
     ConfigurationOptionsDescriptionTypeDef,
     ConfigurationOptionSettingTypeDef,
-    ConfigurationSettingsDescriptionResponseMetadataTypeDef,
+    ConfigurationSettingsDescriptionResponseTypeDef,
     ConfigurationSettingsDescriptionsTypeDef,
     ConfigurationSettingsValidationMessagesTypeDef,
     CreatePlatformVersionResultTypeDef,
     CreateStorageLocationResultMessageTypeDef,
     DeletePlatformVersionResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     DescribeEnvironmentHealthResultTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
     DescribeInstancesHealthResultTypeDef,
     DescribePlatformVersionResultTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnvironmentDescriptionResponseMetadataTypeDef,
+    EnvironmentDescriptionResponseTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
     EnvironmentResourceDescriptionsMessageTypeDef,
     EnvironmentTierTypeDef,
     EventDescriptionsMessageTypeDef,
     ListAvailableSolutionStacksResultMessageTypeDef,
     ListPlatformBranchesResultTypeDef,
     ListPlatformVersionsResultTypeDef,
@@ -251,15 +251,15 @@
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         SourceConfiguration: SourceConfigurationTypeDef = ...,
         EnvironmentId: str = ...,
         Description: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> ConfigurationSettingsDescriptionResponseMetadataTypeDef:
+    ) -> ConfigurationSettingsDescriptionResponseTypeDef:
         """
         Creates an AWS Elastic Beanstalk configuration template, associated with a
         specific Elastic Beanstalk application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/client/#create_configuration_template)
         """
@@ -277,15 +277,15 @@
         VersionLabel: str = ...,
         TemplateName: str = ...,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...,
         OperationsRole: str = ...
-    ) -> EnvironmentDescriptionResponseMetadataTypeDef:
+    ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Launches an AWS Elastic Beanstalk environment for the specified application
         using the specified configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/client/#create_environment)
         """
@@ -690,15 +690,15 @@
     def terminate_environment(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         TerminateResources: bool = ...,
         ForceTerminate: bool = ...
-    ) -> EnvironmentDescriptionResponseMetadataTypeDef:
+    ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Terminates the specified environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.terminate_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/client/#terminate_environment)
         """
 
@@ -739,15 +739,15 @@
         self,
         *,
         ApplicationName: str,
         TemplateName: str,
         Description: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...
-    ) -> ConfigurationSettingsDescriptionResponseMetadataTypeDef:
+    ) -> ConfigurationSettingsDescriptionResponseTypeDef:
         """
         Updates the specified configuration template to have the specified properties or
         configuration option values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.update_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/client/#update_configuration_template)
         """
@@ -763,15 +763,15 @@
         Tier: EnvironmentTierTypeDef = ...,
         VersionLabel: str = ...,
         TemplateName: str = ...,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...
-    ) -> EnvironmentDescriptionResponseMetadataTypeDef:
+    ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Updates the environment description, deploys a new application version, updates
         the configuration settings to an entirely new configuration template, or updates
         select configuration option values in the running environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/client/#update_environment)
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/client.pyi` & `mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -41,28 +41,28 @@
     ApplicationVersionDescriptionMessageTypeDef,
     ApplicationVersionDescriptionsMessageTypeDef,
     ApplyEnvironmentManagedActionResultTypeDef,
     BuildConfigurationTypeDef,
     CheckDNSAvailabilityResultMessageTypeDef,
     ConfigurationOptionsDescriptionTypeDef,
     ConfigurationOptionSettingTypeDef,
-    ConfigurationSettingsDescriptionResponseMetadataTypeDef,
+    ConfigurationSettingsDescriptionResponseTypeDef,
     ConfigurationSettingsDescriptionsTypeDef,
     ConfigurationSettingsValidationMessagesTypeDef,
     CreatePlatformVersionResultTypeDef,
     CreateStorageLocationResultMessageTypeDef,
     DeletePlatformVersionResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     DescribeEnvironmentHealthResultTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
     DescribeInstancesHealthResultTypeDef,
     DescribePlatformVersionResultTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnvironmentDescriptionResponseMetadataTypeDef,
+    EnvironmentDescriptionResponseTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
     EnvironmentResourceDescriptionsMessageTypeDef,
     EnvironmentTierTypeDef,
     EventDescriptionsMessageTypeDef,
     ListAvailableSolutionStacksResultMessageTypeDef,
     ListPlatformBranchesResultTypeDef,
     ListPlatformVersionsResultTypeDef,
@@ -237,15 +237,15 @@
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         SourceConfiguration: SourceConfigurationTypeDef = ...,
         EnvironmentId: str = ...,
         Description: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> ConfigurationSettingsDescriptionResponseMetadataTypeDef:
+    ) -> ConfigurationSettingsDescriptionResponseTypeDef:
         """
         Creates an AWS Elastic Beanstalk configuration template, associated with a
         specific Elastic Beanstalk application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/client/#create_configuration_template)
         """
@@ -262,15 +262,15 @@
         VersionLabel: str = ...,
         TemplateName: str = ...,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...,
         OperationsRole: str = ...
-    ) -> EnvironmentDescriptionResponseMetadataTypeDef:
+    ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Launches an AWS Elastic Beanstalk environment for the specified application
         using the specified configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/client/#create_environment)
         """
@@ -643,15 +643,15 @@
     def terminate_environment(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         TerminateResources: bool = ...,
         ForceTerminate: bool = ...
-    ) -> EnvironmentDescriptionResponseMetadataTypeDef:
+    ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Terminates the specified environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.terminate_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/client/#terminate_environment)
         """
     def update_application(
@@ -688,15 +688,15 @@
         self,
         *,
         ApplicationName: str,
         TemplateName: str,
         Description: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...
-    ) -> ConfigurationSettingsDescriptionResponseMetadataTypeDef:
+    ) -> ConfigurationSettingsDescriptionResponseTypeDef:
         """
         Updates the specified configuration template to have the specified properties or
         configuration option values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.update_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/client/#update_configuration_template)
         """
@@ -711,15 +711,15 @@
         Tier: EnvironmentTierTypeDef = ...,
         VersionLabel: str = ...,
         TemplateName: str = ...,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...
-    ) -> EnvironmentDescriptionResponseMetadataTypeDef:
+    ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Updates the environment description, deploys a new application version, updates
         the configuration settings to an entirely new configuration template, or updates
         select configuration option values in the running environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/client/#update_environment)
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/literals.py` & `mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/literals.pyi` & `mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/paginator.py` & `mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,63 +47,58 @@
     "DescribeApplicationVersionsPaginator",
     "DescribeEnvironmentManagedActionHistoryPaginator",
     "DescribeEnvironmentsPaginator",
     "DescribeEventsPaginator",
     "ListPlatformVersionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeApplicationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeApplicationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeapplicationversionspaginator)
     """
 
     def paginate(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabels: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ApplicationVersionDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeApplicationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeapplicationversionspaginator)
         """
 
-
 class DescribeEnvironmentManagedActionHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironmentManagedActionHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeenvironmentmanagedactionhistorypaginator)
     """
 
     def paginate(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEnvironmentManagedActionHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironmentManagedActionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeenvironmentmanagedactionhistorypaginator)
         """
 
-
 class DescribeEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeenvironmentspaginator)
     """
 
     def paginate(
@@ -111,22 +106,21 @@
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
         IncludedDeletedBackTo: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EnvironmentDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeenvironmentspaginator)
         """
 
-
 class DescribeEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeeventspaginator)
     """
 
     def paginate(
@@ -138,31 +132,30 @@
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeeventspaginator)
         """
 
-
 class ListPlatformVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.ListPlatformVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#listplatformversionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PlatformFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPlatformVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.ListPlatformVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#listplatformversionspaginator)
         """
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/paginator.pyi` & `mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,58 +47,63 @@
     "DescribeApplicationVersionsPaginator",
     "DescribeEnvironmentManagedActionHistoryPaginator",
     "DescribeEnvironmentsPaginator",
     "DescribeEventsPaginator",
     "ListPlatformVersionsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeApplicationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeApplicationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeapplicationversionspaginator)
     """
 
     def paginate(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabels: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ApplicationVersionDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeApplicationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeapplicationversionspaginator)
         """
 
+
 class DescribeEnvironmentManagedActionHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironmentManagedActionHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeenvironmentmanagedactionhistorypaginator)
     """
 
     def paginate(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEnvironmentManagedActionHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironmentManagedActionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeenvironmentmanagedactionhistorypaginator)
         """
 
+
 class DescribeEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeenvironmentspaginator)
     """
 
     def paginate(
@@ -106,21 +111,22 @@
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
         IncludedDeletedBackTo: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EnvironmentDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeenvironmentspaginator)
         """
 
+
 class DescribeEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeeventspaginator)
     """
 
     def paginate(
@@ -132,30 +138,31 @@
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeeventspaginator)
         """
 
+
 class ListPlatformVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.ListPlatformVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#listplatformversionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PlatformFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPlatformVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.ListPlatformVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#listplatformversionspaginator)
         """
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/type_defs.py` & `mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,123 +41,116 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AbortEnvironmentUpdateMessageRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "LatencyTypeDef",
     "StatusCodesTypeDef",
-    "S3LocationOutputTypeDef",
-    "SourceBuildInformationOutputTypeDef",
-    "MaxAgeRuleOutputTypeDef",
-    "MaxCountRuleOutputTypeDef",
+    "S3LocationTypeDef",
+    "SourceBuildInformationTypeDef",
     "MaxAgeRuleTypeDef",
     "MaxCountRuleTypeDef",
     "ApplyEnvironmentManagedActionRequestRequestTypeDef",
-    "ApplyEnvironmentManagedActionResultTypeDef",
     "AssociateEnvironmentOperationsRoleMessageRequestTypeDef",
     "AutoScalingGroupTypeDef",
     "BuildConfigurationTypeDef",
     "BuilderTypeDef",
     "CPUUtilizationTypeDef",
     "CheckDNSAvailabilityMessageRequestTypeDef",
-    "CheckDNSAvailabilityResultMessageTypeDef",
     "ComposeEnvironmentsMessageRequestTypeDef",
     "OptionRestrictionRegexTypeDef",
-    "ConfigurationOptionSettingOutputTypeDef",
     "ConfigurationOptionSettingTypeDef",
     "ValidationMessageTypeDef",
     "TagTypeDef",
-    "S3LocationTypeDef",
-    "SourceBuildInformationTypeDef",
     "SourceConfigurationTypeDef",
     "EnvironmentTierTypeDef",
     "OptionSpecificationTypeDef",
     "PlatformSummaryTypeDef",
-    "CreateStorageLocationResultMessageTypeDef",
     "CustomAmiTypeDef",
     "DeleteApplicationMessageRequestTypeDef",
     "DeleteApplicationVersionMessageRequestTypeDef",
     "DeleteConfigurationTemplateMessageRequestTypeDef",
     "DeleteEnvironmentConfigurationMessageRequestTypeDef",
     "DeletePlatformVersionRequestRequestTypeDef",
     "DeploymentTypeDef",
-    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeApplicationVersionsMessageRequestTypeDef",
     "DescribeApplicationsMessageRequestTypeDef",
     "DescribeConfigurationSettingsMessageRequestTypeDef",
     "DescribeEnvironmentHealthRequestRequestTypeDef",
     "InstanceHealthSummaryTypeDef",
-    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef",
     "ManagedActionHistoryItemTypeDef",
     "DescribeEnvironmentManagedActionsRequestRequestTypeDef",
     "ManagedActionTypeDef",
     "DescribeEnvironmentResourcesMessageRequestTypeDef",
-    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEnvironmentsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
     "DescribeInstancesHealthRequestRequestTypeDef",
     "DescribePlatformVersionRequestRequestTypeDef",
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnvironmentLinkTypeDef",
-    "EnvironmentTierOutputTypeDef",
     "EnvironmentInfoDescriptionTypeDef",
     "InstanceTypeDef",
     "LaunchConfigurationTypeDef",
     "LaunchTemplateTypeDef",
     "LoadBalancerTypeDef",
     "QueueTypeDef",
     "TriggerTypeDef",
     "EventDescriptionTypeDef",
     "SolutionStackDescriptionTypeDef",
     "SearchFilterTypeDef",
     "PlatformBranchSummaryTypeDef",
     "PlatformFilterTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ListenerTypeDef",
-    "PaginatorConfigTypeDef",
     "PlatformFrameworkTypeDef",
     "PlatformProgrammingLanguageTypeDef",
     "RebuildEnvironmentMessageRequestTypeDef",
     "RequestEnvironmentInfoMessageRequestTypeDef",
     "ResourceQuotaTypeDef",
-    "TagOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "RestartAppServerMessageRequestTypeDef",
     "RetrieveEnvironmentInfoMessageRequestTypeDef",
     "SwapEnvironmentCNAMEsMessageRequestTypeDef",
     "TerminateEnvironmentMessageRequestTypeDef",
     "UpdateApplicationMessageRequestTypeDef",
     "UpdateApplicationVersionMessageRequestTypeDef",
+    "ApplyEnvironmentManagedActionResultTypeDef",
+    "CheckDNSAvailabilityResultMessageTypeDef",
+    "CreateStorageLocationResultMessageTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ApplicationMetricsTypeDef",
     "ApplicationVersionDescriptionTypeDef",
-    "ApplicationVersionLifecycleConfigOutputTypeDef",
     "ApplicationVersionLifecycleConfigTypeDef",
     "SystemStatusTypeDef",
     "ConfigurationOptionDescriptionTypeDef",
-    "ConfigurationSettingsDescriptionResponseMetadataTypeDef",
+    "ConfigurationSettingsDescriptionResponseTypeDef",
     "ConfigurationSettingsDescriptionTypeDef",
     "ValidateConfigurationSettingsMessageRequestTypeDef",
     "ConfigurationSettingsValidationMessagesTypeDef",
-    "UpdateTagsForResourceMessageRequestTypeDef",
-    "CreatePlatformVersionRequestRequestTypeDef",
     "CreateApplicationVersionMessageRequestTypeDef",
+    "CreatePlatformVersionRequestRequestTypeDef",
+    "ResourceTagsDescriptionMessageTypeDef",
+    "UpdateTagsForResourceMessageRequestTypeDef",
     "CreateConfigurationTemplateMessageRequestTypeDef",
     "CreateEnvironmentMessageRequestTypeDef",
     "DescribeConfigurationOptionsMessageRequestTypeDef",
     "UpdateConfigurationTemplateMessageRequestTypeDef",
     "UpdateEnvironmentMessageRequestTypeDef",
     "CreatePlatformVersionResultTypeDef",
     "DeletePlatformVersionResultTypeDef",
     "ListPlatformVersionsResultTypeDef",
+    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
+    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryResultTypeDef",
     "DescribeEnvironmentManagedActionsResultTypeDef",
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef",
     "RetrieveEnvironmentInfoResultMessageTypeDef",
     "EnvironmentResourceDescriptionTypeDef",
@@ -166,33 +159,31 @@
     "ListPlatformBranchesRequestRequestTypeDef",
     "ListPlatformBranchesResultTypeDef",
     "ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef",
     "ListPlatformVersionsRequestRequestTypeDef",
     "LoadBalancerDescriptionTypeDef",
     "PlatformDescriptionTypeDef",
     "ResourceQuotasTypeDef",
-    "ResourceTagsDescriptionMessageTypeDef",
     "DescribeEnvironmentHealthResultTypeDef",
     "ApplicationVersionDescriptionMessageTypeDef",
     "ApplicationVersionDescriptionsMessageTypeDef",
-    "ApplicationResourceLifecycleConfigOutputTypeDef",
     "ApplicationResourceLifecycleConfigTypeDef",
     "SingleInstanceHealthTypeDef",
     "ConfigurationOptionsDescriptionTypeDef",
     "ConfigurationSettingsDescriptionsTypeDef",
     "EnvironmentResourceDescriptionsMessageTypeDef",
     "EnvironmentResourcesDescriptionTypeDef",
     "DescribePlatformVersionResultTypeDef",
     "DescribeAccountAttributesResultTypeDef",
     "ApplicationDescriptionTypeDef",
     "ApplicationResourceLifecycleDescriptionMessageTypeDef",
     "CreateApplicationMessageRequestTypeDef",
     "UpdateApplicationResourceLifecycleMessageRequestTypeDef",
     "DescribeInstancesHealthResultTypeDef",
-    "EnvironmentDescriptionResponseMetadataTypeDef",
+    "EnvironmentDescriptionResponseTypeDef",
     "EnvironmentDescriptionTypeDef",
     "ApplicationDescriptionMessageTypeDef",
     "ApplicationDescriptionsMessageTypeDef",
     "EnvironmentDescriptionsMessageTypeDef",
 )
 
 AbortEnvironmentUpdateMessageRequestTypeDef = TypedDict(
@@ -200,14 +191,25 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
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
 LatencyTypeDef = TypedDict(
     "LatencyTypeDef",
     {
         "P999": float,
         "P99": float,
         "P95": float,
         "P90": float,
@@ -226,74 +228,32 @@
         "Status3xx": int,
         "Status4xx": int,
         "Status5xx": int,
     },
     total=False,
 )
 
-S3LocationOutputTypeDef = TypedDict(
-    "S3LocationOutputTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
         "S3Bucket": str,
         "S3Key": str,
     },
     total=False,
 )
 
-SourceBuildInformationOutputTypeDef = TypedDict(
-    "SourceBuildInformationOutputTypeDef",
+SourceBuildInformationTypeDef = TypedDict(
+    "SourceBuildInformationTypeDef",
     {
         "SourceType": SourceTypeType,
         "SourceRepository": SourceRepositoryType,
         "SourceLocation": str,
     },
 )
 
-_RequiredMaxAgeRuleOutputTypeDef = TypedDict(
-    "_RequiredMaxAgeRuleOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalMaxAgeRuleOutputTypeDef = TypedDict(
-    "_OptionalMaxAgeRuleOutputTypeDef",
-    {
-        "MaxAgeInDays": int,
-        "DeleteSourceFromS3": bool,
-    },
-    total=False,
-)
-
-
-class MaxAgeRuleOutputTypeDef(_RequiredMaxAgeRuleOutputTypeDef, _OptionalMaxAgeRuleOutputTypeDef):
-    pass
-
-
-_RequiredMaxCountRuleOutputTypeDef = TypedDict(
-    "_RequiredMaxCountRuleOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalMaxCountRuleOutputTypeDef = TypedDict(
-    "_OptionalMaxCountRuleOutputTypeDef",
-    {
-        "MaxCount": int,
-        "DeleteSourceFromS3": bool,
-    },
-    total=False,
-)
-
-
-class MaxCountRuleOutputTypeDef(
-    _RequiredMaxCountRuleOutputTypeDef, _OptionalMaxCountRuleOutputTypeDef
-):
-    pass
-
-
 _RequiredMaxAgeRuleTypeDef = TypedDict(
     "_RequiredMaxAgeRuleTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalMaxAgeRuleTypeDef = TypedDict(
@@ -349,25 +309,14 @@
 class ApplyEnvironmentManagedActionRequestRequestTypeDef(
     _RequiredApplyEnvironmentManagedActionRequestRequestTypeDef,
     _OptionalApplyEnvironmentManagedActionRequestRequestTypeDef,
 ):
     pass
 
 
-ApplyEnvironmentManagedActionResultTypeDef = TypedDict(
-    "ApplyEnvironmentManagedActionResultTypeDef",
-    {
-        "ActionId": str,
-        "ActionDescription": str,
-        "ActionType": ActionTypeType,
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateEnvironmentOperationsRoleMessageRequestTypeDef = TypedDict(
     "AssociateEnvironmentOperationsRoleMessageRequestTypeDef",
     {
         "EnvironmentName": str,
         "OperationsRole": str,
     },
 )
@@ -430,23 +379,14 @@
 CheckDNSAvailabilityMessageRequestTypeDef = TypedDict(
     "CheckDNSAvailabilityMessageRequestTypeDef",
     {
         "CNAMEPrefix": str,
     },
 )
 
-CheckDNSAvailabilityResultMessageTypeDef = TypedDict(
-    "CheckDNSAvailabilityResultMessageTypeDef",
-    {
-        "Available": bool,
-        "FullyQualifiedCNAME": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ComposeEnvironmentsMessageRequestTypeDef = TypedDict(
     "ComposeEnvironmentsMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "GroupName": str,
         "VersionLabels": Sequence[str],
     },
@@ -458,25 +398,14 @@
     {
         "Pattern": str,
         "Label": str,
     },
     total=False,
 )
 
-ConfigurationOptionSettingOutputTypeDef = TypedDict(
-    "ConfigurationOptionSettingOutputTypeDef",
-    {
-        "ResourceName": str,
-        "Namespace": str,
-        "OptionName": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 ConfigurationOptionSettingTypeDef = TypedDict(
     "ConfigurationOptionSettingTypeDef",
     {
         "ResourceName": str,
         "Namespace": str,
         "OptionName": str,
         "Value": str,
@@ -500,32 +429,14 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
-    {
-        "S3Bucket": str,
-        "S3Key": str,
-    },
-    total=False,
-)
-
-SourceBuildInformationTypeDef = TypedDict(
-    "SourceBuildInformationTypeDef",
-    {
-        "SourceType": SourceTypeType,
-        "SourceRepository": SourceRepositoryType,
-        "SourceLocation": str,
-    },
-)
-
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "ApplicationName": str,
         "TemplateName": str,
     },
     total=False,
@@ -566,22 +477,14 @@
         "PlatformVersion": str,
         "PlatformBranchName": str,
         "PlatformBranchLifecycleState": str,
     },
     total=False,
 )
 
-CreateStorageLocationResultMessageTypeDef = TypedDict(
-    "CreateStorageLocationResultMessageTypeDef",
-    {
-        "S3Bucket": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomAmiTypeDef = TypedDict(
     "CustomAmiTypeDef",
     {
         "VirtualizationType": str,
         "ImageId": str,
     },
     total=False,
@@ -662,20 +565,20 @@
         "DeploymentId": int,
         "Status": str,
         "DeploymentTime": datetime,
     },
     total=False,
 )
 
-DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef = TypedDict(
-    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ApplicationName": str,
-        "VersionLabels": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeApplicationVersionsMessageRequestTypeDef = TypedDict(
     "DescribeApplicationVersionsMessageRequestTypeDef",
     {
@@ -739,24 +642,14 @@
         "Warning": int,
         "Degraded": int,
         "Severe": int,
     },
     total=False,
 )
 
-DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
-    {
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef",
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
         "NextToken": str,
         "MaxItems": int,
@@ -806,28 +699,14 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
-DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "EnvironmentIds": Sequence[str],
-        "EnvironmentNames": Sequence[str],
-        "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -844,32 +723,14 @@
         "IncludedDeletedBackTo": Union[datetime, str],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "TemplateName": str,
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PlatformArn": str,
-        "RequestId": str,
-        "Severity": EventSeverityType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "TemplateName": str,
         "EnvironmentId": str,
@@ -907,40 +768,23 @@
 DisassociateEnvironmentOperationsRoleMessageRequestTypeDef = TypedDict(
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
     {
         "EnvironmentName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnvironmentLinkTypeDef = TypedDict(
     "EnvironmentLinkTypeDef",
     {
         "LinkName": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
-EnvironmentTierOutputTypeDef = TypedDict(
-    "EnvironmentTierOutputTypeDef",
-    {
-        "Name": str,
-        "Type": str,
-        "Version": str,
-    },
-    total=False,
-)
-
 EnvironmentInfoDescriptionTypeDef = TypedDict(
     "EnvironmentInfoDescriptionTypeDef",
     {
         "InfoType": EnvironmentInfoTypeType,
         "Ec2InstanceId": str,
         "SampleTimestamp": datetime,
         "Message": str,
@@ -1066,24 +910,14 @@
     {
         "Protocol": str,
         "Port": int,
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
 PlatformFrameworkTypeDef = TypedDict(
     "PlatformFrameworkTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
@@ -1134,34 +968,14 @@
     "ResourceQuotaTypeDef",
     {
         "Maximum": int,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
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
 RestartAppServerMessageRequestTypeDef = TypedDict(
     "RestartAppServerMessageRequestTypeDef",
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
@@ -1252,14 +1066,49 @@
 class UpdateApplicationVersionMessageRequestTypeDef(
     _RequiredUpdateApplicationVersionMessageRequestTypeDef,
     _OptionalUpdateApplicationVersionMessageRequestTypeDef,
 ):
     pass
 
 
+ApplyEnvironmentManagedActionResultTypeDef = TypedDict(
+    "ApplyEnvironmentManagedActionResultTypeDef",
+    {
+        "ActionId": str,
+        "ActionDescription": str,
+        "ActionType": ActionTypeType,
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CheckDNSAvailabilityResultMessageTypeDef = TypedDict(
+    "CheckDNSAvailabilityResultMessageTypeDef",
+    {
+        "Available": bool,
+        "FullyQualifiedCNAME": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStorageLocationResultMessageTypeDef = TypedDict(
+    "CreateStorageLocationResultMessageTypeDef",
+    {
+        "S3Bucket": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ApplicationMetricsTypeDef = TypedDict(
     "ApplicationMetricsTypeDef",
     {
         "Duration": int,
         "RequestCount": int,
         "StatusCodes": StatusCodesTypeDef,
         "Latency": LatencyTypeDef,
@@ -1270,33 +1119,24 @@
 ApplicationVersionDescriptionTypeDef = TypedDict(
     "ApplicationVersionDescriptionTypeDef",
     {
         "ApplicationVersionArn": str,
         "ApplicationName": str,
         "Description": str,
         "VersionLabel": str,
-        "SourceBuildInformation": SourceBuildInformationOutputTypeDef,
+        "SourceBuildInformation": SourceBuildInformationTypeDef,
         "BuildArn": str,
-        "SourceBundle": S3LocationOutputTypeDef,
+        "SourceBundle": S3LocationTypeDef,
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Status": ApplicationVersionStatusType,
     },
     total=False,
 )
 
-ApplicationVersionLifecycleConfigOutputTypeDef = TypedDict(
-    "ApplicationVersionLifecycleConfigOutputTypeDef",
-    {
-        "MaxCountRule": MaxCountRuleOutputTypeDef,
-        "MaxAgeRule": MaxAgeRuleOutputTypeDef,
-    },
-    total=False,
-)
-
 ApplicationVersionLifecycleConfigTypeDef = TypedDict(
     "ApplicationVersionLifecycleConfigTypeDef",
     {
         "MaxCountRule": MaxCountRuleTypeDef,
         "MaxAgeRule": MaxAgeRuleTypeDef,
     },
     total=False,
@@ -1325,28 +1165,28 @@
         "MaxValue": int,
         "MaxLength": int,
         "Regex": OptionRestrictionRegexTypeDef,
     },
     total=False,
 )
 
-ConfigurationSettingsDescriptionResponseMetadataTypeDef = TypedDict(
-    "ConfigurationSettingsDescriptionResponseMetadataTypeDef",
+ConfigurationSettingsDescriptionResponseTypeDef = TypedDict(
+    "ConfigurationSettingsDescriptionResponseTypeDef",
     {
         "SolutionStackName": str,
         "PlatformArn": str,
         "ApplicationName": str,
         "TemplateName": str,
         "Description": str,
         "EnvironmentName": str,
         "DeploymentStatus": ConfigurationDeploymentStatusType,
         "DateCreated": datetime,
         "DateUpdated": datetime,
-        "OptionSettings": List[ConfigurationOptionSettingOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OptionSettings": List[ConfigurationOptionSettingTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationSettingsDescriptionTypeDef = TypedDict(
     "ConfigurationSettingsDescriptionTypeDef",
     {
         "SolutionStackName": str,
@@ -1354,15 +1194,15 @@
         "ApplicationName": str,
         "TemplateName": str,
         "Description": str,
         "EnvironmentName": str,
         "DeploymentStatus": ConfigurationDeploymentStatusType,
         "DateCreated": datetime,
         "DateUpdated": datetime,
-        "OptionSettings": List[ConfigurationOptionSettingOutputTypeDef],
+        "OptionSettings": List[ConfigurationOptionSettingTypeDef],
     },
     total=False,
 )
 
 _RequiredValidateConfigurationSettingsMessageRequestTypeDef = TypedDict(
     "_RequiredValidateConfigurationSettingsMessageRequestTypeDef",
     {
@@ -1387,37 +1227,43 @@
     pass
 
 
 ConfigurationSettingsValidationMessagesTypeDef = TypedDict(
     "ConfigurationSettingsValidationMessagesTypeDef",
     {
         "Messages": List[ValidationMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
-    "_RequiredUpdateTagsForResourceMessageRequestTypeDef",
+_RequiredCreateApplicationVersionMessageRequestTypeDef = TypedDict(
+    "_RequiredCreateApplicationVersionMessageRequestTypeDef",
     {
-        "ResourceArn": str,
+        "ApplicationName": str,
+        "VersionLabel": str,
     },
 )
-_OptionalUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
-    "_OptionalUpdateTagsForResourceMessageRequestTypeDef",
+_OptionalCreateApplicationVersionMessageRequestTypeDef = TypedDict(
+    "_OptionalCreateApplicationVersionMessageRequestTypeDef",
     {
-        "TagsToAdd": Sequence[TagTypeDef],
-        "TagsToRemove": Sequence[str],
+        "Description": str,
+        "SourceBuildInformation": SourceBuildInformationTypeDef,
+        "SourceBundle": S3LocationTypeDef,
+        "BuildConfiguration": BuildConfigurationTypeDef,
+        "AutoCreateApplication": bool,
+        "Process": bool,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class UpdateTagsForResourceMessageRequestTypeDef(
-    _RequiredUpdateTagsForResourceMessageRequestTypeDef,
-    _OptionalUpdateTagsForResourceMessageRequestTypeDef,
+class CreateApplicationVersionMessageRequestTypeDef(
+    _RequiredCreateApplicationVersionMessageRequestTypeDef,
+    _OptionalCreateApplicationVersionMessageRequestTypeDef,
 ):
     pass
 
 
 _RequiredCreatePlatformVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePlatformVersionRequestRequestTypeDef",
     {
@@ -1440,39 +1286,42 @@
 class CreatePlatformVersionRequestRequestTypeDef(
     _RequiredCreatePlatformVersionRequestRequestTypeDef,
     _OptionalCreatePlatformVersionRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredCreateApplicationVersionMessageRequestTypeDef = TypedDict(
-    "_RequiredCreateApplicationVersionMessageRequestTypeDef",
+ResourceTagsDescriptionMessageTypeDef = TypedDict(
+    "ResourceTagsDescriptionMessageTypeDef",
     {
-        "ApplicationName": str,
-        "VersionLabel": str,
+        "ResourceArn": str,
+        "ResourceTags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateApplicationVersionMessageRequestTypeDef = TypedDict(
-    "_OptionalCreateApplicationVersionMessageRequestTypeDef",
+
+_RequiredUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_RequiredUpdateTagsForResourceMessageRequestTypeDef",
     {
-        "Description": str,
-        "SourceBuildInformation": SourceBuildInformationTypeDef,
-        "SourceBundle": S3LocationTypeDef,
-        "BuildConfiguration": BuildConfigurationTypeDef,
-        "AutoCreateApplication": bool,
-        "Process": bool,
-        "Tags": Sequence[TagTypeDef],
+        "ResourceArn": str,
+    },
+)
+_OptionalUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_OptionalUpdateTagsForResourceMessageRequestTypeDef",
+    {
+        "TagsToAdd": Sequence[TagTypeDef],
+        "TagsToRemove": Sequence[str],
     },
     total=False,
 )
 
 
-class CreateApplicationVersionMessageRequestTypeDef(
-    _RequiredCreateApplicationVersionMessageRequestTypeDef,
-    _OptionalCreateApplicationVersionMessageRequestTypeDef,
+class UpdateTagsForResourceMessageRequestTypeDef(
+    _RequiredUpdateTagsForResourceMessageRequestTypeDef,
+    _OptionalUpdateTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
 
 _RequiredCreateConfigurationTemplateMessageRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationTemplateMessageRequestTypeDef",
     {
@@ -1593,49 +1442,101 @@
 )
 
 CreatePlatformVersionResultTypeDef = TypedDict(
     "CreatePlatformVersionResultTypeDef",
     {
         "PlatformSummary": PlatformSummaryTypeDef,
         "Builder": BuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePlatformVersionResultTypeDef = TypedDict(
     "DeletePlatformVersionResultTypeDef",
     {
         "PlatformSummary": PlatformSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlatformVersionsResultTypeDef = TypedDict(
     "ListPlatformVersionsResultTypeDef",
     {
         "PlatformSummaryList": List[PlatformSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef = TypedDict(
+    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabels": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
+    {
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "EnvironmentIds": Sequence[str],
+        "EnvironmentNames": Sequence[str],
+        "IncludeDeleted": bool,
+        "IncludedDeletedBackTo": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "TemplateName": str,
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PlatformArn": str,
+        "RequestId": str,
+        "Severity": EventSeverityType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 DescribeEnvironmentManagedActionHistoryResultTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionHistoryResultTypeDef",
     {
         "ManagedActionHistoryItems": List[ManagedActionHistoryItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEnvironmentManagedActionsResultTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionsResultTypeDef",
     {
         "ManagedActions": List[ManagedActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef = TypedDict(
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     {
         "ApplicationName": str,
@@ -1683,15 +1584,15 @@
     total=False,
 )
 
 RetrieveEnvironmentInfoResultMessageTypeDef = TypedDict(
     "RetrieveEnvironmentInfoResultMessageTypeDef",
     {
         "EnvironmentInfo": List[EnvironmentInfoDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentResourceDescriptionTypeDef = TypedDict(
     "EnvironmentResourceDescriptionTypeDef",
     {
         "EnvironmentName": str,
@@ -1707,24 +1608,24 @@
 )
 
 EventDescriptionsMessageTypeDef = TypedDict(
     "EventDescriptionsMessageTypeDef",
     {
         "Events": List[EventDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAvailableSolutionStacksResultMessageTypeDef = TypedDict(
     "ListAvailableSolutionStacksResultMessageTypeDef",
     {
         "SolutionStacks": List[str],
         "SolutionStackDetails": List[SolutionStackDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlatformBranchesRequestRequestTypeDef = TypedDict(
     "ListPlatformBranchesRequestRequestTypeDef",
     {
         "Filters": Sequence[SearchFilterTypeDef],
@@ -1735,23 +1636,23 @@
 )
 
 ListPlatformBranchesResultTypeDef = TypedDict(
     "ListPlatformBranchesResultTypeDef",
     {
         "PlatformBranchSummaryList": List[PlatformBranchSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef = TypedDict(
     "ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef",
     {
         "Filters": Sequence[PlatformFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListPlatformVersionsRequestRequestTypeDef = TypedDict(
     "ListPlatformVersionsRequestRequestTypeDef",
     {
@@ -1808,64 +1709,46 @@
         "EnvironmentQuota": ResourceQuotaTypeDef,
         "ConfigurationTemplateQuota": ResourceQuotaTypeDef,
         "CustomPlatformQuota": ResourceQuotaTypeDef,
     },
     total=False,
 )
 
-ResourceTagsDescriptionMessageTypeDef = TypedDict(
-    "ResourceTagsDescriptionMessageTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourceTags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeEnvironmentHealthResultTypeDef = TypedDict(
     "DescribeEnvironmentHealthResultTypeDef",
     {
         "EnvironmentName": str,
         "HealthStatus": str,
         "Status": EnvironmentHealthType,
         "Color": str,
         "Causes": List[str],
         "ApplicationMetrics": ApplicationMetricsTypeDef,
         "InstancesHealth": InstanceHealthSummaryTypeDef,
         "RefreshedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationVersionDescriptionMessageTypeDef = TypedDict(
     "ApplicationVersionDescriptionMessageTypeDef",
     {
         "ApplicationVersion": ApplicationVersionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationVersionDescriptionsMessageTypeDef = TypedDict(
     "ApplicationVersionDescriptionsMessageTypeDef",
     {
         "ApplicationVersions": List[ApplicationVersionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ApplicationResourceLifecycleConfigOutputTypeDef = TypedDict(
-    "ApplicationResourceLifecycleConfigOutputTypeDef",
-    {
-        "ServiceRole": str,
-        "VersionLifecycleConfig": ApplicationVersionLifecycleConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 ApplicationResourceLifecycleConfigTypeDef = TypedDict(
     "ApplicationResourceLifecycleConfigTypeDef",
     {
         "ServiceRole": str,
         "VersionLifecycleConfig": ApplicationVersionLifecycleConfigTypeDef,
     },
     total=False,
@@ -1890,31 +1773,31 @@
 
 ConfigurationOptionsDescriptionTypeDef = TypedDict(
     "ConfigurationOptionsDescriptionTypeDef",
     {
         "SolutionStackName": str,
         "PlatformArn": str,
         "Options": List[ConfigurationOptionDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationSettingsDescriptionsTypeDef = TypedDict(
     "ConfigurationSettingsDescriptionsTypeDef",
     {
         "ConfigurationSettings": List[ConfigurationSettingsDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentResourceDescriptionsMessageTypeDef = TypedDict(
     "EnvironmentResourceDescriptionsMessageTypeDef",
     {
         "EnvironmentResources": EnvironmentResourceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentResourcesDescriptionTypeDef = TypedDict(
     "EnvironmentResourcesDescriptionTypeDef",
     {
         "LoadBalancer": LoadBalancerDescriptionTypeDef,
@@ -1922,47 +1805,47 @@
     total=False,
 )
 
 DescribePlatformVersionResultTypeDef = TypedDict(
     "DescribePlatformVersionResultTypeDef",
     {
         "PlatformDescription": PlatformDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "ResourceQuotas": ResourceQuotasTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationDescriptionTypeDef = TypedDict(
     "ApplicationDescriptionTypeDef",
     {
         "ApplicationArn": str,
         "ApplicationName": str,
         "Description": str,
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Versions": List[str],
         "ConfigurationTemplates": List[str],
-        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigOutputTypeDef,
+        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
     },
     total=False,
 )
 
 ApplicationResourceLifecycleDescriptionMessageTypeDef = TypedDict(
     "ApplicationResourceLifecycleDescriptionMessageTypeDef",
     {
         "ApplicationName": str,
-        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateApplicationMessageRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationMessageRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1995,20 +1878,20 @@
 
 DescribeInstancesHealthResultTypeDef = TypedDict(
     "DescribeInstancesHealthResultTypeDef",
     {
         "InstanceHealthList": List[SingleInstanceHealthTypeDef],
         "RefreshedAt": datetime,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EnvironmentDescriptionResponseMetadataTypeDef = TypedDict(
-    "EnvironmentDescriptionResponseMetadataTypeDef",
+EnvironmentDescriptionResponseTypeDef = TypedDict(
+    "EnvironmentDescriptionResponseTypeDef",
     {
         "EnvironmentName": str,
         "EnvironmentId": str,
         "ApplicationName": str,
         "VersionLabel": str,
         "SolutionStackName": str,
         "PlatformArn": str,
@@ -2019,19 +1902,19 @@
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Status": EnvironmentStatusType,
         "AbortableOperationInProgress": bool,
         "Health": EnvironmentHealthType,
         "HealthStatus": EnvironmentHealthStatusType,
         "Resources": EnvironmentResourcesDescriptionTypeDef,
-        "Tier": EnvironmentTierOutputTypeDef,
+        "Tier": EnvironmentTierTypeDef,
         "EnvironmentLinks": List[EnvironmentLinkTypeDef],
         "EnvironmentArn": str,
         "OperationsRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentDescriptionTypeDef = TypedDict(
     "EnvironmentDescriptionTypeDef",
     {
         "EnvironmentName": str,
@@ -2047,39 +1930,39 @@
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Status": EnvironmentStatusType,
         "AbortableOperationInProgress": bool,
         "Health": EnvironmentHealthType,
         "HealthStatus": EnvironmentHealthStatusType,
         "Resources": EnvironmentResourcesDescriptionTypeDef,
-        "Tier": EnvironmentTierOutputTypeDef,
+        "Tier": EnvironmentTierTypeDef,
         "EnvironmentLinks": List[EnvironmentLinkTypeDef],
         "EnvironmentArn": str,
         "OperationsRole": str,
     },
     total=False,
 )
 
 ApplicationDescriptionMessageTypeDef = TypedDict(
     "ApplicationDescriptionMessageTypeDef",
     {
         "Application": ApplicationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationDescriptionsMessageTypeDef = TypedDict(
     "ApplicationDescriptionsMessageTypeDef",
     {
         "Applications": List[ApplicationDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentDescriptionsMessageTypeDef = TypedDict(
     "EnvironmentDescriptionsMessageTypeDef",
     {
         "Environments": List[EnvironmentDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/type_defs.pyi` & `mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -40,123 +40,116 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AbortEnvironmentUpdateMessageRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "LatencyTypeDef",
     "StatusCodesTypeDef",
-    "S3LocationOutputTypeDef",
-    "SourceBuildInformationOutputTypeDef",
-    "MaxAgeRuleOutputTypeDef",
-    "MaxCountRuleOutputTypeDef",
+    "S3LocationTypeDef",
+    "SourceBuildInformationTypeDef",
     "MaxAgeRuleTypeDef",
     "MaxCountRuleTypeDef",
     "ApplyEnvironmentManagedActionRequestRequestTypeDef",
-    "ApplyEnvironmentManagedActionResultTypeDef",
     "AssociateEnvironmentOperationsRoleMessageRequestTypeDef",
     "AutoScalingGroupTypeDef",
     "BuildConfigurationTypeDef",
     "BuilderTypeDef",
     "CPUUtilizationTypeDef",
     "CheckDNSAvailabilityMessageRequestTypeDef",
-    "CheckDNSAvailabilityResultMessageTypeDef",
     "ComposeEnvironmentsMessageRequestTypeDef",
     "OptionRestrictionRegexTypeDef",
-    "ConfigurationOptionSettingOutputTypeDef",
     "ConfigurationOptionSettingTypeDef",
     "ValidationMessageTypeDef",
     "TagTypeDef",
-    "S3LocationTypeDef",
-    "SourceBuildInformationTypeDef",
     "SourceConfigurationTypeDef",
     "EnvironmentTierTypeDef",
     "OptionSpecificationTypeDef",
     "PlatformSummaryTypeDef",
-    "CreateStorageLocationResultMessageTypeDef",
     "CustomAmiTypeDef",
     "DeleteApplicationMessageRequestTypeDef",
     "DeleteApplicationVersionMessageRequestTypeDef",
     "DeleteConfigurationTemplateMessageRequestTypeDef",
     "DeleteEnvironmentConfigurationMessageRequestTypeDef",
     "DeletePlatformVersionRequestRequestTypeDef",
     "DeploymentTypeDef",
-    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeApplicationVersionsMessageRequestTypeDef",
     "DescribeApplicationsMessageRequestTypeDef",
     "DescribeConfigurationSettingsMessageRequestTypeDef",
     "DescribeEnvironmentHealthRequestRequestTypeDef",
     "InstanceHealthSummaryTypeDef",
-    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef",
     "ManagedActionHistoryItemTypeDef",
     "DescribeEnvironmentManagedActionsRequestRequestTypeDef",
     "ManagedActionTypeDef",
     "DescribeEnvironmentResourcesMessageRequestTypeDef",
-    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEnvironmentsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
     "DescribeInstancesHealthRequestRequestTypeDef",
     "DescribePlatformVersionRequestRequestTypeDef",
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnvironmentLinkTypeDef",
-    "EnvironmentTierOutputTypeDef",
     "EnvironmentInfoDescriptionTypeDef",
     "InstanceTypeDef",
     "LaunchConfigurationTypeDef",
     "LaunchTemplateTypeDef",
     "LoadBalancerTypeDef",
     "QueueTypeDef",
     "TriggerTypeDef",
     "EventDescriptionTypeDef",
     "SolutionStackDescriptionTypeDef",
     "SearchFilterTypeDef",
     "PlatformBranchSummaryTypeDef",
     "PlatformFilterTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ListenerTypeDef",
-    "PaginatorConfigTypeDef",
     "PlatformFrameworkTypeDef",
     "PlatformProgrammingLanguageTypeDef",
     "RebuildEnvironmentMessageRequestTypeDef",
     "RequestEnvironmentInfoMessageRequestTypeDef",
     "ResourceQuotaTypeDef",
-    "TagOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "RestartAppServerMessageRequestTypeDef",
     "RetrieveEnvironmentInfoMessageRequestTypeDef",
     "SwapEnvironmentCNAMEsMessageRequestTypeDef",
     "TerminateEnvironmentMessageRequestTypeDef",
     "UpdateApplicationMessageRequestTypeDef",
     "UpdateApplicationVersionMessageRequestTypeDef",
+    "ApplyEnvironmentManagedActionResultTypeDef",
+    "CheckDNSAvailabilityResultMessageTypeDef",
+    "CreateStorageLocationResultMessageTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ApplicationMetricsTypeDef",
     "ApplicationVersionDescriptionTypeDef",
-    "ApplicationVersionLifecycleConfigOutputTypeDef",
     "ApplicationVersionLifecycleConfigTypeDef",
     "SystemStatusTypeDef",
     "ConfigurationOptionDescriptionTypeDef",
-    "ConfigurationSettingsDescriptionResponseMetadataTypeDef",
+    "ConfigurationSettingsDescriptionResponseTypeDef",
     "ConfigurationSettingsDescriptionTypeDef",
     "ValidateConfigurationSettingsMessageRequestTypeDef",
     "ConfigurationSettingsValidationMessagesTypeDef",
-    "UpdateTagsForResourceMessageRequestTypeDef",
-    "CreatePlatformVersionRequestRequestTypeDef",
     "CreateApplicationVersionMessageRequestTypeDef",
+    "CreatePlatformVersionRequestRequestTypeDef",
+    "ResourceTagsDescriptionMessageTypeDef",
+    "UpdateTagsForResourceMessageRequestTypeDef",
     "CreateConfigurationTemplateMessageRequestTypeDef",
     "CreateEnvironmentMessageRequestTypeDef",
     "DescribeConfigurationOptionsMessageRequestTypeDef",
     "UpdateConfigurationTemplateMessageRequestTypeDef",
     "UpdateEnvironmentMessageRequestTypeDef",
     "CreatePlatformVersionResultTypeDef",
     "DeletePlatformVersionResultTypeDef",
     "ListPlatformVersionsResultTypeDef",
+    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
+    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryResultTypeDef",
     "DescribeEnvironmentManagedActionsResultTypeDef",
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef",
     "RetrieveEnvironmentInfoResultMessageTypeDef",
     "EnvironmentResourceDescriptionTypeDef",
@@ -165,33 +158,31 @@
     "ListPlatformBranchesRequestRequestTypeDef",
     "ListPlatformBranchesResultTypeDef",
     "ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef",
     "ListPlatformVersionsRequestRequestTypeDef",
     "LoadBalancerDescriptionTypeDef",
     "PlatformDescriptionTypeDef",
     "ResourceQuotasTypeDef",
-    "ResourceTagsDescriptionMessageTypeDef",
     "DescribeEnvironmentHealthResultTypeDef",
     "ApplicationVersionDescriptionMessageTypeDef",
     "ApplicationVersionDescriptionsMessageTypeDef",
-    "ApplicationResourceLifecycleConfigOutputTypeDef",
     "ApplicationResourceLifecycleConfigTypeDef",
     "SingleInstanceHealthTypeDef",
     "ConfigurationOptionsDescriptionTypeDef",
     "ConfigurationSettingsDescriptionsTypeDef",
     "EnvironmentResourceDescriptionsMessageTypeDef",
     "EnvironmentResourcesDescriptionTypeDef",
     "DescribePlatformVersionResultTypeDef",
     "DescribeAccountAttributesResultTypeDef",
     "ApplicationDescriptionTypeDef",
     "ApplicationResourceLifecycleDescriptionMessageTypeDef",
     "CreateApplicationMessageRequestTypeDef",
     "UpdateApplicationResourceLifecycleMessageRequestTypeDef",
     "DescribeInstancesHealthResultTypeDef",
-    "EnvironmentDescriptionResponseMetadataTypeDef",
+    "EnvironmentDescriptionResponseTypeDef",
     "EnvironmentDescriptionTypeDef",
     "ApplicationDescriptionMessageTypeDef",
     "ApplicationDescriptionsMessageTypeDef",
     "EnvironmentDescriptionsMessageTypeDef",
 )
 
 AbortEnvironmentUpdateMessageRequestTypeDef = TypedDict(
@@ -199,14 +190,25 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
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
 LatencyTypeDef = TypedDict(
     "LatencyTypeDef",
     {
         "P999": float,
         "P99": float,
         "P95": float,
         "P90": float,
@@ -225,70 +227,32 @@
         "Status3xx": int,
         "Status4xx": int,
         "Status5xx": int,
     },
     total=False,
 )
 
-S3LocationOutputTypeDef = TypedDict(
-    "S3LocationOutputTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
         "S3Bucket": str,
         "S3Key": str,
     },
     total=False,
 )
 
-SourceBuildInformationOutputTypeDef = TypedDict(
-    "SourceBuildInformationOutputTypeDef",
+SourceBuildInformationTypeDef = TypedDict(
+    "SourceBuildInformationTypeDef",
     {
         "SourceType": SourceTypeType,
         "SourceRepository": SourceRepositoryType,
         "SourceLocation": str,
     },
 )
 
-_RequiredMaxAgeRuleOutputTypeDef = TypedDict(
-    "_RequiredMaxAgeRuleOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalMaxAgeRuleOutputTypeDef = TypedDict(
-    "_OptionalMaxAgeRuleOutputTypeDef",
-    {
-        "MaxAgeInDays": int,
-        "DeleteSourceFromS3": bool,
-    },
-    total=False,
-)
-
-class MaxAgeRuleOutputTypeDef(_RequiredMaxAgeRuleOutputTypeDef, _OptionalMaxAgeRuleOutputTypeDef):
-    pass
-
-_RequiredMaxCountRuleOutputTypeDef = TypedDict(
-    "_RequiredMaxCountRuleOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalMaxCountRuleOutputTypeDef = TypedDict(
-    "_OptionalMaxCountRuleOutputTypeDef",
-    {
-        "MaxCount": int,
-        "DeleteSourceFromS3": bool,
-    },
-    total=False,
-)
-
-class MaxCountRuleOutputTypeDef(
-    _RequiredMaxCountRuleOutputTypeDef, _OptionalMaxCountRuleOutputTypeDef
-):
-    pass
-
 _RequiredMaxAgeRuleTypeDef = TypedDict(
     "_RequiredMaxAgeRuleTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalMaxAgeRuleTypeDef = TypedDict(
@@ -338,25 +302,14 @@
 
 class ApplyEnvironmentManagedActionRequestRequestTypeDef(
     _RequiredApplyEnvironmentManagedActionRequestRequestTypeDef,
     _OptionalApplyEnvironmentManagedActionRequestRequestTypeDef,
 ):
     pass
 
-ApplyEnvironmentManagedActionResultTypeDef = TypedDict(
-    "ApplyEnvironmentManagedActionResultTypeDef",
-    {
-        "ActionId": str,
-        "ActionDescription": str,
-        "ActionType": ActionTypeType,
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateEnvironmentOperationsRoleMessageRequestTypeDef = TypedDict(
     "AssociateEnvironmentOperationsRoleMessageRequestTypeDef",
     {
         "EnvironmentName": str,
         "OperationsRole": str,
     },
 )
@@ -417,23 +370,14 @@
 CheckDNSAvailabilityMessageRequestTypeDef = TypedDict(
     "CheckDNSAvailabilityMessageRequestTypeDef",
     {
         "CNAMEPrefix": str,
     },
 )
 
-CheckDNSAvailabilityResultMessageTypeDef = TypedDict(
-    "CheckDNSAvailabilityResultMessageTypeDef",
-    {
-        "Available": bool,
-        "FullyQualifiedCNAME": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ComposeEnvironmentsMessageRequestTypeDef = TypedDict(
     "ComposeEnvironmentsMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "GroupName": str,
         "VersionLabels": Sequence[str],
     },
@@ -445,25 +389,14 @@
     {
         "Pattern": str,
         "Label": str,
     },
     total=False,
 )
 
-ConfigurationOptionSettingOutputTypeDef = TypedDict(
-    "ConfigurationOptionSettingOutputTypeDef",
-    {
-        "ResourceName": str,
-        "Namespace": str,
-        "OptionName": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 ConfigurationOptionSettingTypeDef = TypedDict(
     "ConfigurationOptionSettingTypeDef",
     {
         "ResourceName": str,
         "Namespace": str,
         "OptionName": str,
         "Value": str,
@@ -487,32 +420,14 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
-    {
-        "S3Bucket": str,
-        "S3Key": str,
-    },
-    total=False,
-)
-
-SourceBuildInformationTypeDef = TypedDict(
-    "SourceBuildInformationTypeDef",
-    {
-        "SourceType": SourceTypeType,
-        "SourceRepository": SourceRepositoryType,
-        "SourceLocation": str,
-    },
-)
-
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "ApplicationName": str,
         "TemplateName": str,
     },
     total=False,
@@ -553,22 +468,14 @@
         "PlatformVersion": str,
         "PlatformBranchName": str,
         "PlatformBranchLifecycleState": str,
     },
     total=False,
 )
 
-CreateStorageLocationResultMessageTypeDef = TypedDict(
-    "CreateStorageLocationResultMessageTypeDef",
-    {
-        "S3Bucket": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomAmiTypeDef = TypedDict(
     "CustomAmiTypeDef",
     {
         "VirtualizationType": str,
         "ImageId": str,
     },
     total=False,
@@ -645,20 +552,20 @@
         "DeploymentId": int,
         "Status": str,
         "DeploymentTime": datetime,
     },
     total=False,
 )
 
-DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef = TypedDict(
-    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ApplicationName": str,
-        "VersionLabels": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeApplicationVersionsMessageRequestTypeDef = TypedDict(
     "DescribeApplicationVersionsMessageRequestTypeDef",
     {
@@ -720,24 +627,14 @@
         "Warning": int,
         "Degraded": int,
         "Severe": int,
     },
     total=False,
 )
 
-DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
-    {
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef",
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
         "NextToken": str,
         "MaxItems": int,
@@ -787,28 +684,14 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
-DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "EnvironmentIds": Sequence[str],
-        "EnvironmentNames": Sequence[str],
-        "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -825,32 +708,14 @@
         "IncludedDeletedBackTo": Union[datetime, str],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "TemplateName": str,
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PlatformArn": str,
-        "RequestId": str,
-        "Severity": EventSeverityType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "TemplateName": str,
         "EnvironmentId": str,
@@ -888,40 +753,23 @@
 DisassociateEnvironmentOperationsRoleMessageRequestTypeDef = TypedDict(
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
     {
         "EnvironmentName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnvironmentLinkTypeDef = TypedDict(
     "EnvironmentLinkTypeDef",
     {
         "LinkName": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
-EnvironmentTierOutputTypeDef = TypedDict(
-    "EnvironmentTierOutputTypeDef",
-    {
-        "Name": str,
-        "Type": str,
-        "Version": str,
-    },
-    total=False,
-)
-
 EnvironmentInfoDescriptionTypeDef = TypedDict(
     "EnvironmentInfoDescriptionTypeDef",
     {
         "InfoType": EnvironmentInfoTypeType,
         "Ec2InstanceId": str,
         "SampleTimestamp": datetime,
         "Message": str,
@@ -1047,24 +895,14 @@
     {
         "Protocol": str,
         "Port": int,
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
 PlatformFrameworkTypeDef = TypedDict(
     "PlatformFrameworkTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
@@ -1113,34 +951,14 @@
     "ResourceQuotaTypeDef",
     {
         "Maximum": int,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
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
 RestartAppServerMessageRequestTypeDef = TypedDict(
     "RestartAppServerMessageRequestTypeDef",
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
@@ -1225,14 +1043,49 @@
 
 class UpdateApplicationVersionMessageRequestTypeDef(
     _RequiredUpdateApplicationVersionMessageRequestTypeDef,
     _OptionalUpdateApplicationVersionMessageRequestTypeDef,
 ):
     pass
 
+ApplyEnvironmentManagedActionResultTypeDef = TypedDict(
+    "ApplyEnvironmentManagedActionResultTypeDef",
+    {
+        "ActionId": str,
+        "ActionDescription": str,
+        "ActionType": ActionTypeType,
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CheckDNSAvailabilityResultMessageTypeDef = TypedDict(
+    "CheckDNSAvailabilityResultMessageTypeDef",
+    {
+        "Available": bool,
+        "FullyQualifiedCNAME": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStorageLocationResultMessageTypeDef = TypedDict(
+    "CreateStorageLocationResultMessageTypeDef",
+    {
+        "S3Bucket": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ApplicationMetricsTypeDef = TypedDict(
     "ApplicationMetricsTypeDef",
     {
         "Duration": int,
         "RequestCount": int,
         "StatusCodes": StatusCodesTypeDef,
         "Latency": LatencyTypeDef,
@@ -1243,33 +1096,24 @@
 ApplicationVersionDescriptionTypeDef = TypedDict(
     "ApplicationVersionDescriptionTypeDef",
     {
         "ApplicationVersionArn": str,
         "ApplicationName": str,
         "Description": str,
         "VersionLabel": str,
-        "SourceBuildInformation": SourceBuildInformationOutputTypeDef,
+        "SourceBuildInformation": SourceBuildInformationTypeDef,
         "BuildArn": str,
-        "SourceBundle": S3LocationOutputTypeDef,
+        "SourceBundle": S3LocationTypeDef,
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Status": ApplicationVersionStatusType,
     },
     total=False,
 )
 
-ApplicationVersionLifecycleConfigOutputTypeDef = TypedDict(
-    "ApplicationVersionLifecycleConfigOutputTypeDef",
-    {
-        "MaxCountRule": MaxCountRuleOutputTypeDef,
-        "MaxAgeRule": MaxAgeRuleOutputTypeDef,
-    },
-    total=False,
-)
-
 ApplicationVersionLifecycleConfigTypeDef = TypedDict(
     "ApplicationVersionLifecycleConfigTypeDef",
     {
         "MaxCountRule": MaxCountRuleTypeDef,
         "MaxAgeRule": MaxAgeRuleTypeDef,
     },
     total=False,
@@ -1298,28 +1142,28 @@
         "MaxValue": int,
         "MaxLength": int,
         "Regex": OptionRestrictionRegexTypeDef,
     },
     total=False,
 )
 
-ConfigurationSettingsDescriptionResponseMetadataTypeDef = TypedDict(
-    "ConfigurationSettingsDescriptionResponseMetadataTypeDef",
+ConfigurationSettingsDescriptionResponseTypeDef = TypedDict(
+    "ConfigurationSettingsDescriptionResponseTypeDef",
     {
         "SolutionStackName": str,
         "PlatformArn": str,
         "ApplicationName": str,
         "TemplateName": str,
         "Description": str,
         "EnvironmentName": str,
         "DeploymentStatus": ConfigurationDeploymentStatusType,
         "DateCreated": datetime,
         "DateUpdated": datetime,
-        "OptionSettings": List[ConfigurationOptionSettingOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OptionSettings": List[ConfigurationOptionSettingTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationSettingsDescriptionTypeDef = TypedDict(
     "ConfigurationSettingsDescriptionTypeDef",
     {
         "SolutionStackName": str,
@@ -1327,15 +1171,15 @@
         "ApplicationName": str,
         "TemplateName": str,
         "Description": str,
         "EnvironmentName": str,
         "DeploymentStatus": ConfigurationDeploymentStatusType,
         "DateCreated": datetime,
         "DateUpdated": datetime,
-        "OptionSettings": List[ConfigurationOptionSettingOutputTypeDef],
+        "OptionSettings": List[ConfigurationOptionSettingTypeDef],
     },
     total=False,
 )
 
 _RequiredValidateConfigurationSettingsMessageRequestTypeDef = TypedDict(
     "_RequiredValidateConfigurationSettingsMessageRequestTypeDef",
     {
@@ -1358,36 +1202,42 @@
 ):
     pass
 
 ConfigurationSettingsValidationMessagesTypeDef = TypedDict(
     "ConfigurationSettingsValidationMessagesTypeDef",
     {
         "Messages": List[ValidationMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
-    "_RequiredUpdateTagsForResourceMessageRequestTypeDef",
+_RequiredCreateApplicationVersionMessageRequestTypeDef = TypedDict(
+    "_RequiredCreateApplicationVersionMessageRequestTypeDef",
     {
-        "ResourceArn": str,
+        "ApplicationName": str,
+        "VersionLabel": str,
     },
 )
-_OptionalUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
-    "_OptionalUpdateTagsForResourceMessageRequestTypeDef",
+_OptionalCreateApplicationVersionMessageRequestTypeDef = TypedDict(
+    "_OptionalCreateApplicationVersionMessageRequestTypeDef",
     {
-        "TagsToAdd": Sequence[TagTypeDef],
-        "TagsToRemove": Sequence[str],
+        "Description": str,
+        "SourceBuildInformation": SourceBuildInformationTypeDef,
+        "SourceBundle": S3LocationTypeDef,
+        "BuildConfiguration": BuildConfigurationTypeDef,
+        "AutoCreateApplication": bool,
+        "Process": bool,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class UpdateTagsForResourceMessageRequestTypeDef(
-    _RequiredUpdateTagsForResourceMessageRequestTypeDef,
-    _OptionalUpdateTagsForResourceMessageRequestTypeDef,
+class CreateApplicationVersionMessageRequestTypeDef(
+    _RequiredCreateApplicationVersionMessageRequestTypeDef,
+    _OptionalCreateApplicationVersionMessageRequestTypeDef,
 ):
     pass
 
 _RequiredCreatePlatformVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePlatformVersionRequestRequestTypeDef",
     {
         "PlatformName": str,
@@ -1407,38 +1257,41 @@
 
 class CreatePlatformVersionRequestRequestTypeDef(
     _RequiredCreatePlatformVersionRequestRequestTypeDef,
     _OptionalCreatePlatformVersionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreateApplicationVersionMessageRequestTypeDef = TypedDict(
-    "_RequiredCreateApplicationVersionMessageRequestTypeDef",
+ResourceTagsDescriptionMessageTypeDef = TypedDict(
+    "ResourceTagsDescriptionMessageTypeDef",
     {
-        "ApplicationName": str,
-        "VersionLabel": str,
+        "ResourceArn": str,
+        "ResourceTags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateApplicationVersionMessageRequestTypeDef = TypedDict(
-    "_OptionalCreateApplicationVersionMessageRequestTypeDef",
+
+_RequiredUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_RequiredUpdateTagsForResourceMessageRequestTypeDef",
     {
-        "Description": str,
-        "SourceBuildInformation": SourceBuildInformationTypeDef,
-        "SourceBundle": S3LocationTypeDef,
-        "BuildConfiguration": BuildConfigurationTypeDef,
-        "AutoCreateApplication": bool,
-        "Process": bool,
-        "Tags": Sequence[TagTypeDef],
+        "ResourceArn": str,
+    },
+)
+_OptionalUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_OptionalUpdateTagsForResourceMessageRequestTypeDef",
+    {
+        "TagsToAdd": Sequence[TagTypeDef],
+        "TagsToRemove": Sequence[str],
     },
     total=False,
 )
 
-class CreateApplicationVersionMessageRequestTypeDef(
-    _RequiredCreateApplicationVersionMessageRequestTypeDef,
-    _OptionalCreateApplicationVersionMessageRequestTypeDef,
+class UpdateTagsForResourceMessageRequestTypeDef(
+    _RequiredUpdateTagsForResourceMessageRequestTypeDef,
+    _OptionalUpdateTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
 _RequiredCreateConfigurationTemplateMessageRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationTemplateMessageRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1552,49 +1405,101 @@
 )
 
 CreatePlatformVersionResultTypeDef = TypedDict(
     "CreatePlatformVersionResultTypeDef",
     {
         "PlatformSummary": PlatformSummaryTypeDef,
         "Builder": BuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePlatformVersionResultTypeDef = TypedDict(
     "DeletePlatformVersionResultTypeDef",
     {
         "PlatformSummary": PlatformSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlatformVersionsResultTypeDef = TypedDict(
     "ListPlatformVersionsResultTypeDef",
     {
         "PlatformSummaryList": List[PlatformSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef = TypedDict(
+    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabels": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
+    {
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "EnvironmentIds": Sequence[str],
+        "EnvironmentNames": Sequence[str],
+        "IncludeDeleted": bool,
+        "IncludedDeletedBackTo": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "TemplateName": str,
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PlatformArn": str,
+        "RequestId": str,
+        "Severity": EventSeverityType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 DescribeEnvironmentManagedActionHistoryResultTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionHistoryResultTypeDef",
     {
         "ManagedActionHistoryItems": List[ManagedActionHistoryItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEnvironmentManagedActionsResultTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionsResultTypeDef",
     {
         "ManagedActions": List[ManagedActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef = TypedDict(
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     {
         "ApplicationName": str,
@@ -1642,15 +1547,15 @@
     total=False,
 )
 
 RetrieveEnvironmentInfoResultMessageTypeDef = TypedDict(
     "RetrieveEnvironmentInfoResultMessageTypeDef",
     {
         "EnvironmentInfo": List[EnvironmentInfoDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentResourceDescriptionTypeDef = TypedDict(
     "EnvironmentResourceDescriptionTypeDef",
     {
         "EnvironmentName": str,
@@ -1666,24 +1571,24 @@
 )
 
 EventDescriptionsMessageTypeDef = TypedDict(
     "EventDescriptionsMessageTypeDef",
     {
         "Events": List[EventDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAvailableSolutionStacksResultMessageTypeDef = TypedDict(
     "ListAvailableSolutionStacksResultMessageTypeDef",
     {
         "SolutionStacks": List[str],
         "SolutionStackDetails": List[SolutionStackDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlatformBranchesRequestRequestTypeDef = TypedDict(
     "ListPlatformBranchesRequestRequestTypeDef",
     {
         "Filters": Sequence[SearchFilterTypeDef],
@@ -1694,23 +1599,23 @@
 )
 
 ListPlatformBranchesResultTypeDef = TypedDict(
     "ListPlatformBranchesResultTypeDef",
     {
         "PlatformBranchSummaryList": List[PlatformBranchSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef = TypedDict(
     "ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef",
     {
         "Filters": Sequence[PlatformFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListPlatformVersionsRequestRequestTypeDef = TypedDict(
     "ListPlatformVersionsRequestRequestTypeDef",
     {
@@ -1767,64 +1672,46 @@
         "EnvironmentQuota": ResourceQuotaTypeDef,
         "ConfigurationTemplateQuota": ResourceQuotaTypeDef,
         "CustomPlatformQuota": ResourceQuotaTypeDef,
     },
     total=False,
 )
 
-ResourceTagsDescriptionMessageTypeDef = TypedDict(
-    "ResourceTagsDescriptionMessageTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourceTags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeEnvironmentHealthResultTypeDef = TypedDict(
     "DescribeEnvironmentHealthResultTypeDef",
     {
         "EnvironmentName": str,
         "HealthStatus": str,
         "Status": EnvironmentHealthType,
         "Color": str,
         "Causes": List[str],
         "ApplicationMetrics": ApplicationMetricsTypeDef,
         "InstancesHealth": InstanceHealthSummaryTypeDef,
         "RefreshedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationVersionDescriptionMessageTypeDef = TypedDict(
     "ApplicationVersionDescriptionMessageTypeDef",
     {
         "ApplicationVersion": ApplicationVersionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationVersionDescriptionsMessageTypeDef = TypedDict(
     "ApplicationVersionDescriptionsMessageTypeDef",
     {
         "ApplicationVersions": List[ApplicationVersionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ApplicationResourceLifecycleConfigOutputTypeDef = TypedDict(
-    "ApplicationResourceLifecycleConfigOutputTypeDef",
-    {
-        "ServiceRole": str,
-        "VersionLifecycleConfig": ApplicationVersionLifecycleConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 ApplicationResourceLifecycleConfigTypeDef = TypedDict(
     "ApplicationResourceLifecycleConfigTypeDef",
     {
         "ServiceRole": str,
         "VersionLifecycleConfig": ApplicationVersionLifecycleConfigTypeDef,
     },
     total=False,
@@ -1849,31 +1736,31 @@
 
 ConfigurationOptionsDescriptionTypeDef = TypedDict(
     "ConfigurationOptionsDescriptionTypeDef",
     {
         "SolutionStackName": str,
         "PlatformArn": str,
         "Options": List[ConfigurationOptionDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationSettingsDescriptionsTypeDef = TypedDict(
     "ConfigurationSettingsDescriptionsTypeDef",
     {
         "ConfigurationSettings": List[ConfigurationSettingsDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentResourceDescriptionsMessageTypeDef = TypedDict(
     "EnvironmentResourceDescriptionsMessageTypeDef",
     {
         "EnvironmentResources": EnvironmentResourceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentResourcesDescriptionTypeDef = TypedDict(
     "EnvironmentResourcesDescriptionTypeDef",
     {
         "LoadBalancer": LoadBalancerDescriptionTypeDef,
@@ -1881,47 +1768,47 @@
     total=False,
 )
 
 DescribePlatformVersionResultTypeDef = TypedDict(
     "DescribePlatformVersionResultTypeDef",
     {
         "PlatformDescription": PlatformDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "ResourceQuotas": ResourceQuotasTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationDescriptionTypeDef = TypedDict(
     "ApplicationDescriptionTypeDef",
     {
         "ApplicationArn": str,
         "ApplicationName": str,
         "Description": str,
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Versions": List[str],
         "ConfigurationTemplates": List[str],
-        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigOutputTypeDef,
+        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
     },
     total=False,
 )
 
 ApplicationResourceLifecycleDescriptionMessageTypeDef = TypedDict(
     "ApplicationResourceLifecycleDescriptionMessageTypeDef",
     {
         "ApplicationName": str,
-        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateApplicationMessageRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationMessageRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1952,20 +1839,20 @@
 
 DescribeInstancesHealthResultTypeDef = TypedDict(
     "DescribeInstancesHealthResultTypeDef",
     {
         "InstanceHealthList": List[SingleInstanceHealthTypeDef],
         "RefreshedAt": datetime,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EnvironmentDescriptionResponseMetadataTypeDef = TypedDict(
-    "EnvironmentDescriptionResponseMetadataTypeDef",
+EnvironmentDescriptionResponseTypeDef = TypedDict(
+    "EnvironmentDescriptionResponseTypeDef",
     {
         "EnvironmentName": str,
         "EnvironmentId": str,
         "ApplicationName": str,
         "VersionLabel": str,
         "SolutionStackName": str,
         "PlatformArn": str,
@@ -1976,19 +1863,19 @@
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Status": EnvironmentStatusType,
         "AbortableOperationInProgress": bool,
         "Health": EnvironmentHealthType,
         "HealthStatus": EnvironmentHealthStatusType,
         "Resources": EnvironmentResourcesDescriptionTypeDef,
-        "Tier": EnvironmentTierOutputTypeDef,
+        "Tier": EnvironmentTierTypeDef,
         "EnvironmentLinks": List[EnvironmentLinkTypeDef],
         "EnvironmentArn": str,
         "OperationsRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentDescriptionTypeDef = TypedDict(
     "EnvironmentDescriptionTypeDef",
     {
         "EnvironmentName": str,
@@ -2004,39 +1891,39 @@
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Status": EnvironmentStatusType,
         "AbortableOperationInProgress": bool,
         "Health": EnvironmentHealthType,
         "HealthStatus": EnvironmentHealthStatusType,
         "Resources": EnvironmentResourcesDescriptionTypeDef,
-        "Tier": EnvironmentTierOutputTypeDef,
+        "Tier": EnvironmentTierTypeDef,
         "EnvironmentLinks": List[EnvironmentLinkTypeDef],
         "EnvironmentArn": str,
         "OperationsRole": str,
     },
     total=False,
 )
 
 ApplicationDescriptionMessageTypeDef = TypedDict(
     "ApplicationDescriptionMessageTypeDef",
     {
         "Application": ApplicationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationDescriptionsMessageTypeDef = TypedDict(
     "ApplicationDescriptionsMessageTypeDef",
     {
         "Applications": List[ApplicationDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentDescriptionsMessageTypeDef = TypedDict(
     "EnvironmentDescriptionsMessageTypeDef",
     {
         "Environments": List[EnvironmentDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/waiter.py` & `mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/waiter.pyi` & `mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO` & `mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticbeanstalk
-Version: 1.28.12
-Summary: Type annotations for boto3.ElasticBeanstalk 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ElasticBeanstalk 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticbeanstalk)](https://pepy.tech/project/mypy-boto3-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticBeanstalk 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[boto3.ElasticBeanstalk 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [mypy-boto3-elasticbeanstalk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -395,123 +395,116 @@
 
 `mypy_boto3_elasticbeanstalk.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticbeanstalk.type_defs import (
     AbortEnvironmentUpdateMessageRequestTypeDef,
+    ResponseMetadataTypeDef,
     LatencyTypeDef,
     StatusCodesTypeDef,
-    S3LocationOutputTypeDef,
-    SourceBuildInformationOutputTypeDef,
-    MaxAgeRuleOutputTypeDef,
-    MaxCountRuleOutputTypeDef,
+    S3LocationTypeDef,
+    SourceBuildInformationTypeDef,
     MaxAgeRuleTypeDef,
     MaxCountRuleTypeDef,
     ApplyEnvironmentManagedActionRequestRequestTypeDef,
-    ApplyEnvironmentManagedActionResultTypeDef,
     AssociateEnvironmentOperationsRoleMessageRequestTypeDef,
     AutoScalingGroupTypeDef,
     BuildConfigurationTypeDef,
     BuilderTypeDef,
     CPUUtilizationTypeDef,
     CheckDNSAvailabilityMessageRequestTypeDef,
-    CheckDNSAvailabilityResultMessageTypeDef,
     ComposeEnvironmentsMessageRequestTypeDef,
     OptionRestrictionRegexTypeDef,
-    ConfigurationOptionSettingOutputTypeDef,
     ConfigurationOptionSettingTypeDef,
     ValidationMessageTypeDef,
     TagTypeDef,
-    S3LocationTypeDef,
-    SourceBuildInformationTypeDef,
     SourceConfigurationTypeDef,
     EnvironmentTierTypeDef,
     OptionSpecificationTypeDef,
     PlatformSummaryTypeDef,
-    CreateStorageLocationResultMessageTypeDef,
     CustomAmiTypeDef,
     DeleteApplicationMessageRequestTypeDef,
     DeleteApplicationVersionMessageRequestTypeDef,
     DeleteConfigurationTemplateMessageRequestTypeDef,
     DeleteEnvironmentConfigurationMessageRequestTypeDef,
     DeletePlatformVersionRequestRequestTypeDef,
     DeploymentTypeDef,
-    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeApplicationVersionsMessageRequestTypeDef,
     DescribeApplicationsMessageRequestTypeDef,
     DescribeConfigurationSettingsMessageRequestTypeDef,
     DescribeEnvironmentHealthRequestRequestTypeDef,
     InstanceHealthSummaryTypeDef,
-    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef,
     ManagedActionHistoryItemTypeDef,
     DescribeEnvironmentManagedActionsRequestRequestTypeDef,
     ManagedActionTypeDef,
     DescribeEnvironmentResourcesMessageRequestTypeDef,
-    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeEnvironmentsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeInstancesHealthRequestRequestTypeDef,
     DescribePlatformVersionRequestRequestTypeDef,
     DisassociateEnvironmentOperationsRoleMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnvironmentLinkTypeDef,
-    EnvironmentTierOutputTypeDef,
     EnvironmentInfoDescriptionTypeDef,
     InstanceTypeDef,
     LaunchConfigurationTypeDef,
     LaunchTemplateTypeDef,
     LoadBalancerTypeDef,
     QueueTypeDef,
     TriggerTypeDef,
     EventDescriptionTypeDef,
     SolutionStackDescriptionTypeDef,
     SearchFilterTypeDef,
     PlatformBranchSummaryTypeDef,
     PlatformFilterTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ListenerTypeDef,
-    PaginatorConfigTypeDef,
     PlatformFrameworkTypeDef,
     PlatformProgrammingLanguageTypeDef,
     RebuildEnvironmentMessageRequestTypeDef,
     RequestEnvironmentInfoMessageRequestTypeDef,
     ResourceQuotaTypeDef,
-    TagOutputTypeDef,
-    ResponseMetadataTypeDef,
     RestartAppServerMessageRequestTypeDef,
     RetrieveEnvironmentInfoMessageRequestTypeDef,
     SwapEnvironmentCNAMEsMessageRequestTypeDef,
     TerminateEnvironmentMessageRequestTypeDef,
     UpdateApplicationMessageRequestTypeDef,
     UpdateApplicationVersionMessageRequestTypeDef,
+    ApplyEnvironmentManagedActionResultTypeDef,
+    CheckDNSAvailabilityResultMessageTypeDef,
+    CreateStorageLocationResultMessageTypeDef,
+    EmptyResponseMetadataTypeDef,
     ApplicationMetricsTypeDef,
     ApplicationVersionDescriptionTypeDef,
-    ApplicationVersionLifecycleConfigOutputTypeDef,
     ApplicationVersionLifecycleConfigTypeDef,
     SystemStatusTypeDef,
     ConfigurationOptionDescriptionTypeDef,
-    ConfigurationSettingsDescriptionResponseMetadataTypeDef,
+    ConfigurationSettingsDescriptionResponseTypeDef,
     ConfigurationSettingsDescriptionTypeDef,
     ValidateConfigurationSettingsMessageRequestTypeDef,
     ConfigurationSettingsValidationMessagesTypeDef,
-    UpdateTagsForResourceMessageRequestTypeDef,
-    CreatePlatformVersionRequestRequestTypeDef,
     CreateApplicationVersionMessageRequestTypeDef,
+    CreatePlatformVersionRequestRequestTypeDef,
+    ResourceTagsDescriptionMessageTypeDef,
+    UpdateTagsForResourceMessageRequestTypeDef,
     CreateConfigurationTemplateMessageRequestTypeDef,
     CreateEnvironmentMessageRequestTypeDef,
     DescribeConfigurationOptionsMessageRequestTypeDef,
     UpdateConfigurationTemplateMessageRequestTypeDef,
     UpdateEnvironmentMessageRequestTypeDef,
     CreatePlatformVersionResultTypeDef,
     DeletePlatformVersionResultTypeDef,
     ListPlatformVersionsResultTypeDef,
+    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
+    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
+    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
     DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     EnvironmentResourceDescriptionTypeDef,
@@ -520,33 +513,31 @@
     ListPlatformBranchesRequestRequestTypeDef,
     ListPlatformBranchesResultTypeDef,
     ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef,
     ListPlatformVersionsRequestRequestTypeDef,
     LoadBalancerDescriptionTypeDef,
     PlatformDescriptionTypeDef,
     ResourceQuotasTypeDef,
-    ResourceTagsDescriptionMessageTypeDef,
     DescribeEnvironmentHealthResultTypeDef,
     ApplicationVersionDescriptionMessageTypeDef,
     ApplicationVersionDescriptionsMessageTypeDef,
-    ApplicationResourceLifecycleConfigOutputTypeDef,
     ApplicationResourceLifecycleConfigTypeDef,
     SingleInstanceHealthTypeDef,
     ConfigurationOptionsDescriptionTypeDef,
     ConfigurationSettingsDescriptionsTypeDef,
     EnvironmentResourceDescriptionsMessageTypeDef,
     EnvironmentResourcesDescriptionTypeDef,
     DescribePlatformVersionResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     ApplicationDescriptionTypeDef,
     ApplicationResourceLifecycleDescriptionMessageTypeDef,
     CreateApplicationMessageRequestTypeDef,
     UpdateApplicationResourceLifecycleMessageRequestTypeDef,
     DescribeInstancesHealthResultTypeDef,
-    EnvironmentDescriptionResponseMetadataTypeDef,
+    EnvironmentDescriptionResponseTypeDef,
     EnvironmentDescriptionTypeDef,
     ApplicationDescriptionMessageTypeDef,
     ApplicationDescriptionsMessageTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
 )
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt` & `mypy-boto3-elasticbeanstalk-1.28.15/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.12/setup.py` & `mypy-boto3-elasticbeanstalk-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elasticbeanstalk",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_elasticbeanstalk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticBeanstalk 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ElasticBeanstalk 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

