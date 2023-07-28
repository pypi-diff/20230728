# Comparing `tmp/mypy-boto3-appstream-1.28.12.tar.gz` & `tmp/mypy-boto3-appstream-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appstream-1.28.12.tar", last modified: Thu Jul 27 05:34:18 2023, max compression
+gzip compressed data, was "mypy-boto3-appstream-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
```

## Comparing `mypy-boto3-appstream-1.28.12.tar` & `mypy-boto3-appstream-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.620576 mypy-boto3-appstream-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23892 2023-07-27 05:34:18.620576 mypy-boto3-appstream-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22397 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.616577 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57916 2023-07-27 05:17:35.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57822 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-07-27 05:17:35.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-27 05:17:35.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-07-27 05:17:35.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-07-27 05:17:35.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    74161 2023-07-27 05:17:37.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    74054 2023-07-27 05:17:36.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-27 05:17:35.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-27 05:17:35.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.620576 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23892 2023-07-27 05:34:18.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-27 05:34:18.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:18.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:18.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:18.620576 mypy-boto3-appstream-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.236695 mypy-boto3-appstream-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-07-28 20:42:19.228695 mypy-boto3-appstream-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21982 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.228695 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57916 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57822 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-07-28 20:19:38.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-28 20:19:38.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    70349 2023-07-28 20:19:40.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70250 2023-07-28 20:19:39.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.228695 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-07-28 20:42:18.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-28 20:42:19.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:18.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:18.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.236695 mypy-boto3-appstream-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:19:36.000000 mypy-boto3-appstream-1.28.15/setup.py
```

### Comparing `mypy-boto3-appstream-1.28.12/LICENSE` & `mypy-boto3-appstream-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.12/PKG-INFO` & `mypy-boto3-appstream-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appstream
-Version: 1.28.12
-Summary: Type annotations for boto3.AppStream 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AppStream 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appstream)](https://pepy.tech/project/mypy-boto3-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppStream 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[boto3.AppStream 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
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
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -415,52 +415,45 @@
 ### Typed dictionaries
 
 `mypy_boto3_appstream.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appstream.type_defs import (
-    AccessEndpointOutputTypeDef,
     AccessEndpointTypeDef,
     AppBlockBuilderAppBlockAssociationTypeDef,
     AppBlockBuilderStateChangeReasonTypeDef,
     ResourceErrorTypeDef,
     VpcConfigOutputTypeDef,
     ErrorDetailsTypeDef,
-    S3LocationOutputTypeDef,
+    S3LocationTypeDef,
     ApplicationFleetAssociationTypeDef,
     ApplicationSettingsResponseTypeDef,
     ApplicationSettingsTypeDef,
     AssociateAppBlockBuilderAppBlockRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AssociateApplicationFleetRequestRequestTypeDef,
     AssociateApplicationToEntitlementRequestRequestTypeDef,
     AssociateFleetRequestRequestTypeDef,
     UserStackAssociationTypeDef,
-    CertificateBasedAuthPropertiesOutputTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityStatusTypeDef,
     ComputeCapacityTypeDef,
     CopyImageRequestRequestTypeDef,
-    CopyImageResponseTypeDef,
     VpcConfigTypeDef,
     CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
-    CreateAppBlockBuilderStreamingURLResultTypeDef,
-    S3LocationTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
-    CreateImageBuilderStreamingURLResultTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UserSettingTypeDef,
     CreateStreamingURLRequestRequestTypeDef,
-    CreateStreamingURLResultTypeDef,
     CreateUpdatedImageRequestRequestTypeDef,
-    CreateUsageReportSubscriptionResultTypeDef,
     CreateUserRequestRequestTypeDef,
     DeleteAppBlockBuilderRequestRequestTypeDef,
     DeleteAppBlockRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteDirectoryConfigRequestRequestTypeDef,
     DeleteEntitlementRequestRequestTypeDef,
     DeleteFleetRequestRequestTypeDef,
@@ -470,108 +463,104 @@
     DeleteStackRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef,
     DescribeAppBlockBuildersRequestRequestTypeDef,
     DescribeAppBlocksRequestRequestTypeDef,
     DescribeApplicationFleetAssociationsRequestRequestTypeDef,
     DescribeApplicationsRequestRequestTypeDef,
-    DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDirectoryConfigsRequestRequestTypeDef,
     DescribeEntitlementsRequestRequestTypeDef,
-    DescribeFleetsRequestDescribeFleetsPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeFleetsRequestRequestTypeDef,
-    DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef,
     DescribeImageBuildersRequestRequestTypeDef,
     DescribeImagePermissionsRequestRequestTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
-    DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeSessionsRequestRequestTypeDef,
-    DescribeStacksRequestDescribeStacksPaginateTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeUsageReportSubscriptionsRequestRequestTypeDef,
-    DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
     DescribeUserStackAssociationsRequestRequestTypeDef,
-    UserStackAssociationOutputTypeDef,
-    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UserTypeDef,
-    ServiceAccountCredentialsOutputTypeDef,
     DisableUserRequestRequestTypeDef,
     DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     DisassociateApplicationFleetRequestRequestTypeDef,
     DisassociateApplicationFromEntitlementRequestRequestTypeDef,
     DisassociateFleetRequestRequestTypeDef,
-    DomainJoinInfoOutputTypeDef,
     EnableUserRequestRequestTypeDef,
     EntitledApplicationTypeDef,
-    EntitlementAttributeOutputTypeDef,
     ExpireSessionRequestRequestTypeDef,
     FleetErrorTypeDef,
     ImageBuilderStateChangeReasonTypeDef,
     NetworkAccessConfigurationTypeDef,
-    ImagePermissionsOutputTypeDef,
     ImagePermissionsTypeDef,
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
-    ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
-    ListAssociatedFleetsResultTypeDef,
-    ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
     ListAssociatedStacksRequestRequestTypeDef,
-    ListAssociatedStacksResultTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StackErrorTypeDef,
     StorageConnectorOutputTypeDef,
-    StreamingExperienceSettingsOutputTypeDef,
-    UserSettingOutputTypeDef,
     StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
     StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AssociateAppBlockBuilderAppBlockResultTypeDef,
-    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
     AppBlockBuilderTypeDef,
     ApplicationTypeDef,
-    ScriptDetailsOutputTypeDef,
+    CreateApplicationRequestRequestTypeDef,
+    ScriptDetailsTypeDef,
+    UpdateApplicationRequestRequestTypeDef,
+    AssociateAppBlockBuilderAppBlockResultTypeDef,
     AssociateApplicationFleetResultTypeDef,
+    CopyImageResponseTypeDef,
+    CreateAppBlockBuilderStreamingURLResultTypeDef,
+    CreateImageBuilderStreamingURLResultTypeDef,
+    CreateStreamingURLResultTypeDef,
+    CreateUsageReportSubscriptionResultTypeDef,
+    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
+    ListAssociatedFleetsResultTypeDef,
+    ListAssociatedStacksResultTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchAssociateUserStackRequestRequestTypeDef,
     BatchDisassociateUserStackRequestRequestTypeDef,
+    DescribeUserStackAssociationsResultTypeDef,
+    UserStackAssociationErrorTypeDef,
     CreateAppBlockBuilderRequestRequestTypeDef,
     UpdateAppBlockBuilderRequestRequestTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    ScriptDetailsTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
     CreateDirectoryConfigRequestRequestTypeDef,
+    DirectoryConfigTypeDef,
     UpdateDirectoryConfigRequestRequestTypeDef,
     CreateEntitlementRequestRequestTypeDef,
+    EntitlementTypeDef,
     UpdateEntitlementRequestRequestTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateImageBuilderRequestRequestTypeDef,
     UpdateFleetRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     UpdateStackRequestRequestTypeDef,
+    DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef,
+    DescribeFleetsRequestDescribeFleetsPaginateTypeDef,
+    DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef,
+    DescribeImagesRequestDescribeImagesPaginateTypeDef,
+    DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
+    DescribeStacksRequestDescribeStacksPaginateTypeDef,
+    DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
+    ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
+    ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
     DescribeFleetsRequestFleetStartedWaitTypeDef,
     DescribeFleetsRequestFleetStoppedWaitTypeDef,
-    DescribeUserStackAssociationsResultTypeDef,
-    UserStackAssociationErrorTypeDef,
     DescribeUsersResultTypeDef,
-    DirectoryConfigTypeDef,
     ListEntitledApplicationsResultTypeDef,
-    EntitlementTypeDef,
     FleetTypeDef,
     ImageBuilderTypeDef,
     SessionTypeDef,
     SharedImagePermissionsTypeDef,
     UpdateImagePermissionsRequestRequestTypeDef,
     UsageReportSubscriptionTypeDef,
     StackTypeDef,
@@ -612,15 +601,15 @@
     DeleteImageResultTypeDef,
     DescribeImagesResultTypeDef,
     CreateAppBlockResultTypeDef,
     DescribeAppBlocksResultTypeDef,
 )
 
 
-def get_structure() -> AccessEndpointOutputTypeDef:
+def get_structure() -> AccessEndpointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appstream-1.28.12/README.md` & `mypy-boto3-appstream-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appstream)](https://pepy.tech/project/mypy-boto3-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppStream 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[boto3.AppStream 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
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
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -383,52 +383,45 @@
 ### Typed dictionaries
 
 `mypy_boto3_appstream.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appstream.type_defs import (
-    AccessEndpointOutputTypeDef,
     AccessEndpointTypeDef,
     AppBlockBuilderAppBlockAssociationTypeDef,
     AppBlockBuilderStateChangeReasonTypeDef,
     ResourceErrorTypeDef,
     VpcConfigOutputTypeDef,
     ErrorDetailsTypeDef,
-    S3LocationOutputTypeDef,
+    S3LocationTypeDef,
     ApplicationFleetAssociationTypeDef,
     ApplicationSettingsResponseTypeDef,
     ApplicationSettingsTypeDef,
     AssociateAppBlockBuilderAppBlockRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AssociateApplicationFleetRequestRequestTypeDef,
     AssociateApplicationToEntitlementRequestRequestTypeDef,
     AssociateFleetRequestRequestTypeDef,
     UserStackAssociationTypeDef,
-    CertificateBasedAuthPropertiesOutputTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityStatusTypeDef,
     ComputeCapacityTypeDef,
     CopyImageRequestRequestTypeDef,
-    CopyImageResponseTypeDef,
     VpcConfigTypeDef,
     CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
-    CreateAppBlockBuilderStreamingURLResultTypeDef,
-    S3LocationTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
-    CreateImageBuilderStreamingURLResultTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UserSettingTypeDef,
     CreateStreamingURLRequestRequestTypeDef,
-    CreateStreamingURLResultTypeDef,
     CreateUpdatedImageRequestRequestTypeDef,
-    CreateUsageReportSubscriptionResultTypeDef,
     CreateUserRequestRequestTypeDef,
     DeleteAppBlockBuilderRequestRequestTypeDef,
     DeleteAppBlockRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteDirectoryConfigRequestRequestTypeDef,
     DeleteEntitlementRequestRequestTypeDef,
     DeleteFleetRequestRequestTypeDef,
@@ -438,108 +431,104 @@
     DeleteStackRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef,
     DescribeAppBlockBuildersRequestRequestTypeDef,
     DescribeAppBlocksRequestRequestTypeDef,
     DescribeApplicationFleetAssociationsRequestRequestTypeDef,
     DescribeApplicationsRequestRequestTypeDef,
-    DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDirectoryConfigsRequestRequestTypeDef,
     DescribeEntitlementsRequestRequestTypeDef,
-    DescribeFleetsRequestDescribeFleetsPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeFleetsRequestRequestTypeDef,
-    DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef,
     DescribeImageBuildersRequestRequestTypeDef,
     DescribeImagePermissionsRequestRequestTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
-    DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeSessionsRequestRequestTypeDef,
-    DescribeStacksRequestDescribeStacksPaginateTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeUsageReportSubscriptionsRequestRequestTypeDef,
-    DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
     DescribeUserStackAssociationsRequestRequestTypeDef,
-    UserStackAssociationOutputTypeDef,
-    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UserTypeDef,
-    ServiceAccountCredentialsOutputTypeDef,
     DisableUserRequestRequestTypeDef,
     DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     DisassociateApplicationFleetRequestRequestTypeDef,
     DisassociateApplicationFromEntitlementRequestRequestTypeDef,
     DisassociateFleetRequestRequestTypeDef,
-    DomainJoinInfoOutputTypeDef,
     EnableUserRequestRequestTypeDef,
     EntitledApplicationTypeDef,
-    EntitlementAttributeOutputTypeDef,
     ExpireSessionRequestRequestTypeDef,
     FleetErrorTypeDef,
     ImageBuilderStateChangeReasonTypeDef,
     NetworkAccessConfigurationTypeDef,
-    ImagePermissionsOutputTypeDef,
     ImagePermissionsTypeDef,
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
-    ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
-    ListAssociatedFleetsResultTypeDef,
-    ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
     ListAssociatedStacksRequestRequestTypeDef,
-    ListAssociatedStacksResultTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StackErrorTypeDef,
     StorageConnectorOutputTypeDef,
-    StreamingExperienceSettingsOutputTypeDef,
-    UserSettingOutputTypeDef,
     StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
     StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AssociateAppBlockBuilderAppBlockResultTypeDef,
-    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
     AppBlockBuilderTypeDef,
     ApplicationTypeDef,
-    ScriptDetailsOutputTypeDef,
+    CreateApplicationRequestRequestTypeDef,
+    ScriptDetailsTypeDef,
+    UpdateApplicationRequestRequestTypeDef,
+    AssociateAppBlockBuilderAppBlockResultTypeDef,
     AssociateApplicationFleetResultTypeDef,
+    CopyImageResponseTypeDef,
+    CreateAppBlockBuilderStreamingURLResultTypeDef,
+    CreateImageBuilderStreamingURLResultTypeDef,
+    CreateStreamingURLResultTypeDef,
+    CreateUsageReportSubscriptionResultTypeDef,
+    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
+    ListAssociatedFleetsResultTypeDef,
+    ListAssociatedStacksResultTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchAssociateUserStackRequestRequestTypeDef,
     BatchDisassociateUserStackRequestRequestTypeDef,
+    DescribeUserStackAssociationsResultTypeDef,
+    UserStackAssociationErrorTypeDef,
     CreateAppBlockBuilderRequestRequestTypeDef,
     UpdateAppBlockBuilderRequestRequestTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    ScriptDetailsTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
     CreateDirectoryConfigRequestRequestTypeDef,
+    DirectoryConfigTypeDef,
     UpdateDirectoryConfigRequestRequestTypeDef,
     CreateEntitlementRequestRequestTypeDef,
+    EntitlementTypeDef,
     UpdateEntitlementRequestRequestTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateImageBuilderRequestRequestTypeDef,
     UpdateFleetRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     UpdateStackRequestRequestTypeDef,
+    DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef,
+    DescribeFleetsRequestDescribeFleetsPaginateTypeDef,
+    DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef,
+    DescribeImagesRequestDescribeImagesPaginateTypeDef,
+    DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
+    DescribeStacksRequestDescribeStacksPaginateTypeDef,
+    DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
+    ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
+    ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
     DescribeFleetsRequestFleetStartedWaitTypeDef,
     DescribeFleetsRequestFleetStoppedWaitTypeDef,
-    DescribeUserStackAssociationsResultTypeDef,
-    UserStackAssociationErrorTypeDef,
     DescribeUsersResultTypeDef,
-    DirectoryConfigTypeDef,
     ListEntitledApplicationsResultTypeDef,
-    EntitlementTypeDef,
     FleetTypeDef,
     ImageBuilderTypeDef,
     SessionTypeDef,
     SharedImagePermissionsTypeDef,
     UpdateImagePermissionsRequestRequestTypeDef,
     UsageReportSubscriptionTypeDef,
     StackTypeDef,
@@ -580,15 +569,15 @@
     DeleteImageResultTypeDef,
     DescribeImagesResultTypeDef,
     CreateAppBlockResultTypeDef,
     DescribeAppBlocksResultTypeDef,
 )
 
 
-def get_structure() -> AccessEndpointOutputTypeDef:
+def get_structure() -> AccessEndpointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/__init__.py` & `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/__init__.pyi` & `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/__main__.py` & `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppStream 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.AppStream 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream\nOther"
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

### Comparing `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/client.py` & `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/client.pyi` & `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/literals.py` & `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/literals.pyi` & `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/paginator.py` & `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,48 +83,45 @@
 class DescribeDirectoryConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeDirectoryConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describedirectoryconfigspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        DirectoryNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryNames: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDirectoryConfigsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeDirectoryConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describedirectoryconfigspaginator)
         """
 
 
 class DescribeFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describefleetspaginator)
     """
 
     def paginate(
-        self, *, Names: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Names: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeFleetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describefleetspaginator)
         """
 
 
 class DescribeImageBuildersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImageBuilders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeimagebuilderspaginator)
     """
 
     def paginate(
-        self, *, Names: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Names: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeImageBuildersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImageBuilders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeimagebuilderspaginator)
         """
 
 
@@ -136,15 +133,15 @@
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         Arns: Sequence[str] = ...,
         Type: VisibilityTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeimagespaginator)
         """
 
 
@@ -157,30 +154,30 @@
     def paginate(
         self,
         *,
         StackName: str,
         FleetName: str,
         UserId: str = ...,
         AuthenticationType: AuthenticationTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSessionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describesessionspaginator)
         """
 
 
 class DescribeStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describestackspaginator)
     """
 
     def paginate(
-        self, *, Names: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Names: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStacksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describestackspaginator)
         """
 
 
@@ -192,15 +189,15 @@
 
     def paginate(
         self,
         *,
         StackName: str = ...,
         UserName: str = ...,
         AuthenticationType: AuthenticationTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeUserStackAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeUserStackAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeuserstackassociationspaginator)
         """
 
 
