# Comparing `tmp/mypy-boto3-ds-1.28.12.tar.gz` & `tmp/mypy-boto3-ds-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ds-1.28.12.tar", last modified: Thu Jul 27 05:34:35 2023, max compression
+gzip compressed data, was "mypy-boto3-ds-1.28.15.tar", last modified: Fri Jul 28 20:42:40 2023, max compression
```

## Comparing `mypy-boto3-ds-1.28.12.tar` & `mypy-boto3-ds-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.860529 mypy-boto3-ds-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22251 2023-07-27 05:34:35.856529 mypy-boto3-ds-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20770 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.856529 mypy-boto3-ds-1.28.12/mypy_boto3_ds/
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51628 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51540 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17026 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17009 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59090 2023-07-27 05:20:33.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59017 2023-07-27 05:20:33.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.856529 mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22251 2023-07-27 05:34:35.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-27 05:34:35.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:35.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:35.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:35.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 05:34:35.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:35.860529 mypy-boto3-ds-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-27 05:20:31.000000 mypy-boto3-ds-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:40.700998 mypy-boto3-ds-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-07-28 20:42:40.692998 mypy-boto3-ds-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20644 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:40.680998 mypy-boto3-ds-1.28.15/mypy_boto3_ds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51628 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51540 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-07-28 20:23:23.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-07-28 20:23:23.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16998 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58274 2023-07-28 20:23:25.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58201 2023-07-28 20:23:24.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:40.692998 mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-07-28 20:42:40.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-28 20:42:40.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:40.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:40.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:40.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 20:42:40.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:40.700998 mypy-boto3-ds-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/setup.py
```

### Comparing `mypy-boto3-ds-1.28.12/LICENSE` & `mypy-boto3-ds-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.12/PKG-INFO` & `mypy-boto3-ds-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ds
-Version: 1.28.12
-Summary: Type annotations for boto3.DirectoryService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DirectoryService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ds.svg?color=blue)](https://pypi.org/project/mypy-boto3-ds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ds)](https://pepy.tech/project/mypy-boto3-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectoryService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[boto3.DirectoryService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
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
 [mypy-boto3-ds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/).
 
 See how it helps to find and fix potential bugs:
 
@@ -410,75 +410,57 @@
 
 `mypy_boto3_ds.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ds.type_defs import (
     AcceptSharedDirectoryRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SharedDirectoryTypeDef,
     IpRouteTypeDef,
     DirectoryVpcSettingsTypeDef,
     TagTypeDef,
-    AttributeOutputTypeDef,
     AttributeTypeDef,
     CancelSchemaExtensionRequestRequestTypeDef,
     CertificateInfoTypeDef,
-    ClientCertAuthSettingsOutputTypeDef,
-    ClientAuthenticationSettingInfoTypeDef,
     ClientCertAuthSettingsTypeDef,
+    ClientAuthenticationSettingInfoTypeDef,
     ConditionalForwarderTypeDef,
     DirectoryConnectSettingsTypeDef,
-    ConnectDirectoryResultTypeDef,
     CreateAliasRequestRequestTypeDef,
-    CreateAliasResultTypeDef,
     CreateConditionalForwarderRequestRequestTypeDef,
-    CreateDirectoryResultTypeDef,
     CreateLogSubscriptionRequestRequestTypeDef,
-    CreateMicrosoftADResultTypeDef,
     CreateSnapshotRequestRequestTypeDef,
-    CreateSnapshotResultTypeDef,
     CreateTrustRequestRequestTypeDef,
-    CreateTrustResultTypeDef,
     DeleteConditionalForwarderRequestRequestTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
-    DeleteDirectoryResultTypeDef,
     DeleteLogSubscriptionRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
-    DeleteSnapshotResultTypeDef,
     DeleteTrustRequestRequestTypeDef,
-    DeleteTrustResultTypeDef,
     DeregisterCertificateRequestRequestTypeDef,
     DeregisterEventTopicRequestRequestTypeDef,
     DescribeCertificateRequestRequestTypeDef,
-    DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClientAuthenticationSettingsRequestRequestTypeDef,
     DescribeConditionalForwardersRequestRequestTypeDef,
-    DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef,
     DescribeDirectoriesRequestRequestTypeDef,
-    DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
     DescribeDomainControllersRequestRequestTypeDef,
     DomainControllerTypeDef,
     DescribeEventTopicsRequestRequestTypeDef,
     EventTopicTypeDef,
-    DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
     DescribeLDAPSSettingsRequestRequestTypeDef,
     LDAPSSettingInfoTypeDef,
-    DescribeRegionsRequestDescribeRegionsPaginateTypeDef,
     DescribeRegionsRequestRequestTypeDef,
     DescribeSettingsRequestRequestTypeDef,
     SettingEntryTypeDef,
-    DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
     DescribeSharedDirectoriesRequestRequestTypeDef,
-    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
-    DescribeTrustsRequestDescribeTrustsPaginateTypeDef,
     DescribeTrustsRequestRequestTypeDef,
     TrustTypeDef,
-    DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
     DescribeUpdateDirectoryRequestRequestTypeDef,
     DirectoryConnectSettingsDescriptionTypeDef,
     DirectoryVpcSettingsDescriptionTypeDef,
     RadiusSettingsOutputTypeDef,
     RegionsInfoTypeDef,
     DirectoryLimitsTypeDef,
     DirectoryVpcSettingsOutputTypeDef,
@@ -489,69 +471,84 @@
     EnableClientAuthenticationRequestRequestTypeDef,
     EnableLDAPSRequestRequestTypeDef,
     RadiusSettingsTypeDef,
     EnableSsoRequestRequestTypeDef,
     GetSnapshotLimitsRequestRequestTypeDef,
     SnapshotLimitsTypeDef,
     IpRouteInfoTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
-    ListIpRoutesRequestListIpRoutesPaginateTypeDef,
     ListIpRoutesRequestRequestTypeDef,
-    ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef,
     ListLogSubscriptionsRequestRequestTypeDef,
     LogSubscriptionTypeDef,
-    ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
     ListSchemaExtensionsRequestRequestTypeDef,
     SchemaExtensionInfoTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    OSUpdateSettingsOutputTypeDef,
     OSUpdateSettingsTypeDef,
-    PaginatorConfigTypeDef,
-    RegisterCertificateResultTypeDef,
     RegisterEventTopicRequestRequestTypeDef,
     RejectSharedDirectoryRequestRequestTypeDef,
-    RejectSharedDirectoryResultTypeDef,
     RemoveIpRoutesRequestRequestTypeDef,
     RemoveRegionRequestRequestTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetUserPasswordRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     SettingTypeDef,
     ShareTargetTypeDef,
-    ShareDirectoryResultTypeDef,
     StartSchemaExtensionRequestRequestTypeDef,
-    StartSchemaExtensionResultTypeDef,
     UnshareTargetTypeDef,
-    UnshareDirectoryResultTypeDef,
     UpdateConditionalForwarderRequestRequestTypeDef,
     UpdateNumberOfDomainControllersRequestRequestTypeDef,
-    UpdateSettingsResultTypeDef,
     UpdateTrustRequestRequestTypeDef,
-    UpdateTrustResultTypeDef,
     VerifyTrustRequestRequestTypeDef,
+    ConnectDirectoryResultTypeDef,
+    CreateAliasResultTypeDef,
+    CreateDirectoryResultTypeDef,
+    CreateMicrosoftADResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    CreateTrustResultTypeDef,
+    DeleteDirectoryResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DeleteTrustResultTypeDef,
+    RegisterCertificateResultTypeDef,
+    RejectSharedDirectoryResultTypeDef,
+    ShareDirectoryResultTypeDef,
+    StartSchemaExtensionResultTypeDef,
+    UnshareDirectoryResultTypeDef,
+    UpdateSettingsResultTypeDef,
+    UpdateTrustResultTypeDef,
     VerifyTrustResultTypeDef,
     AcceptSharedDirectoryResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     AddIpRoutesRequestRequestTypeDef,
     AddRegionRequestRequestTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateDirectoryRequestRequestTypeDef,
     CreateMicrosoftADRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     ComputerTypeDef,
     CreateComputerRequestRequestTypeDef,
     ListCertificatesResultTypeDef,
     CertificateTypeDef,
-    DescribeClientAuthenticationSettingsResultTypeDef,
     RegisterCertificateRequestRequestTypeDef,
+    DescribeClientAuthenticationSettingsResultTypeDef,
     DescribeConditionalForwardersResultTypeDef,
     ConnectDirectoryRequestRequestTypeDef,
+    DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef,
+    DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
+    DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
+    DescribeRegionsRequestDescribeRegionsPaginateTypeDef,
+    DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
+    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
+    DescribeTrustsRequestDescribeTrustsPaginateTypeDef,
+    DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListIpRoutesRequestListIpRoutesPaginateTypeDef,
+    ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef,
+    ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeDomainControllersResultTypeDef,
     DescribeEventTopicsResultTypeDef,
     DescribeLDAPSSettingsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
     OwnerDirectoryDescriptionTypeDef,
@@ -559,17 +556,16 @@
     RegionDescriptionTypeDef,
     EnableRadiusRequestRequestTypeDef,
     UpdateRadiusRequestRequestTypeDef,
     GetSnapshotLimitsResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    UpdateValueTypeDef,
     UpdateDirectorySetupRequestRequestTypeDef,
+    UpdateValueTypeDef,
     UpdateSettingsRequestRequestTypeDef,
     ShareDirectoryRequestRequestTypeDef,
     UnshareDirectoryRequestRequestTypeDef,
     CreateComputerResultTypeDef,
     DescribeCertificateResultTypeDef,
     DirectoryDescriptionTypeDef,
     DescribeRegionsResultTypeDef,
```

### Comparing `mypy-boto3-ds-1.28.12/README.md` & `mypy-boto3-ds-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ds.svg?color=blue)](https://pypi.org/project/mypy-boto3-ds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ds)](https://pepy.tech/project/mypy-boto3-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectoryService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[boto3.DirectoryService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
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
 [mypy-boto3-ds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/).
 
 See how it helps to find and fix potential bugs:
 
@@ -378,75 +378,57 @@
 
 `mypy_boto3_ds.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ds.type_defs import (
     AcceptSharedDirectoryRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SharedDirectoryTypeDef,
     IpRouteTypeDef,
     DirectoryVpcSettingsTypeDef,
     TagTypeDef,
-    AttributeOutputTypeDef,
     AttributeTypeDef,
     CancelSchemaExtensionRequestRequestTypeDef,
     CertificateInfoTypeDef,
-    ClientCertAuthSettingsOutputTypeDef,
-    ClientAuthenticationSettingInfoTypeDef,
     ClientCertAuthSettingsTypeDef,
+    ClientAuthenticationSettingInfoTypeDef,
     ConditionalForwarderTypeDef,
     DirectoryConnectSettingsTypeDef,
-    ConnectDirectoryResultTypeDef,
     CreateAliasRequestRequestTypeDef,
-    CreateAliasResultTypeDef,
     CreateConditionalForwarderRequestRequestTypeDef,
-    CreateDirectoryResultTypeDef,
     CreateLogSubscriptionRequestRequestTypeDef,
-    CreateMicrosoftADResultTypeDef,
     CreateSnapshotRequestRequestTypeDef,
-    CreateSnapshotResultTypeDef,
     CreateTrustRequestRequestTypeDef,
-    CreateTrustResultTypeDef,
     DeleteConditionalForwarderRequestRequestTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
-    DeleteDirectoryResultTypeDef,
     DeleteLogSubscriptionRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
-    DeleteSnapshotResultTypeDef,
     DeleteTrustRequestRequestTypeDef,
-    DeleteTrustResultTypeDef,
     DeregisterCertificateRequestRequestTypeDef,
     DeregisterEventTopicRequestRequestTypeDef,
     DescribeCertificateRequestRequestTypeDef,
-    DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClientAuthenticationSettingsRequestRequestTypeDef,
     DescribeConditionalForwardersRequestRequestTypeDef,
-    DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef,
     DescribeDirectoriesRequestRequestTypeDef,
-    DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
     DescribeDomainControllersRequestRequestTypeDef,
     DomainControllerTypeDef,
     DescribeEventTopicsRequestRequestTypeDef,
     EventTopicTypeDef,
-    DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
     DescribeLDAPSSettingsRequestRequestTypeDef,
     LDAPSSettingInfoTypeDef,
-    DescribeRegionsRequestDescribeRegionsPaginateTypeDef,
     DescribeRegionsRequestRequestTypeDef,
     DescribeSettingsRequestRequestTypeDef,
     SettingEntryTypeDef,
-    DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
     DescribeSharedDirectoriesRequestRequestTypeDef,
-    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
-    DescribeTrustsRequestDescribeTrustsPaginateTypeDef,
     DescribeTrustsRequestRequestTypeDef,
     TrustTypeDef,
-    DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
     DescribeUpdateDirectoryRequestRequestTypeDef,
     DirectoryConnectSettingsDescriptionTypeDef,
     DirectoryVpcSettingsDescriptionTypeDef,
     RadiusSettingsOutputTypeDef,
     RegionsInfoTypeDef,
     DirectoryLimitsTypeDef,
     DirectoryVpcSettingsOutputTypeDef,
@@ -457,69 +439,84 @@
     EnableClientAuthenticationRequestRequestTypeDef,
     EnableLDAPSRequestRequestTypeDef,
     RadiusSettingsTypeDef,
     EnableSsoRequestRequestTypeDef,
     GetSnapshotLimitsRequestRequestTypeDef,
     SnapshotLimitsTypeDef,
     IpRouteInfoTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
-    ListIpRoutesRequestListIpRoutesPaginateTypeDef,
     ListIpRoutesRequestRequestTypeDef,
-    ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef,
     ListLogSubscriptionsRequestRequestTypeDef,
     LogSubscriptionTypeDef,
-    ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
     ListSchemaExtensionsRequestRequestTypeDef,
     SchemaExtensionInfoTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    OSUpdateSettingsOutputTypeDef,
     OSUpdateSettingsTypeDef,
-    PaginatorConfigTypeDef,
-    RegisterCertificateResultTypeDef,
     RegisterEventTopicRequestRequestTypeDef,
     RejectSharedDirectoryRequestRequestTypeDef,
-    RejectSharedDirectoryResultTypeDef,
     RemoveIpRoutesRequestRequestTypeDef,
     RemoveRegionRequestRequestTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetUserPasswordRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     SettingTypeDef,
     ShareTargetTypeDef,
-    ShareDirectoryResultTypeDef,
     StartSchemaExtensionRequestRequestTypeDef,
-    StartSchemaExtensionResultTypeDef,
     UnshareTargetTypeDef,
-    UnshareDirectoryResultTypeDef,
     UpdateConditionalForwarderRequestRequestTypeDef,
     UpdateNumberOfDomainControllersRequestRequestTypeDef,
-    UpdateSettingsResultTypeDef,
     UpdateTrustRequestRequestTypeDef,
-    UpdateTrustResultTypeDef,
     VerifyTrustRequestRequestTypeDef,
+    ConnectDirectoryResultTypeDef,
+    CreateAliasResultTypeDef,
+    CreateDirectoryResultTypeDef,
+    CreateMicrosoftADResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    CreateTrustResultTypeDef,
+    DeleteDirectoryResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DeleteTrustResultTypeDef,
+    RegisterCertificateResultTypeDef,
+    RejectSharedDirectoryResultTypeDef,
+    ShareDirectoryResultTypeDef,
+    StartSchemaExtensionResultTypeDef,
+    UnshareDirectoryResultTypeDef,
+    UpdateSettingsResultTypeDef,
+    UpdateTrustResultTypeDef,
     VerifyTrustResultTypeDef,
     AcceptSharedDirectoryResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     AddIpRoutesRequestRequestTypeDef,
     AddRegionRequestRequestTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateDirectoryRequestRequestTypeDef,
     CreateMicrosoftADRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     ComputerTypeDef,
     CreateComputerRequestRequestTypeDef,
     ListCertificatesResultTypeDef,
     CertificateTypeDef,
-    DescribeClientAuthenticationSettingsResultTypeDef,
     RegisterCertificateRequestRequestTypeDef,
+    DescribeClientAuthenticationSettingsResultTypeDef,
     DescribeConditionalForwardersResultTypeDef,
     ConnectDirectoryRequestRequestTypeDef,
+    DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef,
+    DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
+    DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
+    DescribeRegionsRequestDescribeRegionsPaginateTypeDef,
+    DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
+    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
+    DescribeTrustsRequestDescribeTrustsPaginateTypeDef,
+    DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListIpRoutesRequestListIpRoutesPaginateTypeDef,
+    ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef,
+    ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeDomainControllersResultTypeDef,
     DescribeEventTopicsResultTypeDef,
     DescribeLDAPSSettingsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
     OwnerDirectoryDescriptionTypeDef,
@@ -527,17 +524,16 @@
     RegionDescriptionTypeDef,
     EnableRadiusRequestRequestTypeDef,
     UpdateRadiusRequestRequestTypeDef,
     GetSnapshotLimitsResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    UpdateValueTypeDef,
     UpdateDirectorySetupRequestRequestTypeDef,
+    UpdateValueTypeDef,
     UpdateSettingsRequestRequestTypeDef,
     ShareDirectoryRequestRequestTypeDef,
     UnshareDirectoryRequestRequestTypeDef,
     CreateComputerResultTypeDef,
     DescribeCertificateResultTypeDef,
     DirectoryDescriptionTypeDef,
     DescribeRegionsResultTypeDef,
```

### Comparing `mypy-boto3-ds-1.28.12/mypy_boto3_ds/__init__.py` & `mypy-boto3-ds-1.28.15/mypy_boto3_ds/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.12/mypy_boto3_ds/__init__.pyi` & `mypy-boto3-ds-1.28.15/mypy_boto3_ds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.12/mypy_boto3_ds/__main__.py` & `mypy-boto3-ds-1.28.15/mypy_boto3_ds/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DirectoryService 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.DirectoryService 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService\nOther"
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

### Comparing `mypy-boto3-ds-1.28.12/mypy_boto3_ds/client.py` & `mypy-boto3-ds-1.28.15/mypy_boto3_ds/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.12/mypy_boto3_ds/client.pyi` & `mypy-boto3-ds-1.28.15/mypy_boto3_ds/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.12/mypy_boto3_ds/literals.py` & `mypy-boto3-ds-1.28.15/mypy_boto3_ds/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.12/mypy_boto3_ds/literals.pyi` & `mypy-boto3-ds-1.28.15/mypy_boto3_ds/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.12/mypy_boto3_ds/paginator.py` & `mypy-boto3-ds-1.28.15/mypy_boto3_ds/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,30 +110,30 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         Type: ClientAuthenticationTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeClientAuthenticationSettingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeClientAuthenticationSettings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describeclientauthenticationsettingspaginator)
         """
 
 
 class DescribeDirectoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDirectories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describedirectoriespaginator)
     """
 
     def paginate(
-        self, *, DirectoryIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDirectories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describedirectoriespaginator)
         """
 
 
@@ -144,15 +144,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         DomainControllerIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDomainControllersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDomainControllers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describedomaincontrollerspaginator)
         """
 
 
@@ -163,15 +163,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         Type: Literal["Client"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeLDAPSSettingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeLDAPSSettings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describeldapssettingspaginator)
         """
 
 
@@ -182,15 +182,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         RegionName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRegionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeRegions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describeregionspaginator)
         """
 
 
@@ -201,15 +201,15 @@
     """
 
     def paginate(
         self,
         *,
         OwnerDirectoryId: str,
         SharedDirectoryIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSharedDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSharedDirectories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describeshareddirectoriespaginator)
         """
 
 
@@ -220,15 +220,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str = ...,
         SnapshotIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describesnapshotspaginator)
         """
 
 
@@ -239,15 +239,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str = ...,
         TrustIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTrustsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeTrusts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describetrustspaginator)
         """
 
 