@@ -210,43 +207,43 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeuserspaginator)
     """
 
     def paginate(
         self,
         *,
         AuthenticationType: AuthenticationTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeUsersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeuserspaginator)
         """
 
 
 class ListAssociatedFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedfleetspaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociatedFleetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedfleetspaginator)
         """
 
 
 class ListAssociatedStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedstackspaginator)
     """
 
     def paginate(
-        self, *, FleetName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FleetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociatedStacksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedstackspaginator)
         """
```

### Comparing `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/paginator.pyi` & `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/paginator.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -80,46 +80,43 @@
 class DescribeDirectoryConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeDirectoryConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describedirectoryconfigspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        DirectoryNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryNames: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDirectoryConfigsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeDirectoryConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describedirectoryconfigspaginator)
         """
 
 class DescribeFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describefleetspaginator)
     """
 
     def paginate(
-        self, *, Names: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Names: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeFleetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describefleetspaginator)
         """
 
 class DescribeImageBuildersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImageBuilders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeimagebuilderspaginator)
     """
 
     def paginate(
-        self, *, Names: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Names: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeImageBuildersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImageBuilders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeimagebuilderspaginator)
         """
 
 class DescribeImagesPaginator(Paginator):
@@ -130,15 +127,15 @@
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         Arns: Sequence[str] = ...,
         Type: VisibilityTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeimagespaginator)
         """
 
 class DescribeSessionsPaginator(Paginator):
@@ -150,29 +147,29 @@
     def paginate(
         self,
         *,
         StackName: str,
         FleetName: str,
         UserId: str = ...,
         AuthenticationType: AuthenticationTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSessionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describesessionspaginator)
         """
 
 class DescribeStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describestackspaginator)
     """
 
     def paginate(
-        self, *, Names: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Names: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStacksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describestackspaginator)
         """
 
 class DescribeUserStackAssociationsPaginator(Paginator):
@@ -183,15 +180,15 @@
 
     def paginate(
         self,
         *,
         StackName: str = ...,
         UserName: str = ...,
         AuthenticationType: AuthenticationTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeUserStackAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeUserStackAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeuserstackassociationspaginator)
         """
 
 class DescribeUsersPaginator(Paginator):
@@ -200,41 +197,41 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeuserspaginator)
     """
 
     def paginate(
         self,
         *,
         AuthenticationType: AuthenticationTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeUsersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#describeuserspaginator)
         """
 
 class ListAssociatedFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedfleetspaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociatedFleetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedfleetspaginator)
         """
 
 class ListAssociatedStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedstackspaginator)
     """
 
     def paginate(
-        self, *, FleetName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FleetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociatedStacksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/paginators/#listassociatedstackspaginator)
         """
```

### Comparing `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/type_defs.py` & `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for appstream service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_appstream.type_defs import AccessEndpointOutputTypeDef
+    from mypy_boto3_appstream.type_defs import AccessEndpointTypeDef
 
-    data: AccessEndpointOutputTypeDef = {...}
+    data: AccessEndpointTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -53,54 +53,46 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "AccessEndpointOutputTypeDef",
     "AccessEndpointTypeDef",
     "AppBlockBuilderAppBlockAssociationTypeDef",
     "AppBlockBuilderStateChangeReasonTypeDef",
     "ResourceErrorTypeDef",
     "VpcConfigOutputTypeDef",
     "ErrorDetailsTypeDef",
-    "S3LocationOutputTypeDef",
+    "S3LocationTypeDef",
     "ApplicationFleetAssociationTypeDef",
     "ApplicationSettingsResponseTypeDef",
     "ApplicationSettingsTypeDef",
     "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateApplicationFleetRequestRequestTypeDef",
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     "AssociateFleetRequestRequestTypeDef",
     "UserStackAssociationTypeDef",
-    "CertificateBasedAuthPropertiesOutputTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
     "ComputeCapacityStatusTypeDef",
     "ComputeCapacityTypeDef",
     "CopyImageRequestRequestTypeDef",
-    "CopyImageResponseTypeDef",
     "VpcConfigTypeDef",
     "CreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
-    "CreateAppBlockBuilderStreamingURLResultTypeDef",
-    "S3LocationTypeDef",
     "ServiceAccountCredentialsTypeDef",
     "EntitlementAttributeTypeDef",
     "DomainJoinInfoTypeDef",
     "CreateImageBuilderStreamingURLRequestRequestTypeDef",
-    "CreateImageBuilderStreamingURLResultTypeDef",
     "StorageConnectorTypeDef",
     "StreamingExperienceSettingsTypeDef",
     "UserSettingTypeDef",
     "CreateStreamingURLRequestRequestTypeDef",
-    "CreateStreamingURLResultTypeDef",
     "CreateUpdatedImageRequestRequestTypeDef",
-    "CreateUsageReportSubscriptionResultTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DeleteAppBlockBuilderRequestRequestTypeDef",
     "DeleteAppBlockRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteDirectoryConfigRequestRequestTypeDef",
     "DeleteEntitlementRequestRequestTypeDef",
     "DeleteFleetRequestRequestTypeDef",
@@ -110,108 +102,104 @@
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef",
     "DescribeAppBlockBuildersRequestRequestTypeDef",
     "DescribeAppBlocksRequestRequestTypeDef",
     "DescribeApplicationFleetAssociationsRequestRequestTypeDef",
     "DescribeApplicationsRequestRequestTypeDef",
-    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeDirectoryConfigsRequestRequestTypeDef",
     "DescribeEntitlementsRequestRequestTypeDef",
-    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeFleetsRequestRequestTypeDef",
-    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
     "DescribeImageBuildersRequestRequestTypeDef",
     "DescribeImagePermissionsRequestRequestTypeDef",
-    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
-    "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     "DescribeSessionsRequestRequestTypeDef",
-    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
     "DescribeStacksRequestRequestTypeDef",
     "DescribeUsageReportSubscriptionsRequestRequestTypeDef",
-    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
     "DescribeUserStackAssociationsRequestRequestTypeDef",
-    "UserStackAssociationOutputTypeDef",
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
     "UserTypeDef",
-    "ServiceAccountCredentialsOutputTypeDef",
     "DisableUserRequestRequestTypeDef",
     "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "DisassociateApplicationFleetRequestRequestTypeDef",
     "DisassociateApplicationFromEntitlementRequestRequestTypeDef",
     "DisassociateFleetRequestRequestTypeDef",
-    "DomainJoinInfoOutputTypeDef",
     "EnableUserRequestRequestTypeDef",
     "EntitledApplicationTypeDef",
-    "EntitlementAttributeOutputTypeDef",
     "ExpireSessionRequestRequestTypeDef",
     "FleetErrorTypeDef",
     "ImageBuilderStateChangeReasonTypeDef",
     "NetworkAccessConfigurationTypeDef",
-    "ImagePermissionsOutputTypeDef",
     "ImagePermissionsTypeDef",
     "ImageStateChangeReasonTypeDef",
     "LastReportGenerationExecutionErrorTypeDef",
-    "ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
     "ListAssociatedFleetsRequestRequestTypeDef",
-    "ListAssociatedFleetsResultTypeDef",
-    "ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     "ListAssociatedStacksRequestRequestTypeDef",
-    "ListAssociatedStacksResultTypeDef",
     "ListEntitledApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StackErrorTypeDef",
     "StorageConnectorOutputTypeDef",
-    "StreamingExperienceSettingsOutputTypeDef",
-    "UserSettingOutputTypeDef",
     "StartAppBlockBuilderRequestRequestTypeDef",
     "StartFleetRequestRequestTypeDef",
     "StartImageBuilderRequestRequestTypeDef",
     "StopAppBlockBuilderRequestRequestTypeDef",
     "StopFleetRequestRequestTypeDef",
     "StopImageBuilderRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AssociateAppBlockBuilderAppBlockResultTypeDef",
-    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
     "AppBlockBuilderTypeDef",
     "ApplicationTypeDef",
-    "ScriptDetailsOutputTypeDef",
+    "CreateApplicationRequestRequestTypeDef",
+    "ScriptDetailsTypeDef",
+    "UpdateApplicationRequestRequestTypeDef",
+    "AssociateAppBlockBuilderAppBlockResultTypeDef",
     "AssociateApplicationFleetResultTypeDef",
+    "CopyImageResponseTypeDef",
+    "CreateAppBlockBuilderStreamingURLResultTypeDef",
+    "CreateImageBuilderStreamingURLResultTypeDef",
+    "CreateStreamingURLResultTypeDef",
+    "CreateUsageReportSubscriptionResultTypeDef",
+    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
     "DescribeApplicationFleetAssociationsResultTypeDef",
+    "ListAssociatedFleetsResultTypeDef",
+    "ListAssociatedStacksResultTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "BatchAssociateUserStackRequestRequestTypeDef",
     "BatchDisassociateUserStackRequestRequestTypeDef",
+    "DescribeUserStackAssociationsResultTypeDef",
+    "UserStackAssociationErrorTypeDef",
     "CreateAppBlockBuilderRequestRequestTypeDef",
     "UpdateAppBlockBuilderRequestRequestTypeDef",
-    "CreateApplicationRequestRequestTypeDef",
-    "ScriptDetailsTypeDef",
-    "UpdateApplicationRequestRequestTypeDef",
     "CreateDirectoryConfigRequestRequestTypeDef",
+    "DirectoryConfigTypeDef",
     "UpdateDirectoryConfigRequestRequestTypeDef",
     "CreateEntitlementRequestRequestTypeDef",
+    "EntitlementTypeDef",
     "UpdateEntitlementRequestRequestTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateImageBuilderRequestRequestTypeDef",
     "UpdateFleetRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "UpdateStackRequestRequestTypeDef",
+    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
+    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
+    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
+    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
+    "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
+    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
+    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
+    "ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
+    "ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     "DescribeFleetsRequestFleetStartedWaitTypeDef",
     "DescribeFleetsRequestFleetStoppedWaitTypeDef",
-    "DescribeUserStackAssociationsResultTypeDef",
-    "UserStackAssociationErrorTypeDef",
     "DescribeUsersResultTypeDef",
-    "DirectoryConfigTypeDef",
     "ListEntitledApplicationsResultTypeDef",
-    "EntitlementTypeDef",
     "FleetTypeDef",
     "ImageBuilderTypeDef",
     "SessionTypeDef",
     "SharedImagePermissionsTypeDef",
     "UpdateImagePermissionsRequestRequestTypeDef",
     "UsageReportSubscriptionTypeDef",
     "StackTypeDef",
@@ -251,54 +239,31 @@
     "CreateUpdatedImageResultTypeDef",
     "DeleteImageResultTypeDef",
     "DescribeImagesResultTypeDef",
     "CreateAppBlockResultTypeDef",
     "DescribeAppBlocksResultTypeDef",
 )
 
-_RequiredAccessEndpointOutputTypeDef = TypedDict(
-    "_RequiredAccessEndpointOutputTypeDef",
-    {
-        "EndpointType": Literal["STREAMING"],
-    },
-)
-_OptionalAccessEndpointOutputTypeDef = TypedDict(
-    "_OptionalAccessEndpointOutputTypeDef",
-    {
-        "VpceId": str,
-    },
-    total=False,
-)
-
-
-class AccessEndpointOutputTypeDef(
-    _RequiredAccessEndpointOutputTypeDef, _OptionalAccessEndpointOutputTypeDef
-):
-    pass
-
-
 _RequiredAccessEndpointTypeDef = TypedDict(
     "_RequiredAccessEndpointTypeDef",
     {
         "EndpointType": Literal["STREAMING"],
     },
 )
 _OptionalAccessEndpointTypeDef = TypedDict(
     "_OptionalAccessEndpointTypeDef",
     {
         "VpceId": str,
     },
     total=False,
 )
 
-
 class AccessEndpointTypeDef(_RequiredAccessEndpointTypeDef, _OptionalAccessEndpointTypeDef):
     pass
 
-
 AppBlockBuilderAppBlockAssociationTypeDef = TypedDict(
     "AppBlockBuilderAppBlockAssociationTypeDef",
     {
         "AppBlockArn": str,
         "AppBlockBuilderName": str,
     },
 )
@@ -336,33 +301,31 @@
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-_RequiredS3LocationOutputTypeDef = TypedDict(
-    "_RequiredS3LocationOutputTypeDef",
+_RequiredS3LocationTypeDef = TypedDict(
+    "_RequiredS3LocationTypeDef",
     {
         "S3Bucket": str,
     },
 )
-_OptionalS3LocationOutputTypeDef = TypedDict(
-    "_OptionalS3LocationOutputTypeDef",
+_OptionalS3LocationTypeDef = TypedDict(
+    "_OptionalS3LocationTypeDef",
     {
         "S3Key": str,
     },
     total=False,
 )
 
-
-class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
+class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
-
 ApplicationFleetAssociationTypeDef = TypedDict(
     "ApplicationFleetAssociationTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -387,29 +350,38 @@
     "_OptionalApplicationSettingsTypeDef",
     {
         "SettingsGroup": str,
     },
     total=False,
 )
 
-
 class ApplicationSettingsTypeDef(
     _RequiredApplicationSettingsTypeDef, _OptionalApplicationSettingsTypeDef
 ):
     pass
 
-
 AssociateAppBlockBuilderAppBlockRequestRequestTypeDef = TypedDict(
     "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     {
         "AppBlockArn": str,
         "AppBlockBuilderName": str,
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
 AssociateApplicationFleetRequestRequestTypeDef = TypedDict(
     "AssociateApplicationFleetRequestRequestTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -443,30 +415,19 @@
     "_OptionalUserStackAssociationTypeDef",
     {
         "SendEmailNotification": bool,
     },
     total=False,
 )
 
-
 class UserStackAssociationTypeDef(
     _RequiredUserStackAssociationTypeDef, _OptionalUserStackAssociationTypeDef
 ):
     pass
 
-
-CertificateBasedAuthPropertiesOutputTypeDef = TypedDict(
-    "CertificateBasedAuthPropertiesOutputTypeDef",
-    {
-        "Status": CertificateBasedAuthStatusType,
-        "CertificateAuthorityArn": str,
-    },
-    total=False,
-)
-
 CertificateBasedAuthPropertiesTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesTypeDef",
     {
         "Status": CertificateBasedAuthStatusType,
         "CertificateAuthorityArn": str,
     },
     total=False,
@@ -484,21 +445,19 @@
         "Running": int,
         "InUse": int,
         "Available": int,
     },
     total=False,
 )
 
-
 class ComputeCapacityStatusTypeDef(
     _RequiredComputeCapacityStatusTypeDef, _OptionalComputeCapacityStatusTypeDef
 ):
     pass
 
-
 ComputeCapacityTypeDef = TypedDict(
     "ComputeCapacityTypeDef",
     {
         "DesiredInstances": int,
     },
 )
 
@@ -514,29 +473,19 @@
     "_OptionalCopyImageRequestRequestTypeDef",
     {
         "DestinationImageDescription": str,
     },
     total=False,
 )
 
-
 class CopyImageRequestRequestTypeDef(
     _RequiredCopyImageRequestRequestTypeDef, _OptionalCopyImageRequestRequestTypeDef
 ):
     pass
 
-
-CopyImageResponseTypeDef = TypedDict(
-    "CopyImageResponseTypeDef",
-    {
-        "DestinationImageName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VpcConfigTypeDef = TypedDict(
     "VpcConfigTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
@@ -552,50 +501,20 @@
     "_OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
     {
         "Validity": int,
     },
     total=False,
 )
 
-
 class CreateAppBlockBuilderStreamingURLRequestRequestTypeDef(
     _RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
     _OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
 ):
     pass
 
-
-CreateAppBlockBuilderStreamingURLResultTypeDef = TypedDict(
-    "CreateAppBlockBuilderStreamingURLResultTypeDef",
-    {
-        "StreamingURL": str,
-        "Expires": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredS3LocationTypeDef = TypedDict(
-    "_RequiredS3LocationTypeDef",
-    {
-        "S3Bucket": str,
-    },
-)
-_OptionalS3LocationTypeDef = TypedDict(
-    "_OptionalS3LocationTypeDef",
-    {
-        "S3Key": str,
-    },
-    total=False,
-)
-
-
-class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
-    pass
-
-
 ServiceAccountCredentialsTypeDef = TypedDict(
     "ServiceAccountCredentialsTypeDef",
     {
         "AccountName": str,
         "AccountPassword": str,
     },
 )
@@ -627,31 +546,20 @@
     "_OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef",
     {
         "Validity": int,
     },
     total=False,
 )
 
-
 class CreateImageBuilderStreamingURLRequestRequestTypeDef(
     _RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef,
     _OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef,
 ):
     pass
 
-
-CreateImageBuilderStreamingURLResultTypeDef = TypedDict(
-    "CreateImageBuilderStreamingURLResultTypeDef",
-    {
-        "StreamingURL": str,
-        "Expires": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStorageConnectorTypeDef = TypedDict(
     "_RequiredStorageConnectorTypeDef",
     {
         "ConnectorType": StorageConnectorTypeType,
     },
 )
 _OptionalStorageConnectorTypeDef = TypedDict(
@@ -659,19 +567,17 @@
     {
         "ResourceIdentifier": str,
         "Domains": Sequence[str],
     },
     total=False,
 )
 
-
 class StorageConnectorTypeDef(_RequiredStorageConnectorTypeDef, _OptionalStorageConnectorTypeDef):
     pass
 
-
 StreamingExperienceSettingsTypeDef = TypedDict(
     "StreamingExperienceSettingsTypeDef",
     {
         "PreferredProtocol": PreferredProtocolType,
     },
     total=False,
 )
@@ -698,31 +604,20 @@
         "ApplicationId": str,
         "Validity": int,
         "SessionContext": str,
     },
     total=False,
 )
 
-
 class CreateStreamingURLRequestRequestTypeDef(
     _RequiredCreateStreamingURLRequestRequestTypeDef,
     _OptionalCreateStreamingURLRequestRequestTypeDef,
 ):
     pass
 
-
-CreateStreamingURLResultTypeDef = TypedDict(
-    "CreateStreamingURLResultTypeDef",
-    {
-        "StreamingURL": str,
-        "Expires": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUpdatedImageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUpdatedImageRequestRequestTypeDef",
     {
         "existingImageName": str,
         "newImageName": str,
     },
 )
@@ -733,31 +628,20 @@
         "newImageDisplayName": str,
         "newImageTags": Mapping[str, str],
         "dryRun": bool,
     },
     total=False,
 )
 
-
 class CreateUpdatedImageRequestRequestTypeDef(
     _RequiredCreateUpdatedImageRequestRequestTypeDef,
     _OptionalCreateUpdatedImageRequestRequestTypeDef,
 ):
     pass
 
-
-CreateUsageReportSubscriptionResultTypeDef = TypedDict(
-    "CreateUsageReportSubscriptionResultTypeDef",
-    {
-        "S3BucketName": str,
-        "Schedule": Literal["DAILY"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
@@ -767,21 +651,19 @@
         "MessageAction": MessageActionType,
         "FirstName": str,
         "LastName": str,
     },
     total=False,
 )
 
-
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
-
 DeleteAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "DeleteAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -906,19 +788,20 @@
         "Arns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef = TypedDict(
-    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "DirectoryNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeDirectoryConfigsRequestRequestTypeDef = TypedDict(
     "DescribeDirectoryConfigsRequestRequestTypeDef",
     {
@@ -941,31 +824,20 @@
         "Name": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeEntitlementsRequestRequestTypeDef(
     _RequiredDescribeEntitlementsRequestRequestTypeDef,
     _OptionalDescribeEntitlementsRequestRequestTypeDef,
 ):
     pass
 
-
-DescribeFleetsRequestDescribeFleetsPaginateTypeDef = TypedDict(
-    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
-    {
-        "Names": Sequence[str],
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
@@ -976,23 +848,14 @@
     {
         "Names": Sequence[str],
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef = TypedDict(
-    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeImageBuildersRequestRequestTypeDef = TypedDict(
     "DescribeImageBuildersRequestRequestTypeDef",
     {
         "Names": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -1011,70 +874,32 @@
         "MaxResults": int,
         "SharedAwsAccountIds": Sequence[str],
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeImagePermissionsRequestRequestTypeDef(
     _RequiredDescribeImagePermissionsRequestRequestTypeDef,
     _OptionalDescribeImagePermissionsRequestRequestTypeDef,
 ):
     pass
 
-
-DescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "Arns": Sequence[str],
-        "Type": VisibilityTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeImagesRequestRequestTypeDef = TypedDict(
     "DescribeImagesRequestRequestTypeDef",
     {
         "Names": Sequence[str],
         "Arns": Sequence[str],
         "Type": VisibilityTypeType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
-    {
-        "StackName": str,
-        "FleetName": str,
-    },
-)
-_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
-    {
-        "UserId": str,
-        "AuthenticationType": AuthenticationTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
-    _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
-    _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSessionsRequestRequestTypeDef",
     {
         "StackName": str,
         "FleetName": str,
     },
 )
@@ -1085,30 +910,19 @@
         "NextToken": str,
         "Limit": int,
         "AuthenticationType": AuthenticationTypeType,
     },
     total=False,
 )
 
-
 class DescribeSessionsRequestRequestTypeDef(
     _RequiredDescribeSessionsRequestRequestTypeDef, _OptionalDescribeSessionsRequestRequestTypeDef
 ):
     pass
 
-
-DescribeStacksRequestDescribeStacksPaginateTypeDef = TypedDict(
-    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeStacksRequestRequestTypeDef = TypedDict(
     "DescribeStacksRequestRequestTypeDef",
     {
         "Names": Sequence[str],
         "NextToken": str,
     },
     total=False,
@@ -1119,82 +933,26 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef = TypedDict(
-    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
-    {
-        "StackName": str,
-        "UserName": str,
-        "AuthenticationType": AuthenticationTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeUserStackAssociationsRequestRequestTypeDef = TypedDict(
     "DescribeUserStackAssociationsRequestRequestTypeDef",
     {
         "StackName": str,
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredUserStackAssociationOutputTypeDef = TypedDict(
-    "_RequiredUserStackAssociationOutputTypeDef",
-    {
-        "StackName": str,
-        "UserName": str,
-        "AuthenticationType": AuthenticationTypeType,
-    },
-)
-_OptionalUserStackAssociationOutputTypeDef = TypedDict(
-    "_OptionalUserStackAssociationOutputTypeDef",
-    {
-        "SendEmailNotification": bool,
-    },
-    total=False,
-)
-
-
-class UserStackAssociationOutputTypeDef(
-    _RequiredUserStackAssociationOutputTypeDef, _OptionalUserStackAssociationOutputTypeDef
-):
-    pass
-
-
-_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef",
-    {
-        "AuthenticationType": AuthenticationTypeType,
-    },
-)
-_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeUsersRequestDescribeUsersPaginateTypeDef(
-    _RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef,
-    _OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeUsersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeUsersRequestRequestTypeDef",
     {
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 _OptionalDescribeUsersRequestRequestTypeDef = TypedDict(
@@ -1202,21 +960,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeUsersRequestRequestTypeDef(
     _RequiredDescribeUsersRequestRequestTypeDef, _OptionalDescribeUsersRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUserTypeDef = TypedDict(
     "_RequiredUserTypeDef",
     {
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 _OptionalUserTypeDef = TypedDict(
@@ -1229,27 +985,17 @@
         "FirstName": str,
         "LastName": str,
         "CreatedTime": datetime,
     },
     total=False,
 )
 
-
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
-
-ServiceAccountCredentialsOutputTypeDef = TypedDict(
-    "ServiceAccountCredentialsOutputTypeDef",
-    {
-        "AccountName": str,
-        "AccountPassword": str,
-    },
-)
-
 DisableUserRequestRequestTypeDef = TypedDict(
     "DisableUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
@@ -1283,23 +1029,14 @@
     "DisassociateFleetRequestRequestTypeDef",
     {
         "FleetName": str,
         "StackName": str,
     },
 )
 
-DomainJoinInfoOutputTypeDef = TypedDict(
-    "DomainJoinInfoOutputTypeDef",
-    {
-        "DirectoryName": str,
-        "OrganizationalUnitDistinguishedName": str,
-    },
-    total=False,
-)
-
 EnableUserRequestRequestTypeDef = TypedDict(
     "EnableUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
@@ -1307,22 +1044,14 @@
 EntitledApplicationTypeDef = TypedDict(
     "EntitledApplicationTypeDef",
     {
         "ApplicationIdentifier": str,
     },
 )
 
-EntitlementAttributeOutputTypeDef = TypedDict(
-    "EntitlementAttributeOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
-
 ExpireSessionRequestRequestTypeDef = TypedDict(
     "ExpireSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
@@ -1349,23 +1078,14 @@
     {
         "EniPrivateIpAddress": str,
         "EniId": str,
     },
     total=False,
 )
 
-ImagePermissionsOutputTypeDef = TypedDict(
-    "ImagePermissionsOutputTypeDef",
-    {
-        "allowFleet": bool,
-        "allowImageBuilder": bool,
-    },
-    total=False,
-)
-
 ImagePermissionsTypeDef = TypedDict(
     "ImagePermissionsTypeDef",
     {
         "allowFleet": bool,
         "allowImageBuilder": bool,
     },
     total=False,
@@ -1385,120 +1105,54 @@
     {
         "ErrorCode": UsageReportExecutionErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef(
-    _RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
-    _OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssociatedFleetsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedFleetsRequestRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListAssociatedFleetsRequestRequestTypeDef = TypedDict(
     "_OptionalListAssociatedFleetsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAssociatedFleetsRequestRequestTypeDef(
     _RequiredListAssociatedFleetsRequestRequestTypeDef,
     _OptionalListAssociatedFleetsRequestRequestTypeDef,
 ):
     pass
 
-
-ListAssociatedFleetsResultTypeDef = TypedDict(
-    "ListAssociatedFleetsResultTypeDef",
-    {
-        "Names": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
-    {
-        "FleetName": str,
-    },
-)
-_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef(
-    _RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
-    _OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssociatedStacksRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedStacksRequestRequestTypeDef",
     {
         "FleetName": str,
     },
 )
 _OptionalListAssociatedStacksRequestRequestTypeDef = TypedDict(
     "_OptionalListAssociatedStacksRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAssociatedStacksRequestRequestTypeDef(
     _RequiredListAssociatedStacksRequestRequestTypeDef,
     _OptionalListAssociatedStacksRequestRequestTypeDef,
 ):
     pass
 
-
-ListAssociatedStacksResultTypeDef = TypedDict(
-    "ListAssociatedStacksResultTypeDef",
-    {
-        "Names": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListEntitledApplicationsRequestRequestTypeDef = TypedDict(
     "_RequiredListEntitledApplicationsRequestRequestTypeDef",
     {
         "StackName": str,
         "EntitlementName": str,
     },
 )
@@ -1507,58 +1161,27 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListEntitledApplicationsRequestRequestTypeDef(
     _RequiredListEntitledApplicationsRequestRequestTypeDef,
     _OptionalListEntitledApplicationsRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 StackErrorTypeDef = TypedDict(
     "StackErrorTypeDef",
     {
         "ErrorCode": StackErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
@@ -1575,37 +1198,19 @@
     {
         "ResourceIdentifier": str,
         "Domains": List[str],
     },
     total=False,
 )
 
-
 class StorageConnectorOutputTypeDef(
     _RequiredStorageConnectorOutputTypeDef, _OptionalStorageConnectorOutputTypeDef
 ):
     pass
 
-
-StreamingExperienceSettingsOutputTypeDef = TypedDict(
-    "StreamingExperienceSettingsOutputTypeDef",
-    {
-        "PreferredProtocol": PreferredProtocolType,
-    },
-    total=False,
-)
-
-UserSettingOutputTypeDef = TypedDict(
-    "UserSettingOutputTypeDef",
-    {
-        "Action": ActionType,
-        "Permission": PermissionType,
-    },
-)
-
 StartAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "StartAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1626,21 +1231,19 @@
     "_OptionalStartImageBuilderRequestRequestTypeDef",
     {
         "AppstreamAgentVersion": str,
     },
     total=False,
 )
 
-
 class StartImageBuilderRequestRequestTypeDef(
     _RequiredStartImageBuilderRequestRequestTypeDef, _OptionalStartImageBuilderRequestRequestTypeDef
 ):
     pass
 
-
 StopAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "StopAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1670,31 +1273,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-AssociateAppBlockBuilderAppBlockResultTypeDef = TypedDict(
-    "AssociateAppBlockBuilderAppBlockResultTypeDef",
-    {
-        "AppBlockBuilderAppBlockAssociation": AppBlockBuilderAppBlockAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef = TypedDict(
-    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
-    {
-        "AppBlockBuilderAppBlockAssociations": List[AppBlockBuilderAppBlockAssociationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAppBlockBuilderTypeDef = TypedDict(
     "_RequiredAppBlockBuilderTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Platform": Literal["WINDOWS_SERVER_2019"],
         "InstanceType": str,
@@ -1708,83 +1294,218 @@
         "DisplayName": str,
         "Description": str,
         "EnableDefaultInternetAccess": bool,
         "IamRoleArn": str,
         "CreatedTime": datetime,
         "AppBlockBuilderErrors": List[ResourceErrorTypeDef],
         "StateChangeReason": AppBlockBuilderStateChangeReasonTypeDef,
-        "AccessEndpoints": List[AccessEndpointOutputTypeDef],
+        "AccessEndpoints": List[AccessEndpointTypeDef],
     },
     total=False,
 )
 
-
 class AppBlockBuilderTypeDef(_RequiredAppBlockBuilderTypeDef, _OptionalAppBlockBuilderTypeDef):
     pass
 
-
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Name": str,
         "DisplayName": str,
         "IconURL": str,
         "LaunchPath": str,
         "LaunchParameters": str,
         "Enabled": bool,
         "Metadata": Dict[str, str],
         "WorkingDirectory": str,
         "Description": str,
         "Arn": str,
         "AppBlockArn": str,
-        "IconS3Location": S3LocationOutputTypeDef,
+        "IconS3Location": S3LocationTypeDef,
         "Platforms": List[PlatformTypeType],
         "InstanceFamilies": List[str],
         "CreatedTime": datetime,
     },
     total=False,
 )
 
-_RequiredScriptDetailsOutputTypeDef = TypedDict(
-    "_RequiredScriptDetailsOutputTypeDef",
+_RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateApplicationRequestRequestTypeDef",
     {
-        "ScriptS3Location": S3LocationOutputTypeDef,
+        "Name": str,
+        "IconS3Location": S3LocationTypeDef,
+        "LaunchPath": str,
+        "Platforms": Sequence[PlatformTypeType],
+        "InstanceFamilies": Sequence[str],
+        "AppBlockArn": str,
+    },
+)
+_OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateApplicationRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "Description": str,
+        "WorkingDirectory": str,
+        "LaunchParameters": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateApplicationRequestRequestTypeDef(
+    _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
+):
+    pass
+
+_RequiredScriptDetailsTypeDef = TypedDict(
+    "_RequiredScriptDetailsTypeDef",
+    {
+        "ScriptS3Location": S3LocationTypeDef,
         "ExecutablePath": str,
         "TimeoutInSeconds": int,
     },
 )
-_OptionalScriptDetailsOutputTypeDef = TypedDict(
-    "_OptionalScriptDetailsOutputTypeDef",
+_OptionalScriptDetailsTypeDef = TypedDict(
+    "_OptionalScriptDetailsTypeDef",
     {
         "ExecutableParameters": str,
     },
     total=False,
 )
 
+class ScriptDetailsTypeDef(_RequiredScriptDetailsTypeDef, _OptionalScriptDetailsTypeDef):
+    pass
+
+_RequiredUpdateApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateApplicationRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateApplicationRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "Description": str,
+        "IconS3Location": S3LocationTypeDef,
+        "LaunchPath": str,
+        "WorkingDirectory": str,
+        "LaunchParameters": str,
+        "AppBlockArn": str,
+        "AttributesToDelete": Sequence[ApplicationAttributeType],
+    },
+    total=False,
+)
 
-class ScriptDetailsOutputTypeDef(
-    _RequiredScriptDetailsOutputTypeDef, _OptionalScriptDetailsOutputTypeDef
+class UpdateApplicationRequestRequestTypeDef(
+    _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
+AssociateAppBlockBuilderAppBlockResultTypeDef = TypedDict(
+    "AssociateAppBlockBuilderAppBlockResultTypeDef",
+    {
+        "AppBlockBuilderAppBlockAssociation": AppBlockBuilderAppBlockAssociationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 AssociateApplicationFleetResultTypeDef = TypedDict(
     "AssociateApplicationFleetResultTypeDef",
     {
         "ApplicationFleetAssociation": ApplicationFleetAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CopyImageResponseTypeDef = TypedDict(
+    "CopyImageResponseTypeDef",
+    {
+        "DestinationImageName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppBlockBuilderStreamingURLResultTypeDef = TypedDict(
+    "CreateAppBlockBuilderStreamingURLResultTypeDef",
+    {
+        "StreamingURL": str,
+        "Expires": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImageBuilderStreamingURLResultTypeDef = TypedDict(
+    "CreateImageBuilderStreamingURLResultTypeDef",
+    {
+        "StreamingURL": str,
+        "Expires": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStreamingURLResultTypeDef = TypedDict(
+    "CreateStreamingURLResultTypeDef",
+    {
+        "StreamingURL": str,
+        "Expires": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUsageReportSubscriptionResultTypeDef = TypedDict(
+    "CreateUsageReportSubscriptionResultTypeDef",
+    {
+        "S3BucketName": str,
+        "Schedule": Literal["DAILY"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef = TypedDict(
+    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
+    {
+        "AppBlockBuilderAppBlockAssociations": List[AppBlockBuilderAppBlockAssociationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationFleetAssociationsResultTypeDef = TypedDict(
     "DescribeApplicationFleetAssociationsResultTypeDef",
     {
         "ApplicationFleetAssociations": List[ApplicationFleetAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssociatedFleetsResultTypeDef = TypedDict(
+    "ListAssociatedFleetsResultTypeDef",
+    {
+        "Names": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssociatedStacksResultTypeDef = TypedDict(
+    "ListAssociatedStacksResultTypeDef",
+    {
+        "Names": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchAssociateUserStackRequestRequestTypeDef = TypedDict(
     "BatchAssociateUserStackRequestRequestTypeDef",
     {
         "UserStackAssociations": Sequence[UserStackAssociationTypeDef],
@@ -1794,14 +1515,33 @@
 BatchDisassociateUserStackRequestRequestTypeDef = TypedDict(
     "BatchDisassociateUserStackRequestRequestTypeDef",
     {
         "UserStackAssociations": Sequence[UserStackAssociationTypeDef],
     },
 )
 
+DescribeUserStackAssociationsResultTypeDef = TypedDict(
+    "DescribeUserStackAssociationsResultTypeDef",
+    {
+        "UserStackAssociations": List[UserStackAssociationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UserStackAssociationErrorTypeDef = TypedDict(
+    "UserStackAssociationErrorTypeDef",
+    {
+        "UserStackAssociation": UserStackAssociationTypeDef,
+        "ErrorCode": UserStackAssociationErrorCodeType,
+        "ErrorMessage": str,
+    },
+    total=False,
+)
+
 _RequiredCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
         "Platform": Literal["WINDOWS_SERVER_2019"],
         "InstanceType": str,
         "VpcConfig": VpcConfigTypeDef,
@@ -1816,22 +1556,20 @@
         "EnableDefaultInternetAccess": bool,
         "IamRoleArn": str,
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
     },
     total=False,
 )
 
-
 class CreateAppBlockBuilderRequestRequestTypeDef(
     _RequiredCreateAppBlockBuilderRequestRequestTypeDef,
     _OptionalCreateAppBlockBuilderRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
@@ -1846,125 +1584,62 @@
         "IamRoleArn": str,
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
         "AttributesToDelete": Sequence[AppBlockBuilderAttributeType],
     },
     total=False,
 )
 
-
 class UpdateAppBlockBuilderRequestRequestTypeDef(
     _RequiredUpdateAppBlockBuilderRequestRequestTypeDef,
     _OptionalUpdateAppBlockBuilderRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateApplicationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "IconS3Location": S3LocationTypeDef,
-        "LaunchPath": str,
-        "Platforms": Sequence[PlatformTypeType],
-        "InstanceFamilies": Sequence[str],
-        "AppBlockArn": str,
-    },
-)
-_OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateApplicationRequestRequestTypeDef",
-    {
-        "DisplayName": str,
-        "Description": str,
-        "WorkingDirectory": str,
-        "LaunchParameters": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateApplicationRequestRequestTypeDef(
-    _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredScriptDetailsTypeDef = TypedDict(
-    "_RequiredScriptDetailsTypeDef",
-    {
-        "ScriptS3Location": S3LocationTypeDef,
-        "ExecutablePath": str,
-        "TimeoutInSeconds": int,
-    },
-)
-_OptionalScriptDetailsTypeDef = TypedDict(
-    "_OptionalScriptDetailsTypeDef",
-    {
-        "ExecutableParameters": str,
-    },
-    total=False,
-)
-
-
-class ScriptDetailsTypeDef(_RequiredScriptDetailsTypeDef, _OptionalScriptDetailsTypeDef):
-    pass
-
-
-_RequiredUpdateApplicationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateApplicationRequestRequestTypeDef",
+_RequiredCreateDirectoryConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDirectoryConfigRequestRequestTypeDef",
     {
-        "Name": str,
+        "DirectoryName": str,
+        "OrganizationalUnitDistinguishedNames": Sequence[str],
     },
 )
-_OptionalUpdateApplicationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateApplicationRequestRequestTypeDef",
+_OptionalCreateDirectoryConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDirectoryConfigRequestRequestTypeDef",
     {
-        "DisplayName": str,
-        "Description": str,
-        "IconS3Location": S3LocationTypeDef,
-        "LaunchPath": str,
-        "WorkingDirectory": str,
-        "LaunchParameters": str,
-        "AppBlockArn": str,
-        "AttributesToDelete": Sequence[ApplicationAttributeType],
+        "ServiceAccountCredentials": ServiceAccountCredentialsTypeDef,
+        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
     },
     total=False,
 )
 
-
-class UpdateApplicationRequestRequestTypeDef(
-    _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
+class CreateDirectoryConfigRequestRequestTypeDef(
+    _RequiredCreateDirectoryConfigRequestRequestTypeDef,
+    _OptionalCreateDirectoryConfigRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredCreateDirectoryConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDirectoryConfigRequestRequestTypeDef",
+_RequiredDirectoryConfigTypeDef = TypedDict(
+    "_RequiredDirectoryConfigTypeDef",
     {
         "DirectoryName": str,
-        "OrganizationalUnitDistinguishedNames": Sequence[str],
     },
 )
-_OptionalCreateDirectoryConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDirectoryConfigRequestRequestTypeDef",
+_OptionalDirectoryConfigTypeDef = TypedDict(
+    "_OptionalDirectoryConfigTypeDef",
     {
+        "OrganizationalUnitDistinguishedNames": List[str],
         "ServiceAccountCredentials": ServiceAccountCredentialsTypeDef,
+        "CreatedTime": datetime,
         "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
     },
     total=False,
 )
 
-
-class CreateDirectoryConfigRequestRequestTypeDef(
-    _RequiredCreateDirectoryConfigRequestRequestTypeDef,
-    _OptionalCreateDirectoryConfigRequestRequestTypeDef,
-):
+class DirectoryConfigTypeDef(_RequiredDirectoryConfigTypeDef, _OptionalDirectoryConfigTypeDef):
     pass
 
-
 _RequiredUpdateDirectoryConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDirectoryConfigRequestRequestTypeDef",
     {
         "DirectoryName": str,
     },
 )
 _OptionalUpdateDirectoryConfigRequestRequestTypeDef = TypedDict(
@@ -1973,22 +1648,20 @@
         "OrganizationalUnitDistinguishedNames": Sequence[str],
         "ServiceAccountCredentials": ServiceAccountCredentialsTypeDef,
         "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDirectoryConfigRequestRequestTypeDef(
     _RequiredUpdateDirectoryConfigRequestRequestTypeDef,
     _OptionalUpdateDirectoryConfigRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateEntitlementRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntitlementRequestRequestTypeDef",
     {
         "Name": str,
         "StackName": str,
         "AppVisibility": AppVisibilityType,
         "Attributes": Sequence[EntitlementAttributeTypeDef],
@@ -1998,20 +1671,40 @@
     "_OptionalCreateEntitlementRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateEntitlementRequestRequestTypeDef(
     _RequiredCreateEntitlementRequestRequestTypeDef, _OptionalCreateEntitlementRequestRequestTypeDef
 ):
     pass
 
+_RequiredEntitlementTypeDef = TypedDict(
+    "_RequiredEntitlementTypeDef",
+    {
+        "Name": str,
+        "StackName": str,
+        "AppVisibility": AppVisibilityType,
+        "Attributes": List[EntitlementAttributeTypeDef],
+    },
+)
+_OptionalEntitlementTypeDef = TypedDict(
+    "_OptionalEntitlementTypeDef",
+    {
+        "Description": str,
+        "CreatedTime": datetime,
+        "LastModifiedTime": datetime,
+    },
+    total=False,
+)
+
+class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
+    pass
 
 _RequiredUpdateEntitlementRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEntitlementRequestRequestTypeDef",
     {
         "Name": str,
         "StackName": str,
     },
@@ -2022,21 +1715,19 @@
         "Description": str,
         "AppVisibility": AppVisibilityType,
         "Attributes": Sequence[EntitlementAttributeTypeDef],
     },
     total=False,
 )
 
-
 class UpdateEntitlementRequestRequestTypeDef(
     _RequiredUpdateEntitlementRequestRequestTypeDef, _OptionalUpdateEntitlementRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFleetRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceType": str,
     },
 )
@@ -2062,21 +1753,19 @@
         "MaxConcurrentSessions": int,
         "UsbDeviceFilterStrings": Sequence[str],
         "SessionScriptS3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
-
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateImageBuilderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageBuilderRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceType": str,
     },
 )
@@ -2094,22 +1783,20 @@
         "AppstreamAgentVersion": str,
         "Tags": Mapping[str, str],
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
     },
     total=False,
 )
 
-
 class CreateImageBuilderRequestRequestTypeDef(
     _RequiredCreateImageBuilderRequestRequestTypeDef,
     _OptionalCreateImageBuilderRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateFleetRequestRequestTypeDef = TypedDict(
     "UpdateFleetRequestRequestTypeDef",
     {
         "ImageName": str,
         "ImageArn": str,
         "Name": str,
         "InstanceType": str,
@@ -2154,21 +1841,19 @@
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
         "EmbedHostDomains": Sequence[str],
         "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
     },
     total=False,
 )
 
-
 class CreateStackRequestRequestTypeDef(
     _RequiredCreateStackRequestRequestTypeDef, _OptionalCreateStackRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateStackRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStackRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateStackRequestRequestTypeDef = TypedDict(
@@ -2186,123 +1871,197 @@
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
         "EmbedHostDomains": Sequence[str],
         "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateStackRequestRequestTypeDef(
     _RequiredUpdateStackRequestRequestTypeDef, _OptionalUpdateStackRequestRequestTypeDef
 ):
     pass
 
+DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef = TypedDict(
+    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
+    {
+        "DirectoryNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-DescribeFleetsRequestFleetStartedWaitTypeDef = TypedDict(
-    "DescribeFleetsRequestFleetStartedWaitTypeDef",
+DescribeFleetsRequestDescribeFleetsPaginateTypeDef = TypedDict(
+    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
     {
         "Names": Sequence[str],
-        "NextToken": str,
-        "WaiterConfig": WaiterConfigTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeFleetsRequestFleetStoppedWaitTypeDef = TypedDict(
-    "DescribeFleetsRequestFleetStoppedWaitTypeDef",
+DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef = TypedDict(
+    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
     {
         "Names": Sequence[str],
-        "NextToken": str,
-        "WaiterConfig": WaiterConfigTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeUserStackAssociationsResultTypeDef = TypedDict(
-    "DescribeUserStackAssociationsResultTypeDef",
+DescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
-        "UserStackAssociations": List[UserStackAssociationOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Names": Sequence[str],
+        "Arns": Sequence[str],
+        "Type": VisibilityTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-UserStackAssociationErrorTypeDef = TypedDict(
-    "UserStackAssociationErrorTypeDef",
+_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     {
-        "UserStackAssociation": UserStackAssociationOutputTypeDef,
-        "ErrorCode": UserStackAssociationErrorCodeType,
-        "ErrorMessage": str,
+        "StackName": str,
+        "FleetName": str,
+    },
+)
+_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
+    {
+        "UserId": str,
+        "AuthenticationType": AuthenticationTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeUsersResultTypeDef = TypedDict(
-    "DescribeUsersResultTypeDef",
+class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
+    _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
+    _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
+):
+    pass
+
+DescribeStacksRequestDescribeStacksPaginateTypeDef = TypedDict(
+    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
     {
-        "Users": List[UserTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Names": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredDirectoryConfigTypeDef = TypedDict(
-    "_RequiredDirectoryConfigTypeDef",
+DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef = TypedDict(
+    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
     {
-        "DirectoryName": str,
+        "StackName": str,
+        "UserName": str,
+        "AuthenticationType": AuthenticationTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalDirectoryConfigTypeDef = TypedDict(
-    "_OptionalDirectoryConfigTypeDef",
+
+_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef",
     {
-        "OrganizationalUnitDistinguishedNames": List[str],
-        "ServiceAccountCredentials": ServiceAccountCredentialsOutputTypeDef,
-        "CreatedTime": datetime,
-        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesOutputTypeDef,
+        "AuthenticationType": AuthenticationTypeType,
+    },
+)
+_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class DirectoryConfigTypeDef(_RequiredDirectoryConfigTypeDef, _OptionalDirectoryConfigTypeDef):
+class DescribeUsersRequestDescribeUsersPaginateTypeDef(
+    _RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef,
+    _OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef,
+):
     pass
 
-
-ListEntitledApplicationsResultTypeDef = TypedDict(
-    "ListEntitledApplicationsResultTypeDef",
+_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
     {
-        "EntitledApplications": List[EntitledApplicationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StackName": str,
+    },
+)
+_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredEntitlementTypeDef = TypedDict(
-    "_RequiredEntitlementTypeDef",
+class ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef(
+    _RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
+    _OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
+):
+    pass
+
+_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     {
-        "Name": str,
-        "StackName": str,
-        "AppVisibility": AppVisibilityType,
-        "Attributes": List[EntitlementAttributeOutputTypeDef],
+        "FleetName": str,
     },
 )
-_OptionalEntitlementTypeDef = TypedDict(
-    "_OptionalEntitlementTypeDef",
+_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     {
-        "Description": str,
-        "CreatedTime": datetime,
-        "LastModifiedTime": datetime,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
+class ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef(
+    _RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
+    _OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
+):
     pass
 
+DescribeFleetsRequestFleetStartedWaitTypeDef = TypedDict(
+    "DescribeFleetsRequestFleetStartedWaitTypeDef",
+    {
+        "Names": Sequence[str],
+        "NextToken": str,
+        "WaiterConfig": WaiterConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeFleetsRequestFleetStoppedWaitTypeDef = TypedDict(
+    "DescribeFleetsRequestFleetStoppedWaitTypeDef",
+    {
+        "Names": Sequence[str],
+        "NextToken": str,
+        "WaiterConfig": WaiterConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeUsersResultTypeDef = TypedDict(
+    "DescribeUsersResultTypeDef",
+    {
+        "Users": List[UserTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEntitledApplicationsResultTypeDef = TypedDict(
+    "ListEntitledApplicationsResultTypeDef",
+    {
+        "EntitledApplications": List[EntitledApplicationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredFleetTypeDef = TypedDict(
     "_RequiredFleetTypeDef",
     {
         "Arn": str,
         "Name": str,
         "InstanceType": str,
@@ -2320,31 +2079,29 @@
         "FleetType": FleetTypeType,
         "MaxUserDurationInSeconds": int,
         "DisconnectTimeoutInSeconds": int,
         "VpcConfig": VpcConfigOutputTypeDef,
         "CreatedTime": datetime,
         "FleetErrors": List[FleetErrorTypeDef],
         "EnableDefaultInternetAccess": bool,
-        "DomainJoinInfo": DomainJoinInfoOutputTypeDef,
+        "DomainJoinInfo": DomainJoinInfoTypeDef,
         "IdleDisconnectTimeoutInSeconds": int,
         "IamRoleArn": str,
         "StreamView": StreamViewType,
         "Platform": PlatformTypeType,
         "MaxConcurrentSessions": int,
         "UsbDeviceFilterStrings": List[str],
-        "SessionScriptS3Location": S3LocationOutputTypeDef,
+        "SessionScriptS3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
-
 class FleetTypeDef(_RequiredFleetTypeDef, _OptionalFleetTypeDef):
     pass
 
-
 _RequiredImageBuilderTypeDef = TypedDict(
     "_RequiredImageBuilderTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalImageBuilderTypeDef = TypedDict(
@@ -2358,28 +2115,26 @@
         "InstanceType": str,
         "Platform": PlatformTypeType,
         "IamRoleArn": str,
         "State": ImageBuilderStateType,
         "StateChangeReason": ImageBuilderStateChangeReasonTypeDef,
         "CreatedTime": datetime,
         "EnableDefaultInternetAccess": bool,
-        "DomainJoinInfo": DomainJoinInfoOutputTypeDef,
+        "DomainJoinInfo": DomainJoinInfoTypeDef,
         "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
         "ImageBuilderErrors": List[ResourceErrorTypeDef],
         "AppstreamAgentVersion": str,
-        "AccessEndpoints": List[AccessEndpointOutputTypeDef],
+        "AccessEndpoints": List[AccessEndpointTypeDef],
     },
     total=False,
 )
 
-
 class ImageBuilderTypeDef(_RequiredImageBuilderTypeDef, _OptionalImageBuilderTypeDef):
     pass
 
-
 _RequiredSessionTypeDef = TypedDict(
     "_RequiredSessionTypeDef",
     {
         "Id": str,
         "UserId": str,
         "StackName": str,
         "FleetName": str,
@@ -2394,24 +2149,22 @@
         "MaxExpirationTime": datetime,
         "AuthenticationType": AuthenticationTypeType,
         "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
     pass
 
-
 SharedImagePermissionsTypeDef = TypedDict(
     "SharedImagePermissionsTypeDef",
     {
         "sharedAccountId": str,
-        "imagePermissions": ImagePermissionsOutputTypeDef,
+        "imagePermissions": ImagePermissionsTypeDef,
     },
 )
 
 UpdateImagePermissionsRequestRequestTypeDef = TypedDict(
     "UpdateImagePermissionsRequestRequestTypeDef",
     {
         "Name": str,
@@ -2444,83 +2197,81 @@
         "Description": str,
         "DisplayName": str,
         "CreatedTime": datetime,
         "StorageConnectors": List[StorageConnectorOutputTypeDef],
         "RedirectURL": str,
         "FeedbackURL": str,
         "StackErrors": List[StackErrorTypeDef],
-        "UserSettings": List[UserSettingOutputTypeDef],
+        "UserSettings": List[UserSettingTypeDef],
         "ApplicationSettings": ApplicationSettingsResponseTypeDef,
-        "AccessEndpoints": List[AccessEndpointOutputTypeDef],
+        "AccessEndpoints": List[AccessEndpointTypeDef],
         "EmbedHostDomains": List[str],
-        "StreamingExperienceSettings": StreamingExperienceSettingsOutputTypeDef,
+        "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
     },
     total=False,
 )
 
-
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
 
-
 CreateAppBlockBuilderResultTypeDef = TypedDict(
     "CreateAppBlockBuilderResultTypeDef",
     {
         "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppBlockBuildersResultTypeDef = TypedDict(
     "DescribeAppBlockBuildersResultTypeDef",
     {
         "AppBlockBuilders": List[AppBlockBuilderTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartAppBlockBuilderResultTypeDef = TypedDict(
     "StartAppBlockBuilderResultTypeDef",
     {
         "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopAppBlockBuilderResultTypeDef = TypedDict(
     "StopAppBlockBuilderResultTypeDef",
     {
         "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppBlockBuilderResultTypeDef = TypedDict(
     "UpdateAppBlockBuilderResultTypeDef",
     {
         "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateApplicationResultTypeDef = TypedDict(
     "CreateApplicationResultTypeDef",
     {
         "Application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationsResultTypeDef = TypedDict(
     "DescribeApplicationsResultTypeDef",
     {
         "Applications": List[ApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImageTypeDef = TypedDict(
     "_RequiredImageTypeDef",
     {
         "Name": str,
@@ -2539,30 +2290,28 @@
         "Platform": PlatformTypeType,
         "Description": str,
         "StateChangeReason": ImageStateChangeReasonTypeDef,
         "Applications": List[ApplicationTypeDef],
         "CreatedTime": datetime,
         "PublicBaseImageReleasedDate": datetime,
         "AppstreamAgentVersion": str,
-        "ImagePermissions": ImagePermissionsOutputTypeDef,
+        "ImagePermissions": ImagePermissionsTypeDef,
         "ImageErrors": List[ResourceErrorTypeDef],
     },
     total=False,
 )
 
-
 class ImageTypeDef(_RequiredImageTypeDef, _OptionalImageTypeDef):
     pass
 
-
 UpdateApplicationResultTypeDef = TypedDict(
     "UpdateApplicationResultTypeDef",
     {
         "Application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAppBlockTypeDef = TypedDict(
     "_RequiredAppBlockTypeDef",
     {
         "Name": str,
@@ -2570,30 +2319,28 @@
     },
 )
 _OptionalAppBlockTypeDef = TypedDict(
     "_OptionalAppBlockTypeDef",
     {
         "Description": str,
         "DisplayName": str,
-        "SourceS3Location": S3LocationOutputTypeDef,
-        "SetupScriptDetails": ScriptDetailsOutputTypeDef,
+        "SourceS3Location": S3LocationTypeDef,
+        "SetupScriptDetails": ScriptDetailsTypeDef,
         "CreatedTime": datetime,
-        "PostSetupScriptDetails": ScriptDetailsOutputTypeDef,
+        "PostSetupScriptDetails": ScriptDetailsTypeDef,
         "PackagingType": PackagingTypeType,
         "State": AppBlockStateType,
         "AppBlockErrors": List[ErrorDetailsTypeDef],
     },
     total=False,
 )
 
-
 class AppBlockTypeDef(_RequiredAppBlockTypeDef, _OptionalAppBlockTypeDef):
     pass
 
-
 _RequiredCreateAppBlockRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppBlockRequestRequestTypeDef",
     {
         "Name": str,
         "SourceS3Location": S3LocationTypeDef,
     },
 )
@@ -2606,241 +2353,239 @@
         "Tags": Mapping[str, str],
         "PostSetupScriptDetails": ScriptDetailsTypeDef,
         "PackagingType": PackagingTypeType,
     },
     total=False,
 )
 
-
 class CreateAppBlockRequestRequestTypeDef(
     _RequiredCreateAppBlockRequestRequestTypeDef, _OptionalCreateAppBlockRequestRequestTypeDef
 ):
     pass
 
-
 BatchAssociateUserStackResultTypeDef = TypedDict(
     "BatchAssociateUserStackResultTypeDef",
     {
         "errors": List[UserStackAssociationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateUserStackResultTypeDef = TypedDict(
     "BatchDisassociateUserStackResultTypeDef",
     {
         "errors": List[UserStackAssociationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDirectoryConfigResultTypeDef = TypedDict(
     "CreateDirectoryConfigResultTypeDef",
     {
         "DirectoryConfig": DirectoryConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDirectoryConfigsResultTypeDef = TypedDict(
     "DescribeDirectoryConfigsResultTypeDef",
     {
         "DirectoryConfigs": List[DirectoryConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDirectoryConfigResultTypeDef = TypedDict(
     "UpdateDirectoryConfigResultTypeDef",
     {
         "DirectoryConfig": DirectoryConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEntitlementResultTypeDef = TypedDict(
     "CreateEntitlementResultTypeDef",
     {
         "Entitlement": EntitlementTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEntitlementsResultTypeDef = TypedDict(
     "DescribeEntitlementsResultTypeDef",
     {
         "Entitlements": List[EntitlementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEntitlementResultTypeDef = TypedDict(
     "UpdateEntitlementResultTypeDef",
     {
         "Entitlement": EntitlementTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFleetResultTypeDef = TypedDict(
     "CreateFleetResultTypeDef",
     {
         "Fleet": FleetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFleetsResultTypeDef = TypedDict(
     "DescribeFleetsResultTypeDef",
     {
         "Fleets": List[FleetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFleetResultTypeDef = TypedDict(
     "UpdateFleetResultTypeDef",
     {
         "Fleet": FleetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateImageBuilderResultTypeDef = TypedDict(
     "CreateImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteImageBuilderResultTypeDef = TypedDict(
     "DeleteImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImageBuildersResultTypeDef = TypedDict(
     "DescribeImageBuildersResultTypeDef",
     {
         "ImageBuilders": List[ImageBuilderTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartImageBuilderResultTypeDef = TypedDict(
     "StartImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopImageBuilderResultTypeDef = TypedDict(
     "StopImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSessionsResultTypeDef = TypedDict(
     "DescribeSessionsResultTypeDef",
     {
         "Sessions": List[SessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImagePermissionsResultTypeDef = TypedDict(
     "DescribeImagePermissionsResultTypeDef",
     {
         "Name": str,
         "SharedImagePermissionsList": List[SharedImagePermissionsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUsageReportSubscriptionsResultTypeDef = TypedDict(
     "DescribeUsageReportSubscriptionsResultTypeDef",
     {
         "UsageReportSubscriptions": List[UsageReportSubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStackResultTypeDef = TypedDict(
     "CreateStackResultTypeDef",
     {
         "Stack": StackTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStacksResultTypeDef = TypedDict(
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStackResultTypeDef = TypedDict(
     "UpdateStackResultTypeDef",
     {
         "Stack": StackTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateUpdatedImageResultTypeDef = TypedDict(
     "CreateUpdatedImageResultTypeDef",
     {
         "image": ImageTypeDef,
         "canUpdateImage": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteImageResultTypeDef = TypedDict(
     "DeleteImageResultTypeDef",
     {
         "Image": ImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImagesResultTypeDef = TypedDict(
     "DescribeImagesResultTypeDef",
     {
         "Images": List[ImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAppBlockResultTypeDef = TypedDict(
     "CreateAppBlockResultTypeDef",
     {
         "AppBlock": AppBlockTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppBlocksResultTypeDef = TypedDict(
     "DescribeAppBlocksResultTypeDef",
     {
         "AppBlocks": List[AppBlockTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/type_defs.pyi` & `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for appstream service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_appstream.type_defs import AccessEndpointOutputTypeDef
+    from mypy_boto3_appstream.type_defs import AccessEndpointTypeDef
 
-    data: AccessEndpointOutputTypeDef = {...}
+    data: AccessEndpointTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -53,53 +53,47 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "AccessEndpointOutputTypeDef",
     "AccessEndpointTypeDef",
     "AppBlockBuilderAppBlockAssociationTypeDef",
     "AppBlockBuilderStateChangeReasonTypeDef",
     "ResourceErrorTypeDef",
     "VpcConfigOutputTypeDef",
     "ErrorDetailsTypeDef",
-    "S3LocationOutputTypeDef",
+    "S3LocationTypeDef",
     "ApplicationFleetAssociationTypeDef",
     "ApplicationSettingsResponseTypeDef",
     "ApplicationSettingsTypeDef",
     "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateApplicationFleetRequestRequestTypeDef",
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     "AssociateFleetRequestRequestTypeDef",
     "UserStackAssociationTypeDef",
-    "CertificateBasedAuthPropertiesOutputTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
     "ComputeCapacityStatusTypeDef",
     "ComputeCapacityTypeDef",
     "CopyImageRequestRequestTypeDef",
-    "CopyImageResponseTypeDef",
     "VpcConfigTypeDef",
     "CreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
-    "CreateAppBlockBuilderStreamingURLResultTypeDef",
-    "S3LocationTypeDef",
     "ServiceAccountCredentialsTypeDef",
     "EntitlementAttributeTypeDef",
     "DomainJoinInfoTypeDef",
     "CreateImageBuilderStreamingURLRequestRequestTypeDef",
-    "CreateImageBuilderStreamingURLResultTypeDef",
     "StorageConnectorTypeDef",
     "StreamingExperienceSettingsTypeDef",
     "UserSettingTypeDef",
     "CreateStreamingURLRequestRequestTypeDef",
-    "CreateStreamingURLResultTypeDef",
     "CreateUpdatedImageRequestRequestTypeDef",
-    "CreateUsageReportSubscriptionResultTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DeleteAppBlockBuilderRequestRequestTypeDef",
     "DeleteAppBlockRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteDirectoryConfigRequestRequestTypeDef",
     "DeleteEntitlementRequestRequestTypeDef",
     "DeleteFleetRequestRequestTypeDef",
@@ -109,108 +103,104 @@
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef",
     "DescribeAppBlockBuildersRequestRequestTypeDef",
     "DescribeAppBlocksRequestRequestTypeDef",
     "DescribeApplicationFleetAssociationsRequestRequestTypeDef",
     "DescribeApplicationsRequestRequestTypeDef",
-    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeDirectoryConfigsRequestRequestTypeDef",
     "DescribeEntitlementsRequestRequestTypeDef",
-    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeFleetsRequestRequestTypeDef",
-    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
     "DescribeImageBuildersRequestRequestTypeDef",
     "DescribeImagePermissionsRequestRequestTypeDef",
-    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
-    "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     "DescribeSessionsRequestRequestTypeDef",
-    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
     "DescribeStacksRequestRequestTypeDef",
     "DescribeUsageReportSubscriptionsRequestRequestTypeDef",
-    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
     "DescribeUserStackAssociationsRequestRequestTypeDef",
-    "UserStackAssociationOutputTypeDef",
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
     "UserTypeDef",
-    "ServiceAccountCredentialsOutputTypeDef",
     "DisableUserRequestRequestTypeDef",
     "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "DisassociateApplicationFleetRequestRequestTypeDef",
     "DisassociateApplicationFromEntitlementRequestRequestTypeDef",
     "DisassociateFleetRequestRequestTypeDef",
-    "DomainJoinInfoOutputTypeDef",
     "EnableUserRequestRequestTypeDef",
     "EntitledApplicationTypeDef",
-    "EntitlementAttributeOutputTypeDef",
     "ExpireSessionRequestRequestTypeDef",
     "FleetErrorTypeDef",
     "ImageBuilderStateChangeReasonTypeDef",
     "NetworkAccessConfigurationTypeDef",
-    "ImagePermissionsOutputTypeDef",
     "ImagePermissionsTypeDef",
     "ImageStateChangeReasonTypeDef",
     "LastReportGenerationExecutionErrorTypeDef",
-    "ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
     "ListAssociatedFleetsRequestRequestTypeDef",
-    "ListAssociatedFleetsResultTypeDef",
-    "ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     "ListAssociatedStacksRequestRequestTypeDef",
-    "ListAssociatedStacksResultTypeDef",
     "ListEntitledApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StackErrorTypeDef",
     "StorageConnectorOutputTypeDef",
-    "StreamingExperienceSettingsOutputTypeDef",
-    "UserSettingOutputTypeDef",
     "StartAppBlockBuilderRequestRequestTypeDef",
     "StartFleetRequestRequestTypeDef",
     "StartImageBuilderRequestRequestTypeDef",
     "StopAppBlockBuilderRequestRequestTypeDef",
     "StopFleetRequestRequestTypeDef",
     "StopImageBuilderRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AssociateAppBlockBuilderAppBlockResultTypeDef",
-    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
     "AppBlockBuilderTypeDef",
     "ApplicationTypeDef",
-    "ScriptDetailsOutputTypeDef",
+    "CreateApplicationRequestRequestTypeDef",
+    "ScriptDetailsTypeDef",
+    "UpdateApplicationRequestRequestTypeDef",
+    "AssociateAppBlockBuilderAppBlockResultTypeDef",
     "AssociateApplicationFleetResultTypeDef",
+    "CopyImageResponseTypeDef",
+    "CreateAppBlockBuilderStreamingURLResultTypeDef",
+    "CreateImageBuilderStreamingURLResultTypeDef",
+    "CreateStreamingURLResultTypeDef",
+    "CreateUsageReportSubscriptionResultTypeDef",
+    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
     "DescribeApplicationFleetAssociationsResultTypeDef",
+    "ListAssociatedFleetsResultTypeDef",
+    "ListAssociatedStacksResultTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "BatchAssociateUserStackRequestRequestTypeDef",
     "BatchDisassociateUserStackRequestRequestTypeDef",
+    "DescribeUserStackAssociationsResultTypeDef",
+    "UserStackAssociationErrorTypeDef",
     "CreateAppBlockBuilderRequestRequestTypeDef",
     "UpdateAppBlockBuilderRequestRequestTypeDef",
-    "CreateApplicationRequestRequestTypeDef",
-    "ScriptDetailsTypeDef",
-    "UpdateApplicationRequestRequestTypeDef",
     "CreateDirectoryConfigRequestRequestTypeDef",
+    "DirectoryConfigTypeDef",
     "UpdateDirectoryConfigRequestRequestTypeDef",
     "CreateEntitlementRequestRequestTypeDef",
+    "EntitlementTypeDef",
     "UpdateEntitlementRequestRequestTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateImageBuilderRequestRequestTypeDef",
     "UpdateFleetRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "UpdateStackRequestRequestTypeDef",
+    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
+    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
+    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
+    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
+    "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
+    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
+    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
+    "ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
+    "ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     "DescribeFleetsRequestFleetStartedWaitTypeDef",
     "DescribeFleetsRequestFleetStoppedWaitTypeDef",
-    "DescribeUserStackAssociationsResultTypeDef",
-    "UserStackAssociationErrorTypeDef",
     "DescribeUsersResultTypeDef",
-    "DirectoryConfigTypeDef",
     "ListEntitledApplicationsResultTypeDef",
-    "EntitlementTypeDef",
     "FleetTypeDef",
     "ImageBuilderTypeDef",
     "SessionTypeDef",
     "SharedImagePermissionsTypeDef",
     "UpdateImagePermissionsRequestRequestTypeDef",
     "UsageReportSubscriptionTypeDef",
     "StackTypeDef",
@@ -250,50 +240,33 @@
     "CreateUpdatedImageResultTypeDef",
     "DeleteImageResultTypeDef",
     "DescribeImagesResultTypeDef",
     "CreateAppBlockResultTypeDef",
     "DescribeAppBlocksResultTypeDef",
 )
 
-_RequiredAccessEndpointOutputTypeDef = TypedDict(
-    "_RequiredAccessEndpointOutputTypeDef",
-    {
-        "EndpointType": Literal["STREAMING"],
-    },
-)
-_OptionalAccessEndpointOutputTypeDef = TypedDict(
-    "_OptionalAccessEndpointOutputTypeDef",
-    {
-        "VpceId": str,
-    },
-    total=False,
-)
-
-class AccessEndpointOutputTypeDef(
-    _RequiredAccessEndpointOutputTypeDef, _OptionalAccessEndpointOutputTypeDef
-):
-    pass
-
 _RequiredAccessEndpointTypeDef = TypedDict(
     "_RequiredAccessEndpointTypeDef",
     {
         "EndpointType": Literal["STREAMING"],
     },
 )
 _OptionalAccessEndpointTypeDef = TypedDict(
     "_OptionalAccessEndpointTypeDef",
     {
         "VpceId": str,
     },
     total=False,
 )
 
+
 class AccessEndpointTypeDef(_RequiredAccessEndpointTypeDef, _OptionalAccessEndpointTypeDef):
     pass
 
+
 AppBlockBuilderAppBlockAssociationTypeDef = TypedDict(
     "AppBlockBuilderAppBlockAssociationTypeDef",
     {
         "AppBlockArn": str,
         "AppBlockBuilderName": str,
     },
 )
@@ -331,31 +304,33 @@
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-_RequiredS3LocationOutputTypeDef = TypedDict(
-    "_RequiredS3LocationOutputTypeDef",
+_RequiredS3LocationTypeDef = TypedDict(
+    "_RequiredS3LocationTypeDef",
     {
         "S3Bucket": str,
     },
 )
-_OptionalS3LocationOutputTypeDef = TypedDict(
-    "_OptionalS3LocationOutputTypeDef",
+_OptionalS3LocationTypeDef = TypedDict(
+    "_OptionalS3LocationTypeDef",
     {
         "S3Key": str,
     },
     total=False,
 )
 
-class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
+
+class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
+
 ApplicationFleetAssociationTypeDef = TypedDict(
     "ApplicationFleetAssociationTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -380,27 +355,40 @@
     "_OptionalApplicationSettingsTypeDef",
     {
         "SettingsGroup": str,
     },
     total=False,
 )
 
+
 class ApplicationSettingsTypeDef(
     _RequiredApplicationSettingsTypeDef, _OptionalApplicationSettingsTypeDef
 ):
     pass
 
+
 AssociateAppBlockBuilderAppBlockRequestRequestTypeDef = TypedDict(
     "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     {
         "AppBlockArn": str,
         "AppBlockBuilderName": str,
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
 AssociateApplicationFleetRequestRequestTypeDef = TypedDict(
     "AssociateApplicationFleetRequestRequestTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -434,27 +422,20 @@
     "_OptionalUserStackAssociationTypeDef",
     {
         "SendEmailNotification": bool,
     },
     total=False,
 )
 
+
 class UserStackAssociationTypeDef(
     _RequiredUserStackAssociationTypeDef, _OptionalUserStackAssociationTypeDef
 ):
     pass
 
-CertificateBasedAuthPropertiesOutputTypeDef = TypedDict(
-    "CertificateBasedAuthPropertiesOutputTypeDef",
-    {
-        "Status": CertificateBasedAuthStatusType,
-        "CertificateAuthorityArn": str,
-    },
-    total=False,
-)
 
 CertificateBasedAuthPropertiesTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesTypeDef",
     {
         "Status": CertificateBasedAuthStatusType,
         "CertificateAuthorityArn": str,
     },
@@ -473,19 +454,21 @@
         "Running": int,
         "InUse": int,
         "Available": int,
     },
     total=False,
 )
 
+
 class ComputeCapacityStatusTypeDef(
     _RequiredComputeCapacityStatusTypeDef, _OptionalComputeCapacityStatusTypeDef
 ):
     pass
 
+
 ComputeCapacityTypeDef = TypedDict(
     "ComputeCapacityTypeDef",
     {
         "DesiredInstances": int,
     },
 )
 
@@ -501,26 +484,20 @@
     "_OptionalCopyImageRequestRequestTypeDef",
     {
         "DestinationImageDescription": str,
     },
     total=False,
 )
 
+
 class CopyImageRequestRequestTypeDef(
     _RequiredCopyImageRequestRequestTypeDef, _OptionalCopyImageRequestRequestTypeDef
 ):
     pass
 
-CopyImageResponseTypeDef = TypedDict(
-    "CopyImageResponseTypeDef",
-    {
-        "DestinationImageName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 VpcConfigTypeDef = TypedDict(
     "VpcConfigTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
@@ -537,45 +514,21 @@
     "_OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
     {
         "Validity": int,
     },
     total=False,
 )
 
+
 class CreateAppBlockBuilderStreamingURLRequestRequestTypeDef(
     _RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
     _OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
 ):
     pass
 
-CreateAppBlockBuilderStreamingURLResultTypeDef = TypedDict(
-    "CreateAppBlockBuilderStreamingURLResultTypeDef",
-    {
-        "StreamingURL": str,
-        "Expires": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredS3LocationTypeDef = TypedDict(
-    "_RequiredS3LocationTypeDef",
-    {
-        "S3Bucket": str,
-    },
-)
-_OptionalS3LocationTypeDef = TypedDict(
-    "_OptionalS3LocationTypeDef",
-    {
-        "S3Key": str,
-    },
-    total=False,
-)
-
-class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
-    pass
 
 ServiceAccountCredentialsTypeDef = TypedDict(
     "ServiceAccountCredentialsTypeDef",
     {
         "AccountName": str,
         "AccountPassword": str,
     },
@@ -608,28 +561,21 @@
     "_OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef",
     {
         "Validity": int,
     },
     total=False,
 )
 
+
 class CreateImageBuilderStreamingURLRequestRequestTypeDef(
     _RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef,
     _OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef,
 ):
     pass
 
-CreateImageBuilderStreamingURLResultTypeDef = TypedDict(
-    "CreateImageBuilderStreamingURLResultTypeDef",
-    {
-        "StreamingURL": str,
-        "Expires": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredStorageConnectorTypeDef = TypedDict(
     "_RequiredStorageConnectorTypeDef",
     {
         "ConnectorType": StorageConnectorTypeType,
     },
 )
@@ -638,17 +584,19 @@
     {
         "ResourceIdentifier": str,
         "Domains": Sequence[str],
     },
     total=False,
 )
 
+
 class StorageConnectorTypeDef(_RequiredStorageConnectorTypeDef, _OptionalStorageConnectorTypeDef):
     pass
 
+
 StreamingExperienceSettingsTypeDef = TypedDict(
     "StreamingExperienceSettingsTypeDef",
     {
         "PreferredProtocol": PreferredProtocolType,
     },
     total=False,
 )
@@ -675,28 +623,21 @@
         "ApplicationId": str,
         "Validity": int,
         "SessionContext": str,
     },
     total=False,
 )
 
+
 class CreateStreamingURLRequestRequestTypeDef(
     _RequiredCreateStreamingURLRequestRequestTypeDef,
     _OptionalCreateStreamingURLRequestRequestTypeDef,
 ):
     pass
 
-CreateStreamingURLResultTypeDef = TypedDict(
-    "CreateStreamingURLResultTypeDef",
-    {
-        "StreamingURL": str,
-        "Expires": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateUpdatedImageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUpdatedImageRequestRequestTypeDef",
     {
         "existingImageName": str,
         "newImageName": str,
     },
@@ -708,28 +649,21 @@
         "newImageDisplayName": str,
         "newImageTags": Mapping[str, str],
         "dryRun": bool,
     },
     total=False,
 )
 
+
 class CreateUpdatedImageRequestRequestTypeDef(
     _RequiredCreateUpdatedImageRequestRequestTypeDef,
     _OptionalCreateUpdatedImageRequestRequestTypeDef,
 ):
     pass
 
-CreateUsageReportSubscriptionResultTypeDef = TypedDict(
-    "CreateUsageReportSubscriptionResultTypeDef",
-    {
-        "S3BucketName": str,
-        "Schedule": Literal["DAILY"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
@@ -740,19 +674,21 @@
         "MessageAction": MessageActionType,
         "FirstName": str,
         "LastName": str,
     },
     total=False,
 )
 
+
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
+
 DeleteAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "DeleteAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -877,19 +813,20 @@
         "Arns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef = TypedDict(
-    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "DirectoryNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeDirectoryConfigsRequestRequestTypeDef = TypedDict(
     "DescribeDirectoryConfigsRequestRequestTypeDef",
     {
@@ -912,28 +849,21 @@
         "Name": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeEntitlementsRequestRequestTypeDef(
     _RequiredDescribeEntitlementsRequestRequestTypeDef,
     _OptionalDescribeEntitlementsRequestRequestTypeDef,
 ):
     pass
 
-DescribeFleetsRequestDescribeFleetsPaginateTypeDef = TypedDict(
-    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
@@ -945,23 +875,14 @@
     {
         "Names": Sequence[str],
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef = TypedDict(
-    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeImageBuildersRequestRequestTypeDef = TypedDict(
     "DescribeImageBuildersRequestRequestTypeDef",
     {
         "Names": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -980,66 +901,34 @@
         "MaxResults": int,
         "SharedAwsAccountIds": Sequence[str],
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeImagePermissionsRequestRequestTypeDef(
     _RequiredDescribeImagePermissionsRequestRequestTypeDef,
     _OptionalDescribeImagePermissionsRequestRequestTypeDef,
 ):
     pass
 
-DescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
-    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "Arns": Sequence[str],
-        "Type": VisibilityTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 DescribeImagesRequestRequestTypeDef = TypedDict(
     "DescribeImagesRequestRequestTypeDef",
     {
         "Names": Sequence[str],
         "Arns": Sequence[str],
         "Type": VisibilityTypeType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
-    {
-        "StackName": str,
-        "FleetName": str,
-    },
-)
-_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
-    {
-        "UserId": str,
-        "AuthenticationType": AuthenticationTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
-    _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
-    _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSessionsRequestRequestTypeDef",
     {
         "StackName": str,
         "FleetName": str,
     },
 )
@@ -1050,27 +939,20 @@
         "NextToken": str,
         "Limit": int,
         "AuthenticationType": AuthenticationTypeType,
     },
     total=False,
 )
 
+
 class DescribeSessionsRequestRequestTypeDef(
     _RequiredDescribeSessionsRequestRequestTypeDef, _OptionalDescribeSessionsRequestRequestTypeDef
 ):
     pass
 
-DescribeStacksRequestDescribeStacksPaginateTypeDef = TypedDict(
-    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 DescribeStacksRequestRequestTypeDef = TypedDict(
     "DescribeStacksRequestRequestTypeDef",
     {
         "Names": Sequence[str],
         "NextToken": str,
     },
@@ -1082,78 +964,26 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef = TypedDict(
-    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
-    {
-        "StackName": str,
-        "UserName": str,
-        "AuthenticationType": AuthenticationTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeUserStackAssociationsRequestRequestTypeDef = TypedDict(
     "DescribeUserStackAssociationsRequestRequestTypeDef",
     {
         "StackName": str,
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredUserStackAssociationOutputTypeDef = TypedDict(
-    "_RequiredUserStackAssociationOutputTypeDef",
-    {
-        "StackName": str,
-        "UserName": str,
-        "AuthenticationType": AuthenticationTypeType,
-    },
-)
-_OptionalUserStackAssociationOutputTypeDef = TypedDict(
-    "_OptionalUserStackAssociationOutputTypeDef",
-    {
-        "SendEmailNotification": bool,
-    },
-    total=False,
-)
-
-class UserStackAssociationOutputTypeDef(
-    _RequiredUserStackAssociationOutputTypeDef, _OptionalUserStackAssociationOutputTypeDef
-):
-    pass
-
-_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef",
-    {
-        "AuthenticationType": AuthenticationTypeType,
-    },
-)
-_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeUsersRequestDescribeUsersPaginateTypeDef(
-    _RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef,
-    _OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeUsersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeUsersRequestRequestTypeDef",
     {
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 _OptionalDescribeUsersRequestRequestTypeDef = TypedDict(
@@ -1161,19 +991,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeUsersRequestRequestTypeDef(
     _RequiredDescribeUsersRequestRequestTypeDef, _OptionalDescribeUsersRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUserTypeDef = TypedDict(
     "_RequiredUserTypeDef",
     {
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 _OptionalUserTypeDef = TypedDict(
@@ -1186,24 +1018,18 @@
         "FirstName": str,
         "LastName": str,
         "CreatedTime": datetime,
     },
     total=False,
 )
 
+
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
-ServiceAccountCredentialsOutputTypeDef = TypedDict(
-    "ServiceAccountCredentialsOutputTypeDef",
-    {
-        "AccountName": str,
-        "AccountPassword": str,
-    },
-)
 
 DisableUserRequestRequestTypeDef = TypedDict(
     "DisableUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
@@ -1238,23 +1064,14 @@
     "DisassociateFleetRequestRequestTypeDef",
     {
         "FleetName": str,
         "StackName": str,
     },
 )
 
-DomainJoinInfoOutputTypeDef = TypedDict(
-    "DomainJoinInfoOutputTypeDef",
-    {
-        "DirectoryName": str,
-        "OrganizationalUnitDistinguishedName": str,
-    },
-    total=False,
-)
-
 EnableUserRequestRequestTypeDef = TypedDict(
     "EnableUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
@@ -1262,22 +1079,14 @@
 EntitledApplicationTypeDef = TypedDict(
     "EntitledApplicationTypeDef",
     {
         "ApplicationIdentifier": str,
     },
 )
 
-EntitlementAttributeOutputTypeDef = TypedDict(
-    "EntitlementAttributeOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
-
 ExpireSessionRequestRequestTypeDef = TypedDict(
     "ExpireSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
@@ -1304,23 +1113,14 @@
     {
         "EniPrivateIpAddress": str,
         "EniId": str,
     },
     total=False,
 )
 
-ImagePermissionsOutputTypeDef = TypedDict(
-    "ImagePermissionsOutputTypeDef",
-    {
-        "allowFleet": bool,
-        "allowImageBuilder": bool,
-    },
-    total=False,
-)
-
 ImagePermissionsTypeDef = TypedDict(
     "ImagePermissionsTypeDef",
     {
         "allowFleet": bool,
         "allowImageBuilder": bool,
     },
     total=False,
@@ -1340,82 +1140,35 @@
     {
         "ErrorCode": UsageReportExecutionErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef(
-    _RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
-    _OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssociatedFleetsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedFleetsRequestRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListAssociatedFleetsRequestRequestTypeDef = TypedDict(
     "_OptionalListAssociatedFleetsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAssociatedFleetsRequestRequestTypeDef(
     _RequiredListAssociatedFleetsRequestRequestTypeDef,
     _OptionalListAssociatedFleetsRequestRequestTypeDef,
 ):
     pass
 
-ListAssociatedFleetsResultTypeDef = TypedDict(
-    "ListAssociatedFleetsResultTypeDef",
-    {
-        "Names": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
-    {
-        "FleetName": str,
-    },
-)
-_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef(
-    _RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
-    _OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
-):
-    pass
 
 _RequiredListAssociatedStacksRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedStacksRequestRequestTypeDef",
     {
         "FleetName": str,
     },
 )
@@ -1423,28 +1176,21 @@
     "_OptionalListAssociatedStacksRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAssociatedStacksRequestRequestTypeDef(
     _RequiredListAssociatedStacksRequestRequestTypeDef,
     _OptionalListAssociatedStacksRequestRequestTypeDef,
 ):
     pass
 
-ListAssociatedStacksResultTypeDef = TypedDict(
-    "ListAssociatedStacksResultTypeDef",
-    {
-        "Names": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredListEntitledApplicationsRequestRequestTypeDef = TypedDict(
     "_RequiredListEntitledApplicationsRequestRequestTypeDef",
     {
         "StackName": str,
         "EntitlementName": str,
     },
@@ -1454,56 +1200,29 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListEntitledApplicationsRequestRequestTypeDef(
     _RequiredListEntitledApplicationsRequestRequestTypeDef,
     _OptionalListEntitledApplicationsRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 StackErrorTypeDef = TypedDict(
     "StackErrorTypeDef",
     {
         "ErrorCode": StackErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
@@ -1520,34 +1239,20 @@
     {
         "ResourceIdentifier": str,
         "Domains": List[str],
     },
     total=False,
 )
 
+
 class StorageConnectorOutputTypeDef(
     _RequiredStorageConnectorOutputTypeDef, _OptionalStorageConnectorOutputTypeDef
 ):
     pass
 
-StreamingExperienceSettingsOutputTypeDef = TypedDict(
-    "StreamingExperienceSettingsOutputTypeDef",
-    {
-        "PreferredProtocol": PreferredProtocolType,
-    },
-    total=False,
-)
-
-UserSettingOutputTypeDef = TypedDict(
-    "UserSettingOutputTypeDef",
-    {
-        "Action": ActionType,
-        "Permission": PermissionType,
-    },
-)
 
 StartAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "StartAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
@@ -1569,19 +1274,21 @@
     "_OptionalStartImageBuilderRequestRequestTypeDef",
     {
         "AppstreamAgentVersion": str,
     },
     total=False,
 )
 
+
 class StartImageBuilderRequestRequestTypeDef(
     _RequiredStartImageBuilderRequestRequestTypeDef, _OptionalStartImageBuilderRequestRequestTypeDef
 ):
     pass
 
+
 StopAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "StopAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1611,31 +1318,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-AssociateAppBlockBuilderAppBlockResultTypeDef = TypedDict(
-    "AssociateAppBlockBuilderAppBlockResultTypeDef",
-    {
-        "AppBlockBuilderAppBlockAssociation": AppBlockBuilderAppBlockAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef = TypedDict(
-    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
-    {
-        "AppBlockBuilderAppBlockAssociations": List[AppBlockBuilderAppBlockAssociationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAppBlockBuilderTypeDef = TypedDict(
     "_RequiredAppBlockBuilderTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Platform": Literal["WINDOWS_SERVER_2019"],
         "InstanceType": str,
@@ -1649,79 +1339,226 @@
         "DisplayName": str,
         "Description": str,
         "EnableDefaultInternetAccess": bool,
         "IamRoleArn": str,
         "CreatedTime": datetime,
         "AppBlockBuilderErrors": List[ResourceErrorTypeDef],
         "StateChangeReason": AppBlockBuilderStateChangeReasonTypeDef,
-        "AccessEndpoints": List[AccessEndpointOutputTypeDef],
+        "AccessEndpoints": List[AccessEndpointTypeDef],
     },
     total=False,
 )
 
+
 class AppBlockBuilderTypeDef(_RequiredAppBlockBuilderTypeDef, _OptionalAppBlockBuilderTypeDef):
     pass
 
+
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Name": str,
         "DisplayName": str,
         "IconURL": str,
         "LaunchPath": str,
         "LaunchParameters": str,
         "Enabled": bool,
         "Metadata": Dict[str, str],
         "WorkingDirectory": str,
         "Description": str,
         "Arn": str,
         "AppBlockArn": str,
-        "IconS3Location": S3LocationOutputTypeDef,
+        "IconS3Location": S3LocationTypeDef,
         "Platforms": List[PlatformTypeType],
         "InstanceFamilies": List[str],
         "CreatedTime": datetime,
     },
     total=False,
 )
 
-_RequiredScriptDetailsOutputTypeDef = TypedDict(
-    "_RequiredScriptDetailsOutputTypeDef",
+_RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateApplicationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "IconS3Location": S3LocationTypeDef,
+        "LaunchPath": str,
+        "Platforms": Sequence[PlatformTypeType],
+        "InstanceFamilies": Sequence[str],
+        "AppBlockArn": str,
+    },
+)
+_OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateApplicationRequestRequestTypeDef",
     {
-        "ScriptS3Location": S3LocationOutputTypeDef,
+        "DisplayName": str,
+        "Description": str,
+        "WorkingDirectory": str,
+        "LaunchParameters": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateApplicationRequestRequestTypeDef(
+    _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredScriptDetailsTypeDef = TypedDict(
+    "_RequiredScriptDetailsTypeDef",
+    {
+        "ScriptS3Location": S3LocationTypeDef,
         "ExecutablePath": str,
         "TimeoutInSeconds": int,
     },
 )
-_OptionalScriptDetailsOutputTypeDef = TypedDict(
-    "_OptionalScriptDetailsOutputTypeDef",
+_OptionalScriptDetailsTypeDef = TypedDict(
+    "_OptionalScriptDetailsTypeDef",
     {
         "ExecutableParameters": str,
     },
     total=False,
 )
 
-class ScriptDetailsOutputTypeDef(
-    _RequiredScriptDetailsOutputTypeDef, _OptionalScriptDetailsOutputTypeDef
+
+class ScriptDetailsTypeDef(_RequiredScriptDetailsTypeDef, _OptionalScriptDetailsTypeDef):
+    pass
+
+
+_RequiredUpdateApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateApplicationRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateApplicationRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "Description": str,
+        "IconS3Location": S3LocationTypeDef,
+        "LaunchPath": str,
+        "WorkingDirectory": str,
+        "LaunchParameters": str,
+        "AppBlockArn": str,
+        "AttributesToDelete": Sequence[ApplicationAttributeType],
+    },
+    total=False,
+)
+
+
+class UpdateApplicationRequestRequestTypeDef(
+    _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
+
+AssociateAppBlockBuilderAppBlockResultTypeDef = TypedDict(
+    "AssociateAppBlockBuilderAppBlockResultTypeDef",
+    {
+        "AppBlockBuilderAppBlockAssociation": AppBlockBuilderAppBlockAssociationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AssociateApplicationFleetResultTypeDef = TypedDict(
     "AssociateApplicationFleetResultTypeDef",
     {
         "ApplicationFleetAssociation": ApplicationFleetAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CopyImageResponseTypeDef = TypedDict(
+    "CopyImageResponseTypeDef",
+    {
+        "DestinationImageName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppBlockBuilderStreamingURLResultTypeDef = TypedDict(
+    "CreateAppBlockBuilderStreamingURLResultTypeDef",
+    {
+        "StreamingURL": str,
+        "Expires": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImageBuilderStreamingURLResultTypeDef = TypedDict(
+    "CreateImageBuilderStreamingURLResultTypeDef",
+    {
+        "StreamingURL": str,
+        "Expires": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStreamingURLResultTypeDef = TypedDict(
+    "CreateStreamingURLResultTypeDef",
+    {
+        "StreamingURL": str,
+        "Expires": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUsageReportSubscriptionResultTypeDef = TypedDict(
+    "CreateUsageReportSubscriptionResultTypeDef",
+    {
+        "S3BucketName": str,
+        "Schedule": Literal["DAILY"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef = TypedDict(
+    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
+    {
+        "AppBlockBuilderAppBlockAssociations": List[AppBlockBuilderAppBlockAssociationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationFleetAssociationsResultTypeDef = TypedDict(
     "DescribeApplicationFleetAssociationsResultTypeDef",
     {
         "ApplicationFleetAssociations": List[ApplicationFleetAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssociatedFleetsResultTypeDef = TypedDict(
+    "ListAssociatedFleetsResultTypeDef",
+    {
+        "Names": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssociatedStacksResultTypeDef = TypedDict(
+    "ListAssociatedStacksResultTypeDef",
+    {
+        "Names": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchAssociateUserStackRequestRequestTypeDef = TypedDict(
     "BatchAssociateUserStackRequestRequestTypeDef",
     {
         "UserStackAssociations": Sequence[UserStackAssociationTypeDef],
@@ -1731,14 +1568,33 @@
 BatchDisassociateUserStackRequestRequestTypeDef = TypedDict(
     "BatchDisassociateUserStackRequestRequestTypeDef",
     {
         "UserStackAssociations": Sequence[UserStackAssociationTypeDef],
     },
 )
 
+DescribeUserStackAssociationsResultTypeDef = TypedDict(
+    "DescribeUserStackAssociationsResultTypeDef",
+    {
+        "UserStackAssociations": List[UserStackAssociationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UserStackAssociationErrorTypeDef = TypedDict(
+    "UserStackAssociationErrorTypeDef",
+    {
+        "UserStackAssociation": UserStackAssociationTypeDef,
+        "ErrorCode": UserStackAssociationErrorCodeType,
+        "ErrorMessage": str,
+    },
+    total=False,
+)
+
 _RequiredCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
         "Platform": Literal["WINDOWS_SERVER_2019"],
         "InstanceType": str,
         "VpcConfig": VpcConfigTypeDef,
@@ -1753,20 +1609,22 @@
         "EnableDefaultInternetAccess": bool,
         "IamRoleArn": str,
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
     },
     total=False,
 )
 
+
 class CreateAppBlockBuilderRequestRequestTypeDef(
     _RequiredCreateAppBlockBuilderRequestRequestTypeDef,
     _OptionalCreateAppBlockBuilderRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
@@ -1781,115 +1639,68 @@
         "IamRoleArn": str,
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
         "AttributesToDelete": Sequence[AppBlockBuilderAttributeType],
     },
     total=False,
 )
 
+
 class UpdateAppBlockBuilderRequestRequestTypeDef(
     _RequiredUpdateAppBlockBuilderRequestRequestTypeDef,
     _OptionalUpdateAppBlockBuilderRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateApplicationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "IconS3Location": S3LocationTypeDef,
-        "LaunchPath": str,
-        "Platforms": Sequence[PlatformTypeType],
-        "InstanceFamilies": Sequence[str],
-        "AppBlockArn": str,
-    },
-)
-_OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateApplicationRequestRequestTypeDef",
-    {
-        "DisplayName": str,
-        "Description": str,
-        "WorkingDirectory": str,
-        "LaunchParameters": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateApplicationRequestRequestTypeDef(
-    _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
-):
-    pass
 
-_RequiredScriptDetailsTypeDef = TypedDict(
-    "_RequiredScriptDetailsTypeDef",
+_RequiredCreateDirectoryConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDirectoryConfigRequestRequestTypeDef",
     {
-        "ScriptS3Location": S3LocationTypeDef,
-        "ExecutablePath": str,
-        "TimeoutInSeconds": int,
+        "DirectoryName": str,
+        "OrganizationalUnitDistinguishedNames": Sequence[str],
     },
 )
-_OptionalScriptDetailsTypeDef = TypedDict(
-    "_OptionalScriptDetailsTypeDef",
+_OptionalCreateDirectoryConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDirectoryConfigRequestRequestTypeDef",
     {
-        "ExecutableParameters": str,
+        "ServiceAccountCredentials": ServiceAccountCredentialsTypeDef,
+        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
     },
     total=False,
 )
 
-class ScriptDetailsTypeDef(_RequiredScriptDetailsTypeDef, _OptionalScriptDetailsTypeDef):
-    pass
-
-_RequiredUpdateApplicationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateApplicationRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateApplicationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateApplicationRequestRequestTypeDef",
-    {
-        "DisplayName": str,
-        "Description": str,
-        "IconS3Location": S3LocationTypeDef,
-        "LaunchPath": str,
-        "WorkingDirectory": str,
-        "LaunchParameters": str,
-        "AppBlockArn": str,
-        "AttributesToDelete": Sequence[ApplicationAttributeType],
-    },
-    total=False,
-)
 
-class UpdateApplicationRequestRequestTypeDef(
-    _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
+class CreateDirectoryConfigRequestRequestTypeDef(
+    _RequiredCreateDirectoryConfigRequestRequestTypeDef,
+    _OptionalCreateDirectoryConfigRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreateDirectoryConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDirectoryConfigRequestRequestTypeDef",
+
+_RequiredDirectoryConfigTypeDef = TypedDict(
+    "_RequiredDirectoryConfigTypeDef",
     {
         "DirectoryName": str,
-        "OrganizationalUnitDistinguishedNames": Sequence[str],
     },
 )
-_OptionalCreateDirectoryConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDirectoryConfigRequestRequestTypeDef",
+_OptionalDirectoryConfigTypeDef = TypedDict(
+    "_OptionalDirectoryConfigTypeDef",
     {
+        "OrganizationalUnitDistinguishedNames": List[str],
         "ServiceAccountCredentials": ServiceAccountCredentialsTypeDef,
+        "CreatedTime": datetime,
         "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
     },
     total=False,
 )
 
-class CreateDirectoryConfigRequestRequestTypeDef(
-    _RequiredCreateDirectoryConfigRequestRequestTypeDef,
-    _OptionalCreateDirectoryConfigRequestRequestTypeDef,
-):
+
+class DirectoryConfigTypeDef(_RequiredDirectoryConfigTypeDef, _OptionalDirectoryConfigTypeDef):
     pass
 
+
 _RequiredUpdateDirectoryConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDirectoryConfigRequestRequestTypeDef",
     {
         "DirectoryName": str,
     },
 )
 _OptionalUpdateDirectoryConfigRequestRequestTypeDef = TypedDict(
@@ -1898,20 +1709,22 @@
         "OrganizationalUnitDistinguishedNames": Sequence[str],
         "ServiceAccountCredentials": ServiceAccountCredentialsTypeDef,
         "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDirectoryConfigRequestRequestTypeDef(
     _RequiredUpdateDirectoryConfigRequestRequestTypeDef,
     _OptionalUpdateDirectoryConfigRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateEntitlementRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntitlementRequestRequestTypeDef",
     {
         "Name": str,
         "StackName": str,
         "AppVisibility": AppVisibilityType,
         "Attributes": Sequence[EntitlementAttributeTypeDef],
@@ -1921,19 +1734,45 @@
     "_OptionalCreateEntitlementRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateEntitlementRequestRequestTypeDef(
     _RequiredCreateEntitlementRequestRequestTypeDef, _OptionalCreateEntitlementRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredEntitlementTypeDef = TypedDict(
+    "_RequiredEntitlementTypeDef",
+    {
+        "Name": str,
+        "StackName": str,
+        "AppVisibility": AppVisibilityType,
+        "Attributes": List[EntitlementAttributeTypeDef],
+    },
+)
+_OptionalEntitlementTypeDef = TypedDict(
+    "_OptionalEntitlementTypeDef",
+    {
+        "Description": str,
+        "CreatedTime": datetime,
+        "LastModifiedTime": datetime,
+    },
+    total=False,
+)
+
+
+class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
+    pass
+
+
 _RequiredUpdateEntitlementRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEntitlementRequestRequestTypeDef",
     {
         "Name": str,
         "StackName": str,
     },
 )
@@ -1943,19 +1782,21 @@
         "Description": str,
         "AppVisibility": AppVisibilityType,
         "Attributes": Sequence[EntitlementAttributeTypeDef],
     },
     total=False,
 )
 
+
 class UpdateEntitlementRequestRequestTypeDef(
     _RequiredUpdateEntitlementRequestRequestTypeDef, _OptionalUpdateEntitlementRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFleetRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceType": str,
     },
 )
@@ -1981,19 +1822,21 @@
         "MaxConcurrentSessions": int,
         "UsbDeviceFilterStrings": Sequence[str],
         "SessionScriptS3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
+
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateImageBuilderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageBuilderRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceType": str,
     },
 )
@@ -2011,20 +1854,22 @@
         "AppstreamAgentVersion": str,
         "Tags": Mapping[str, str],
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
     },
     total=False,
 )
 
+
 class CreateImageBuilderRequestRequestTypeDef(
     _RequiredCreateImageBuilderRequestRequestTypeDef,
     _OptionalCreateImageBuilderRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateFleetRequestRequestTypeDef = TypedDict(
     "UpdateFleetRequestRequestTypeDef",
     {
         "ImageName": str,
         "ImageArn": str,
         "Name": str,
         "InstanceType": str,
@@ -2069,19 +1914,21 @@
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
         "EmbedHostDomains": Sequence[str],
         "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
     },
     total=False,
 )
 
+
 class CreateStackRequestRequestTypeDef(
     _RequiredCreateStackRequestRequestTypeDef, _OptionalCreateStackRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateStackRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStackRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateStackRequestRequestTypeDef = TypedDict(
@@ -2099,118 +1946,208 @@
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
         "EmbedHostDomains": Sequence[str],
         "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateStackRequestRequestTypeDef(
     _RequiredUpdateStackRequestRequestTypeDef, _OptionalUpdateStackRequestRequestTypeDef
 ):
     pass
 
-DescribeFleetsRequestFleetStartedWaitTypeDef = TypedDict(
-    "DescribeFleetsRequestFleetStartedWaitTypeDef",
+
+DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef = TypedDict(
+    "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
+    {
+        "DirectoryNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeFleetsRequestDescribeFleetsPaginateTypeDef = TypedDict(
+    "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
     {
         "Names": Sequence[str],
-        "NextToken": str,
-        "WaiterConfig": WaiterConfigTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeFleetsRequestFleetStoppedWaitTypeDef = TypedDict(
-    "DescribeFleetsRequestFleetStoppedWaitTypeDef",
+DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef = TypedDict(
+    "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
     {
         "Names": Sequence[str],
-        "NextToken": str,
-        "WaiterConfig": WaiterConfigTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeUserStackAssociationsResultTypeDef = TypedDict(
-    "DescribeUserStackAssociationsResultTypeDef",
+DescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
+    "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
-        "UserStackAssociations": List[UserStackAssociationOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Names": Sequence[str],
+        "Arns": Sequence[str],
+        "Type": VisibilityTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-UserStackAssociationErrorTypeDef = TypedDict(
-    "UserStackAssociationErrorTypeDef",
+_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     {
-        "UserStackAssociation": UserStackAssociationOutputTypeDef,
-        "ErrorCode": UserStackAssociationErrorCodeType,
-        "ErrorMessage": str,
+        "StackName": str,
+        "FleetName": str,
+    },
+)
+_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
+    {
+        "UserId": str,
+        "AuthenticationType": AuthenticationTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeUsersResultTypeDef = TypedDict(
-    "DescribeUsersResultTypeDef",
+
+class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
+    _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
+    _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
+):
+    pass
+
+
+DescribeStacksRequestDescribeStacksPaginateTypeDef = TypedDict(
+    "DescribeStacksRequestDescribeStacksPaginateTypeDef",
     {
-        "Users": List[UserTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Names": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredDirectoryConfigTypeDef = TypedDict(
-    "_RequiredDirectoryConfigTypeDef",
+DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef = TypedDict(
+    "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
     {
-        "DirectoryName": str,
+        "StackName": str,
+        "UserName": str,
+        "AuthenticationType": AuthenticationTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalDirectoryConfigTypeDef = TypedDict(
-    "_OptionalDirectoryConfigTypeDef",
+
+_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef",
     {
-        "OrganizationalUnitDistinguishedNames": List[str],
-        "ServiceAccountCredentials": ServiceAccountCredentialsOutputTypeDef,
-        "CreatedTime": datetime,
-        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesOutputTypeDef,
+        "AuthenticationType": AuthenticationTypeType,
+    },
+)
+_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class DirectoryConfigTypeDef(_RequiredDirectoryConfigTypeDef, _OptionalDirectoryConfigTypeDef):
+
+class DescribeUsersRequestDescribeUsersPaginateTypeDef(
+    _RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef,
+    _OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef,
+):
     pass
 
-ListEntitledApplicationsResultTypeDef = TypedDict(
-    "ListEntitledApplicationsResultTypeDef",
+
+_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
     {
-        "EntitledApplications": List[EntitledApplicationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StackName": str,
+    },
+)
+_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredEntitlementTypeDef = TypedDict(
-    "_RequiredEntitlementTypeDef",
+
+class ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef(
+    _RequiredListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
+    _OptionalListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     {
-        "Name": str,
-        "StackName": str,
-        "AppVisibility": AppVisibilityType,
-        "Attributes": List[EntitlementAttributeOutputTypeDef],
+        "FleetName": str,
     },
 )
-_OptionalEntitlementTypeDef = TypedDict(
-    "_OptionalEntitlementTypeDef",
+_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     {
-        "Description": str,
-        "CreatedTime": datetime,
-        "LastModifiedTime": datetime,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
+
+class ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef(
+    _RequiredListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
+    _OptionalListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
+):
     pass
 
+
+DescribeFleetsRequestFleetStartedWaitTypeDef = TypedDict(
+    "DescribeFleetsRequestFleetStartedWaitTypeDef",
+    {
+        "Names": Sequence[str],
+        "NextToken": str,
+        "WaiterConfig": WaiterConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeFleetsRequestFleetStoppedWaitTypeDef = TypedDict(
+    "DescribeFleetsRequestFleetStoppedWaitTypeDef",
+    {
+        "Names": Sequence[str],
+        "NextToken": str,
+        "WaiterConfig": WaiterConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeUsersResultTypeDef = TypedDict(
+    "DescribeUsersResultTypeDef",
+    {
+        "Users": List[UserTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEntitledApplicationsResultTypeDef = TypedDict(
+    "ListEntitledApplicationsResultTypeDef",
+    {
+        "EntitledApplications": List[EntitledApplicationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredFleetTypeDef = TypedDict(
     "_RequiredFleetTypeDef",
     {
         "Arn": str,
         "Name": str,
         "InstanceType": str,
         "ComputeCapacityStatus": ComputeCapacityStatusTypeDef,
@@ -2227,29 +2164,31 @@
         "FleetType": FleetTypeType,
         "MaxUserDurationInSeconds": int,
         "DisconnectTimeoutInSeconds": int,
         "VpcConfig": VpcConfigOutputTypeDef,
         "CreatedTime": datetime,
         "FleetErrors": List[FleetErrorTypeDef],
         "EnableDefaultInternetAccess": bool,
-        "DomainJoinInfo": DomainJoinInfoOutputTypeDef,
+        "DomainJoinInfo": DomainJoinInfoTypeDef,
         "IdleDisconnectTimeoutInSeconds": int,
         "IamRoleArn": str,
         "StreamView": StreamViewType,
         "Platform": PlatformTypeType,
         "MaxConcurrentSessions": int,
         "UsbDeviceFilterStrings": List[str],
-        "SessionScriptS3Location": S3LocationOutputTypeDef,
+        "SessionScriptS3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
+
 class FleetTypeDef(_RequiredFleetTypeDef, _OptionalFleetTypeDef):
     pass
 
+
 _RequiredImageBuilderTypeDef = TypedDict(
     "_RequiredImageBuilderTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalImageBuilderTypeDef = TypedDict(
@@ -2263,26 +2202,28 @@
         "InstanceType": str,
         "Platform": PlatformTypeType,
         "IamRoleArn": str,
         "State": ImageBuilderStateType,
         "StateChangeReason": ImageBuilderStateChangeReasonTypeDef,
         "CreatedTime": datetime,
         "EnableDefaultInternetAccess": bool,
-        "DomainJoinInfo": DomainJoinInfoOutputTypeDef,
+        "DomainJoinInfo": DomainJoinInfoTypeDef,
         "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
         "ImageBuilderErrors": List[ResourceErrorTypeDef],
         "AppstreamAgentVersion": str,
-        "AccessEndpoints": List[AccessEndpointOutputTypeDef],
+        "AccessEndpoints": List[AccessEndpointTypeDef],
     },
     total=False,
 )
 
+
 class ImageBuilderTypeDef(_RequiredImageBuilderTypeDef, _OptionalImageBuilderTypeDef):
     pass
 
+
 _RequiredSessionTypeDef = TypedDict(
     "_RequiredSessionTypeDef",
     {
         "Id": str,
         "UserId": str,
         "StackName": str,
         "FleetName": str,
@@ -2297,22 +2238,24 @@
         "MaxExpirationTime": datetime,
         "AuthenticationType": AuthenticationTypeType,
         "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
     pass
 
+
 SharedImagePermissionsTypeDef = TypedDict(
     "SharedImagePermissionsTypeDef",
     {
         "sharedAccountId": str,
-        "imagePermissions": ImagePermissionsOutputTypeDef,
+        "imagePermissions": ImagePermissionsTypeDef,
     },
 )
 
 UpdateImagePermissionsRequestRequestTypeDef = TypedDict(
     "UpdateImagePermissionsRequestRequestTypeDef",
     {
         "Name": str,
@@ -2345,81 +2288,83 @@
         "Description": str,
         "DisplayName": str,
         "CreatedTime": datetime,
         "StorageConnectors": List[StorageConnectorOutputTypeDef],
         "RedirectURL": str,
         "FeedbackURL": str,
         "StackErrors": List[StackErrorTypeDef],
-        "UserSettings": List[UserSettingOutputTypeDef],
+        "UserSettings": List[UserSettingTypeDef],
         "ApplicationSettings": ApplicationSettingsResponseTypeDef,
-        "AccessEndpoints": List[AccessEndpointOutputTypeDef],
+        "AccessEndpoints": List[AccessEndpointTypeDef],
         "EmbedHostDomains": List[str],
-        "StreamingExperienceSettings": StreamingExperienceSettingsOutputTypeDef,
+        "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
     },
     total=False,
 )
 
+
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
 
+
 CreateAppBlockBuilderResultTypeDef = TypedDict(
     "CreateAppBlockBuilderResultTypeDef",
     {
         "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppBlockBuildersResultTypeDef = TypedDict(
     "DescribeAppBlockBuildersResultTypeDef",
     {
         "AppBlockBuilders": List[AppBlockBuilderTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartAppBlockBuilderResultTypeDef = TypedDict(
     "StartAppBlockBuilderResultTypeDef",
     {
         "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopAppBlockBuilderResultTypeDef = TypedDict(
     "StopAppBlockBuilderResultTypeDef",
     {
         "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppBlockBuilderResultTypeDef = TypedDict(
     "UpdateAppBlockBuilderResultTypeDef",
     {
         "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateApplicationResultTypeDef = TypedDict(
     "CreateApplicationResultTypeDef",
     {
         "Application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationsResultTypeDef = TypedDict(
     "DescribeApplicationsResultTypeDef",
     {
         "Applications": List[ApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImageTypeDef = TypedDict(
     "_RequiredImageTypeDef",
     {
         "Name": str,
@@ -2438,28 +2383,30 @@
         "Platform": PlatformTypeType,
         "Description": str,
         "StateChangeReason": ImageStateChangeReasonTypeDef,
         "Applications": List[ApplicationTypeDef],
         "CreatedTime": datetime,
         "PublicBaseImageReleasedDate": datetime,
         "AppstreamAgentVersion": str,
-        "ImagePermissions": ImagePermissionsOutputTypeDef,
+        "ImagePermissions": ImagePermissionsTypeDef,
         "ImageErrors": List[ResourceErrorTypeDef],
     },
     total=False,
 )
 
+
 class ImageTypeDef(_RequiredImageTypeDef, _OptionalImageTypeDef):
     pass
 
+
 UpdateApplicationResultTypeDef = TypedDict(
     "UpdateApplicationResultTypeDef",
     {
         "Application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAppBlockTypeDef = TypedDict(
     "_RequiredAppBlockTypeDef",
     {
         "Name": str,
@@ -2467,28 +2414,30 @@
     },
 )
 _OptionalAppBlockTypeDef = TypedDict(
     "_OptionalAppBlockTypeDef",
     {
         "Description": str,
         "DisplayName": str,
-        "SourceS3Location": S3LocationOutputTypeDef,
-        "SetupScriptDetails": ScriptDetailsOutputTypeDef,
+        "SourceS3Location": S3LocationTypeDef,
+        "SetupScriptDetails": ScriptDetailsTypeDef,
         "CreatedTime": datetime,
-        "PostSetupScriptDetails": ScriptDetailsOutputTypeDef,
+        "PostSetupScriptDetails": ScriptDetailsTypeDef,
         "PackagingType": PackagingTypeType,
         "State": AppBlockStateType,
         "AppBlockErrors": List[ErrorDetailsTypeDef],
     },
     total=False,
 )
 
+
 class AppBlockTypeDef(_RequiredAppBlockTypeDef, _OptionalAppBlockTypeDef):
     pass
 
+
 _RequiredCreateAppBlockRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppBlockRequestRequestTypeDef",
     {
         "Name": str,
         "SourceS3Location": S3LocationTypeDef,
     },
 )
@@ -2501,239 +2450,241 @@
         "Tags": Mapping[str, str],
         "PostSetupScriptDetails": ScriptDetailsTypeDef,
         "PackagingType": PackagingTypeType,
     },
     total=False,
 )
 
+
 class CreateAppBlockRequestRequestTypeDef(
     _RequiredCreateAppBlockRequestRequestTypeDef, _OptionalCreateAppBlockRequestRequestTypeDef
 ):
     pass
 
+
 BatchAssociateUserStackResultTypeDef = TypedDict(
     "BatchAssociateUserStackResultTypeDef",
     {
         "errors": List[UserStackAssociationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateUserStackResultTypeDef = TypedDict(
     "BatchDisassociateUserStackResultTypeDef",
     {
         "errors": List[UserStackAssociationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDirectoryConfigResultTypeDef = TypedDict(
     "CreateDirectoryConfigResultTypeDef",
     {
         "DirectoryConfig": DirectoryConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDirectoryConfigsResultTypeDef = TypedDict(
     "DescribeDirectoryConfigsResultTypeDef",
     {
         "DirectoryConfigs": List[DirectoryConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDirectoryConfigResultTypeDef = TypedDict(
     "UpdateDirectoryConfigResultTypeDef",
     {
         "DirectoryConfig": DirectoryConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEntitlementResultTypeDef = TypedDict(
     "CreateEntitlementResultTypeDef",
     {
         "Entitlement": EntitlementTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEntitlementsResultTypeDef = TypedDict(
     "DescribeEntitlementsResultTypeDef",
     {
         "Entitlements": List[EntitlementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEntitlementResultTypeDef = TypedDict(
     "UpdateEntitlementResultTypeDef",
     {
         "Entitlement": EntitlementTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFleetResultTypeDef = TypedDict(
     "CreateFleetResultTypeDef",
     {
         "Fleet": FleetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFleetsResultTypeDef = TypedDict(
     "DescribeFleetsResultTypeDef",
     {
         "Fleets": List[FleetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFleetResultTypeDef = TypedDict(
     "UpdateFleetResultTypeDef",
     {
         "Fleet": FleetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateImageBuilderResultTypeDef = TypedDict(
     "CreateImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteImageBuilderResultTypeDef = TypedDict(
     "DeleteImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImageBuildersResultTypeDef = TypedDict(
     "DescribeImageBuildersResultTypeDef",
     {
         "ImageBuilders": List[ImageBuilderTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartImageBuilderResultTypeDef = TypedDict(
     "StartImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopImageBuilderResultTypeDef = TypedDict(
     "StopImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSessionsResultTypeDef = TypedDict(
     "DescribeSessionsResultTypeDef",
     {
         "Sessions": List[SessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImagePermissionsResultTypeDef = TypedDict(
     "DescribeImagePermissionsResultTypeDef",
     {
         "Name": str,
         "SharedImagePermissionsList": List[SharedImagePermissionsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUsageReportSubscriptionsResultTypeDef = TypedDict(
     "DescribeUsageReportSubscriptionsResultTypeDef",
     {
         "UsageReportSubscriptions": List[UsageReportSubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStackResultTypeDef = TypedDict(
     "CreateStackResultTypeDef",
     {
         "Stack": StackTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStacksResultTypeDef = TypedDict(
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStackResultTypeDef = TypedDict(
     "UpdateStackResultTypeDef",
     {
         "Stack": StackTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateUpdatedImageResultTypeDef = TypedDict(
     "CreateUpdatedImageResultTypeDef",
     {
         "image": ImageTypeDef,
         "canUpdateImage": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteImageResultTypeDef = TypedDict(
     "DeleteImageResultTypeDef",
     {
         "Image": ImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImagesResultTypeDef = TypedDict(
     "DescribeImagesResultTypeDef",
     {
         "Images": List[ImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAppBlockResultTypeDef = TypedDict(
     "CreateAppBlockResultTypeDef",
     {
         "AppBlock": AppBlockTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppBlocksResultTypeDef = TypedDict(
     "DescribeAppBlocksResultTypeDef",
     {
         "AppBlocks": List[AppBlockTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/waiter.py` & `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/waiter.pyi` & `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/PKG-INFO` & `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appstream
-Version: 1.28.12
-Summary: Type annotations for boto3.AppStream 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AppStream 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appstream)](https://pepy.tech/project/mypy-boto3-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppStream 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[boto3.AppStream 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
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
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -415,52 +415,45 @@
 ### Typed dictionaries
 
 `mypy_boto3_appstream.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appstream.type_defs import (
-    AccessEndpointOutputTypeDef,
     AccessEndpointTypeDef,
     AppBlockBuilderAppBlockAssociationTypeDef,
     AppBlockBuilderStateChangeReasonTypeDef,
     ResourceErrorTypeDef,
     VpcConfigOutputTypeDef,
     ErrorDetailsTypeDef,
-    S3LocationOutputTypeDef,
+    S3LocationTypeDef,
     ApplicationFleetAssociationTypeDef,
     ApplicationSettingsResponseTypeDef,
     ApplicationSettingsTypeDef,
     AssociateAppBlockBuilderAppBlockRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AssociateApplicationFleetRequestRequestTypeDef,
     AssociateApplicationToEntitlementRequestRequestTypeDef,
     AssociateFleetRequestRequestTypeDef,
     UserStackAssociationTypeDef,
-    CertificateBasedAuthPropertiesOutputTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityStatusTypeDef,
     ComputeCapacityTypeDef,
     CopyImageRequestRequestTypeDef,
-    CopyImageResponseTypeDef,
     VpcConfigTypeDef,
     CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
-    CreateAppBlockBuilderStreamingURLResultTypeDef,
-    S3LocationTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
-    CreateImageBuilderStreamingURLResultTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UserSettingTypeDef,
     CreateStreamingURLRequestRequestTypeDef,
-    CreateStreamingURLResultTypeDef,
     CreateUpdatedImageRequestRequestTypeDef,
-    CreateUsageReportSubscriptionResultTypeDef,
     CreateUserRequestRequestTypeDef,
     DeleteAppBlockBuilderRequestRequestTypeDef,
     DeleteAppBlockRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteDirectoryConfigRequestRequestTypeDef,
     DeleteEntitlementRequestRequestTypeDef,
     DeleteFleetRequestRequestTypeDef,
@@ -470,108 +463,104 @@
     DeleteStackRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef,
     DescribeAppBlockBuildersRequestRequestTypeDef,
     DescribeAppBlocksRequestRequestTypeDef,
     DescribeApplicationFleetAssociationsRequestRequestTypeDef,
     DescribeApplicationsRequestRequestTypeDef,
-    DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDirectoryConfigsRequestRequestTypeDef,
     DescribeEntitlementsRequestRequestTypeDef,
-    DescribeFleetsRequestDescribeFleetsPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeFleetsRequestRequestTypeDef,
-    DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef,
     DescribeImageBuildersRequestRequestTypeDef,
     DescribeImagePermissionsRequestRequestTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
-    DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeSessionsRequestRequestTypeDef,
-    DescribeStacksRequestDescribeStacksPaginateTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeUsageReportSubscriptionsRequestRequestTypeDef,
-    DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
     DescribeUserStackAssociationsRequestRequestTypeDef,
-    UserStackAssociationOutputTypeDef,
-    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UserTypeDef,
-    ServiceAccountCredentialsOutputTypeDef,
     DisableUserRequestRequestTypeDef,
     DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     DisassociateApplicationFleetRequestRequestTypeDef,
     DisassociateApplicationFromEntitlementRequestRequestTypeDef,
     DisassociateFleetRequestRequestTypeDef,
-    DomainJoinInfoOutputTypeDef,
     EnableUserRequestRequestTypeDef,
     EntitledApplicationTypeDef,
-    EntitlementAttributeOutputTypeDef,
     ExpireSessionRequestRequestTypeDef,
     FleetErrorTypeDef,
     ImageBuilderStateChangeReasonTypeDef,
     NetworkAccessConfigurationTypeDef,
-    ImagePermissionsOutputTypeDef,
     ImagePermissionsTypeDef,
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
-    ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
-    ListAssociatedFleetsResultTypeDef,
-    ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
     ListAssociatedStacksRequestRequestTypeDef,
-    ListAssociatedStacksResultTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StackErrorTypeDef,
     StorageConnectorOutputTypeDef,
-    StreamingExperienceSettingsOutputTypeDef,
-    UserSettingOutputTypeDef,
     StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
     StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AssociateAppBlockBuilderAppBlockResultTypeDef,
-    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
     AppBlockBuilderTypeDef,
     ApplicationTypeDef,
-    ScriptDetailsOutputTypeDef,
+    CreateApplicationRequestRequestTypeDef,
+    ScriptDetailsTypeDef,
+    UpdateApplicationRequestRequestTypeDef,
+    AssociateAppBlockBuilderAppBlockResultTypeDef,
     AssociateApplicationFleetResultTypeDef,
+    CopyImageResponseTypeDef,
+    CreateAppBlockBuilderStreamingURLResultTypeDef,
+    CreateImageBuilderStreamingURLResultTypeDef,
+    CreateStreamingURLResultTypeDef,
+    CreateUsageReportSubscriptionResultTypeDef,
+    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
+    ListAssociatedFleetsResultTypeDef,
+    ListAssociatedStacksResultTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchAssociateUserStackRequestRequestTypeDef,
     BatchDisassociateUserStackRequestRequestTypeDef,
+    DescribeUserStackAssociationsResultTypeDef,
+    UserStackAssociationErrorTypeDef,
     CreateAppBlockBuilderRequestRequestTypeDef,
     UpdateAppBlockBuilderRequestRequestTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    ScriptDetailsTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
     CreateDirectoryConfigRequestRequestTypeDef,
+    DirectoryConfigTypeDef,
     UpdateDirectoryConfigRequestRequestTypeDef,
     CreateEntitlementRequestRequestTypeDef,
+    EntitlementTypeDef,
     UpdateEntitlementRequestRequestTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateImageBuilderRequestRequestTypeDef,
     UpdateFleetRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     UpdateStackRequestRequestTypeDef,
+    DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef,
+    DescribeFleetsRequestDescribeFleetsPaginateTypeDef,
+    DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef,
+    DescribeImagesRequestDescribeImagesPaginateTypeDef,
+    DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
+    DescribeStacksRequestDescribeStacksPaginateTypeDef,
+    DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
+    ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
+    ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
     DescribeFleetsRequestFleetStartedWaitTypeDef,
     DescribeFleetsRequestFleetStoppedWaitTypeDef,
-    DescribeUserStackAssociationsResultTypeDef,
-    UserStackAssociationErrorTypeDef,
     DescribeUsersResultTypeDef,
-    DirectoryConfigTypeDef,
     ListEntitledApplicationsResultTypeDef,
-    EntitlementTypeDef,
     FleetTypeDef,
     ImageBuilderTypeDef,
     SessionTypeDef,
     SharedImagePermissionsTypeDef,
     UpdateImagePermissionsRequestRequestTypeDef,
     UsageReportSubscriptionTypeDef,
     StackTypeDef,
@@ -612,15 +601,15 @@
     DeleteImageResultTypeDef,
     DescribeImagesResultTypeDef,
     CreateAppBlockResultTypeDef,
     DescribeAppBlocksResultTypeDef,
 )
 
 
-def get_structure() -> AccessEndpointOutputTypeDef:
+def get_structure() -> AccessEndpointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/SOURCES.txt` & `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.12/setup.py` & `mypy-boto3-appstream-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appstream",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_appstream"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppStream 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.AppStream 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