@@ -259,88 +259,88 @@
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         UpdateType: Literal["OS"],
         RegionName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeUpdateDirectoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeUpdateDirectory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describeupdatedirectorypaginator)
         """
 
 
 class ListCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listcertificatespaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCertificatesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listcertificatespaginator)
         """
 
 
 class ListIpRoutesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListIpRoutes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listiproutespaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIpRoutesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListIpRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listiproutespaginator)
         """
 
 
 class ListLogSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListLogSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listlogsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLogSubscriptionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListLogSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listlogsubscriptionspaginator)
         """
 
 
 class ListSchemaExtensionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListSchemaExtensions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listschemaextensionspaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchemaExtensionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListSchemaExtensions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listschemaextensionspaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-ds-1.28.12/mypy_boto3_ds/paginator.pyi` & `mypy-boto3-ds-1.28.15/mypy_boto3_ds/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -106,29 +106,29 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         Type: ClientAuthenticationTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeClientAuthenticationSettingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeClientAuthenticationSettings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describeclientauthenticationsettingspaginator)
         """
 
 class DescribeDirectoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDirectories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describedirectoriespaginator)
     """
 
     def paginate(
-        self, *, DirectoryIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDirectories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describedirectoriespaginator)
         """
 
 class DescribeDomainControllersPaginator(Paginator):
@@ -138,15 +138,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         DomainControllerIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDomainControllersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDomainControllers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describedomaincontrollerspaginator)
         """
 
 class DescribeLDAPSSettingsPaginator(Paginator):
@@ -156,15 +156,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         Type: Literal["Client"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeLDAPSSettingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeLDAPSSettings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describeldapssettingspaginator)
         """
 
 class DescribeRegionsPaginator(Paginator):
@@ -174,15 +174,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         RegionName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRegionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeRegions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describeregionspaginator)
         """
 
 class DescribeSharedDirectoriesPaginator(Paginator):
@@ -192,15 +192,15 @@
     """
 
     def paginate(
         self,
         *,
         OwnerDirectoryId: str,
         SharedDirectoryIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSharedDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSharedDirectories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describeshareddirectoriespaginator)
         """
 
 class DescribeSnapshotsPaginator(Paginator):
@@ -210,15 +210,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str = ...,
         SnapshotIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describesnapshotspaginator)
         """
 
 class DescribeTrustsPaginator(Paginator):
@@ -228,15 +228,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str = ...,
         TrustIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTrustsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeTrusts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describetrustspaginator)
         """
 
 class DescribeUpdateDirectoryPaginator(Paginator):
@@ -247,83 +247,83 @@
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         UpdateType: Literal["OS"],
         RegionName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeUpdateDirectoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeUpdateDirectory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#describeupdatedirectorypaginator)
         """
 
 class ListCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listcertificatespaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCertificatesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listcertificatespaginator)
         """
 
 class ListIpRoutesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListIpRoutes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listiproutespaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIpRoutesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListIpRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listiproutespaginator)
         """
 
 class ListLogSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListLogSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listlogsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLogSubscriptionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListLogSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listlogsubscriptionspaginator)
         """
 
 class ListSchemaExtensionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListSchemaExtensions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listschemaextensionspaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchemaExtensionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListSchemaExtensions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listschemaextensionspaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-ds-1.28.12/mypy_boto3_ds/type_defs.py` & `mypy-boto3-ds-1.28.15/mypy_boto3_ds/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,75 +53,57 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptSharedDirectoryRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SharedDirectoryTypeDef",
     "IpRouteTypeDef",
     "DirectoryVpcSettingsTypeDef",
     "TagTypeDef",
-    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "CancelSchemaExtensionRequestRequestTypeDef",
     "CertificateInfoTypeDef",
-    "ClientCertAuthSettingsOutputTypeDef",
-    "ClientAuthenticationSettingInfoTypeDef",
     "ClientCertAuthSettingsTypeDef",
+    "ClientAuthenticationSettingInfoTypeDef",
     "ConditionalForwarderTypeDef",
     "DirectoryConnectSettingsTypeDef",
-    "ConnectDirectoryResultTypeDef",
     "CreateAliasRequestRequestTypeDef",
-    "CreateAliasResultTypeDef",
     "CreateConditionalForwarderRequestRequestTypeDef",
-    "CreateDirectoryResultTypeDef",
     "CreateLogSubscriptionRequestRequestTypeDef",
-    "CreateMicrosoftADResultTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
-    "CreateSnapshotResultTypeDef",
     "CreateTrustRequestRequestTypeDef",
-    "CreateTrustResultTypeDef",
     "DeleteConditionalForwarderRequestRequestTypeDef",
     "DeleteDirectoryRequestRequestTypeDef",
-    "DeleteDirectoryResultTypeDef",
     "DeleteLogSubscriptionRequestRequestTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
-    "DeleteSnapshotResultTypeDef",
     "DeleteTrustRequestRequestTypeDef",
-    "DeleteTrustResultTypeDef",
     "DeregisterCertificateRequestRequestTypeDef",
     "DeregisterEventTopicRequestRequestTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
-    "DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeClientAuthenticationSettingsRequestRequestTypeDef",
     "DescribeConditionalForwardersRequestRequestTypeDef",
-    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
     "DescribeDirectoriesRequestRequestTypeDef",
-    "DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
     "DescribeDomainControllersRequestRequestTypeDef",
     "DomainControllerTypeDef",
     "DescribeEventTopicsRequestRequestTypeDef",
     "EventTopicTypeDef",
-    "DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
     "DescribeLDAPSSettingsRequestRequestTypeDef",
     "LDAPSSettingInfoTypeDef",
-    "DescribeRegionsRequestDescribeRegionsPaginateTypeDef",
     "DescribeRegionsRequestRequestTypeDef",
     "DescribeSettingsRequestRequestTypeDef",
     "SettingEntryTypeDef",
-    "DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
     "DescribeSharedDirectoriesRequestRequestTypeDef",
-    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
     "DescribeSnapshotsRequestRequestTypeDef",
     "SnapshotTypeDef",
-    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
     "DescribeTrustsRequestRequestTypeDef",
     "TrustTypeDef",
-    "DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
     "DescribeUpdateDirectoryRequestRequestTypeDef",
     "DirectoryConnectSettingsDescriptionTypeDef",
     "DirectoryVpcSettingsDescriptionTypeDef",
     "RadiusSettingsOutputTypeDef",
     "RegionsInfoTypeDef",
     "DirectoryLimitsTypeDef",
     "DirectoryVpcSettingsOutputTypeDef",
@@ -132,69 +114,84 @@
     "EnableClientAuthenticationRequestRequestTypeDef",
     "EnableLDAPSRequestRequestTypeDef",
     "RadiusSettingsTypeDef",
     "EnableSsoRequestRequestTypeDef",
     "GetSnapshotLimitsRequestRequestTypeDef",
     "SnapshotLimitsTypeDef",
     "IpRouteInfoTypeDef",
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListCertificatesRequestRequestTypeDef",
-    "ListIpRoutesRequestListIpRoutesPaginateTypeDef",
     "ListIpRoutesRequestRequestTypeDef",
-    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
     "ListLogSubscriptionsRequestRequestTypeDef",
     "LogSubscriptionTypeDef",
-    "ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
     "ListSchemaExtensionsRequestRequestTypeDef",
     "SchemaExtensionInfoTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "OSUpdateSettingsOutputTypeDef",
     "OSUpdateSettingsTypeDef",
-    "PaginatorConfigTypeDef",
-    "RegisterCertificateResultTypeDef",
     "RegisterEventTopicRequestRequestTypeDef",
     "RejectSharedDirectoryRequestRequestTypeDef",
-    "RejectSharedDirectoryResultTypeDef",
     "RemoveIpRoutesRequestRequestTypeDef",
     "RemoveRegionRequestRequestTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
     "ResetUserPasswordRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreFromSnapshotRequestRequestTypeDef",
     "SettingTypeDef",
     "ShareTargetTypeDef",
-    "ShareDirectoryResultTypeDef",
     "StartSchemaExtensionRequestRequestTypeDef",
-    "StartSchemaExtensionResultTypeDef",
     "UnshareTargetTypeDef",
-    "UnshareDirectoryResultTypeDef",
     "UpdateConditionalForwarderRequestRequestTypeDef",
     "UpdateNumberOfDomainControllersRequestRequestTypeDef",
-    "UpdateSettingsResultTypeDef",
     "UpdateTrustRequestRequestTypeDef",
-    "UpdateTrustResultTypeDef",
     "VerifyTrustRequestRequestTypeDef",
+    "ConnectDirectoryResultTypeDef",
+    "CreateAliasResultTypeDef",
+    "CreateDirectoryResultTypeDef",
+    "CreateMicrosoftADResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "CreateTrustResultTypeDef",
+    "DeleteDirectoryResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DeleteTrustResultTypeDef",
+    "RegisterCertificateResultTypeDef",
+    "RejectSharedDirectoryResultTypeDef",
+    "ShareDirectoryResultTypeDef",
+    "StartSchemaExtensionResultTypeDef",
+    "UnshareDirectoryResultTypeDef",
+    "UpdateSettingsResultTypeDef",
+    "UpdateTrustResultTypeDef",
     "VerifyTrustResultTypeDef",
     "AcceptSharedDirectoryResultTypeDef",
     "DescribeSharedDirectoriesResultTypeDef",
     "AddIpRoutesRequestRequestTypeDef",
     "AddRegionRequestRequestTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
     "CreateMicrosoftADRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "ComputerTypeDef",
     "CreateComputerRequestRequestTypeDef",
     "ListCertificatesResultTypeDef",
     "CertificateTypeDef",
-    "DescribeClientAuthenticationSettingsResultTypeDef",
     "RegisterCertificateRequestRequestTypeDef",
+    "DescribeClientAuthenticationSettingsResultTypeDef",
     "DescribeConditionalForwardersResultTypeDef",
     "ConnectDirectoryRequestRequestTypeDef",
+    "DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
+    "DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
+    "DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
+    "DescribeRegionsRequestDescribeRegionsPaginateTypeDef",
+    "DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
+    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
+    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
+    "DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    "ListIpRoutesRequestListIpRoutesPaginateTypeDef",
+    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
+    "ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeDomainControllersResultTypeDef",
     "DescribeEventTopicsResultTypeDef",
     "DescribeLDAPSSettingsResultTypeDef",
     "DescribeSettingsResultTypeDef",
     "DescribeSnapshotsResultTypeDef",
     "DescribeTrustsResultTypeDef",
     "OwnerDirectoryDescriptionTypeDef",
@@ -202,17 +199,16 @@
     "RegionDescriptionTypeDef",
     "EnableRadiusRequestRequestTypeDef",
     "UpdateRadiusRequestRequestTypeDef",
     "GetSnapshotLimitsResultTypeDef",
     "ListIpRoutesResultTypeDef",
     "ListLogSubscriptionsResultTypeDef",
     "ListSchemaExtensionsResultTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "UpdateValueTypeDef",
     "UpdateDirectorySetupRequestRequestTypeDef",
+    "UpdateValueTypeDef",
     "UpdateSettingsRequestRequestTypeDef",
     "ShareDirectoryRequestRequestTypeDef",
     "UnshareDirectoryRequestRequestTypeDef",
     "CreateComputerResultTypeDef",
     "DescribeCertificateResultTypeDef",
     "DirectoryDescriptionTypeDef",
     "DescribeRegionsResultTypeDef",
@@ -224,14 +220,25 @@
 AcceptSharedDirectoryRequestRequestTypeDef = TypedDict(
     "AcceptSharedDirectoryRequestRequestTypeDef",
     {
         "SharedDirectoryId": str,
     },
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
 SharedDirectoryTypeDef = TypedDict(
     "SharedDirectoryTypeDef",
     {
         "OwnerAccountId": str,
         "OwnerDirectoryId": str,
         "ShareMethod": ShareMethodType,
         "SharedAccountId": str,
@@ -265,23 +272,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-AttributeOutputTypeDef = TypedDict(
-    "AttributeOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
@@ -303,16 +301,16 @@
         "State": CertificateStateType,
         "ExpiryDateTime": datetime,
         "Type": CertificateTypeType,
     },
     total=False,
 )
 
-ClientCertAuthSettingsOutputTypeDef = TypedDict(
-    "ClientCertAuthSettingsOutputTypeDef",
+ClientCertAuthSettingsTypeDef = TypedDict(
+    "ClientCertAuthSettingsTypeDef",
     {
         "OCSPUrl": str,
     },
     total=False,
 )
 
 ClientAuthenticationSettingInfoTypeDef = TypedDict(
@@ -321,22 +319,14 @@
         "Type": ClientAuthenticationTypeType,
         "Status": ClientAuthenticationStatusType,
         "LastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-ClientCertAuthSettingsTypeDef = TypedDict(
-    "ClientCertAuthSettingsTypeDef",
-    {
-        "OCSPUrl": str,
-    },
-    total=False,
-)
-
 ConditionalForwarderTypeDef = TypedDict(
     "ConditionalForwarderTypeDef",
     {
         "RemoteDomainName": str,
         "DnsIpAddrs": List[str],
         "ReplicationScope": Literal["Domain"],
     },
@@ -349,72 +339,39 @@
         "VpcId": str,
         "SubnetIds": Sequence[str],
         "CustomerDnsIps": Sequence[str],
         "CustomerUserName": str,
     },
 )
 
-ConnectDirectoryResultTypeDef = TypedDict(
-    "ConnectDirectoryResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateAliasRequestRequestTypeDef = TypedDict(
     "CreateAliasRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Alias": str,
     },
 )
 
-CreateAliasResultTypeDef = TypedDict(
-    "CreateAliasResultTypeDef",
-    {
-        "DirectoryId": str,
-        "Alias": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateConditionalForwarderRequestRequestTypeDef = TypedDict(
     "CreateConditionalForwarderRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
         "DnsIpAddrs": Sequence[str],
     },
 )
 
-CreateDirectoryResultTypeDef = TypedDict(
-    "CreateDirectoryResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateLogSubscriptionRequestRequestTypeDef = TypedDict(
     "CreateLogSubscriptionRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "LogGroupName": str,
     },
 )
 
-CreateMicrosoftADResultTypeDef = TypedDict(
-    "CreateMicrosoftADResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalCreateSnapshotRequestRequestTypeDef = TypedDict(
@@ -428,22 +385,14 @@
 
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
 
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "SnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateTrustRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
         "TrustPassword": str,
         "TrustDirection": TrustDirectionType,
@@ -462,22 +411,14 @@
 
 class CreateTrustRequestRequestTypeDef(
     _RequiredCreateTrustRequestRequestTypeDef, _OptionalCreateTrustRequestRequestTypeDef
 ):
     pass
 
 
-CreateTrustResultTypeDef = TypedDict(
-    "CreateTrustResultTypeDef",
-    {
-        "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteConditionalForwarderRequestRequestTypeDef = TypedDict(
     "DeleteConditionalForwarderRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
     },
 )
@@ -485,44 +426,28 @@
 DeleteDirectoryRequestRequestTypeDef = TypedDict(
     "DeleteDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
-DeleteDirectoryResultTypeDef = TypedDict(
-    "DeleteDirectoryResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLogSubscriptionRequestRequestTypeDef = TypedDict(
     "DeleteLogSubscriptionRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
 DeleteSnapshotRequestRequestTypeDef = TypedDict(
     "DeleteSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
-    {
-        "SnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTrustRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTrustRequestRequestTypeDef",
     {
         "TrustId": str,
     },
 )
 _OptionalDeleteTrustRequestRequestTypeDef = TypedDict(
@@ -536,22 +461,14 @@
 
 class DeleteTrustRequestRequestTypeDef(
     _RequiredDeleteTrustRequestRequestTypeDef, _OptionalDeleteTrustRequestRequestTypeDef
 ):
     pass
 
 
-DeleteTrustResultTypeDef = TypedDict(
-    "DeleteTrustResultTypeDef",
-    {
-        "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeregisterCertificateRequestRequestTypeDef = TypedDict(
     "DeregisterCertificateRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CertificateId": str,
     },
 )
@@ -568,37 +485,24 @@
     "DescribeCertificateRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CertificateId": str,
     },
 )
 
-_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Type": ClientAuthenticationTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef(
-    _RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
-    _OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeClientAuthenticationSettingsRequestRequestTypeDef = TypedDict(
@@ -637,56 +541,24 @@
 class DescribeConditionalForwardersRequestRequestTypeDef(
     _RequiredDescribeConditionalForwardersRequestRequestTypeDef,
     _OptionalDescribeConditionalForwardersRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef = TypedDict(
-    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
-    {
-        "DirectoryIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDirectoriesRequestRequestTypeDef = TypedDict(
     "DescribeDirectoriesRequestRequestTypeDef",
     {
         "DirectoryIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
-    {
-        "DomainControllerIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef(
-    _RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
-    _OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeDomainControllersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDomainControllersRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeDomainControllersRequestRequestTypeDef = TypedDict(
@@ -741,37 +613,14 @@
         "TopicArn": str,
         "CreatedDateTime": datetime,
         "Status": TopicStatusType,
     },
     total=False,
 )
 
-_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
-    {
-        "Type": Literal["Client"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef(
-    _RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
-    _OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeLDAPSSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLDAPSSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeLDAPSSettingsRequestRequestTypeDef = TypedDict(
@@ -798,37 +647,14 @@
         "LDAPSStatus": LDAPSStatusType,
         "LDAPSStatusReason": str,
         "LastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
-    {
-        "RegionName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeRegionsRequestDescribeRegionsPaginateTypeDef(
-    _RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
-    _OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeRegionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRegionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeRegionsRequestRequestTypeDef = TypedDict(
@@ -883,37 +709,14 @@
         "LastUpdatedDateTime": datetime,
         "LastRequestedDateTime": datetime,
         "DataType": str,
     },
     total=False,
 )
 
-_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
-    {
-        "OwnerDirectoryId": str,
-    },
-)
-_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
-    {
-        "SharedDirectoryIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef(
-    _RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
-    _OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeSharedDirectoriesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSharedDirectoriesRequestRequestTypeDef",
     {
         "OwnerDirectoryId": str,
     },
 )
 _OptionalDescribeSharedDirectoriesRequestRequestTypeDef = TypedDict(
@@ -930,24 +733,14 @@
 class DescribeSharedDirectoriesRequestRequestTypeDef(
     _RequiredDescribeSharedDirectoriesRequestRequestTypeDef,
     _OptionalDescribeSharedDirectoriesRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "SnapshotIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSnapshotsRequestRequestTypeDef = TypedDict(
     "DescribeSnapshotsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "SnapshotIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
@@ -964,24 +757,14 @@
         "Name": str,
         "Status": SnapshotStatusType,
         "StartTime": datetime,
     },
     total=False,
 )
 
-DescribeTrustsRequestDescribeTrustsPaginateTypeDef = TypedDict(
-    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "TrustIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTrustsRequestRequestTypeDef = TypedDict(
     "DescribeTrustsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "TrustIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
@@ -1003,38 +786,14 @@
         "StateLastUpdatedDateTime": datetime,
         "TrustStateReason": str,
         "SelectiveAuth": SelectiveAuthType,
     },
     total=False,
 )
 
-_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
-    "_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "UpdateType": Literal["OS"],
-    },
-)
-_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
-    "_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
-    {
-        "RegionName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef(
-    _RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
-    _OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeUpdateDirectoryRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeUpdateDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UpdateType": Literal["OS"],
     },
 )
@@ -1251,36 +1010,14 @@
         "AddedDateTime": datetime,
         "IpRouteStatusReason": str,
         "Description": str,
     },
     total=False,
 )
 
-_RequiredListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "_RequiredListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "_OptionalListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListCertificatesRequestListCertificatesPaginateTypeDef(
-    _RequiredListCertificatesRequestListCertificatesPaginateTypeDef,
-    _OptionalListCertificatesRequestListCertificatesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListCertificatesRequestRequestTypeDef = TypedDict(
     "_RequiredListCertificatesRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListCertificatesRequestRequestTypeDef = TypedDict(
@@ -1295,36 +1032,14 @@
 
 class ListCertificatesRequestRequestTypeDef(
     _RequiredListCertificatesRequestRequestTypeDef, _OptionalListCertificatesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListIpRoutesRequestListIpRoutesPaginateTypeDef(
-    _RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef,
-    _OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListIpRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredListIpRoutesRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListIpRoutesRequestRequestTypeDef = TypedDict(
@@ -1339,23 +1054,14 @@
 
 class ListIpRoutesRequestRequestTypeDef(
     _RequiredListIpRoutesRequestRequestTypeDef, _OptionalListIpRoutesRequestRequestTypeDef
 ):
     pass
 
 
-ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef = TypedDict(
-    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLogSubscriptionsRequestRequestTypeDef = TypedDict(
     "ListLogSubscriptionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "NextToken": str,
         "Limit": int,
     },
@@ -1368,36 +1074,14 @@
         "DirectoryId": str,
         "LogGroupName": str,
         "SubscriptionCreatedDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
-    "_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
-    "_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef(
-    _RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
-    _OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSchemaExtensionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemaExtensionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListSchemaExtensionsRequestRequestTypeDef = TypedDict(
@@ -1427,36 +1111,14 @@
         "SchemaExtensionStatusReason": str,
         "StartDateTime": datetime,
         "EndDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1472,56 +1134,22 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-OSUpdateSettingsOutputTypeDef = TypedDict(
-    "OSUpdateSettingsOutputTypeDef",
-    {
-        "OSVersion": OSVersionType,
-    },
-    total=False,
-)
-
 OSUpdateSettingsTypeDef = TypedDict(
     "OSUpdateSettingsTypeDef",
     {
         "OSVersion": OSVersionType,
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
-RegisterCertificateResultTypeDef = TypedDict(
-    "RegisterCertificateResultTypeDef",
-    {
-        "CertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterEventTopicRequestRequestTypeDef = TypedDict(
     "RegisterEventTopicRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "TopicName": str,
     },
 )
@@ -1529,22 +1157,14 @@
 RejectSharedDirectoryRequestRequestTypeDef = TypedDict(
     "RejectSharedDirectoryRequestRequestTypeDef",
     {
         "SharedDirectoryId": str,
     },
 )
 
-RejectSharedDirectoryResultTypeDef = TypedDict(
-    "RejectSharedDirectoryResultTypeDef",
-    {
-        "SharedDirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveIpRoutesRequestRequestTypeDef = TypedDict(
     "RemoveIpRoutesRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CidrIps": Sequence[str],
     },
 )
@@ -1569,25 +1189,14 @@
     {
         "DirectoryId": str,
         "UserName": str,
         "NewPassword": str,
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
 RestoreFromSnapshotRequestRequestTypeDef = TypedDict(
     "RestoreFromSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 
@@ -1603,56 +1212,32 @@
     "ShareTargetTypeDef",
     {
         "Id": str,
         "Type": Literal["ACCOUNT"],
     },
 )
 
-ShareDirectoryResultTypeDef = TypedDict(
-    "ShareDirectoryResultTypeDef",
-    {
-        "SharedDirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartSchemaExtensionRequestRequestTypeDef = TypedDict(
     "StartSchemaExtensionRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CreateSnapshotBeforeSchemaExtension": bool,
         "LdifContent": str,
         "Description": str,
     },
 )
 
-StartSchemaExtensionResultTypeDef = TypedDict(
-    "StartSchemaExtensionResultTypeDef",
-    {
-        "SchemaExtensionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnshareTargetTypeDef = TypedDict(
     "UnshareTargetTypeDef",
     {
         "Id": str,
         "Type": Literal["ACCOUNT"],
     },
 )
 
-UnshareDirectoryResultTypeDef = TypedDict(
-    "UnshareDirectoryResultTypeDef",
-    {
-        "SharedDirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateConditionalForwarderRequestRequestTypeDef = TypedDict(
     "UpdateConditionalForwarderRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
         "DnsIpAddrs": Sequence[str],
     },
@@ -1662,22 +1247,14 @@
     "UpdateNumberOfDomainControllersRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "DesiredNumber": int,
     },
 )
 
-UpdateSettingsResultTypeDef = TypedDict(
-    "UpdateSettingsResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTrustRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrustRequestRequestTypeDef",
     {
         "TrustId": str,
     },
 )
 _OptionalUpdateTrustRequestRequestTypeDef = TypedDict(
@@ -1691,52 +1268,173 @@
 
 class UpdateTrustRequestRequestTypeDef(
     _RequiredUpdateTrustRequestRequestTypeDef, _OptionalUpdateTrustRequestRequestTypeDef
 ):
     pass
 
 
-UpdateTrustResultTypeDef = TypedDict(
-    "UpdateTrustResultTypeDef",
+VerifyTrustRequestRequestTypeDef = TypedDict(
+    "VerifyTrustRequestRequestTypeDef",
     {
-        "RequestId": str,
         "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-VerifyTrustRequestRequestTypeDef = TypedDict(
-    "VerifyTrustRequestRequestTypeDef",
+ConnectDirectoryResultTypeDef = TypedDict(
+    "ConnectDirectoryResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAliasResultTypeDef = TypedDict(
+    "CreateAliasResultTypeDef",
+    {
+        "DirectoryId": str,
+        "Alias": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDirectoryResultTypeDef = TypedDict(
+    "CreateDirectoryResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMicrosoftADResultTypeDef = TypedDict(
+    "CreateMicrosoftADResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
+    {
+        "SnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrustResultTypeDef = TypedDict(
+    "CreateTrustResultTypeDef",
+    {
+        "TrustId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDirectoryResultTypeDef = TypedDict(
+    "DeleteDirectoryResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "SnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTrustResultTypeDef = TypedDict(
+    "DeleteTrustResultTypeDef",
+    {
+        "TrustId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterCertificateResultTypeDef = TypedDict(
+    "RegisterCertificateResultTypeDef",
+    {
+        "CertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RejectSharedDirectoryResultTypeDef = TypedDict(
+    "RejectSharedDirectoryResultTypeDef",
     {
+        "SharedDirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ShareDirectoryResultTypeDef = TypedDict(
+    "ShareDirectoryResultTypeDef",
+    {
+        "SharedDirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSchemaExtensionResultTypeDef = TypedDict(
+    "StartSchemaExtensionResultTypeDef",
+    {
+        "SchemaExtensionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnshareDirectoryResultTypeDef = TypedDict(
+    "UnshareDirectoryResultTypeDef",
+    {
+        "SharedDirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSettingsResultTypeDef = TypedDict(
+    "UpdateSettingsResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTrustResultTypeDef = TypedDict(
+    "UpdateTrustResultTypeDef",
+    {
+        "RequestId": str,
         "TrustId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VerifyTrustResultTypeDef = TypedDict(
     "VerifyTrustResultTypeDef",
     {
         "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptSharedDirectoryResultTypeDef = TypedDict(
     "AcceptSharedDirectoryResultTypeDef",
     {
         "SharedDirectory": SharedDirectoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSharedDirectoriesResultTypeDef = TypedDict(
     "DescribeSharedDirectoriesResultTypeDef",
     {
         "SharedDirectories": List[SharedDirectoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAddIpRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredAddIpRoutesRequestRequestTypeDef",
     {
         "DirectoryId": str,
@@ -1823,20 +1521,29 @@
 
 class CreateMicrosoftADRequestRequestTypeDef(
     _RequiredCreateMicrosoftADRequestRequestTypeDef, _OptionalCreateMicrosoftADRequestRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ComputerTypeDef = TypedDict(
     "ComputerTypeDef",
     {
         "ComputerId": str,
         "ComputerName": str,
-        "ComputerAttributes": List[AttributeOutputTypeDef],
+        "ComputerAttributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateComputerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateComputerRequestRequestTypeDef",
     {
@@ -1862,42 +1569,33 @@
 
 
 ListCertificatesResultTypeDef = TypedDict(
     "ListCertificatesResultTypeDef",
     {
         "NextToken": str,
         "CertificatesInfo": List[CertificateInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateId": str,
         "State": CertificateStateType,
         "StateReason": str,
         "CommonName": str,
         "RegisteredDateTime": datetime,
         "ExpiryDateTime": datetime,
         "Type": CertificateTypeType,
-        "ClientCertAuthSettings": ClientCertAuthSettingsOutputTypeDef,
+        "ClientCertAuthSettings": ClientCertAuthSettingsTypeDef,
     },
     total=False,
 )
 
-DescribeClientAuthenticationSettingsResultTypeDef = TypedDict(
-    "DescribeClientAuthenticationSettingsResultTypeDef",
-    {
-        "ClientAuthenticationSettingsInfo": List[ClientAuthenticationSettingInfoTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterCertificateRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CertificateData": str,
     },
 )
@@ -1914,19 +1612,28 @@
 class RegisterCertificateRequestRequestTypeDef(
     _RequiredRegisterCertificateRequestRequestTypeDef,
     _OptionalRegisterCertificateRequestRequestTypeDef,
 ):
     pass
 
 
+DescribeClientAuthenticationSettingsResultTypeDef = TypedDict(
+    "DescribeClientAuthenticationSettingsResultTypeDef",
+    {
+        "ClientAuthenticationSettingsInfo": List[ClientAuthenticationSettingInfoTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeConditionalForwardersResultTypeDef = TypedDict(
     "DescribeConditionalForwardersResultTypeDef",
     {
         "ConditionalForwarders": List[ConditionalForwarderTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredConnectDirectoryRequestRequestTypeDef = TypedDict(
     "_RequiredConnectDirectoryRequestRequestTypeDef",
     {
         "Name": str,
@@ -1948,65 +1655,330 @@
 
 class ConnectDirectoryRequestRequestTypeDef(
     _RequiredConnectDirectoryRequestRequestTypeDef, _OptionalConnectDirectoryRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    {
+        "Type": ClientAuthenticationTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef(
+    _RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    _OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+):
+    pass
+
+
+DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef = TypedDict(
+    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
+    {
+        "DirectoryIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
+    {
+        "DomainControllerIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef(
+    _RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
+    _OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
+    {
+        "Type": Literal["Client"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef(
+    _RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
+    _OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
+    {
+        "RegionName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeRegionsRequestDescribeRegionsPaginateTypeDef(
+    _RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
+    _OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
+    {
+        "OwnerDirectoryId": str,
+    },
+)
+_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
+    {
+        "SharedDirectoryIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef(
+    _RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
+    _OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
+):
+    pass
+
+
+DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "SnapshotIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeTrustsRequestDescribeTrustsPaginateTypeDef = TypedDict(
+    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "TrustIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
+    "_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "UpdateType": Literal["OS"],
+    },
+)
+_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
+    "_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
+    {
+        "RegionName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef(
+    _RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
+    _OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "_RequiredListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "_OptionalListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListCertificatesRequestListCertificatesPaginateTypeDef(
+    _RequiredListCertificatesRequestListCertificatesPaginateTypeDef,
+    _OptionalListCertificatesRequestListCertificatesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListIpRoutesRequestListIpRoutesPaginateTypeDef(
+    _RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef,
+    _OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef,
+):
+    pass
+
+
+ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef = TypedDict(
+    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
+    "_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
+    "_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef(
+    _RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
+    _OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 DescribeDomainControllersResultTypeDef = TypedDict(
     "DescribeDomainControllersResultTypeDef",
     {
         "DomainControllers": List[DomainControllerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventTopicsResultTypeDef = TypedDict(
     "DescribeEventTopicsResultTypeDef",
     {
         "EventTopics": List[EventTopicTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLDAPSSettingsResultTypeDef = TypedDict(
     "DescribeLDAPSSettingsResultTypeDef",
     {
         "LDAPSSettingsInfo": List[LDAPSSettingInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSettingsResultTypeDef = TypedDict(
     "DescribeSettingsResultTypeDef",
     {
         "DirectoryId": str,
         "SettingEntries": List[SettingEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSnapshotsResultTypeDef = TypedDict(
     "DescribeSnapshotsResultTypeDef",
     {
         "Snapshots": List[SnapshotTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustsResultTypeDef = TypedDict(
     "DescribeTrustsResultTypeDef",
     {
         "Trusts": List[TrustTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OwnerDirectoryDescriptionTypeDef = TypedDict(
     "OwnerDirectoryDescriptionTypeDef",
     {
         "DirectoryId": str,
@@ -2019,15 +1991,15 @@
     total=False,
 )
 
 GetDirectoryLimitsResultTypeDef = TypedDict(
     "GetDirectoryLimitsResultTypeDef",
     {
         "DirectoryLimits": DirectoryLimitsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegionDescriptionTypeDef = TypedDict(
     "RegionDescriptionTypeDef",
     {
         "DirectoryId": str,
@@ -2059,60 +2031,43 @@
     },
 )
 
 GetSnapshotLimitsResultTypeDef = TypedDict(
     "GetSnapshotLimitsResultTypeDef",
     {
         "SnapshotLimits": SnapshotLimitsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIpRoutesResultTypeDef = TypedDict(
     "ListIpRoutesResultTypeDef",
     {
         "IpRoutesInfo": List[IpRouteInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLogSubscriptionsResultTypeDef = TypedDict(
     "ListLogSubscriptionsResultTypeDef",
     {
         "LogSubscriptions": List[LogSubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemaExtensionsResultTypeDef = TypedDict(
     "ListSchemaExtensionsResultTypeDef",
     {
         "SchemaExtensionsInfo": List[SchemaExtensionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateValueTypeDef = TypedDict(
-    "UpdateValueTypeDef",
-    {
-        "OSUpdateSettings": OSUpdateSettingsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredUpdateDirectorySetupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDirectorySetupRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UpdateType": Literal["OS"],
@@ -2131,14 +2086,22 @@
 class UpdateDirectorySetupRequestRequestTypeDef(
     _RequiredUpdateDirectorySetupRequestRequestTypeDef,
     _OptionalUpdateDirectorySetupRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateValueTypeDef = TypedDict(
+    "UpdateValueTypeDef",
+    {
+        "OSUpdateSettings": OSUpdateSettingsTypeDef,
+    },
+    total=False,
+)
+
 UpdateSettingsRequestRequestTypeDef = TypedDict(
     "UpdateSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Settings": Sequence[SettingTypeDef],
     },
 )
@@ -2174,23 +2137,23 @@
     },
 )
 
 CreateComputerResultTypeDef = TypedDict(
     "CreateComputerResultTypeDef",
     {
         "Computer": ComputerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCertificateResultTypeDef = TypedDict(
     "DescribeCertificateResultTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DirectoryDescriptionTypeDef = TypedDict(
     "DirectoryDescriptionTypeDef",
     {
         "DirectoryId": str,
@@ -2224,15 +2187,15 @@
 )
 
 DescribeRegionsResultTypeDef = TypedDict(
     "DescribeRegionsResultTypeDef",
     {
         "RegionsDescription": List[RegionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInfoEntryTypeDef = TypedDict(
     "UpdateInfoEntryTypeDef",
     {
         "Region": str,
@@ -2248,19 +2211,19 @@
 )
 
 DescribeDirectoriesResultTypeDef = TypedDict(
     "DescribeDirectoriesResultTypeDef",
     {
         "DirectoryDescriptions": List[DirectoryDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUpdateDirectoryResultTypeDef = TypedDict(
     "DescribeUpdateDirectoryResultTypeDef",
     {
         "UpdateActivities": List[UpdateInfoEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ds-1.28.12/mypy_boto3_ds/type_defs.pyi` & `mypy-boto3-ds-1.28.15/mypy_boto3_ds/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -52,75 +52,57 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptSharedDirectoryRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SharedDirectoryTypeDef",
     "IpRouteTypeDef",
     "DirectoryVpcSettingsTypeDef",
     "TagTypeDef",
-    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "CancelSchemaExtensionRequestRequestTypeDef",
     "CertificateInfoTypeDef",
-    "ClientCertAuthSettingsOutputTypeDef",
-    "ClientAuthenticationSettingInfoTypeDef",
     "ClientCertAuthSettingsTypeDef",
+    "ClientAuthenticationSettingInfoTypeDef",
     "ConditionalForwarderTypeDef",
     "DirectoryConnectSettingsTypeDef",
-    "ConnectDirectoryResultTypeDef",
     "CreateAliasRequestRequestTypeDef",
-    "CreateAliasResultTypeDef",
     "CreateConditionalForwarderRequestRequestTypeDef",
-    "CreateDirectoryResultTypeDef",
     "CreateLogSubscriptionRequestRequestTypeDef",
-    "CreateMicrosoftADResultTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
-    "CreateSnapshotResultTypeDef",
     "CreateTrustRequestRequestTypeDef",
-    "CreateTrustResultTypeDef",
     "DeleteConditionalForwarderRequestRequestTypeDef",
     "DeleteDirectoryRequestRequestTypeDef",
-    "DeleteDirectoryResultTypeDef",
     "DeleteLogSubscriptionRequestRequestTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
-    "DeleteSnapshotResultTypeDef",
     "DeleteTrustRequestRequestTypeDef",
-    "DeleteTrustResultTypeDef",
     "DeregisterCertificateRequestRequestTypeDef",
     "DeregisterEventTopicRequestRequestTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
-    "DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeClientAuthenticationSettingsRequestRequestTypeDef",
     "DescribeConditionalForwardersRequestRequestTypeDef",
-    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
     "DescribeDirectoriesRequestRequestTypeDef",
-    "DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
     "DescribeDomainControllersRequestRequestTypeDef",
     "DomainControllerTypeDef",
     "DescribeEventTopicsRequestRequestTypeDef",
     "EventTopicTypeDef",
-    "DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
     "DescribeLDAPSSettingsRequestRequestTypeDef",
     "LDAPSSettingInfoTypeDef",
-    "DescribeRegionsRequestDescribeRegionsPaginateTypeDef",
     "DescribeRegionsRequestRequestTypeDef",
     "DescribeSettingsRequestRequestTypeDef",
     "SettingEntryTypeDef",
-    "DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
     "DescribeSharedDirectoriesRequestRequestTypeDef",
-    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
     "DescribeSnapshotsRequestRequestTypeDef",
     "SnapshotTypeDef",
-    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
     "DescribeTrustsRequestRequestTypeDef",
     "TrustTypeDef",
-    "DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
     "DescribeUpdateDirectoryRequestRequestTypeDef",
     "DirectoryConnectSettingsDescriptionTypeDef",
     "DirectoryVpcSettingsDescriptionTypeDef",
     "RadiusSettingsOutputTypeDef",
     "RegionsInfoTypeDef",
     "DirectoryLimitsTypeDef",
     "DirectoryVpcSettingsOutputTypeDef",
@@ -131,69 +113,84 @@
     "EnableClientAuthenticationRequestRequestTypeDef",
     "EnableLDAPSRequestRequestTypeDef",
     "RadiusSettingsTypeDef",
     "EnableSsoRequestRequestTypeDef",
     "GetSnapshotLimitsRequestRequestTypeDef",
     "SnapshotLimitsTypeDef",
     "IpRouteInfoTypeDef",
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListCertificatesRequestRequestTypeDef",
-    "ListIpRoutesRequestListIpRoutesPaginateTypeDef",
     "ListIpRoutesRequestRequestTypeDef",
-    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
     "ListLogSubscriptionsRequestRequestTypeDef",
     "LogSubscriptionTypeDef",
-    "ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
     "ListSchemaExtensionsRequestRequestTypeDef",
     "SchemaExtensionInfoTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "OSUpdateSettingsOutputTypeDef",
     "OSUpdateSettingsTypeDef",
-    "PaginatorConfigTypeDef",
-    "RegisterCertificateResultTypeDef",
     "RegisterEventTopicRequestRequestTypeDef",
     "RejectSharedDirectoryRequestRequestTypeDef",
-    "RejectSharedDirectoryResultTypeDef",
     "RemoveIpRoutesRequestRequestTypeDef",
     "RemoveRegionRequestRequestTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
     "ResetUserPasswordRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreFromSnapshotRequestRequestTypeDef",
     "SettingTypeDef",
     "ShareTargetTypeDef",
-    "ShareDirectoryResultTypeDef",
     "StartSchemaExtensionRequestRequestTypeDef",
-    "StartSchemaExtensionResultTypeDef",
     "UnshareTargetTypeDef",
-    "UnshareDirectoryResultTypeDef",
     "UpdateConditionalForwarderRequestRequestTypeDef",
     "UpdateNumberOfDomainControllersRequestRequestTypeDef",
-    "UpdateSettingsResultTypeDef",
     "UpdateTrustRequestRequestTypeDef",
-    "UpdateTrustResultTypeDef",
     "VerifyTrustRequestRequestTypeDef",
+    "ConnectDirectoryResultTypeDef",
+    "CreateAliasResultTypeDef",
+    "CreateDirectoryResultTypeDef",
+    "CreateMicrosoftADResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "CreateTrustResultTypeDef",
+    "DeleteDirectoryResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DeleteTrustResultTypeDef",
+    "RegisterCertificateResultTypeDef",
+    "RejectSharedDirectoryResultTypeDef",
+    "ShareDirectoryResultTypeDef",
+    "StartSchemaExtensionResultTypeDef",
+    "UnshareDirectoryResultTypeDef",
+    "UpdateSettingsResultTypeDef",
+    "UpdateTrustResultTypeDef",
     "VerifyTrustResultTypeDef",
     "AcceptSharedDirectoryResultTypeDef",
     "DescribeSharedDirectoriesResultTypeDef",
     "AddIpRoutesRequestRequestTypeDef",
     "AddRegionRequestRequestTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
     "CreateMicrosoftADRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "ComputerTypeDef",
     "CreateComputerRequestRequestTypeDef",
     "ListCertificatesResultTypeDef",
     "CertificateTypeDef",
-    "DescribeClientAuthenticationSettingsResultTypeDef",
     "RegisterCertificateRequestRequestTypeDef",
+    "DescribeClientAuthenticationSettingsResultTypeDef",
     "DescribeConditionalForwardersResultTypeDef",
     "ConnectDirectoryRequestRequestTypeDef",
+    "DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
+    "DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
+    "DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
+    "DescribeRegionsRequestDescribeRegionsPaginateTypeDef",
+    "DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
+    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
+    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
+    "DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    "ListIpRoutesRequestListIpRoutesPaginateTypeDef",
+    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
+    "ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeDomainControllersResultTypeDef",
     "DescribeEventTopicsResultTypeDef",
     "DescribeLDAPSSettingsResultTypeDef",
     "DescribeSettingsResultTypeDef",
     "DescribeSnapshotsResultTypeDef",
     "DescribeTrustsResultTypeDef",
     "OwnerDirectoryDescriptionTypeDef",
@@ -201,17 +198,16 @@
     "RegionDescriptionTypeDef",
     "EnableRadiusRequestRequestTypeDef",
     "UpdateRadiusRequestRequestTypeDef",
     "GetSnapshotLimitsResultTypeDef",
     "ListIpRoutesResultTypeDef",
     "ListLogSubscriptionsResultTypeDef",
     "ListSchemaExtensionsResultTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "UpdateValueTypeDef",
     "UpdateDirectorySetupRequestRequestTypeDef",
+    "UpdateValueTypeDef",
     "UpdateSettingsRequestRequestTypeDef",
     "ShareDirectoryRequestRequestTypeDef",
     "UnshareDirectoryRequestRequestTypeDef",
     "CreateComputerResultTypeDef",
     "DescribeCertificateResultTypeDef",
     "DirectoryDescriptionTypeDef",
     "DescribeRegionsResultTypeDef",
@@ -223,14 +219,25 @@
 AcceptSharedDirectoryRequestRequestTypeDef = TypedDict(
     "AcceptSharedDirectoryRequestRequestTypeDef",
     {
         "SharedDirectoryId": str,
     },
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
 SharedDirectoryTypeDef = TypedDict(
     "SharedDirectoryTypeDef",
     {
         "OwnerAccountId": str,
         "OwnerDirectoryId": str,
         "ShareMethod": ShareMethodType,
         "SharedAccountId": str,
@@ -264,23 +271,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-AttributeOutputTypeDef = TypedDict(
-    "AttributeOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
@@ -302,16 +300,16 @@
         "State": CertificateStateType,
         "ExpiryDateTime": datetime,
         "Type": CertificateTypeType,
     },
     total=False,
 )
 
-ClientCertAuthSettingsOutputTypeDef = TypedDict(
-    "ClientCertAuthSettingsOutputTypeDef",
+ClientCertAuthSettingsTypeDef = TypedDict(
+    "ClientCertAuthSettingsTypeDef",
     {
         "OCSPUrl": str,
     },
     total=False,
 )
 
 ClientAuthenticationSettingInfoTypeDef = TypedDict(
@@ -320,22 +318,14 @@
         "Type": ClientAuthenticationTypeType,
         "Status": ClientAuthenticationStatusType,
         "LastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-ClientCertAuthSettingsTypeDef = TypedDict(
-    "ClientCertAuthSettingsTypeDef",
-    {
-        "OCSPUrl": str,
-    },
-    total=False,
-)
-
 ConditionalForwarderTypeDef = TypedDict(
     "ConditionalForwarderTypeDef",
     {
         "RemoteDomainName": str,
         "DnsIpAddrs": List[str],
         "ReplicationScope": Literal["Domain"],
     },
@@ -348,72 +338,39 @@
         "VpcId": str,
         "SubnetIds": Sequence[str],
         "CustomerDnsIps": Sequence[str],
         "CustomerUserName": str,
     },
 )
 
-ConnectDirectoryResultTypeDef = TypedDict(
-    "ConnectDirectoryResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateAliasRequestRequestTypeDef = TypedDict(
     "CreateAliasRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Alias": str,
     },
 )
 
-CreateAliasResultTypeDef = TypedDict(
-    "CreateAliasResultTypeDef",
-    {
-        "DirectoryId": str,
-        "Alias": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateConditionalForwarderRequestRequestTypeDef = TypedDict(
     "CreateConditionalForwarderRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
         "DnsIpAddrs": Sequence[str],
     },
 )
 
-CreateDirectoryResultTypeDef = TypedDict(
-    "CreateDirectoryResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateLogSubscriptionRequestRequestTypeDef = TypedDict(
     "CreateLogSubscriptionRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "LogGroupName": str,
     },
 )
 
-CreateMicrosoftADResultTypeDef = TypedDict(
-    "CreateMicrosoftADResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalCreateSnapshotRequestRequestTypeDef = TypedDict(
@@ -425,22 +382,14 @@
 )
 
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "SnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateTrustRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
         "TrustPassword": str,
         "TrustDirection": TrustDirectionType,
@@ -457,22 +406,14 @@
 )
 
 class CreateTrustRequestRequestTypeDef(
     _RequiredCreateTrustRequestRequestTypeDef, _OptionalCreateTrustRequestRequestTypeDef
 ):
     pass
 
-CreateTrustResultTypeDef = TypedDict(
-    "CreateTrustResultTypeDef",
-    {
-        "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteConditionalForwarderRequestRequestTypeDef = TypedDict(
     "DeleteConditionalForwarderRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
     },
 )
@@ -480,44 +421,28 @@
 DeleteDirectoryRequestRequestTypeDef = TypedDict(
     "DeleteDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
-DeleteDirectoryResultTypeDef = TypedDict(
-    "DeleteDirectoryResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLogSubscriptionRequestRequestTypeDef = TypedDict(
     "DeleteLogSubscriptionRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
 DeleteSnapshotRequestRequestTypeDef = TypedDict(
     "DeleteSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
-    {
-        "SnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTrustRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTrustRequestRequestTypeDef",
     {
         "TrustId": str,
     },
 )
 _OptionalDeleteTrustRequestRequestTypeDef = TypedDict(
@@ -529,22 +454,14 @@
 )
 
 class DeleteTrustRequestRequestTypeDef(
     _RequiredDeleteTrustRequestRequestTypeDef, _OptionalDeleteTrustRequestRequestTypeDef
 ):
     pass
 
-DeleteTrustResultTypeDef = TypedDict(
-    "DeleteTrustResultTypeDef",
-    {
-        "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeregisterCertificateRequestRequestTypeDef = TypedDict(
     "DeregisterCertificateRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CertificateId": str,
     },
 )
@@ -561,35 +478,24 @@
     "DescribeCertificateRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CertificateId": str,
     },
 )
 
-_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Type": ClientAuthenticationTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef(
-    _RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
-    _OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeClientAuthenticationSettingsRequestRequestTypeDef = TypedDict(
@@ -624,54 +530,24 @@
 
 class DescribeConditionalForwardersRequestRequestTypeDef(
     _RequiredDescribeConditionalForwardersRequestRequestTypeDef,
     _OptionalDescribeConditionalForwardersRequestRequestTypeDef,
 ):
     pass
 
-DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef = TypedDict(
-    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
-    {
-        "DirectoryIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDirectoriesRequestRequestTypeDef = TypedDict(
     "DescribeDirectoriesRequestRequestTypeDef",
     {
         "DirectoryIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
-    {
-        "DomainControllerIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef(
-    _RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
-    _OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeDomainControllersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDomainControllersRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeDomainControllersRequestRequestTypeDef = TypedDict(
@@ -724,35 +600,14 @@
         "TopicArn": str,
         "CreatedDateTime": datetime,
         "Status": TopicStatusType,
     },
     total=False,
 )
 
-_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
-    {
-        "Type": Literal["Client"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef(
-    _RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
-    _OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeLDAPSSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLDAPSSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeLDAPSSettingsRequestRequestTypeDef = TypedDict(
@@ -777,35 +632,14 @@
         "LDAPSStatus": LDAPSStatusType,
         "LDAPSStatusReason": str,
         "LastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
-    {
-        "RegionName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeRegionsRequestDescribeRegionsPaginateTypeDef(
-    _RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
-    _OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeRegionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRegionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeRegionsRequestRequestTypeDef = TypedDict(
@@ -856,35 +690,14 @@
         "LastUpdatedDateTime": datetime,
         "LastRequestedDateTime": datetime,
         "DataType": str,
     },
     total=False,
 )
 
-_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
-    {
-        "OwnerDirectoryId": str,
-    },
-)
-_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
-    {
-        "SharedDirectoryIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef(
-    _RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
-    _OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeSharedDirectoriesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSharedDirectoriesRequestRequestTypeDef",
     {
         "OwnerDirectoryId": str,
     },
 )
 _OptionalDescribeSharedDirectoriesRequestRequestTypeDef = TypedDict(
@@ -899,24 +712,14 @@
 
 class DescribeSharedDirectoriesRequestRequestTypeDef(
     _RequiredDescribeSharedDirectoriesRequestRequestTypeDef,
     _OptionalDescribeSharedDirectoriesRequestRequestTypeDef,
 ):
     pass
 
-DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "SnapshotIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSnapshotsRequestRequestTypeDef = TypedDict(
     "DescribeSnapshotsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "SnapshotIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
@@ -933,24 +736,14 @@
         "Name": str,
         "Status": SnapshotStatusType,
         "StartTime": datetime,
     },
     total=False,
 )
 
-DescribeTrustsRequestDescribeTrustsPaginateTypeDef = TypedDict(
-    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "TrustIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTrustsRequestRequestTypeDef = TypedDict(
     "DescribeTrustsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "TrustIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
@@ -972,36 +765,14 @@
         "StateLastUpdatedDateTime": datetime,
         "TrustStateReason": str,
         "SelectiveAuth": SelectiveAuthType,
     },
     total=False,
 )
 
-_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
-    "_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "UpdateType": Literal["OS"],
-    },
-)
-_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
-    "_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
-    {
-        "RegionName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef(
-    _RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
-    _OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeUpdateDirectoryRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeUpdateDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UpdateType": Literal["OS"],
     },
 )
@@ -1212,34 +983,14 @@
         "AddedDateTime": datetime,
         "IpRouteStatusReason": str,
         "Description": str,
     },
     total=False,
 )
 
-_RequiredListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "_RequiredListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "_OptionalListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListCertificatesRequestListCertificatesPaginateTypeDef(
-    _RequiredListCertificatesRequestListCertificatesPaginateTypeDef,
-    _OptionalListCertificatesRequestListCertificatesPaginateTypeDef,
-):
-    pass
-
 _RequiredListCertificatesRequestRequestTypeDef = TypedDict(
     "_RequiredListCertificatesRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListCertificatesRequestRequestTypeDef = TypedDict(
@@ -1252,34 +1003,14 @@
 )
 
 class ListCertificatesRequestRequestTypeDef(
     _RequiredListCertificatesRequestRequestTypeDef, _OptionalListCertificatesRequestRequestTypeDef
 ):
     pass
 
-_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListIpRoutesRequestListIpRoutesPaginateTypeDef(
-    _RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef,
-    _OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef,
-):
-    pass
-
 _RequiredListIpRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredListIpRoutesRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListIpRoutesRequestRequestTypeDef = TypedDict(
@@ -1292,23 +1023,14 @@
 )
 
 class ListIpRoutesRequestRequestTypeDef(
     _RequiredListIpRoutesRequestRequestTypeDef, _OptionalListIpRoutesRequestRequestTypeDef
 ):
     pass
 
-ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef = TypedDict(
-    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLogSubscriptionsRequestRequestTypeDef = TypedDict(
     "ListLogSubscriptionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "NextToken": str,
         "Limit": int,
     },
@@ -1321,34 +1043,14 @@
         "DirectoryId": str,
         "LogGroupName": str,
         "SubscriptionCreatedDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
-    "_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
-    "_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef(
-    _RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
-    _OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListSchemaExtensionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemaExtensionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListSchemaExtensionsRequestRequestTypeDef = TypedDict(
@@ -1376,34 +1078,14 @@
         "SchemaExtensionStatusReason": str,
         "StartDateTime": datetime,
         "EndDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1417,56 +1099,22 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-OSUpdateSettingsOutputTypeDef = TypedDict(
-    "OSUpdateSettingsOutputTypeDef",
-    {
-        "OSVersion": OSVersionType,
-    },
-    total=False,
-)
-
 OSUpdateSettingsTypeDef = TypedDict(
     "OSUpdateSettingsTypeDef",
     {
         "OSVersion": OSVersionType,
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
-RegisterCertificateResultTypeDef = TypedDict(
-    "RegisterCertificateResultTypeDef",
-    {
-        "CertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterEventTopicRequestRequestTypeDef = TypedDict(
     "RegisterEventTopicRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "TopicName": str,
     },
 )
@@ -1474,22 +1122,14 @@
 RejectSharedDirectoryRequestRequestTypeDef = TypedDict(
     "RejectSharedDirectoryRequestRequestTypeDef",
     {
         "SharedDirectoryId": str,
     },
 )
 
-RejectSharedDirectoryResultTypeDef = TypedDict(
-    "RejectSharedDirectoryResultTypeDef",
-    {
-        "SharedDirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveIpRoutesRequestRequestTypeDef = TypedDict(
     "RemoveIpRoutesRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CidrIps": Sequence[str],
     },
 )
@@ -1514,25 +1154,14 @@
     {
         "DirectoryId": str,
         "UserName": str,
         "NewPassword": str,
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
 RestoreFromSnapshotRequestRequestTypeDef = TypedDict(
     "RestoreFromSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 
@@ -1548,56 +1177,32 @@
     "ShareTargetTypeDef",
     {
         "Id": str,
         "Type": Literal["ACCOUNT"],
     },
 )
 
-ShareDirectoryResultTypeDef = TypedDict(
-    "ShareDirectoryResultTypeDef",
-    {
-        "SharedDirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartSchemaExtensionRequestRequestTypeDef = TypedDict(
     "StartSchemaExtensionRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CreateSnapshotBeforeSchemaExtension": bool,
         "LdifContent": str,
         "Description": str,
     },
 )
 
-StartSchemaExtensionResultTypeDef = TypedDict(
-    "StartSchemaExtensionResultTypeDef",
-    {
-        "SchemaExtensionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnshareTargetTypeDef = TypedDict(
     "UnshareTargetTypeDef",
     {
         "Id": str,
         "Type": Literal["ACCOUNT"],
     },
 )
 
-UnshareDirectoryResultTypeDef = TypedDict(
-    "UnshareDirectoryResultTypeDef",
-    {
-        "SharedDirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateConditionalForwarderRequestRequestTypeDef = TypedDict(
     "UpdateConditionalForwarderRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
         "DnsIpAddrs": Sequence[str],
     },
@@ -1607,22 +1212,14 @@
     "UpdateNumberOfDomainControllersRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "DesiredNumber": int,
     },
 )
 
-UpdateSettingsResultTypeDef = TypedDict(
-    "UpdateSettingsResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTrustRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrustRequestRequestTypeDef",
     {
         "TrustId": str,
     },
 )
 _OptionalUpdateTrustRequestRequestTypeDef = TypedDict(
@@ -1634,52 +1231,173 @@
 )
 
 class UpdateTrustRequestRequestTypeDef(
     _RequiredUpdateTrustRequestRequestTypeDef, _OptionalUpdateTrustRequestRequestTypeDef
 ):
     pass
 
-UpdateTrustResultTypeDef = TypedDict(
-    "UpdateTrustResultTypeDef",
+VerifyTrustRequestRequestTypeDef = TypedDict(
+    "VerifyTrustRequestRequestTypeDef",
     {
-        "RequestId": str,
         "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-VerifyTrustRequestRequestTypeDef = TypedDict(
-    "VerifyTrustRequestRequestTypeDef",
+ConnectDirectoryResultTypeDef = TypedDict(
+    "ConnectDirectoryResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAliasResultTypeDef = TypedDict(
+    "CreateAliasResultTypeDef",
+    {
+        "DirectoryId": str,
+        "Alias": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDirectoryResultTypeDef = TypedDict(
+    "CreateDirectoryResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMicrosoftADResultTypeDef = TypedDict(
+    "CreateMicrosoftADResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
+    {
+        "SnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrustResultTypeDef = TypedDict(
+    "CreateTrustResultTypeDef",
+    {
+        "TrustId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDirectoryResultTypeDef = TypedDict(
+    "DeleteDirectoryResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "SnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTrustResultTypeDef = TypedDict(
+    "DeleteTrustResultTypeDef",
+    {
+        "TrustId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterCertificateResultTypeDef = TypedDict(
+    "RegisterCertificateResultTypeDef",
+    {
+        "CertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RejectSharedDirectoryResultTypeDef = TypedDict(
+    "RejectSharedDirectoryResultTypeDef",
+    {
+        "SharedDirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ShareDirectoryResultTypeDef = TypedDict(
+    "ShareDirectoryResultTypeDef",
+    {
+        "SharedDirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSchemaExtensionResultTypeDef = TypedDict(
+    "StartSchemaExtensionResultTypeDef",
+    {
+        "SchemaExtensionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnshareDirectoryResultTypeDef = TypedDict(
+    "UnshareDirectoryResultTypeDef",
+    {
+        "SharedDirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSettingsResultTypeDef = TypedDict(
+    "UpdateSettingsResultTypeDef",
     {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTrustResultTypeDef = TypedDict(
+    "UpdateTrustResultTypeDef",
+    {
+        "RequestId": str,
         "TrustId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VerifyTrustResultTypeDef = TypedDict(
     "VerifyTrustResultTypeDef",
     {
         "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptSharedDirectoryResultTypeDef = TypedDict(
     "AcceptSharedDirectoryResultTypeDef",
     {
         "SharedDirectory": SharedDirectoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSharedDirectoriesResultTypeDef = TypedDict(
     "DescribeSharedDirectoriesResultTypeDef",
     {
         "SharedDirectories": List[SharedDirectoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAddIpRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredAddIpRoutesRequestRequestTypeDef",
     {
         "DirectoryId": str,
@@ -1760,20 +1478,29 @@
 )
 
 class CreateMicrosoftADRequestRequestTypeDef(
     _RequiredCreateMicrosoftADRequestRequestTypeDef, _OptionalCreateMicrosoftADRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ComputerTypeDef = TypedDict(
     "ComputerTypeDef",
     {
         "ComputerId": str,
         "ComputerName": str,
-        "ComputerAttributes": List[AttributeOutputTypeDef],
+        "ComputerAttributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateComputerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateComputerRequestRequestTypeDef",
     {
@@ -1797,42 +1524,33 @@
     pass
 
 ListCertificatesResultTypeDef = TypedDict(
     "ListCertificatesResultTypeDef",
     {
         "NextToken": str,
         "CertificatesInfo": List[CertificateInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateId": str,
         "State": CertificateStateType,
         "StateReason": str,
         "CommonName": str,
         "RegisteredDateTime": datetime,
         "ExpiryDateTime": datetime,
         "Type": CertificateTypeType,
-        "ClientCertAuthSettings": ClientCertAuthSettingsOutputTypeDef,
+        "ClientCertAuthSettings": ClientCertAuthSettingsTypeDef,
     },
     total=False,
 )
 
-DescribeClientAuthenticationSettingsResultTypeDef = TypedDict(
-    "DescribeClientAuthenticationSettingsResultTypeDef",
-    {
-        "ClientAuthenticationSettingsInfo": List[ClientAuthenticationSettingInfoTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterCertificateRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CertificateData": str,
     },
 )
@@ -1847,19 +1565,28 @@
 
 class RegisterCertificateRequestRequestTypeDef(
     _RequiredRegisterCertificateRequestRequestTypeDef,
     _OptionalRegisterCertificateRequestRequestTypeDef,
 ):
     pass
 
+DescribeClientAuthenticationSettingsResultTypeDef = TypedDict(
+    "DescribeClientAuthenticationSettingsResultTypeDef",
+    {
+        "ClientAuthenticationSettingsInfo": List[ClientAuthenticationSettingInfoTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeConditionalForwardersResultTypeDef = TypedDict(
     "DescribeConditionalForwardersResultTypeDef",
     {
         "ConditionalForwarders": List[ConditionalForwarderTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredConnectDirectoryRequestRequestTypeDef = TypedDict(
     "_RequiredConnectDirectoryRequestRequestTypeDef",
     {
         "Name": str,
@@ -1879,65 +1606,310 @@
 )
 
 class ConnectDirectoryRequestRequestTypeDef(
     _RequiredConnectDirectoryRequestRequestTypeDef, _OptionalConnectDirectoryRequestRequestTypeDef
 ):
     pass
 
+_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    {
+        "Type": ClientAuthenticationTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef(
+    _RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    _OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+):
+    pass
+
+DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef = TypedDict(
+    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
+    {
+        "DirectoryIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
+    {
+        "DomainControllerIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef(
+    _RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
+    _OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
+    {
+        "Type": Literal["Client"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef(
+    _RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
+    _OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
+    {
+        "RegionName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeRegionsRequestDescribeRegionsPaginateTypeDef(
+    _RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
+    _OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
+    {
+        "OwnerDirectoryId": str,
+    },
+)
+_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
+    {
+        "SharedDirectoryIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef(
+    _RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
+    _OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
+):
+    pass
+
+DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "SnapshotIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeTrustsRequestDescribeTrustsPaginateTypeDef = TypedDict(
+    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "TrustIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
+    "_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "UpdateType": Literal["OS"],
+    },
+)
+_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
+    "_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
+    {
+        "RegionName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef(
+    _RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
+    _OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
+):
+    pass
+
+_RequiredListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "_RequiredListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "_OptionalListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListCertificatesRequestListCertificatesPaginateTypeDef(
+    _RequiredListCertificatesRequestListCertificatesPaginateTypeDef,
+    _OptionalListCertificatesRequestListCertificatesPaginateTypeDef,
+):
+    pass
+
+_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListIpRoutesRequestListIpRoutesPaginateTypeDef(
+    _RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef,
+    _OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef,
+):
+    pass
+
+ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef = TypedDict(
+    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
+    "_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
+    "_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef(
+    _RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
+    _OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 DescribeDomainControllersResultTypeDef = TypedDict(
     "DescribeDomainControllersResultTypeDef",
     {
         "DomainControllers": List[DomainControllerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventTopicsResultTypeDef = TypedDict(
     "DescribeEventTopicsResultTypeDef",
     {
         "EventTopics": List[EventTopicTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLDAPSSettingsResultTypeDef = TypedDict(
     "DescribeLDAPSSettingsResultTypeDef",
     {
         "LDAPSSettingsInfo": List[LDAPSSettingInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSettingsResultTypeDef = TypedDict(
     "DescribeSettingsResultTypeDef",
     {
         "DirectoryId": str,
         "SettingEntries": List[SettingEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSnapshotsResultTypeDef = TypedDict(
     "DescribeSnapshotsResultTypeDef",
     {
         "Snapshots": List[SnapshotTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustsResultTypeDef = TypedDict(
     "DescribeTrustsResultTypeDef",
     {
         "Trusts": List[TrustTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OwnerDirectoryDescriptionTypeDef = TypedDict(
     "OwnerDirectoryDescriptionTypeDef",
     {
         "DirectoryId": str,
@@ -1950,15 +1922,15 @@
     total=False,
 )
 
 GetDirectoryLimitsResultTypeDef = TypedDict(
     "GetDirectoryLimitsResultTypeDef",
     {
         "DirectoryLimits": DirectoryLimitsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegionDescriptionTypeDef = TypedDict(
     "RegionDescriptionTypeDef",
     {
         "DirectoryId": str,
@@ -1990,60 +1962,43 @@
     },
 )
 
 GetSnapshotLimitsResultTypeDef = TypedDict(
     "GetSnapshotLimitsResultTypeDef",
     {
         "SnapshotLimits": SnapshotLimitsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIpRoutesResultTypeDef = TypedDict(
     "ListIpRoutesResultTypeDef",
     {
         "IpRoutesInfo": List[IpRouteInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLogSubscriptionsResultTypeDef = TypedDict(
     "ListLogSubscriptionsResultTypeDef",
     {
         "LogSubscriptions": List[LogSubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemaExtensionsResultTypeDef = TypedDict(
     "ListSchemaExtensionsResultTypeDef",
     {
         "SchemaExtensionsInfo": List[SchemaExtensionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateValueTypeDef = TypedDict(
-    "UpdateValueTypeDef",
-    {
-        "OSUpdateSettings": OSUpdateSettingsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredUpdateDirectorySetupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDirectorySetupRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UpdateType": Literal["OS"],
@@ -2060,14 +2015,22 @@
 
 class UpdateDirectorySetupRequestRequestTypeDef(
     _RequiredUpdateDirectorySetupRequestRequestTypeDef,
     _OptionalUpdateDirectorySetupRequestRequestTypeDef,
 ):
     pass
 
+UpdateValueTypeDef = TypedDict(
+    "UpdateValueTypeDef",
+    {
+        "OSUpdateSettings": OSUpdateSettingsTypeDef,
+    },
+    total=False,
+)
+
 UpdateSettingsRequestRequestTypeDef = TypedDict(
     "UpdateSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Settings": Sequence[SettingTypeDef],
     },
 )
@@ -2101,23 +2064,23 @@
     },
 )
 
 CreateComputerResultTypeDef = TypedDict(
     "CreateComputerResultTypeDef",
     {
         "Computer": ComputerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCertificateResultTypeDef = TypedDict(
     "DescribeCertificateResultTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DirectoryDescriptionTypeDef = TypedDict(
     "DirectoryDescriptionTypeDef",
     {
         "DirectoryId": str,
@@ -2151,15 +2114,15 @@
 )
 
 DescribeRegionsResultTypeDef = TypedDict(
     "DescribeRegionsResultTypeDef",
     {
         "RegionsDescription": List[RegionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInfoEntryTypeDef = TypedDict(
     "UpdateInfoEntryTypeDef",
     {
         "Region": str,
@@ -2175,19 +2138,19 @@
 )
 
 DescribeDirectoriesResultTypeDef = TypedDict(
     "DescribeDirectoriesResultTypeDef",
     {
         "DirectoryDescriptions": List[DirectoryDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUpdateDirectoryResultTypeDef = TypedDict(
     "DescribeUpdateDirectoryResultTypeDef",
     {
         "UpdateActivities": List[UpdateInfoEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/PKG-INFO` & `mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ds
-Version: 1.28.12
-Summary: Type annotations for boto3.DirectoryService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DirectoryService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ds.svg?color=blue)](https://pypi.org/project/mypy-boto3-ds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ds)](https://pepy.tech/project/mypy-boto3-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectoryService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[boto3.DirectoryService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
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
 [mypy-boto3-ds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/).
 
 See how it helps to find and fix potential bugs:
 
@@ -410,75 +410,57 @@
 
 `mypy_boto3_ds.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ds.type_defs import (
     AcceptSharedDirectoryRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SharedDirectoryTypeDef,
     IpRouteTypeDef,
     DirectoryVpcSettingsTypeDef,
     TagTypeDef,
-    AttributeOutputTypeDef,
     AttributeTypeDef,
     CancelSchemaExtensionRequestRequestTypeDef,
     CertificateInfoTypeDef,
-    ClientCertAuthSettingsOutputTypeDef,
-    ClientAuthenticationSettingInfoTypeDef,
     ClientCertAuthSettingsTypeDef,
+    ClientAuthenticationSettingInfoTypeDef,
     ConditionalForwarderTypeDef,
     DirectoryConnectSettingsTypeDef,
-    ConnectDirectoryResultTypeDef,
     CreateAliasRequestRequestTypeDef,
-    CreateAliasResultTypeDef,
     CreateConditionalForwarderRequestRequestTypeDef,
-    CreateDirectoryResultTypeDef,
     CreateLogSubscriptionRequestRequestTypeDef,
-    CreateMicrosoftADResultTypeDef,
     CreateSnapshotRequestRequestTypeDef,
-    CreateSnapshotResultTypeDef,
     CreateTrustRequestRequestTypeDef,
-    CreateTrustResultTypeDef,
     DeleteConditionalForwarderRequestRequestTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
-    DeleteDirectoryResultTypeDef,
     DeleteLogSubscriptionRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
-    DeleteSnapshotResultTypeDef,
     DeleteTrustRequestRequestTypeDef,
-    DeleteTrustResultTypeDef,
     DeregisterCertificateRequestRequestTypeDef,
     DeregisterEventTopicRequestRequestTypeDef,
     DescribeCertificateRequestRequestTypeDef,
-    DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClientAuthenticationSettingsRequestRequestTypeDef,
     DescribeConditionalForwardersRequestRequestTypeDef,
-    DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef,
     DescribeDirectoriesRequestRequestTypeDef,
-    DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
     DescribeDomainControllersRequestRequestTypeDef,
     DomainControllerTypeDef,
     DescribeEventTopicsRequestRequestTypeDef,
     EventTopicTypeDef,
-    DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
     DescribeLDAPSSettingsRequestRequestTypeDef,
     LDAPSSettingInfoTypeDef,
-    DescribeRegionsRequestDescribeRegionsPaginateTypeDef,
     DescribeRegionsRequestRequestTypeDef,
     DescribeSettingsRequestRequestTypeDef,
     SettingEntryTypeDef,
-    DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
     DescribeSharedDirectoriesRequestRequestTypeDef,
-    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
-    DescribeTrustsRequestDescribeTrustsPaginateTypeDef,
     DescribeTrustsRequestRequestTypeDef,
     TrustTypeDef,
-    DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
     DescribeUpdateDirectoryRequestRequestTypeDef,
     DirectoryConnectSettingsDescriptionTypeDef,
     DirectoryVpcSettingsDescriptionTypeDef,
     RadiusSettingsOutputTypeDef,
     RegionsInfoTypeDef,
     DirectoryLimitsTypeDef,
     DirectoryVpcSettingsOutputTypeDef,
@@ -489,69 +471,84 @@
     EnableClientAuthenticationRequestRequestTypeDef,
     EnableLDAPSRequestRequestTypeDef,
     RadiusSettingsTypeDef,
     EnableSsoRequestRequestTypeDef,
     GetSnapshotLimitsRequestRequestTypeDef,
     SnapshotLimitsTypeDef,
     IpRouteInfoTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
-    ListIpRoutesRequestListIpRoutesPaginateTypeDef,
     ListIpRoutesRequestRequestTypeDef,
-    ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef,
     ListLogSubscriptionsRequestRequestTypeDef,
     LogSubscriptionTypeDef,
-    ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
     ListSchemaExtensionsRequestRequestTypeDef,
     SchemaExtensionInfoTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    OSUpdateSettingsOutputTypeDef,
     OSUpdateSettingsTypeDef,
-    PaginatorConfigTypeDef,
-    RegisterCertificateResultTypeDef,
     RegisterEventTopicRequestRequestTypeDef,
     RejectSharedDirectoryRequestRequestTypeDef,
-    RejectSharedDirectoryResultTypeDef,
     RemoveIpRoutesRequestRequestTypeDef,
     RemoveRegionRequestRequestTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetUserPasswordRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     SettingTypeDef,
     ShareTargetTypeDef,
-    ShareDirectoryResultTypeDef,
     StartSchemaExtensionRequestRequestTypeDef,
-    StartSchemaExtensionResultTypeDef,
     UnshareTargetTypeDef,
-    UnshareDirectoryResultTypeDef,
     UpdateConditionalForwarderRequestRequestTypeDef,
     UpdateNumberOfDomainControllersRequestRequestTypeDef,
-    UpdateSettingsResultTypeDef,
     UpdateTrustRequestRequestTypeDef,
-    UpdateTrustResultTypeDef,
     VerifyTrustRequestRequestTypeDef,
+    ConnectDirectoryResultTypeDef,
+    CreateAliasResultTypeDef,
+    CreateDirectoryResultTypeDef,
+    CreateMicrosoftADResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    CreateTrustResultTypeDef,
+    DeleteDirectoryResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DeleteTrustResultTypeDef,
+    RegisterCertificateResultTypeDef,
+    RejectSharedDirectoryResultTypeDef,
+    ShareDirectoryResultTypeDef,
+    StartSchemaExtensionResultTypeDef,
+    UnshareDirectoryResultTypeDef,
+    UpdateSettingsResultTypeDef,
+    UpdateTrustResultTypeDef,
     VerifyTrustResultTypeDef,
     AcceptSharedDirectoryResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     AddIpRoutesRequestRequestTypeDef,
     AddRegionRequestRequestTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateDirectoryRequestRequestTypeDef,
     CreateMicrosoftADRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     ComputerTypeDef,
     CreateComputerRequestRequestTypeDef,
     ListCertificatesResultTypeDef,
     CertificateTypeDef,
-    DescribeClientAuthenticationSettingsResultTypeDef,
     RegisterCertificateRequestRequestTypeDef,
+    DescribeClientAuthenticationSettingsResultTypeDef,
     DescribeConditionalForwardersResultTypeDef,
     ConnectDirectoryRequestRequestTypeDef,
+    DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef,
+    DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
+    DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
+    DescribeRegionsRequestDescribeRegionsPaginateTypeDef,
+    DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
+    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
+    DescribeTrustsRequestDescribeTrustsPaginateTypeDef,
+    DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListIpRoutesRequestListIpRoutesPaginateTypeDef,
+    ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef,
+    ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeDomainControllersResultTypeDef,
     DescribeEventTopicsResultTypeDef,
     DescribeLDAPSSettingsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
     OwnerDirectoryDescriptionTypeDef,
@@ -559,17 +556,16 @@
     RegionDescriptionTypeDef,
     EnableRadiusRequestRequestTypeDef,
     UpdateRadiusRequestRequestTypeDef,
     GetSnapshotLimitsResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    UpdateValueTypeDef,
     UpdateDirectorySetupRequestRequestTypeDef,
+    UpdateValueTypeDef,
     UpdateSettingsRequestRequestTypeDef,
     ShareDirectoryRequestRequestTypeDef,
     UnshareDirectoryRequestRequestTypeDef,
     CreateComputerResultTypeDef,
     DescribeCertificateResultTypeDef,
     DirectoryDescriptionTypeDef,
     DescribeRegionsResultTypeDef,
```

### Comparing `mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/SOURCES.txt` & `mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.12/setup.py` & `mypy-boto3-ds-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ds",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_ds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DirectoryService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.DirectoryService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

