# Comparing `tmp/mypy-boto3-license-manager-1.28.12.tar.gz` & `tmp/mypy-boto3-license-manager-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-license-manager-1.28.12.tar", last modified: Thu Jul 27 05:34:56 2023, max compression
+gzip compressed data, was "mypy-boto3-license-manager-1.28.15.tar", last modified: Fri Jul 28 20:43:08 2023, max compression
```

## Comparing `mypy-boto3-license-manager-1.28.12.tar` & `mypy-boto3-license-manager-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.392458 mypy-boto3-license-manager-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20817 2023-07-27 05:34:56.392458 mypy-boto3-license-manager-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19299 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.392458 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40707 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40645 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60234 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60153 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.392458 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20817 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:56.392458 mypy-boto3-license-manager-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-27 05:25:18.000000 mypy-boto3-license-manager-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.965387 mypy-boto3-license-manager-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:05.000000 mypy-boto3-license-manager-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20362 2023-07-28 20:43:08.965387 mypy-boto3-license-manager-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18844 2023-07-28 20:30:05.000000 mypy-boto3-license-manager-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.957387 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-28 20:30:05.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-28 20:30:05.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-28 20:30:06.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40707 2023-07-28 20:30:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40645 2023-07-28 20:30:06.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-28 20:30:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-07-28 20:30:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-28 20:30:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-28 20:30:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:06.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56131 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56058 2023-07-28 20:30:09.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:05.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.965387 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20362 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:08.965387 mypy-boto3-license-manager-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-28 20:30:05.000000 mypy-boto3-license-manager-1.28.15/setup.py
```

### Comparing `mypy-boto3-license-manager-1.28.12/LICENSE` & `mypy-boto3-license-manager-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.12/PKG-INFO` & `mypy-boto3-license-manager-1.28.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-license-manager
-Version: 1.28.12
-Summary: Type annotations for boto3.LicenseManager 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 license-manager type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-license-manager"></a>
 
 # mypy-boto3-license-manager
 
 [![PyPI - mypy-boto3-license-manager](https://img.shields.io/pypi/v/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager)](https://pepy.tech/project/mypy-boto3-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManager 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[boto3.LicenseManager 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [mypy-boto3-license-manager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,151 +332,138 @@
 
 `mypy_boto3_license_manager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_license_manager.type_defs import (
     AcceptGrantRequestRequestTypeDef,
-    AcceptGrantResponseTypeDef,
+    ResponseMetadataTypeDef,
     AutomatedDiscoveryInformationTypeDef,
-    BorrowConfigurationOutputTypeDef,
     BorrowConfigurationTypeDef,
     CheckInLicenseRequestRequestTypeDef,
     EntitlementDataTypeDef,
     MetadataTypeDef,
-    EntitlementDataOutputTypeDef,
-    MetadataOutputTypeDef,
     ConsumedLicenseSummaryTypeDef,
-    ProvisionalConfigurationOutputTypeDef,
     ProvisionalConfigurationTypeDef,
     CreateGrantRequestRequestTypeDef,
-    CreateGrantResponseTypeDef,
     OptionsTypeDef,
-    CreateGrantVersionResponseTypeDef,
     TagTypeDef,
-    CreateLicenseConfigurationResponseTypeDef,
     LicenseConversionContextTypeDef,
-    CreateLicenseConversionTaskForResourceResponseTypeDef,
     ReportContextTypeDef,
     ReportFrequencyTypeDef,
-    CreateLicenseManagerReportGeneratorResponseTypeDef,
     DatetimeRangeTypeDef,
     EntitlementTypeDef,
     IssuerTypeDef,
-    CreateLicenseResponseTypeDef,
-    CreateLicenseVersionResponseTypeDef,
     CreateTokenRequestRequestTypeDef,
-    CreateTokenResponseTypeDef,
-    DatetimeRangeOutputTypeDef,
     DeleteGrantRequestRequestTypeDef,
-    DeleteGrantResponseTypeDef,
     DeleteLicenseConfigurationRequestRequestTypeDef,
     DeleteLicenseManagerReportGeneratorRequestRequestTypeDef,
     DeleteLicenseRequestRequestTypeDef,
-    DeleteLicenseResponseTypeDef,
     DeleteTokenRequestRequestTypeDef,
-    EntitlementOutputTypeDef,
     EntitlementUsageTypeDef,
     ExtendLicenseConsumptionRequestRequestTypeDef,
-    ExtendLicenseConsumptionResponseTypeDef,
     FilterTypeDef,
     GetAccessTokenRequestRequestTypeDef,
-    GetAccessTokenResponseTypeDef,
     GetGrantRequestRequestTypeDef,
     GetLicenseConfigurationRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
-    TagOutputTypeDef,
     GetLicenseConversionTaskRequestRequestTypeDef,
-    LicenseConversionContextOutputTypeDef,
     GetLicenseManagerReportGeneratorRequestRequestTypeDef,
     GetLicenseRequestRequestTypeDef,
     GetLicenseUsageRequestRequestTypeDef,
-    OrganizationConfigurationOutputTypeDef,
-    OptionsOutputTypeDef,
+    OrganizationConfigurationTypeDef,
     IssuerDetailsTypeDef,
     ReceivedMetadataTypeDef,
     InventoryFilterTypeDef,
     LicenseConfigurationAssociationTypeDef,
     LicenseConfigurationUsageTypeDef,
-    LicenseSpecificationOutputTypeDef,
     LicenseSpecificationTypeDef,
-    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
-    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     ListLicenseSpecificationsForResourceRequestRequestTypeDef,
     ListLicenseVersionsRequestRequestTypeDef,
     ResourceInventoryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TokenDataTypeDef,
-    OrganizationConfigurationTypeDef,
-    PaginatorConfigTypeDef,
     ProductInformationFilterOutputTypeDef,
     ProductInformationFilterTypeDef,
     RejectGrantRequestRequestTypeDef,
-    RejectGrantResponseTypeDef,
     ReportContextOutputTypeDef,
-    ReportFrequencyOutputTypeDef,
     S3LocationTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AcceptGrantResponseTypeDef,
+    CreateGrantResponseTypeDef,
+    CreateGrantVersionResponseTypeDef,
+    CreateLicenseConfigurationResponseTypeDef,
+    CreateLicenseConversionTaskForResourceResponseTypeDef,
+    CreateLicenseManagerReportGeneratorResponseTypeDef,
+    CreateLicenseResponseTypeDef,
+    CreateLicenseVersionResponseTypeDef,
+    CreateTokenResponseTypeDef,
+    DeleteGrantResponseTypeDef,
+    DeleteLicenseResponseTypeDef,
+    ExtendLicenseConsumptionResponseTypeDef,
+    GetAccessTokenResponseTypeDef,
+    RejectGrantResponseTypeDef,
     CheckoutLicenseRequestRequestTypeDef,
-    CheckoutBorrowLicenseRequestRequestTypeDef,
     CheckoutLicenseResponseTypeDef,
+    CheckoutBorrowLicenseRequestRequestTypeDef,
     CheckoutBorrowLicenseResponseTypeDef,
     LicenseOperationFailureTypeDef,
-    ConsumptionConfigurationOutputTypeDef,
     ConsumptionConfigurationTypeDef,
     CreateGrantVersionRequestRequestTypeDef,
+    GrantTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateLicenseConversionTaskForResourceRequestRequestTypeDef,
+    GetLicenseConversionTaskResponseTypeDef,
+    LicenseConversionTaskTypeDef,
     CreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     UpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     LicenseUsageTypeDef,
     ListDistributedGrantsRequestRequestTypeDef,
-    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
     ListLicenseConfigurationsRequestRequestTypeDef,
     ListLicenseConversionTasksRequestRequestTypeDef,
     ListLicenseManagerReportGeneratorsRequestRequestTypeDef,
     ListLicensesRequestRequestTypeDef,
     ListReceivedGrantsForOrganizationRequestRequestTypeDef,
     ListReceivedGrantsRequestRequestTypeDef,
     ListReceivedLicensesForOrganizationRequestRequestTypeDef,
     ListReceivedLicensesRequestRequestTypeDef,
     ListTokensRequestRequestTypeDef,
-    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListUsageForLicenseConfigurationRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GetLicenseConversionTaskResponseTypeDef,
-    LicenseConversionTaskTypeDef,
     GetServiceSettingsResponseTypeDef,
-    GrantTypeDef,
-    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
+    UpdateServiceSettingsRequestRequestTypeDef,
     ListResourceInventoryRequestRequestTypeDef,
     ListAssociationsForLicenseConfigurationResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     ListLicenseSpecificationsForResourceResponseTypeDef,
     UpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
+    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
+    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
+    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTokensResponseTypeDef,
-    UpdateServiceSettingsRequestRequestTypeDef,
     ProductInformationOutputTypeDef,
     ProductInformationTypeDef,
     ReportGeneratorTypeDef,
     ListFailuresForLicenseConfigurationOperationsResponseTypeDef,
-    GrantedLicenseTypeDef,
-    LicenseTypeDef,
     CreateLicenseRequestRequestTypeDef,
     CreateLicenseVersionRequestRequestTypeDef,
-    GetLicenseUsageResponseTypeDef,
-    ListLicenseConversionTasksResponseTypeDef,
+    GrantedLicenseTypeDef,
+    LicenseTypeDef,
     GetGrantResponseTypeDef,
     ListDistributedGrantsResponseTypeDef,
     ListReceivedGrantsForOrganizationResponseTypeDef,
     ListReceivedGrantsResponseTypeDef,
+    ListLicenseConversionTasksResponseTypeDef,
+    GetLicenseUsageResponseTypeDef,
     GetLicenseConfigurationResponseTypeDef,
     LicenseConfigurationTypeDef,
     CreateLicenseConfigurationRequestRequestTypeDef,
     UpdateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseManagerReportGeneratorResponseTypeDef,
     ListLicenseManagerReportGeneratorsResponseTypeDef,
     ListReceivedLicensesForOrganizationResponseTypeDef,
```

### Comparing `mypy-boto3-license-manager-1.28.12/README.md` & `mypy-boto3-license-manager-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-license-manager
+Version: 1.28.15
+Summary: Type annotations for boto3.LicenseManager 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 license-manager type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-license-manager"></a>
 
 # mypy-boto3-license-manager
 
 [![PyPI - mypy-boto3-license-manager](https://img.shields.io/pypi/v/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager)](https://pepy.tech/project/mypy-boto3-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManager 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[boto3.LicenseManager 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [mypy-boto3-license-manager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,151 +364,138 @@
 
 `mypy_boto3_license_manager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_license_manager.type_defs import (
     AcceptGrantRequestRequestTypeDef,
-    AcceptGrantResponseTypeDef,
+    ResponseMetadataTypeDef,
     AutomatedDiscoveryInformationTypeDef,
-    BorrowConfigurationOutputTypeDef,
     BorrowConfigurationTypeDef,
     CheckInLicenseRequestRequestTypeDef,
     EntitlementDataTypeDef,
     MetadataTypeDef,
-    EntitlementDataOutputTypeDef,
-    MetadataOutputTypeDef,
     ConsumedLicenseSummaryTypeDef,
-    ProvisionalConfigurationOutputTypeDef,
     ProvisionalConfigurationTypeDef,
     CreateGrantRequestRequestTypeDef,
-    CreateGrantResponseTypeDef,
     OptionsTypeDef,
-    CreateGrantVersionResponseTypeDef,
     TagTypeDef,
-    CreateLicenseConfigurationResponseTypeDef,
     LicenseConversionContextTypeDef,
-    CreateLicenseConversionTaskForResourceResponseTypeDef,
     ReportContextTypeDef,
     ReportFrequencyTypeDef,
-    CreateLicenseManagerReportGeneratorResponseTypeDef,
     DatetimeRangeTypeDef,
     EntitlementTypeDef,
     IssuerTypeDef,
-    CreateLicenseResponseTypeDef,
-    CreateLicenseVersionResponseTypeDef,
     CreateTokenRequestRequestTypeDef,
-    CreateTokenResponseTypeDef,
-    DatetimeRangeOutputTypeDef,
     DeleteGrantRequestRequestTypeDef,
-    DeleteGrantResponseTypeDef,
     DeleteLicenseConfigurationRequestRequestTypeDef,
     DeleteLicenseManagerReportGeneratorRequestRequestTypeDef,
     DeleteLicenseRequestRequestTypeDef,
-    DeleteLicenseResponseTypeDef,
     DeleteTokenRequestRequestTypeDef,
-    EntitlementOutputTypeDef,
     EntitlementUsageTypeDef,
     ExtendLicenseConsumptionRequestRequestTypeDef,
-    ExtendLicenseConsumptionResponseTypeDef,
     FilterTypeDef,
     GetAccessTokenRequestRequestTypeDef,
-    GetAccessTokenResponseTypeDef,
     GetGrantRequestRequestTypeDef,
     GetLicenseConfigurationRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
-    TagOutputTypeDef,
     GetLicenseConversionTaskRequestRequestTypeDef,
-    LicenseConversionContextOutputTypeDef,
     GetLicenseManagerReportGeneratorRequestRequestTypeDef,
     GetLicenseRequestRequestTypeDef,
     GetLicenseUsageRequestRequestTypeDef,
-    OrganizationConfigurationOutputTypeDef,
-    OptionsOutputTypeDef,
+    OrganizationConfigurationTypeDef,
     IssuerDetailsTypeDef,
     ReceivedMetadataTypeDef,
     InventoryFilterTypeDef,
     LicenseConfigurationAssociationTypeDef,
     LicenseConfigurationUsageTypeDef,
-    LicenseSpecificationOutputTypeDef,
     LicenseSpecificationTypeDef,
-    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
-    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     ListLicenseSpecificationsForResourceRequestRequestTypeDef,
     ListLicenseVersionsRequestRequestTypeDef,
     ResourceInventoryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TokenDataTypeDef,
-    OrganizationConfigurationTypeDef,
-    PaginatorConfigTypeDef,
     ProductInformationFilterOutputTypeDef,
     ProductInformationFilterTypeDef,
     RejectGrantRequestRequestTypeDef,
-    RejectGrantResponseTypeDef,
     ReportContextOutputTypeDef,
-    ReportFrequencyOutputTypeDef,
     S3LocationTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AcceptGrantResponseTypeDef,
+    CreateGrantResponseTypeDef,
+    CreateGrantVersionResponseTypeDef,
+    CreateLicenseConfigurationResponseTypeDef,
+    CreateLicenseConversionTaskForResourceResponseTypeDef,
+    CreateLicenseManagerReportGeneratorResponseTypeDef,
+    CreateLicenseResponseTypeDef,
+    CreateLicenseVersionResponseTypeDef,
+    CreateTokenResponseTypeDef,
+    DeleteGrantResponseTypeDef,
+    DeleteLicenseResponseTypeDef,
+    ExtendLicenseConsumptionResponseTypeDef,
+    GetAccessTokenResponseTypeDef,
+    RejectGrantResponseTypeDef,
     CheckoutLicenseRequestRequestTypeDef,
-    CheckoutBorrowLicenseRequestRequestTypeDef,
     CheckoutLicenseResponseTypeDef,
+    CheckoutBorrowLicenseRequestRequestTypeDef,
     CheckoutBorrowLicenseResponseTypeDef,
     LicenseOperationFailureTypeDef,
-    ConsumptionConfigurationOutputTypeDef,
     ConsumptionConfigurationTypeDef,
     CreateGrantVersionRequestRequestTypeDef,
+    GrantTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateLicenseConversionTaskForResourceRequestRequestTypeDef,
+    GetLicenseConversionTaskResponseTypeDef,
+    LicenseConversionTaskTypeDef,
     CreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     UpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     LicenseUsageTypeDef,
     ListDistributedGrantsRequestRequestTypeDef,
-    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
     ListLicenseConfigurationsRequestRequestTypeDef,
     ListLicenseConversionTasksRequestRequestTypeDef,
     ListLicenseManagerReportGeneratorsRequestRequestTypeDef,
     ListLicensesRequestRequestTypeDef,
     ListReceivedGrantsForOrganizationRequestRequestTypeDef,
     ListReceivedGrantsRequestRequestTypeDef,
     ListReceivedLicensesForOrganizationRequestRequestTypeDef,
     ListReceivedLicensesRequestRequestTypeDef,
     ListTokensRequestRequestTypeDef,
-    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListUsageForLicenseConfigurationRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GetLicenseConversionTaskResponseTypeDef,
-    LicenseConversionTaskTypeDef,
     GetServiceSettingsResponseTypeDef,
-    GrantTypeDef,
-    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
+    UpdateServiceSettingsRequestRequestTypeDef,
     ListResourceInventoryRequestRequestTypeDef,
     ListAssociationsForLicenseConfigurationResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     ListLicenseSpecificationsForResourceResponseTypeDef,
     UpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
+    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
+    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
+    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTokensResponseTypeDef,
-    UpdateServiceSettingsRequestRequestTypeDef,
     ProductInformationOutputTypeDef,
     ProductInformationTypeDef,
     ReportGeneratorTypeDef,
     ListFailuresForLicenseConfigurationOperationsResponseTypeDef,
-    GrantedLicenseTypeDef,
-    LicenseTypeDef,
     CreateLicenseRequestRequestTypeDef,
     CreateLicenseVersionRequestRequestTypeDef,
-    GetLicenseUsageResponseTypeDef,
-    ListLicenseConversionTasksResponseTypeDef,
+    GrantedLicenseTypeDef,
+    LicenseTypeDef,
     GetGrantResponseTypeDef,
     ListDistributedGrantsResponseTypeDef,
     ListReceivedGrantsForOrganizationResponseTypeDef,
     ListReceivedGrantsResponseTypeDef,
+    ListLicenseConversionTasksResponseTypeDef,
+    GetLicenseUsageResponseTypeDef,
     GetLicenseConfigurationResponseTypeDef,
     LicenseConfigurationTypeDef,
     CreateLicenseConfigurationRequestRequestTypeDef,
     UpdateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseManagerReportGeneratorResponseTypeDef,
     ListLicenseManagerReportGeneratorsResponseTypeDef,
     ListReceivedLicensesForOrganizationResponseTypeDef,
```

### Comparing `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/__init__.py` & `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/__init__.pyi` & `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/__main__.py` & `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LicenseManager 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.LicenseManager 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager\nOther"
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

### Comparing `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/client.py` & `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/client.pyi` & `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/literals.py` & `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/literals.pyi` & `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/paginator.py` & `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 class ListAssociationsForLicenseConfigurationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListAssociationsForLicenseConfiguration)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listassociationsforlicenseconfigurationpaginator)
     """
 
     def paginate(
-        self, *, LicenseConfigurationArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, LicenseConfigurationArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociationsForLicenseConfigurationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListAssociationsForLicenseConfiguration.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listassociationsforlicenseconfigurationpaginator)
         """
 
 
@@ -83,30 +83,30 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLicenseConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listlicenseconfigurationspaginator)
         """
 
 
 class ListLicenseSpecificationsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseSpecificationsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listlicensespecificationsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLicenseSpecificationsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseSpecificationsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listlicensespecificationsforresourcepaginator)
         """
 
 
@@ -116,15 +116,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listresourceinventorypaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceInventoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListResourceInventory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listresourceinventorypaginator)
         """
 
 
@@ -135,13 +135,13 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsageForLicenseConfigurationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListUsageForLicenseConfiguration.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listusageforlicenseconfigurationpaginator)
         """
```

### Comparing `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/paginator.pyi` & `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 class ListAssociationsForLicenseConfigurationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListAssociationsForLicenseConfiguration)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listassociationsforlicenseconfigurationpaginator)
     """
 
     def paginate(
-        self, *, LicenseConfigurationArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, LicenseConfigurationArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociationsForLicenseConfigurationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListAssociationsForLicenseConfiguration.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listassociationsforlicenseconfigurationpaginator)
         """
 
 class ListLicenseConfigurationsPaginator(Paginator):
@@ -79,29 +79,29 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLicenseConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listlicenseconfigurationspaginator)
         """
 
 class ListLicenseSpecificationsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseSpecificationsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listlicensespecificationsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLicenseSpecificationsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseSpecificationsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listlicensespecificationsforresourcepaginator)
         """
 
 class ListResourceInventoryPaginator(Paginator):
@@ -110,15 +110,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listresourceinventorypaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceInventoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListResourceInventory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listresourceinventorypaginator)
         """
 
 class ListUsageForLicenseConfigurationPaginator(Paginator):
@@ -128,13 +128,13 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsageForLicenseConfigurationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListUsageForLicenseConfiguration.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listusageforlicenseconfigurationpaginator)
         """
```

### Comparing `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/type_defs.py` & `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,151 +43,138 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptGrantRequestRequestTypeDef",
-    "AcceptGrantResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AutomatedDiscoveryInformationTypeDef",
-    "BorrowConfigurationOutputTypeDef",
     "BorrowConfigurationTypeDef",
     "CheckInLicenseRequestRequestTypeDef",
     "EntitlementDataTypeDef",
     "MetadataTypeDef",
-    "EntitlementDataOutputTypeDef",
-    "MetadataOutputTypeDef",
     "ConsumedLicenseSummaryTypeDef",
-    "ProvisionalConfigurationOutputTypeDef",
     "ProvisionalConfigurationTypeDef",
     "CreateGrantRequestRequestTypeDef",
-    "CreateGrantResponseTypeDef",
     "OptionsTypeDef",
-    "CreateGrantVersionResponseTypeDef",
     "TagTypeDef",
-    "CreateLicenseConfigurationResponseTypeDef",
     "LicenseConversionContextTypeDef",
-    "CreateLicenseConversionTaskForResourceResponseTypeDef",
     "ReportContextTypeDef",
     "ReportFrequencyTypeDef",
-    "CreateLicenseManagerReportGeneratorResponseTypeDef",
     "DatetimeRangeTypeDef",
     "EntitlementTypeDef",
     "IssuerTypeDef",
-    "CreateLicenseResponseTypeDef",
-    "CreateLicenseVersionResponseTypeDef",
     "CreateTokenRequestRequestTypeDef",
-    "CreateTokenResponseTypeDef",
-    "DatetimeRangeOutputTypeDef",
     "DeleteGrantRequestRequestTypeDef",
-    "DeleteGrantResponseTypeDef",
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     "DeleteLicenseManagerReportGeneratorRequestRequestTypeDef",
     "DeleteLicenseRequestRequestTypeDef",
-    "DeleteLicenseResponseTypeDef",
     "DeleteTokenRequestRequestTypeDef",
-    "EntitlementOutputTypeDef",
     "EntitlementUsageTypeDef",
     "ExtendLicenseConsumptionRequestRequestTypeDef",
-    "ExtendLicenseConsumptionResponseTypeDef",
     "FilterTypeDef",
     "GetAccessTokenRequestRequestTypeDef",
-    "GetAccessTokenResponseTypeDef",
     "GetGrantRequestRequestTypeDef",
     "GetLicenseConfigurationRequestRequestTypeDef",
     "ManagedResourceSummaryTypeDef",
-    "TagOutputTypeDef",
     "GetLicenseConversionTaskRequestRequestTypeDef",
-    "LicenseConversionContextOutputTypeDef",
     "GetLicenseManagerReportGeneratorRequestRequestTypeDef",
     "GetLicenseRequestRequestTypeDef",
     "GetLicenseUsageRequestRequestTypeDef",
-    "OrganizationConfigurationOutputTypeDef",
-    "OptionsOutputTypeDef",
+    "OrganizationConfigurationTypeDef",
     "IssuerDetailsTypeDef",
     "ReceivedMetadataTypeDef",
     "InventoryFilterTypeDef",
     "LicenseConfigurationAssociationTypeDef",
     "LicenseConfigurationUsageTypeDef",
-    "LicenseSpecificationOutputTypeDef",
     "LicenseSpecificationTypeDef",
-    "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     "ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
-    "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
     "ListLicenseSpecificationsForResourceRequestRequestTypeDef",
     "ListLicenseVersionsRequestRequestTypeDef",
     "ResourceInventoryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TokenDataTypeDef",
-    "OrganizationConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
     "ProductInformationFilterOutputTypeDef",
     "ProductInformationFilterTypeDef",
     "RejectGrantRequestRequestTypeDef",
-    "RejectGrantResponseTypeDef",
     "ReportContextOutputTypeDef",
-    "ReportFrequencyOutputTypeDef",
     "S3LocationTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AcceptGrantResponseTypeDef",
+    "CreateGrantResponseTypeDef",
+    "CreateGrantVersionResponseTypeDef",
+    "CreateLicenseConfigurationResponseTypeDef",
+    "CreateLicenseConversionTaskForResourceResponseTypeDef",
+    "CreateLicenseManagerReportGeneratorResponseTypeDef",
+    "CreateLicenseResponseTypeDef",
+    "CreateLicenseVersionResponseTypeDef",
+    "CreateTokenResponseTypeDef",
+    "DeleteGrantResponseTypeDef",
+    "DeleteLicenseResponseTypeDef",
+    "ExtendLicenseConsumptionResponseTypeDef",
+    "GetAccessTokenResponseTypeDef",
+    "RejectGrantResponseTypeDef",
     "CheckoutLicenseRequestRequestTypeDef",
-    "CheckoutBorrowLicenseRequestRequestTypeDef",
     "CheckoutLicenseResponseTypeDef",
+    "CheckoutBorrowLicenseRequestRequestTypeDef",
     "CheckoutBorrowLicenseResponseTypeDef",
     "LicenseOperationFailureTypeDef",
-    "ConsumptionConfigurationOutputTypeDef",
     "ConsumptionConfigurationTypeDef",
     "CreateGrantVersionRequestRequestTypeDef",
+    "GrantTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateLicenseConversionTaskForResourceRequestRequestTypeDef",
+    "GetLicenseConversionTaskResponseTypeDef",
+    "LicenseConversionTaskTypeDef",
     "CreateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "UpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "LicenseUsageTypeDef",
     "ListDistributedGrantsRequestRequestTypeDef",
-    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
     "ListLicenseConfigurationsRequestRequestTypeDef",
     "ListLicenseConversionTasksRequestRequestTypeDef",
     "ListLicenseManagerReportGeneratorsRequestRequestTypeDef",
     "ListLicensesRequestRequestTypeDef",
     "ListReceivedGrantsForOrganizationRequestRequestTypeDef",
     "ListReceivedGrantsRequestRequestTypeDef",
     "ListReceivedLicensesForOrganizationRequestRequestTypeDef",
     "ListReceivedLicensesRequestRequestTypeDef",
     "ListTokensRequestRequestTypeDef",
-    "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListUsageForLicenseConfigurationRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "GetLicenseConversionTaskResponseTypeDef",
-    "LicenseConversionTaskTypeDef",
     "GetServiceSettingsResponseTypeDef",
-    "GrantTypeDef",
-    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
+    "UpdateServiceSettingsRequestRequestTypeDef",
     "ListResourceInventoryRequestRequestTypeDef",
     "ListAssociationsForLicenseConfigurationResponseTypeDef",
     "ListUsageForLicenseConfigurationResponseTypeDef",
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     "UpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
+    "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
+    "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
+    "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListResourceInventoryResponseTypeDef",
     "ListTokensResponseTypeDef",
-    "UpdateServiceSettingsRequestRequestTypeDef",
     "ProductInformationOutputTypeDef",
     "ProductInformationTypeDef",
     "ReportGeneratorTypeDef",
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
-    "GrantedLicenseTypeDef",
-    "LicenseTypeDef",
     "CreateLicenseRequestRequestTypeDef",
     "CreateLicenseVersionRequestRequestTypeDef",
-    "GetLicenseUsageResponseTypeDef",
-    "ListLicenseConversionTasksResponseTypeDef",
+    "GrantedLicenseTypeDef",
+    "LicenseTypeDef",
     "GetGrantResponseTypeDef",
     "ListDistributedGrantsResponseTypeDef",
     "ListReceivedGrantsForOrganizationResponseTypeDef",
     "ListReceivedGrantsResponseTypeDef",
+    "ListLicenseConversionTasksResponseTypeDef",
+    "GetLicenseUsageResponseTypeDef",
     "GetLicenseConfigurationResponseTypeDef",
     "LicenseConfigurationTypeDef",
     "CreateLicenseConfigurationRequestRequestTypeDef",
     "UpdateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     "ListReceivedLicensesForOrganizationResponseTypeDef",
@@ -201,40 +188,33 @@
 AcceptGrantRequestRequestTypeDef = TypedDict(
     "AcceptGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 
-AcceptGrantResponseTypeDef = TypedDict(
-    "AcceptGrantResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AutomatedDiscoveryInformationTypeDef = TypedDict(
     "AutomatedDiscoveryInformationTypeDef",
     {
         "LastRunTime": datetime,
     },
     total=False,
 )
 
-BorrowConfigurationOutputTypeDef = TypedDict(
-    "BorrowConfigurationOutputTypeDef",
-    {
-        "AllowEarlyCheckIn": bool,
-        "MaxTimeToLiveInMinutes": int,
-    },
-)
-
 BorrowConfigurationTypeDef = TypedDict(
     "BorrowConfigurationTypeDef",
     {
         "AllowEarlyCheckIn": bool,
         "MaxTimeToLiveInMinutes": int,
     },
 )
@@ -285,61 +265,23 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredEntitlementDataOutputTypeDef = TypedDict(
-    "_RequiredEntitlementDataOutputTypeDef",
-    {
-        "Name": str,
-        "Unit": EntitlementDataUnitType,
-    },
-)
-_OptionalEntitlementDataOutputTypeDef = TypedDict(
-    "_OptionalEntitlementDataOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-
-class EntitlementDataOutputTypeDef(
-    _RequiredEntitlementDataOutputTypeDef, _OptionalEntitlementDataOutputTypeDef
-):
-    pass
-
-
-MetadataOutputTypeDef = TypedDict(
-    "MetadataOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 ConsumedLicenseSummaryTypeDef = TypedDict(
     "ConsumedLicenseSummaryTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "ConsumedLicenses": int,
     },
     total=False,
 )
 
-ProvisionalConfigurationOutputTypeDef = TypedDict(
-    "ProvisionalConfigurationOutputTypeDef",
-    {
-        "MaxTimeToLiveInMinutes": int,
-    },
-)
-
 ProvisionalConfigurationTypeDef = TypedDict(
     "ProvisionalConfigurationTypeDef",
     {
         "MaxTimeToLiveInMinutes": int,
     },
 )
 
@@ -351,75 +293,39 @@
         "LicenseArn": str,
         "Principals": Sequence[str],
         "HomeRegion": str,
         "AllowedOperations": Sequence[AllowedOperationType],
     },
 )
 
-CreateGrantResponseTypeDef = TypedDict(
-    "CreateGrantResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OptionsTypeDef = TypedDict(
     "OptionsTypeDef",
     {
         "ActivationOverrideBehavior": ActivationOverrideBehaviorType,
     },
     total=False,
 )
 
-CreateGrantVersionResponseTypeDef = TypedDict(
-    "CreateGrantVersionResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-CreateLicenseConfigurationResponseTypeDef = TypedDict(
-    "CreateLicenseConfigurationResponseTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LicenseConversionContextTypeDef = TypedDict(
     "LicenseConversionContextTypeDef",
     {
         "UsageOperation": str,
     },
     total=False,
 )
 
-CreateLicenseConversionTaskForResourceResponseTypeDef = TypedDict(
-    "CreateLicenseConversionTaskForResourceResponseTypeDef",
-    {
-        "LicenseConversionTaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReportContextTypeDef = TypedDict(
     "ReportContextTypeDef",
     {
         "licenseConfigurationArns": Sequence[str],
     },
 )
 
@@ -428,22 +334,14 @@
     {
         "value": int,
         "period": ReportFrequencyTypeType,
     },
     total=False,
 )
 
-CreateLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
-    "CreateLicenseManagerReportGeneratorResponseTypeDef",
-    {
-        "LicenseManagerReportGeneratorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDatetimeRangeTypeDef = TypedDict(
     "_RequiredDatetimeRangeTypeDef",
     {
         "Begin": str,
     },
 )
 _OptionalDatetimeRangeTypeDef = TypedDict(
@@ -497,34 +395,14 @@
 )
 
 
 class IssuerTypeDef(_RequiredIssuerTypeDef, _OptionalIssuerTypeDef):
     pass
 
 
-CreateLicenseResponseTypeDef = TypedDict(
-    "CreateLicenseResponseTypeDef",
-    {
-        "LicenseArn": str,
-        "Status": LicenseStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateLicenseVersionResponseTypeDef = TypedDict(
-    "CreateLicenseVersionResponseTypeDef",
-    {
-        "LicenseArn": str,
-        "Version": str,
-        "Status": LicenseStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTokenRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "ClientToken": str,
     },
 )
@@ -541,45 +419,14 @@
 
 class CreateTokenRequestRequestTypeDef(
     _RequiredCreateTokenRequestRequestTypeDef, _OptionalCreateTokenRequestRequestTypeDef
 ):
     pass
 
 
-CreateTokenResponseTypeDef = TypedDict(
-    "CreateTokenResponseTypeDef",
-    {
-        "TokenId": str,
-        "TokenType": Literal["REFRESH_TOKEN"],
-        "Token": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDatetimeRangeOutputTypeDef = TypedDict(
-    "_RequiredDatetimeRangeOutputTypeDef",
-    {
-        "Begin": str,
-    },
-)
-_OptionalDatetimeRangeOutputTypeDef = TypedDict(
-    "_OptionalDatetimeRangeOutputTypeDef",
-    {
-        "End": str,
-    },
-    total=False,
-)
-
-
-class DatetimeRangeOutputTypeDef(
-    _RequiredDatetimeRangeOutputTypeDef, _OptionalDatetimeRangeOutputTypeDef
-):
-    pass
-
-
 _RequiredDeleteGrantRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
         "Version": str,
     },
 )
@@ -594,24 +441,14 @@
 
 class DeleteGrantRequestRequestTypeDef(
     _RequiredDeleteGrantRequestRequestTypeDef, _OptionalDeleteGrantRequestRequestTypeDef
 ):
     pass
 
 
-DeleteGrantResponseTypeDef = TypedDict(
-    "DeleteGrantResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 
@@ -626,55 +463,21 @@
     "DeleteLicenseRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "SourceVersion": str,
     },
 )
 
-DeleteLicenseResponseTypeDef = TypedDict(
-    "DeleteLicenseResponseTypeDef",
-    {
-        "Status": LicenseDeletionStatusType,
-        "DeletionDate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTokenRequestRequestTypeDef = TypedDict(
     "DeleteTokenRequestRequestTypeDef",
     {
         "TokenId": str,
     },
 )
 
-_RequiredEntitlementOutputTypeDef = TypedDict(
-    "_RequiredEntitlementOutputTypeDef",
-    {
-        "Name": str,
-        "Unit": EntitlementUnitType,
-    },
-)
-_OptionalEntitlementOutputTypeDef = TypedDict(
-    "_OptionalEntitlementOutputTypeDef",
-    {
-        "Value": str,
-        "MaxCount": int,
-        "Overage": bool,
-        "AllowCheckIn": bool,
-    },
-    total=False,
-)
-
-
-class EntitlementOutputTypeDef(
-    _RequiredEntitlementOutputTypeDef, _OptionalEntitlementOutputTypeDef
-):
-    pass
-
-
 _RequiredEntitlementUsageTypeDef = TypedDict(
     "_RequiredEntitlementUsageTypeDef",
     {
         "Name": str,
         "ConsumedValue": str,
         "Unit": EntitlementDataUnitType,
     },
@@ -710,23 +513,14 @@
 class ExtendLicenseConsumptionRequestRequestTypeDef(
     _RequiredExtendLicenseConsumptionRequestRequestTypeDef,
     _OptionalExtendLicenseConsumptionRequestRequestTypeDef,
 ):
     pass
 
 
-ExtendLicenseConsumptionResponseTypeDef = TypedDict(
-    "ExtendLicenseConsumptionResponseTypeDef",
-    {
-        "LicenseConsumptionToken": str,
-        "Expiration": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -749,22 +543,14 @@
 
 class GetAccessTokenRequestRequestTypeDef(
     _RequiredGetAccessTokenRequestRequestTypeDef, _OptionalGetAccessTokenRequestRequestTypeDef
 ):
     pass
 
 
-GetAccessTokenResponseTypeDef = TypedDict(
-    "GetAccessTokenResponseTypeDef",
-    {
-        "AccessToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetGrantRequestRequestTypeDef = TypedDict(
     "_RequiredGetGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 _OptionalGetGrantRequestRequestTypeDef = TypedDict(
@@ -794,38 +580,21 @@
     {
         "ResourceType": ResourceTypeType,
         "AssociationCount": int,
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
 GetLicenseConversionTaskRequestRequestTypeDef = TypedDict(
     "GetLicenseConversionTaskRequestRequestTypeDef",
     {
         "LicenseConversionTaskId": str,
     },
 )
 
-LicenseConversionContextOutputTypeDef = TypedDict(
-    "LicenseConversionContextOutputTypeDef",
-    {
-        "UsageOperation": str,
-    },
-    total=False,
-)
-
 GetLicenseManagerReportGeneratorRequestRequestTypeDef = TypedDict(
     "GetLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "LicenseManagerReportGeneratorArn": str,
     },
 )
 
@@ -853,29 +622,21 @@
 GetLicenseUsageRequestRequestTypeDef = TypedDict(
     "GetLicenseUsageRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 
-OrganizationConfigurationOutputTypeDef = TypedDict(
-    "OrganizationConfigurationOutputTypeDef",
+OrganizationConfigurationTypeDef = TypedDict(
+    "OrganizationConfigurationTypeDef",
     {
         "EnableIntegration": bool,
     },
 )
 
-OptionsOutputTypeDef = TypedDict(
-    "OptionsOutputTypeDef",
-    {
-        "ActivationOverrideBehavior": ActivationOverrideBehaviorType,
-    },
-    total=False,
-)
-
 IssuerDetailsTypeDef = TypedDict(
     "IssuerDetailsTypeDef",
     {
         "Name": str,
         "SignKey": str,
         "KeyFingerprint": str,
     },
@@ -933,35 +694,14 @@
         "ResourceOwnerId": str,
         "AssociationTime": datetime,
         "ConsumedLicenses": int,
     },
     total=False,
 )
 
-_RequiredLicenseSpecificationOutputTypeDef = TypedDict(
-    "_RequiredLicenseSpecificationOutputTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalLicenseSpecificationOutputTypeDef = TypedDict(
-    "_OptionalLicenseSpecificationOutputTypeDef",
-    {
-        "AmiAssociationScope": str,
-    },
-    total=False,
-)
-
-
-class LicenseSpecificationOutputTypeDef(
-    _RequiredLicenseSpecificationOutputTypeDef, _OptionalLicenseSpecificationOutputTypeDef
-):
-    pass
-
-
 _RequiredLicenseSpecificationTypeDef = TypedDict(
     "_RequiredLicenseSpecificationTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalLicenseSpecificationTypeDef = TypedDict(
@@ -975,36 +715,24 @@
 
 class LicenseSpecificationTypeDef(
     _RequiredLicenseSpecificationTypeDef, _OptionalLicenseSpecificationTypeDef
 ):
     pass
 
 
-_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
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
 
-
-class ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef(
-    _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
-    _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListAssociationsForLicenseConfigurationRequestRequestTypeDef = TypedDict(
@@ -1043,36 +771,14 @@
 class ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef(
     _RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
     _OptionalListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef(
-    _RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
-    _OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
@@ -1145,31 +851,14 @@
         "TokenProperties": List[str],
         "RoleArns": List[str],
         "Status": str,
     },
     total=False,
 )
 
-OrganizationConfigurationTypeDef = TypedDict(
-    "OrganizationConfigurationTypeDef",
-    {
-        "EnableIntegration": bool,
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
 _RequiredProductInformationFilterOutputTypeDef = TypedDict(
     "_RequiredProductInformationFilterOutputTypeDef",
     {
         "ProductInformationFilterName": str,
         "ProductInformationFilterComparator": str,
     },
 )
@@ -1213,65 +902,165 @@
 RejectGrantRequestRequestTypeDef = TypedDict(
     "RejectGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 
-RejectGrantResponseTypeDef = TypedDict(
-    "RejectGrantResponseTypeDef",
+ReportContextOutputTypeDef = TypedDict(
+    "ReportContextOutputTypeDef",
+    {
+        "licenseConfigurationArns": List[str],
+    },
+)
+
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
+    {
+        "bucket": str,
+        "keyPrefix": str,
+    },
+    total=False,
+)
+
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
+    },
+)
+
+AcceptGrantResponseTypeDef = TypedDict(
+    "AcceptGrantResponseTypeDef",
     {
         "GrantArn": str,
         "Status": GrantStatusType,
         "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReportContextOutputTypeDef = TypedDict(
-    "ReportContextOutputTypeDef",
+CreateGrantResponseTypeDef = TypedDict(
+    "CreateGrantResponseTypeDef",
     {
-        "licenseConfigurationArns": List[str],
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGrantVersionResponseTypeDef = TypedDict(
+    "CreateGrantVersionResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReportFrequencyOutputTypeDef = TypedDict(
-    "ReportFrequencyOutputTypeDef",
+CreateLicenseConfigurationResponseTypeDef = TypedDict(
+    "CreateLicenseConfigurationResponseTypeDef",
     {
-        "value": int,
-        "period": ReportFrequencyTypeType,
+        "LicenseConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
+CreateLicenseConversionTaskForResourceResponseTypeDef = TypedDict(
+    "CreateLicenseConversionTaskForResourceResponseTypeDef",
     {
-        "bucket": str,
-        "keyPrefix": str,
+        "LicenseConversionTaskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
+    "CreateLicenseManagerReportGeneratorResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "LicenseManagerReportGeneratorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+CreateLicenseResponseTypeDef = TypedDict(
+    "CreateLicenseResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "LicenseArn": str,
+        "Status": LicenseStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLicenseVersionResponseTypeDef = TypedDict(
+    "CreateLicenseVersionResponseTypeDef",
+    {
+        "LicenseArn": str,
+        "Version": str,
+        "Status": LicenseStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTokenResponseTypeDef = TypedDict(
+    "CreateTokenResponseTypeDef",
+    {
+        "TokenId": str,
+        "TokenType": Literal["REFRESH_TOKEN"],
+        "Token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteGrantResponseTypeDef = TypedDict(
+    "DeleteGrantResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteLicenseResponseTypeDef = TypedDict(
+    "DeleteLicenseResponseTypeDef",
+    {
+        "Status": LicenseDeletionStatusType,
+        "DeletionDate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExtendLicenseConsumptionResponseTypeDef = TypedDict(
+    "ExtendLicenseConsumptionResponseTypeDef",
+    {
+        "LicenseConsumptionToken": str,
+        "Expiration": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccessTokenResponseTypeDef = TypedDict(
+    "GetAccessTokenResponseTypeDef",
+    {
+        "AccessToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RejectGrantResponseTypeDef = TypedDict(
+    "RejectGrantResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCheckoutLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCheckoutLicenseRequestRequestTypeDef",
     {
         "ProductSKU": str,
@@ -1293,14 +1082,29 @@
 
 class CheckoutLicenseRequestRequestTypeDef(
     _RequiredCheckoutLicenseRequestRequestTypeDef, _OptionalCheckoutLicenseRequestRequestTypeDef
 ):
     pass
 
 
+CheckoutLicenseResponseTypeDef = TypedDict(
+    "CheckoutLicenseResponseTypeDef",
+    {
+        "CheckoutType": CheckoutTypeType,
+        "LicenseConsumptionToken": str,
+        "EntitlementsAllowed": List[EntitlementDataTypeDef],
+        "SignedToken": str,
+        "NodeId": str,
+        "IssuedAt": str,
+        "Expiration": str,
+        "LicenseArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCheckoutBorrowLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCheckoutBorrowLicenseRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "Entitlements": Sequence[EntitlementDataTypeDef],
         "DigitalSignatureMethod": Literal["JWT_PS384"],
         "ClientToken": str,
@@ -1319,65 +1123,40 @@
 class CheckoutBorrowLicenseRequestRequestTypeDef(
     _RequiredCheckoutBorrowLicenseRequestRequestTypeDef,
     _OptionalCheckoutBorrowLicenseRequestRequestTypeDef,
 ):
     pass
 
 
-CheckoutLicenseResponseTypeDef = TypedDict(
-    "CheckoutLicenseResponseTypeDef",
-    {
-        "CheckoutType": CheckoutTypeType,
-        "LicenseConsumptionToken": str,
-        "EntitlementsAllowed": List[EntitlementDataOutputTypeDef],
-        "SignedToken": str,
-        "NodeId": str,
-        "IssuedAt": str,
-        "Expiration": str,
-        "LicenseArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CheckoutBorrowLicenseResponseTypeDef = TypedDict(
     "CheckoutBorrowLicenseResponseTypeDef",
     {
         "LicenseArn": str,
         "LicenseConsumptionToken": str,
-        "EntitlementsAllowed": List[EntitlementDataOutputTypeDef],
+        "EntitlementsAllowed": List[EntitlementDataTypeDef],
         "NodeId": str,
         "SignedToken": str,
         "IssuedAt": str,
         "Expiration": str,
-        "CheckoutMetadata": List[MetadataOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CheckoutMetadata": List[MetadataTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LicenseOperationFailureTypeDef = TypedDict(
     "LicenseOperationFailureTypeDef",
     {
         "ResourceArn": str,
         "ResourceType": ResourceTypeType,
         "ErrorMessage": str,
         "FailureTime": datetime,
         "OperationName": str,
         "ResourceOwnerId": str,
         "OperationRequestedBy": str,
-        "MetadataList": List[MetadataOutputTypeDef],
-    },
-    total=False,
-)
-
-ConsumptionConfigurationOutputTypeDef = TypedDict(
-    "ConsumptionConfigurationOutputTypeDef",
-    {
-        "RenewType": RenewTypeType,
-        "ProvisionalConfiguration": ProvisionalConfigurationOutputTypeDef,
-        "BorrowConfiguration": BorrowConfigurationOutputTypeDef,
+        "MetadataList": List[MetadataTypeDef],
     },
     total=False,
 )
 
 ConsumptionConfigurationTypeDef = TypedDict(
     "ConsumptionConfigurationTypeDef",
     {
@@ -1412,14 +1191,50 @@
 class CreateGrantVersionRequestRequestTypeDef(
     _RequiredCreateGrantVersionRequestRequestTypeDef,
     _OptionalCreateGrantVersionRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredGrantTypeDef = TypedDict(
+    "_RequiredGrantTypeDef",
+    {
+        "GrantArn": str,
+        "GrantName": str,
+        "ParentArn": str,
+        "LicenseArn": str,
+        "GranteePrincipalArn": str,
+        "HomeRegion": str,
+        "GrantStatus": GrantStatusType,
+        "Version": str,
+        "GrantedOperations": List[AllowedOperationType],
+    },
+)
+_OptionalGrantTypeDef = TypedDict(
+    "_OptionalGrantTypeDef",
+    {
+        "StatusReason": str,
+        "Options": OptionsTypeDef,
+    },
+    total=False,
+)
+
+
+class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
+    pass
+
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1429,14 +1244,46 @@
     {
         "ResourceArn": str,
         "SourceLicenseContext": LicenseConversionContextTypeDef,
         "DestinationLicenseContext": LicenseConversionContextTypeDef,
     },
 )
 
+GetLicenseConversionTaskResponseTypeDef = TypedDict(
+    "GetLicenseConversionTaskResponseTypeDef",
+    {
+        "LicenseConversionTaskId": str,
+        "ResourceArn": str,
+        "SourceLicenseContext": LicenseConversionContextTypeDef,
+        "DestinationLicenseContext": LicenseConversionContextTypeDef,
+        "StatusMessage": str,
+        "Status": LicenseConversionTaskStatusType,
+        "StartTime": datetime,
+        "LicenseConversionTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LicenseConversionTaskTypeDef = TypedDict(
+    "LicenseConversionTaskTypeDef",
+    {
+        "LicenseConversionTaskId": str,
+        "ResourceArn": str,
+        "SourceLicenseContext": LicenseConversionContextTypeDef,
+        "DestinationLicenseContext": LicenseConversionContextTypeDef,
+        "Status": LicenseConversionTaskStatusType,
+        "StatusMessage": str,
+        "StartTime": datetime,
+        "LicenseConversionTime": datetime,
+        "EndTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredCreateLicenseManagerReportGeneratorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "ReportGeneratorName": str,
         "Type": Sequence[ReportTypeType],
         "ReportContext": ReportContextTypeDef,
         "ReportFrequency": ReportFrequencyTypeDef,
@@ -1502,24 +1349,14 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef = TypedDict(
-    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
-    {
-        "LicenseConfigurationArns": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLicenseConfigurationsRequestRequestTypeDef = TypedDict(
     "ListLicenseConfigurationsRequestRequestTypeDef",
     {
         "LicenseConfigurationArns": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
@@ -1621,37 +1458,14 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef(
-    _RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
-    _OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredListUsageForLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
@@ -1668,99 +1482,33 @@
 class ListUsageForLicenseConfigurationRequestRequestTypeDef(
     _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef,
     _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetLicenseConversionTaskResponseTypeDef = TypedDict(
-    "GetLicenseConversionTaskResponseTypeDef",
-    {
-        "LicenseConversionTaskId": str,
-        "ResourceArn": str,
-        "SourceLicenseContext": LicenseConversionContextOutputTypeDef,
-        "DestinationLicenseContext": LicenseConversionContextOutputTypeDef,
-        "StatusMessage": str,
-        "Status": LicenseConversionTaskStatusType,
-        "StartTime": datetime,
-        "LicenseConversionTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LicenseConversionTaskTypeDef = TypedDict(
-    "LicenseConversionTaskTypeDef",
-    {
-        "LicenseConversionTaskId": str,
-        "ResourceArn": str,
-        "SourceLicenseContext": LicenseConversionContextOutputTypeDef,
-        "DestinationLicenseContext": LicenseConversionContextOutputTypeDef,
-        "Status": LicenseConversionTaskStatusType,
-        "StatusMessage": str,
-        "StartTime": datetime,
-        "LicenseConversionTime": datetime,
-        "EndTime": datetime,
-    },
-    total=False,
-)
-
 GetServiceSettingsResponseTypeDef = TypedDict(
     "GetServiceSettingsResponseTypeDef",
     {
         "S3BucketArn": str,
         "SnsTopicArn": str,
-        "OrganizationConfiguration": OrganizationConfigurationOutputTypeDef,
+        "OrganizationConfiguration": OrganizationConfigurationTypeDef,
         "EnableCrossAccountsDiscovery": bool,
         "LicenseManagerResourceShareArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGrantTypeDef = TypedDict(
-    "_RequiredGrantTypeDef",
-    {
-        "GrantArn": str,
-        "GrantName": str,
-        "ParentArn": str,
-        "LicenseArn": str,
-        "GranteePrincipalArn": str,
-        "HomeRegion": str,
-        "GrantStatus": GrantStatusType,
-        "Version": str,
-        "GrantedOperations": List[AllowedOperationType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalGrantTypeDef = TypedDict(
-    "_OptionalGrantTypeDef",
-    {
-        "StatusReason": str,
-        "Options": OptionsOutputTypeDef,
-    },
-    total=False,
-)
 
-
-class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
-    pass
-
-
-ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
-    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
+UpdateServiceSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateServiceSettingsRequestRequestTypeDef",
     {
-        "Filters": Sequence[InventoryFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "S3BucketArn": str,
+        "SnsTopicArn": str,
+        "OrganizationConfiguration": OrganizationConfigurationTypeDef,
+        "EnableCrossAccountsDiscovery": bool,
     },
     total=False,
 )
 
 ListResourceInventoryRequestRequestTypeDef = TypedDict(
     "ListResourceInventoryRequestRequestTypeDef",
     {
@@ -1772,33 +1520,33 @@
 )
 
 ListAssociationsForLicenseConfigurationResponseTypeDef = TypedDict(
     "ListAssociationsForLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationAssociations": List[LicenseConfigurationAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsageForLicenseConfigurationResponseTypeDef = TypedDict(
     "ListUsageForLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationUsageList": List[LicenseConfigurationUsageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseSpecificationsForResourceResponseTypeDef = TypedDict(
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     {
-        "LicenseSpecifications": List[LicenseSpecificationOutputTypeDef],
+        "LicenseSpecifications": List[LicenseSpecificationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1817,43 +1565,118 @@
 class UpdateLicenseSpecificationsForResourceRequestRequestTypeDef(
     _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
     _OptionalUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef(
+    _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+):
+    pass
+
+
+ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef = TypedDict(
+    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
+    {
+        "LicenseConfigurationArns": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef(
+    _RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+    _OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+):
+    pass
+
+
+ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
+    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
+    {
+        "Filters": Sequence[InventoryFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef(
+    _RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
+    _OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
+):
+    pass
+
+
 ListResourceInventoryResponseTypeDef = TypedDict(
     "ListResourceInventoryResponseTypeDef",
     {
         "ResourceInventoryList": List[ResourceInventoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTokensResponseTypeDef = TypedDict(
     "ListTokensResponseTypeDef",
     {
         "Tokens": List[TokenDataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateServiceSettingsRequestRequestTypeDef",
-    {
-        "S3BucketArn": str,
-        "SnsTopicArn": str,
-        "OrganizationConfiguration": OrganizationConfigurationTypeDef,
-        "EnableCrossAccountsDiscovery": bool,
-    },
-    total=False,
-)
-
 ProductInformationOutputTypeDef = TypedDict(
     "ProductInformationOutputTypeDef",
     {
         "ResourceType": str,
         "ProductInformationFilterList": List[ProductInformationFilterOutputTypeDef],
     },
 )
@@ -1868,80 +1691,37 @@
 
 ReportGeneratorTypeDef = TypedDict(
     "ReportGeneratorTypeDef",
     {
         "ReportGeneratorName": str,
         "ReportType": List[ReportTypeType],
         "ReportContext": ReportContextOutputTypeDef,
-        "ReportFrequency": ReportFrequencyOutputTypeDef,
+        "ReportFrequency": ReportFrequencyTypeDef,
         "LicenseManagerReportGeneratorArn": str,
         "LastRunStatus": str,
         "LastRunFailureReason": str,
         "LastReportGenerationTime": str,
         "ReportCreatorAccount": str,
         "Description": str,
         "S3Location": S3LocationTypeDef,
         "CreateTime": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 ListFailuresForLicenseConfigurationOperationsResponseTypeDef = TypedDict(
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     {
         "LicenseOperationFailureList": List[LicenseOperationFailureTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GrantedLicenseTypeDef = TypedDict(
-    "GrantedLicenseTypeDef",
-    {
-        "LicenseArn": str,
-        "LicenseName": str,
-        "ProductName": str,
-        "ProductSKU": str,
-        "Issuer": IssuerDetailsTypeDef,
-        "HomeRegion": str,
-        "Status": LicenseStatusType,
-        "Validity": DatetimeRangeOutputTypeDef,
-        "Beneficiary": str,
-        "Entitlements": List[EntitlementOutputTypeDef],
-        "ConsumptionConfiguration": ConsumptionConfigurationOutputTypeDef,
-        "LicenseMetadata": List[MetadataOutputTypeDef],
-        "CreateTime": str,
-        "Version": str,
-        "ReceivedMetadata": ReceivedMetadataTypeDef,
-    },
-    total=False,
-)
-
-LicenseTypeDef = TypedDict(
-    "LicenseTypeDef",
-    {
-        "LicenseArn": str,
-        "LicenseName": str,
-        "ProductName": str,
-        "ProductSKU": str,
-        "Issuer": IssuerDetailsTypeDef,
-        "HomeRegion": str,
-        "Status": LicenseStatusType,
-        "Validity": DatetimeRangeOutputTypeDef,
-        "Beneficiary": str,
-        "Entitlements": List[EntitlementOutputTypeDef],
-        "ConsumptionConfiguration": ConsumptionConfigurationOutputTypeDef,
-        "LicenseMetadata": List[MetadataOutputTypeDef],
-        "CreateTime": str,
-        "Version": str,
-    },
-    total=False,
-)
-
 _RequiredCreateLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseRequestRequestTypeDef",
     {
         "LicenseName": str,
         "ProductName": str,
         "ProductSKU": str,
         "Issuer": IssuerTypeDef,
@@ -1996,63 +1776,106 @@
 class CreateLicenseVersionRequestRequestTypeDef(
     _RequiredCreateLicenseVersionRequestRequestTypeDef,
     _OptionalCreateLicenseVersionRequestRequestTypeDef,
 ):
     pass
 
 
-GetLicenseUsageResponseTypeDef = TypedDict(
-    "GetLicenseUsageResponseTypeDef",
+GrantedLicenseTypeDef = TypedDict(
+    "GrantedLicenseTypeDef",
     {
-        "LicenseUsage": LicenseUsageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LicenseArn": str,
+        "LicenseName": str,
+        "ProductName": str,
+        "ProductSKU": str,
+        "Issuer": IssuerDetailsTypeDef,
+        "HomeRegion": str,
+        "Status": LicenseStatusType,
+        "Validity": DatetimeRangeTypeDef,
+        "Beneficiary": str,
+        "Entitlements": List[EntitlementTypeDef],
+        "ConsumptionConfiguration": ConsumptionConfigurationTypeDef,
+        "LicenseMetadata": List[MetadataTypeDef],
+        "CreateTime": str,
+        "Version": str,
+        "ReceivedMetadata": ReceivedMetadataTypeDef,
     },
+    total=False,
 )
 
-ListLicenseConversionTasksResponseTypeDef = TypedDict(
-    "ListLicenseConversionTasksResponseTypeDef",
+LicenseTypeDef = TypedDict(
+    "LicenseTypeDef",
     {
-        "LicenseConversionTasks": List[LicenseConversionTaskTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LicenseArn": str,
+        "LicenseName": str,
+        "ProductName": str,
+        "ProductSKU": str,
+        "Issuer": IssuerDetailsTypeDef,
+        "HomeRegion": str,
+        "Status": LicenseStatusType,
+        "Validity": DatetimeRangeTypeDef,
+        "Beneficiary": str,
+        "Entitlements": List[EntitlementTypeDef],
+        "ConsumptionConfiguration": ConsumptionConfigurationTypeDef,
+        "LicenseMetadata": List[MetadataTypeDef],
+        "CreateTime": str,
+        "Version": str,
     },
+    total=False,
 )
 
 GetGrantResponseTypeDef = TypedDict(
     "GetGrantResponseTypeDef",
     {
         "Grant": GrantTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributedGrantsResponseTypeDef = TypedDict(
     "ListDistributedGrantsResponseTypeDef",
     {
         "Grants": List[GrantTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedGrantsForOrganizationResponseTypeDef = TypedDict(
     "ListReceivedGrantsForOrganizationResponseTypeDef",
     {
         "Grants": List[GrantTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedGrantsResponseTypeDef = TypedDict(
     "ListReceivedGrantsResponseTypeDef",
     {
         "Grants": List[GrantTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListLicenseConversionTasksResponseTypeDef = TypedDict(
+    "ListLicenseConversionTasksResponseTypeDef",
+    {
+        "LicenseConversionTasks": List[LicenseConversionTaskTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLicenseUsageResponseTypeDef = TypedDict(
+    "GetLicenseUsageResponseTypeDef",
+    {
+        "LicenseUsage": LicenseUsageTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLicenseConfigurationResponseTypeDef = TypedDict(
     "GetLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationId": str,
@@ -2064,19 +1887,19 @@
         "LicenseCount": int,
         "LicenseCountHardLimit": bool,
         "ConsumedLicenses": int,
         "Status": str,
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ProductInformationList": List[ProductInformationOutputTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
         "DisassociateWhenNotFound": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LicenseConfigurationTypeDef = TypedDict(
     "LicenseConfigurationTypeDef",
     {
         "LicenseConfigurationId": str,
@@ -2157,72 +1980,72 @@
     pass
 
 
 GetLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     {
         "ReportGenerator": ReportGeneratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseManagerReportGeneratorsResponseTypeDef = TypedDict(
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     {
         "ReportGenerators": List[ReportGeneratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedLicensesForOrganizationResponseTypeDef = TypedDict(
     "ListReceivedLicensesForOrganizationResponseTypeDef",
     {
         "Licenses": List[GrantedLicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedLicensesResponseTypeDef = TypedDict(
     "ListReceivedLicensesResponseTypeDef",
     {
         "Licenses": List[GrantedLicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLicenseResponseTypeDef = TypedDict(
     "GetLicenseResponseTypeDef",
     {
         "License": LicenseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseVersionsResponseTypeDef = TypedDict(
     "ListLicenseVersionsResponseTypeDef",
     {
         "Licenses": List[LicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicensesResponseTypeDef = TypedDict(
     "ListLicensesResponseTypeDef",
     {
         "Licenses": List[LicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseConfigurationsResponseTypeDef = TypedDict(
     "ListLicenseConfigurationsResponseTypeDef",
     {
         "LicenseConfigurations": List[LicenseConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/type_defs.pyi` & `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -42,151 +42,138 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptGrantRequestRequestTypeDef",
-    "AcceptGrantResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AutomatedDiscoveryInformationTypeDef",
-    "BorrowConfigurationOutputTypeDef",
     "BorrowConfigurationTypeDef",
     "CheckInLicenseRequestRequestTypeDef",
     "EntitlementDataTypeDef",
     "MetadataTypeDef",
-    "EntitlementDataOutputTypeDef",
-    "MetadataOutputTypeDef",
     "ConsumedLicenseSummaryTypeDef",
-    "ProvisionalConfigurationOutputTypeDef",
     "ProvisionalConfigurationTypeDef",
     "CreateGrantRequestRequestTypeDef",
-    "CreateGrantResponseTypeDef",
     "OptionsTypeDef",
-    "CreateGrantVersionResponseTypeDef",
     "TagTypeDef",
-    "CreateLicenseConfigurationResponseTypeDef",
     "LicenseConversionContextTypeDef",
-    "CreateLicenseConversionTaskForResourceResponseTypeDef",
     "ReportContextTypeDef",
     "ReportFrequencyTypeDef",
-    "CreateLicenseManagerReportGeneratorResponseTypeDef",
     "DatetimeRangeTypeDef",
     "EntitlementTypeDef",
     "IssuerTypeDef",
-    "CreateLicenseResponseTypeDef",
-    "CreateLicenseVersionResponseTypeDef",
     "CreateTokenRequestRequestTypeDef",
-    "CreateTokenResponseTypeDef",
-    "DatetimeRangeOutputTypeDef",
     "DeleteGrantRequestRequestTypeDef",
-    "DeleteGrantResponseTypeDef",
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     "DeleteLicenseManagerReportGeneratorRequestRequestTypeDef",
     "DeleteLicenseRequestRequestTypeDef",
-    "DeleteLicenseResponseTypeDef",
     "DeleteTokenRequestRequestTypeDef",
-    "EntitlementOutputTypeDef",
     "EntitlementUsageTypeDef",
     "ExtendLicenseConsumptionRequestRequestTypeDef",
-    "ExtendLicenseConsumptionResponseTypeDef",
     "FilterTypeDef",
     "GetAccessTokenRequestRequestTypeDef",
-    "GetAccessTokenResponseTypeDef",
     "GetGrantRequestRequestTypeDef",
     "GetLicenseConfigurationRequestRequestTypeDef",
     "ManagedResourceSummaryTypeDef",
-    "TagOutputTypeDef",
     "GetLicenseConversionTaskRequestRequestTypeDef",
-    "LicenseConversionContextOutputTypeDef",
     "GetLicenseManagerReportGeneratorRequestRequestTypeDef",
     "GetLicenseRequestRequestTypeDef",
     "GetLicenseUsageRequestRequestTypeDef",
-    "OrganizationConfigurationOutputTypeDef",
-    "OptionsOutputTypeDef",
+    "OrganizationConfigurationTypeDef",
     "IssuerDetailsTypeDef",
     "ReceivedMetadataTypeDef",
     "InventoryFilterTypeDef",
     "LicenseConfigurationAssociationTypeDef",
     "LicenseConfigurationUsageTypeDef",
-    "LicenseSpecificationOutputTypeDef",
     "LicenseSpecificationTypeDef",
-    "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     "ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
-    "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
     "ListLicenseSpecificationsForResourceRequestRequestTypeDef",
     "ListLicenseVersionsRequestRequestTypeDef",
     "ResourceInventoryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TokenDataTypeDef",
-    "OrganizationConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
     "ProductInformationFilterOutputTypeDef",
     "ProductInformationFilterTypeDef",
     "RejectGrantRequestRequestTypeDef",
-    "RejectGrantResponseTypeDef",
     "ReportContextOutputTypeDef",
-    "ReportFrequencyOutputTypeDef",
     "S3LocationTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AcceptGrantResponseTypeDef",
+    "CreateGrantResponseTypeDef",
+    "CreateGrantVersionResponseTypeDef",
+    "CreateLicenseConfigurationResponseTypeDef",
+    "CreateLicenseConversionTaskForResourceResponseTypeDef",
+    "CreateLicenseManagerReportGeneratorResponseTypeDef",
+    "CreateLicenseResponseTypeDef",
+    "CreateLicenseVersionResponseTypeDef",
+    "CreateTokenResponseTypeDef",
+    "DeleteGrantResponseTypeDef",
+    "DeleteLicenseResponseTypeDef",
+    "ExtendLicenseConsumptionResponseTypeDef",
+    "GetAccessTokenResponseTypeDef",
+    "RejectGrantResponseTypeDef",
     "CheckoutLicenseRequestRequestTypeDef",
-    "CheckoutBorrowLicenseRequestRequestTypeDef",
     "CheckoutLicenseResponseTypeDef",
+    "CheckoutBorrowLicenseRequestRequestTypeDef",
     "CheckoutBorrowLicenseResponseTypeDef",
     "LicenseOperationFailureTypeDef",
-    "ConsumptionConfigurationOutputTypeDef",
     "ConsumptionConfigurationTypeDef",
     "CreateGrantVersionRequestRequestTypeDef",
+    "GrantTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateLicenseConversionTaskForResourceRequestRequestTypeDef",
+    "GetLicenseConversionTaskResponseTypeDef",
+    "LicenseConversionTaskTypeDef",
     "CreateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "UpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "LicenseUsageTypeDef",
     "ListDistributedGrantsRequestRequestTypeDef",
-    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
     "ListLicenseConfigurationsRequestRequestTypeDef",
     "ListLicenseConversionTasksRequestRequestTypeDef",
     "ListLicenseManagerReportGeneratorsRequestRequestTypeDef",
     "ListLicensesRequestRequestTypeDef",
     "ListReceivedGrantsForOrganizationRequestRequestTypeDef",
     "ListReceivedGrantsRequestRequestTypeDef",
     "ListReceivedLicensesForOrganizationRequestRequestTypeDef",
     "ListReceivedLicensesRequestRequestTypeDef",
     "ListTokensRequestRequestTypeDef",
-    "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListUsageForLicenseConfigurationRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "GetLicenseConversionTaskResponseTypeDef",
-    "LicenseConversionTaskTypeDef",
     "GetServiceSettingsResponseTypeDef",
-    "GrantTypeDef",
-    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
+    "UpdateServiceSettingsRequestRequestTypeDef",
     "ListResourceInventoryRequestRequestTypeDef",
     "ListAssociationsForLicenseConfigurationResponseTypeDef",
     "ListUsageForLicenseConfigurationResponseTypeDef",
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     "UpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
+    "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
+    "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
+    "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListResourceInventoryResponseTypeDef",
     "ListTokensResponseTypeDef",
-    "UpdateServiceSettingsRequestRequestTypeDef",
     "ProductInformationOutputTypeDef",
     "ProductInformationTypeDef",
     "ReportGeneratorTypeDef",
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
-    "GrantedLicenseTypeDef",
-    "LicenseTypeDef",
     "CreateLicenseRequestRequestTypeDef",
     "CreateLicenseVersionRequestRequestTypeDef",
-    "GetLicenseUsageResponseTypeDef",
-    "ListLicenseConversionTasksResponseTypeDef",
+    "GrantedLicenseTypeDef",
+    "LicenseTypeDef",
     "GetGrantResponseTypeDef",
     "ListDistributedGrantsResponseTypeDef",
     "ListReceivedGrantsForOrganizationResponseTypeDef",
     "ListReceivedGrantsResponseTypeDef",
+    "ListLicenseConversionTasksResponseTypeDef",
+    "GetLicenseUsageResponseTypeDef",
     "GetLicenseConfigurationResponseTypeDef",
     "LicenseConfigurationTypeDef",
     "CreateLicenseConfigurationRequestRequestTypeDef",
     "UpdateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     "ListReceivedLicensesForOrganizationResponseTypeDef",
@@ -200,40 +187,33 @@
 AcceptGrantRequestRequestTypeDef = TypedDict(
     "AcceptGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 
-AcceptGrantResponseTypeDef = TypedDict(
-    "AcceptGrantResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AutomatedDiscoveryInformationTypeDef = TypedDict(
     "AutomatedDiscoveryInformationTypeDef",
     {
         "LastRunTime": datetime,
     },
     total=False,
 )
 
-BorrowConfigurationOutputTypeDef = TypedDict(
-    "BorrowConfigurationOutputTypeDef",
-    {
-        "AllowEarlyCheckIn": bool,
-        "MaxTimeToLiveInMinutes": int,
-    },
-)
-
 BorrowConfigurationTypeDef = TypedDict(
     "BorrowConfigurationTypeDef",
     {
         "AllowEarlyCheckIn": bool,
         "MaxTimeToLiveInMinutes": int,
     },
 )
@@ -280,59 +260,23 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredEntitlementDataOutputTypeDef = TypedDict(
-    "_RequiredEntitlementDataOutputTypeDef",
-    {
-        "Name": str,
-        "Unit": EntitlementDataUnitType,
-    },
-)
-_OptionalEntitlementDataOutputTypeDef = TypedDict(
-    "_OptionalEntitlementDataOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-class EntitlementDataOutputTypeDef(
-    _RequiredEntitlementDataOutputTypeDef, _OptionalEntitlementDataOutputTypeDef
-):
-    pass
-
-MetadataOutputTypeDef = TypedDict(
-    "MetadataOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 ConsumedLicenseSummaryTypeDef = TypedDict(
     "ConsumedLicenseSummaryTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "ConsumedLicenses": int,
     },
     total=False,
 )
 
-ProvisionalConfigurationOutputTypeDef = TypedDict(
-    "ProvisionalConfigurationOutputTypeDef",
-    {
-        "MaxTimeToLiveInMinutes": int,
-    },
-)
-
 ProvisionalConfigurationTypeDef = TypedDict(
     "ProvisionalConfigurationTypeDef",
     {
         "MaxTimeToLiveInMinutes": int,
     },
 )
 
@@ -344,75 +288,39 @@
         "LicenseArn": str,
         "Principals": Sequence[str],
         "HomeRegion": str,
         "AllowedOperations": Sequence[AllowedOperationType],
     },
 )
 
-CreateGrantResponseTypeDef = TypedDict(
-    "CreateGrantResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OptionsTypeDef = TypedDict(
     "OptionsTypeDef",
     {
         "ActivationOverrideBehavior": ActivationOverrideBehaviorType,
     },
     total=False,
 )
 
-CreateGrantVersionResponseTypeDef = TypedDict(
-    "CreateGrantVersionResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-CreateLicenseConfigurationResponseTypeDef = TypedDict(
-    "CreateLicenseConfigurationResponseTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LicenseConversionContextTypeDef = TypedDict(
     "LicenseConversionContextTypeDef",
     {
         "UsageOperation": str,
     },
     total=False,
 )
 
-CreateLicenseConversionTaskForResourceResponseTypeDef = TypedDict(
-    "CreateLicenseConversionTaskForResourceResponseTypeDef",
-    {
-        "LicenseConversionTaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReportContextTypeDef = TypedDict(
     "ReportContextTypeDef",
     {
         "licenseConfigurationArns": Sequence[str],
     },
 )
 
@@ -421,22 +329,14 @@
     {
         "value": int,
         "period": ReportFrequencyTypeType,
     },
     total=False,
 )
 
-CreateLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
-    "CreateLicenseManagerReportGeneratorResponseTypeDef",
-    {
-        "LicenseManagerReportGeneratorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDatetimeRangeTypeDef = TypedDict(
     "_RequiredDatetimeRangeTypeDef",
     {
         "Begin": str,
     },
 )
 _OptionalDatetimeRangeTypeDef = TypedDict(
@@ -484,34 +384,14 @@
     },
     total=False,
 )
 
 class IssuerTypeDef(_RequiredIssuerTypeDef, _OptionalIssuerTypeDef):
     pass
 
-CreateLicenseResponseTypeDef = TypedDict(
-    "CreateLicenseResponseTypeDef",
-    {
-        "LicenseArn": str,
-        "Status": LicenseStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateLicenseVersionResponseTypeDef = TypedDict(
-    "CreateLicenseVersionResponseTypeDef",
-    {
-        "LicenseArn": str,
-        "Version": str,
-        "Status": LicenseStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTokenRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "ClientToken": str,
     },
 )
@@ -526,43 +406,14 @@
 )
 
 class CreateTokenRequestRequestTypeDef(
     _RequiredCreateTokenRequestRequestTypeDef, _OptionalCreateTokenRequestRequestTypeDef
 ):
     pass
 
-CreateTokenResponseTypeDef = TypedDict(
-    "CreateTokenResponseTypeDef",
-    {
-        "TokenId": str,
-        "TokenType": Literal["REFRESH_TOKEN"],
-        "Token": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDatetimeRangeOutputTypeDef = TypedDict(
-    "_RequiredDatetimeRangeOutputTypeDef",
-    {
-        "Begin": str,
-    },
-)
-_OptionalDatetimeRangeOutputTypeDef = TypedDict(
-    "_OptionalDatetimeRangeOutputTypeDef",
-    {
-        "End": str,
-    },
-    total=False,
-)
-
-class DatetimeRangeOutputTypeDef(
-    _RequiredDatetimeRangeOutputTypeDef, _OptionalDatetimeRangeOutputTypeDef
-):
-    pass
-
 _RequiredDeleteGrantRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
         "Version": str,
     },
 )
@@ -575,24 +426,14 @@
 )
 
 class DeleteGrantRequestRequestTypeDef(
     _RequiredDeleteGrantRequestRequestTypeDef, _OptionalDeleteGrantRequestRequestTypeDef
 ):
     pass
 
-DeleteGrantResponseTypeDef = TypedDict(
-    "DeleteGrantResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 
@@ -607,53 +448,21 @@
     "DeleteLicenseRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "SourceVersion": str,
     },
 )
 
-DeleteLicenseResponseTypeDef = TypedDict(
-    "DeleteLicenseResponseTypeDef",
-    {
-        "Status": LicenseDeletionStatusType,
-        "DeletionDate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTokenRequestRequestTypeDef = TypedDict(
     "DeleteTokenRequestRequestTypeDef",
     {
         "TokenId": str,
     },
 )
 
-_RequiredEntitlementOutputTypeDef = TypedDict(
-    "_RequiredEntitlementOutputTypeDef",
-    {
-        "Name": str,
-        "Unit": EntitlementUnitType,
-    },
-)
-_OptionalEntitlementOutputTypeDef = TypedDict(
-    "_OptionalEntitlementOutputTypeDef",
-    {
-        "Value": str,
-        "MaxCount": int,
-        "Overage": bool,
-        "AllowCheckIn": bool,
-    },
-    total=False,
-)
-
-class EntitlementOutputTypeDef(
-    _RequiredEntitlementOutputTypeDef, _OptionalEntitlementOutputTypeDef
-):
-    pass
-
 _RequiredEntitlementUsageTypeDef = TypedDict(
     "_RequiredEntitlementUsageTypeDef",
     {
         "Name": str,
         "ConsumedValue": str,
         "Unit": EntitlementDataUnitType,
     },
@@ -685,23 +494,14 @@
 
 class ExtendLicenseConsumptionRequestRequestTypeDef(
     _RequiredExtendLicenseConsumptionRequestRequestTypeDef,
     _OptionalExtendLicenseConsumptionRequestRequestTypeDef,
 ):
     pass
 
-ExtendLicenseConsumptionResponseTypeDef = TypedDict(
-    "ExtendLicenseConsumptionResponseTypeDef",
-    {
-        "LicenseConsumptionToken": str,
-        "Expiration": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -722,22 +522,14 @@
 )
 
 class GetAccessTokenRequestRequestTypeDef(
     _RequiredGetAccessTokenRequestRequestTypeDef, _OptionalGetAccessTokenRequestRequestTypeDef
 ):
     pass
 
-GetAccessTokenResponseTypeDef = TypedDict(
-    "GetAccessTokenResponseTypeDef",
-    {
-        "AccessToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetGrantRequestRequestTypeDef = TypedDict(
     "_RequiredGetGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 _OptionalGetGrantRequestRequestTypeDef = TypedDict(
@@ -765,38 +557,21 @@
     {
         "ResourceType": ResourceTypeType,
         "AssociationCount": int,
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
 GetLicenseConversionTaskRequestRequestTypeDef = TypedDict(
     "GetLicenseConversionTaskRequestRequestTypeDef",
     {
         "LicenseConversionTaskId": str,
     },
 )
 
-LicenseConversionContextOutputTypeDef = TypedDict(
-    "LicenseConversionContextOutputTypeDef",
-    {
-        "UsageOperation": str,
-    },
-    total=False,
-)
-
 GetLicenseManagerReportGeneratorRequestRequestTypeDef = TypedDict(
     "GetLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "LicenseManagerReportGeneratorArn": str,
     },
 )
 
@@ -822,29 +597,21 @@
 GetLicenseUsageRequestRequestTypeDef = TypedDict(
     "GetLicenseUsageRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 
-OrganizationConfigurationOutputTypeDef = TypedDict(
-    "OrganizationConfigurationOutputTypeDef",
+OrganizationConfigurationTypeDef = TypedDict(
+    "OrganizationConfigurationTypeDef",
     {
         "EnableIntegration": bool,
     },
 )
 
-OptionsOutputTypeDef = TypedDict(
-    "OptionsOutputTypeDef",
-    {
-        "ActivationOverrideBehavior": ActivationOverrideBehaviorType,
-    },
-    total=False,
-)
-
 IssuerDetailsTypeDef = TypedDict(
     "IssuerDetailsTypeDef",
     {
         "Name": str,
         "SignKey": str,
         "KeyFingerprint": str,
     },
@@ -900,33 +667,14 @@
         "ResourceOwnerId": str,
         "AssociationTime": datetime,
         "ConsumedLicenses": int,
     },
     total=False,
 )
 
-_RequiredLicenseSpecificationOutputTypeDef = TypedDict(
-    "_RequiredLicenseSpecificationOutputTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalLicenseSpecificationOutputTypeDef = TypedDict(
-    "_OptionalLicenseSpecificationOutputTypeDef",
-    {
-        "AmiAssociationScope": str,
-    },
-    total=False,
-)
-
-class LicenseSpecificationOutputTypeDef(
-    _RequiredLicenseSpecificationOutputTypeDef, _OptionalLicenseSpecificationOutputTypeDef
-):
-    pass
-
 _RequiredLicenseSpecificationTypeDef = TypedDict(
     "_RequiredLicenseSpecificationTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalLicenseSpecificationTypeDef = TypedDict(
@@ -938,34 +686,24 @@
 )
 
 class LicenseSpecificationTypeDef(
     _RequiredLicenseSpecificationTypeDef, _OptionalLicenseSpecificationTypeDef
 ):
     pass
 
-_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
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
 
-class ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef(
-    _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
-    _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListAssociationsForLicenseConfigurationRequestRequestTypeDef = TypedDict(
@@ -1000,34 +738,14 @@
 
 class ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef(
     _RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
     _OptionalListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef(
-    _RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
-    _OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
@@ -1096,31 +814,14 @@
         "TokenProperties": List[str],
         "RoleArns": List[str],
         "Status": str,
     },
     total=False,
 )
 
-OrganizationConfigurationTypeDef = TypedDict(
-    "OrganizationConfigurationTypeDef",
-    {
-        "EnableIntegration": bool,
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
 _RequiredProductInformationFilterOutputTypeDef = TypedDict(
     "_RequiredProductInformationFilterOutputTypeDef",
     {
         "ProductInformationFilterName": str,
         "ProductInformationFilterComparator": str,
     },
 )
@@ -1160,65 +861,165 @@
 RejectGrantRequestRequestTypeDef = TypedDict(
     "RejectGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 
-RejectGrantResponseTypeDef = TypedDict(
-    "RejectGrantResponseTypeDef",
+ReportContextOutputTypeDef = TypedDict(
+    "ReportContextOutputTypeDef",
+    {
+        "licenseConfigurationArns": List[str],
+    },
+)
+
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
+    {
+        "bucket": str,
+        "keyPrefix": str,
+    },
+    total=False,
+)
+
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
+    },
+)
+
+AcceptGrantResponseTypeDef = TypedDict(
+    "AcceptGrantResponseTypeDef",
     {
         "GrantArn": str,
         "Status": GrantStatusType,
         "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReportContextOutputTypeDef = TypedDict(
-    "ReportContextOutputTypeDef",
+CreateGrantResponseTypeDef = TypedDict(
+    "CreateGrantResponseTypeDef",
     {
-        "licenseConfigurationArns": List[str],
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReportFrequencyOutputTypeDef = TypedDict(
-    "ReportFrequencyOutputTypeDef",
+CreateGrantVersionResponseTypeDef = TypedDict(
+    "CreateGrantVersionResponseTypeDef",
     {
-        "value": int,
-        "period": ReportFrequencyTypeType,
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
+CreateLicenseConfigurationResponseTypeDef = TypedDict(
+    "CreateLicenseConfigurationResponseTypeDef",
     {
-        "bucket": str,
-        "keyPrefix": str,
+        "LicenseConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateLicenseConversionTaskForResourceResponseTypeDef = TypedDict(
+    "CreateLicenseConversionTaskForResourceResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "LicenseConversionTaskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+CreateLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
+    "CreateLicenseManagerReportGeneratorResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "LicenseManagerReportGeneratorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLicenseResponseTypeDef = TypedDict(
+    "CreateLicenseResponseTypeDef",
+    {
+        "LicenseArn": str,
+        "Status": LicenseStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLicenseVersionResponseTypeDef = TypedDict(
+    "CreateLicenseVersionResponseTypeDef",
+    {
+        "LicenseArn": str,
+        "Version": str,
+        "Status": LicenseStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTokenResponseTypeDef = TypedDict(
+    "CreateTokenResponseTypeDef",
+    {
+        "TokenId": str,
+        "TokenType": Literal["REFRESH_TOKEN"],
+        "Token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteGrantResponseTypeDef = TypedDict(
+    "DeleteGrantResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteLicenseResponseTypeDef = TypedDict(
+    "DeleteLicenseResponseTypeDef",
+    {
+        "Status": LicenseDeletionStatusType,
+        "DeletionDate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExtendLicenseConsumptionResponseTypeDef = TypedDict(
+    "ExtendLicenseConsumptionResponseTypeDef",
+    {
+        "LicenseConsumptionToken": str,
+        "Expiration": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccessTokenResponseTypeDef = TypedDict(
+    "GetAccessTokenResponseTypeDef",
+    {
+        "AccessToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RejectGrantResponseTypeDef = TypedDict(
+    "RejectGrantResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCheckoutLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCheckoutLicenseRequestRequestTypeDef",
     {
         "ProductSKU": str,
@@ -1238,14 +1039,29 @@
 )
 
 class CheckoutLicenseRequestRequestTypeDef(
     _RequiredCheckoutLicenseRequestRequestTypeDef, _OptionalCheckoutLicenseRequestRequestTypeDef
 ):
     pass
 
+CheckoutLicenseResponseTypeDef = TypedDict(
+    "CheckoutLicenseResponseTypeDef",
+    {
+        "CheckoutType": CheckoutTypeType,
+        "LicenseConsumptionToken": str,
+        "EntitlementsAllowed": List[EntitlementDataTypeDef],
+        "SignedToken": str,
+        "NodeId": str,
+        "IssuedAt": str,
+        "Expiration": str,
+        "LicenseArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCheckoutBorrowLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCheckoutBorrowLicenseRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "Entitlements": Sequence[EntitlementDataTypeDef],
         "DigitalSignatureMethod": Literal["JWT_PS384"],
         "ClientToken": str,
@@ -1262,65 +1078,40 @@
 
 class CheckoutBorrowLicenseRequestRequestTypeDef(
     _RequiredCheckoutBorrowLicenseRequestRequestTypeDef,
     _OptionalCheckoutBorrowLicenseRequestRequestTypeDef,
 ):
     pass
 
-CheckoutLicenseResponseTypeDef = TypedDict(
-    "CheckoutLicenseResponseTypeDef",
-    {
-        "CheckoutType": CheckoutTypeType,
-        "LicenseConsumptionToken": str,
-        "EntitlementsAllowed": List[EntitlementDataOutputTypeDef],
-        "SignedToken": str,
-        "NodeId": str,
-        "IssuedAt": str,
-        "Expiration": str,
-        "LicenseArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CheckoutBorrowLicenseResponseTypeDef = TypedDict(
     "CheckoutBorrowLicenseResponseTypeDef",
     {
         "LicenseArn": str,
         "LicenseConsumptionToken": str,
-        "EntitlementsAllowed": List[EntitlementDataOutputTypeDef],
+        "EntitlementsAllowed": List[EntitlementDataTypeDef],
         "NodeId": str,
         "SignedToken": str,
         "IssuedAt": str,
         "Expiration": str,
-        "CheckoutMetadata": List[MetadataOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CheckoutMetadata": List[MetadataTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LicenseOperationFailureTypeDef = TypedDict(
     "LicenseOperationFailureTypeDef",
     {
         "ResourceArn": str,
         "ResourceType": ResourceTypeType,
         "ErrorMessage": str,
         "FailureTime": datetime,
         "OperationName": str,
         "ResourceOwnerId": str,
         "OperationRequestedBy": str,
-        "MetadataList": List[MetadataOutputTypeDef],
-    },
-    total=False,
-)
-
-ConsumptionConfigurationOutputTypeDef = TypedDict(
-    "ConsumptionConfigurationOutputTypeDef",
-    {
-        "RenewType": RenewTypeType,
-        "ProvisionalConfiguration": ProvisionalConfigurationOutputTypeDef,
-        "BorrowConfiguration": BorrowConfigurationOutputTypeDef,
+        "MetadataList": List[MetadataTypeDef],
     },
     total=False,
 )
 
 ConsumptionConfigurationTypeDef = TypedDict(
     "ConsumptionConfigurationTypeDef",
     {
@@ -1353,14 +1144,48 @@
 
 class CreateGrantVersionRequestRequestTypeDef(
     _RequiredCreateGrantVersionRequestRequestTypeDef,
     _OptionalCreateGrantVersionRequestRequestTypeDef,
 ):
     pass
 
+_RequiredGrantTypeDef = TypedDict(
+    "_RequiredGrantTypeDef",
+    {
+        "GrantArn": str,
+        "GrantName": str,
+        "ParentArn": str,
+        "LicenseArn": str,
+        "GranteePrincipalArn": str,
+        "HomeRegion": str,
+        "GrantStatus": GrantStatusType,
+        "Version": str,
+        "GrantedOperations": List[AllowedOperationType],
+    },
+)
+_OptionalGrantTypeDef = TypedDict(
+    "_OptionalGrantTypeDef",
+    {
+        "StatusReason": str,
+        "Options": OptionsTypeDef,
+    },
+    total=False,
+)
+
+class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
+    pass
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1370,14 +1195,46 @@
     {
         "ResourceArn": str,
         "SourceLicenseContext": LicenseConversionContextTypeDef,
         "DestinationLicenseContext": LicenseConversionContextTypeDef,
     },
 )
 
+GetLicenseConversionTaskResponseTypeDef = TypedDict(
+    "GetLicenseConversionTaskResponseTypeDef",
+    {
+        "LicenseConversionTaskId": str,
+        "ResourceArn": str,
+        "SourceLicenseContext": LicenseConversionContextTypeDef,
+        "DestinationLicenseContext": LicenseConversionContextTypeDef,
+        "StatusMessage": str,
+        "Status": LicenseConversionTaskStatusType,
+        "StartTime": datetime,
+        "LicenseConversionTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LicenseConversionTaskTypeDef = TypedDict(
+    "LicenseConversionTaskTypeDef",
+    {
+        "LicenseConversionTaskId": str,
+        "ResourceArn": str,
+        "SourceLicenseContext": LicenseConversionContextTypeDef,
+        "DestinationLicenseContext": LicenseConversionContextTypeDef,
+        "Status": LicenseConversionTaskStatusType,
+        "StatusMessage": str,
+        "StartTime": datetime,
+        "LicenseConversionTime": datetime,
+        "EndTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredCreateLicenseManagerReportGeneratorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "ReportGeneratorName": str,
         "Type": Sequence[ReportTypeType],
         "ReportContext": ReportContextTypeDef,
         "ReportFrequency": ReportFrequencyTypeDef,
@@ -1439,24 +1296,14 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef = TypedDict(
-    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
-    {
-        "LicenseConfigurationArns": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLicenseConfigurationsRequestRequestTypeDef = TypedDict(
     "ListLicenseConfigurationsRequestRequestTypeDef",
     {
         "LicenseConfigurationArns": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
@@ -1556,35 +1403,14 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef(
-    _RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
-    _OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
-):
-    pass
-
 _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredListUsageForLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
@@ -1599,97 +1425,33 @@
 
 class ListUsageForLicenseConfigurationRequestRequestTypeDef(
     _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef,
     _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetLicenseConversionTaskResponseTypeDef = TypedDict(
-    "GetLicenseConversionTaskResponseTypeDef",
-    {
-        "LicenseConversionTaskId": str,
-        "ResourceArn": str,
-        "SourceLicenseContext": LicenseConversionContextOutputTypeDef,
-        "DestinationLicenseContext": LicenseConversionContextOutputTypeDef,
-        "StatusMessage": str,
-        "Status": LicenseConversionTaskStatusType,
-        "StartTime": datetime,
-        "LicenseConversionTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LicenseConversionTaskTypeDef = TypedDict(
-    "LicenseConversionTaskTypeDef",
-    {
-        "LicenseConversionTaskId": str,
-        "ResourceArn": str,
-        "SourceLicenseContext": LicenseConversionContextOutputTypeDef,
-        "DestinationLicenseContext": LicenseConversionContextOutputTypeDef,
-        "Status": LicenseConversionTaskStatusType,
-        "StatusMessage": str,
-        "StartTime": datetime,
-        "LicenseConversionTime": datetime,
-        "EndTime": datetime,
-    },
-    total=False,
-)
-
 GetServiceSettingsResponseTypeDef = TypedDict(
     "GetServiceSettingsResponseTypeDef",
     {
         "S3BucketArn": str,
         "SnsTopicArn": str,
-        "OrganizationConfiguration": OrganizationConfigurationOutputTypeDef,
+        "OrganizationConfiguration": OrganizationConfigurationTypeDef,
         "EnableCrossAccountsDiscovery": bool,
         "LicenseManagerResourceShareArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGrantTypeDef = TypedDict(
-    "_RequiredGrantTypeDef",
-    {
-        "GrantArn": str,
-        "GrantName": str,
-        "ParentArn": str,
-        "LicenseArn": str,
-        "GranteePrincipalArn": str,
-        "HomeRegion": str,
-        "GrantStatus": GrantStatusType,
-        "Version": str,
-        "GrantedOperations": List[AllowedOperationType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalGrantTypeDef = TypedDict(
-    "_OptionalGrantTypeDef",
-    {
-        "StatusReason": str,
-        "Options": OptionsOutputTypeDef,
-    },
-    total=False,
-)
 
-class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
-    pass
-
-ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
-    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
+UpdateServiceSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateServiceSettingsRequestRequestTypeDef",
     {
-        "Filters": Sequence[InventoryFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "S3BucketArn": str,
+        "SnsTopicArn": str,
+        "OrganizationConfiguration": OrganizationConfigurationTypeDef,
+        "EnableCrossAccountsDiscovery": bool,
     },
     total=False,
 )
 
 ListResourceInventoryRequestRequestTypeDef = TypedDict(
     "ListResourceInventoryRequestRequestTypeDef",
     {
@@ -1701,33 +1463,33 @@
 )
 
 ListAssociationsForLicenseConfigurationResponseTypeDef = TypedDict(
     "ListAssociationsForLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationAssociations": List[LicenseConfigurationAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsageForLicenseConfigurationResponseTypeDef = TypedDict(
     "ListUsageForLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationUsageList": List[LicenseConfigurationUsageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseSpecificationsForResourceResponseTypeDef = TypedDict(
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     {
-        "LicenseSpecifications": List[LicenseSpecificationOutputTypeDef],
+        "LicenseSpecifications": List[LicenseSpecificationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1744,41 +1506,110 @@
 
 class UpdateLicenseSpecificationsForResourceRequestRequestTypeDef(
     _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
     _OptionalUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef(
+    _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+):
+    pass
+
+ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef = TypedDict(
+    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
+    {
+        "LicenseConfigurationArns": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef(
+    _RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+    _OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+):
+    pass
+
+ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
+    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
+    {
+        "Filters": Sequence[InventoryFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef(
+    _RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
+    _OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
+):
+    pass
+
 ListResourceInventoryResponseTypeDef = TypedDict(
     "ListResourceInventoryResponseTypeDef",
     {
         "ResourceInventoryList": List[ResourceInventoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTokensResponseTypeDef = TypedDict(
     "ListTokensResponseTypeDef",
     {
         "Tokens": List[TokenDataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateServiceSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateServiceSettingsRequestRequestTypeDef",
-    {
-        "S3BucketArn": str,
-        "SnsTopicArn": str,
-        "OrganizationConfiguration": OrganizationConfigurationTypeDef,
-        "EnableCrossAccountsDiscovery": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ProductInformationOutputTypeDef = TypedDict(
     "ProductInformationOutputTypeDef",
     {
         "ResourceType": str,
         "ProductInformationFilterList": List[ProductInformationFilterOutputTypeDef],
@@ -1795,78 +1626,35 @@
 
 ReportGeneratorTypeDef = TypedDict(
     "ReportGeneratorTypeDef",
     {
         "ReportGeneratorName": str,
         "ReportType": List[ReportTypeType],
         "ReportContext": ReportContextOutputTypeDef,
-        "ReportFrequency": ReportFrequencyOutputTypeDef,
+        "ReportFrequency": ReportFrequencyTypeDef,
         "LicenseManagerReportGeneratorArn": str,
         "LastRunStatus": str,
         "LastRunFailureReason": str,
         "LastReportGenerationTime": str,
         "ReportCreatorAccount": str,
         "Description": str,
         "S3Location": S3LocationTypeDef,
         "CreateTime": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 ListFailuresForLicenseConfigurationOperationsResponseTypeDef = TypedDict(
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     {
         "LicenseOperationFailureList": List[LicenseOperationFailureTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GrantedLicenseTypeDef = TypedDict(
-    "GrantedLicenseTypeDef",
-    {
-        "LicenseArn": str,
-        "LicenseName": str,
-        "ProductName": str,
-        "ProductSKU": str,
-        "Issuer": IssuerDetailsTypeDef,
-        "HomeRegion": str,
-        "Status": LicenseStatusType,
-        "Validity": DatetimeRangeOutputTypeDef,
-        "Beneficiary": str,
-        "Entitlements": List[EntitlementOutputTypeDef],
-        "ConsumptionConfiguration": ConsumptionConfigurationOutputTypeDef,
-        "LicenseMetadata": List[MetadataOutputTypeDef],
-        "CreateTime": str,
-        "Version": str,
-        "ReceivedMetadata": ReceivedMetadataTypeDef,
-    },
-    total=False,
-)
-
-LicenseTypeDef = TypedDict(
-    "LicenseTypeDef",
-    {
-        "LicenseArn": str,
-        "LicenseName": str,
-        "ProductName": str,
-        "ProductSKU": str,
-        "Issuer": IssuerDetailsTypeDef,
-        "HomeRegion": str,
-        "Status": LicenseStatusType,
-        "Validity": DatetimeRangeOutputTypeDef,
-        "Beneficiary": str,
-        "Entitlements": List[EntitlementOutputTypeDef],
-        "ConsumptionConfiguration": ConsumptionConfigurationOutputTypeDef,
-        "LicenseMetadata": List[MetadataOutputTypeDef],
-        "CreateTime": str,
-        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseRequestRequestTypeDef",
     {
         "LicenseName": str,
         "ProductName": str,
@@ -1919,63 +1707,106 @@
 
 class CreateLicenseVersionRequestRequestTypeDef(
     _RequiredCreateLicenseVersionRequestRequestTypeDef,
     _OptionalCreateLicenseVersionRequestRequestTypeDef,
 ):
     pass
 
-GetLicenseUsageResponseTypeDef = TypedDict(
-    "GetLicenseUsageResponseTypeDef",
+GrantedLicenseTypeDef = TypedDict(
+    "GrantedLicenseTypeDef",
     {
-        "LicenseUsage": LicenseUsageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LicenseArn": str,
+        "LicenseName": str,
+        "ProductName": str,
+        "ProductSKU": str,
+        "Issuer": IssuerDetailsTypeDef,
+        "HomeRegion": str,
+        "Status": LicenseStatusType,
+        "Validity": DatetimeRangeTypeDef,
+        "Beneficiary": str,
+        "Entitlements": List[EntitlementTypeDef],
+        "ConsumptionConfiguration": ConsumptionConfigurationTypeDef,
+        "LicenseMetadata": List[MetadataTypeDef],
+        "CreateTime": str,
+        "Version": str,
+        "ReceivedMetadata": ReceivedMetadataTypeDef,
     },
+    total=False,
 )
 
-ListLicenseConversionTasksResponseTypeDef = TypedDict(
-    "ListLicenseConversionTasksResponseTypeDef",
+LicenseTypeDef = TypedDict(
+    "LicenseTypeDef",
     {
-        "LicenseConversionTasks": List[LicenseConversionTaskTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LicenseArn": str,
+        "LicenseName": str,
+        "ProductName": str,
+        "ProductSKU": str,
+        "Issuer": IssuerDetailsTypeDef,
+        "HomeRegion": str,
+        "Status": LicenseStatusType,
+        "Validity": DatetimeRangeTypeDef,
+        "Beneficiary": str,
+        "Entitlements": List[EntitlementTypeDef],
+        "ConsumptionConfiguration": ConsumptionConfigurationTypeDef,
+        "LicenseMetadata": List[MetadataTypeDef],
+        "CreateTime": str,
+        "Version": str,
     },
+    total=False,
 )
 
 GetGrantResponseTypeDef = TypedDict(
     "GetGrantResponseTypeDef",
     {
         "Grant": GrantTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributedGrantsResponseTypeDef = TypedDict(
     "ListDistributedGrantsResponseTypeDef",
     {
         "Grants": List[GrantTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedGrantsForOrganizationResponseTypeDef = TypedDict(
     "ListReceivedGrantsForOrganizationResponseTypeDef",
     {
         "Grants": List[GrantTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedGrantsResponseTypeDef = TypedDict(
     "ListReceivedGrantsResponseTypeDef",
     {
         "Grants": List[GrantTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListLicenseConversionTasksResponseTypeDef = TypedDict(
+    "ListLicenseConversionTasksResponseTypeDef",
+    {
+        "LicenseConversionTasks": List[LicenseConversionTaskTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLicenseUsageResponseTypeDef = TypedDict(
+    "GetLicenseUsageResponseTypeDef",
+    {
+        "LicenseUsage": LicenseUsageTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLicenseConfigurationResponseTypeDef = TypedDict(
     "GetLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationId": str,
@@ -1987,19 +1818,19 @@
         "LicenseCount": int,
         "LicenseCountHardLimit": bool,
         "ConsumedLicenses": int,
         "Status": str,
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ProductInformationList": List[ProductInformationOutputTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
         "DisassociateWhenNotFound": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LicenseConfigurationTypeDef = TypedDict(
     "LicenseConfigurationTypeDef",
     {
         "LicenseConfigurationId": str,
@@ -2076,72 +1907,72 @@
 ):
     pass
 
 GetLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     {
         "ReportGenerator": ReportGeneratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseManagerReportGeneratorsResponseTypeDef = TypedDict(
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     {
         "ReportGenerators": List[ReportGeneratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedLicensesForOrganizationResponseTypeDef = TypedDict(
     "ListReceivedLicensesForOrganizationResponseTypeDef",
     {
         "Licenses": List[GrantedLicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedLicensesResponseTypeDef = TypedDict(
     "ListReceivedLicensesResponseTypeDef",
     {
         "Licenses": List[GrantedLicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLicenseResponseTypeDef = TypedDict(
     "GetLicenseResponseTypeDef",
     {
         "License": LicenseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseVersionsResponseTypeDef = TypedDict(
     "ListLicenseVersionsResponseTypeDef",
     {
         "Licenses": List[LicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicensesResponseTypeDef = TypedDict(
     "ListLicensesResponseTypeDef",
     {
         "Licenses": List[LicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseConfigurationsResponseTypeDef = TypedDict(
     "ListLicenseConfigurationsResponseTypeDef",
     {
         "LicenseConfigurations": List[LicenseConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/PKG-INFO` & `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager
-Version: 1.28.12
-Summary: Type annotations for boto3.LicenseManager 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LicenseManager 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager)](https://pepy.tech/project/mypy-boto3-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManager 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[boto3.LicenseManager 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [mypy-boto3-license-manager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,151 +364,138 @@
 
 `mypy_boto3_license_manager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_license_manager.type_defs import (
     AcceptGrantRequestRequestTypeDef,
-    AcceptGrantResponseTypeDef,
+    ResponseMetadataTypeDef,
     AutomatedDiscoveryInformationTypeDef,
-    BorrowConfigurationOutputTypeDef,
     BorrowConfigurationTypeDef,
     CheckInLicenseRequestRequestTypeDef,
     EntitlementDataTypeDef,
     MetadataTypeDef,
-    EntitlementDataOutputTypeDef,
-    MetadataOutputTypeDef,
     ConsumedLicenseSummaryTypeDef,
-    ProvisionalConfigurationOutputTypeDef,
     ProvisionalConfigurationTypeDef,
     CreateGrantRequestRequestTypeDef,
-    CreateGrantResponseTypeDef,
     OptionsTypeDef,
-    CreateGrantVersionResponseTypeDef,
     TagTypeDef,
-    CreateLicenseConfigurationResponseTypeDef,
     LicenseConversionContextTypeDef,
-    CreateLicenseConversionTaskForResourceResponseTypeDef,
     ReportContextTypeDef,
     ReportFrequencyTypeDef,
-    CreateLicenseManagerReportGeneratorResponseTypeDef,
     DatetimeRangeTypeDef,
     EntitlementTypeDef,
     IssuerTypeDef,
-    CreateLicenseResponseTypeDef,
-    CreateLicenseVersionResponseTypeDef,
     CreateTokenRequestRequestTypeDef,
-    CreateTokenResponseTypeDef,
-    DatetimeRangeOutputTypeDef,
     DeleteGrantRequestRequestTypeDef,
-    DeleteGrantResponseTypeDef,
     DeleteLicenseConfigurationRequestRequestTypeDef,
     DeleteLicenseManagerReportGeneratorRequestRequestTypeDef,
     DeleteLicenseRequestRequestTypeDef,
-    DeleteLicenseResponseTypeDef,
     DeleteTokenRequestRequestTypeDef,
-    EntitlementOutputTypeDef,
     EntitlementUsageTypeDef,
     ExtendLicenseConsumptionRequestRequestTypeDef,
-    ExtendLicenseConsumptionResponseTypeDef,
     FilterTypeDef,
     GetAccessTokenRequestRequestTypeDef,
-    GetAccessTokenResponseTypeDef,
     GetGrantRequestRequestTypeDef,
     GetLicenseConfigurationRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
-    TagOutputTypeDef,
     GetLicenseConversionTaskRequestRequestTypeDef,
-    LicenseConversionContextOutputTypeDef,
     GetLicenseManagerReportGeneratorRequestRequestTypeDef,
     GetLicenseRequestRequestTypeDef,
     GetLicenseUsageRequestRequestTypeDef,
-    OrganizationConfigurationOutputTypeDef,
-    OptionsOutputTypeDef,
+    OrganizationConfigurationTypeDef,
     IssuerDetailsTypeDef,
     ReceivedMetadataTypeDef,
     InventoryFilterTypeDef,
     LicenseConfigurationAssociationTypeDef,
     LicenseConfigurationUsageTypeDef,
-    LicenseSpecificationOutputTypeDef,
     LicenseSpecificationTypeDef,
-    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
-    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     ListLicenseSpecificationsForResourceRequestRequestTypeDef,
     ListLicenseVersionsRequestRequestTypeDef,
     ResourceInventoryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TokenDataTypeDef,
-    OrganizationConfigurationTypeDef,
-    PaginatorConfigTypeDef,
     ProductInformationFilterOutputTypeDef,
     ProductInformationFilterTypeDef,
     RejectGrantRequestRequestTypeDef,
-    RejectGrantResponseTypeDef,
     ReportContextOutputTypeDef,
-    ReportFrequencyOutputTypeDef,
     S3LocationTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AcceptGrantResponseTypeDef,
+    CreateGrantResponseTypeDef,
+    CreateGrantVersionResponseTypeDef,
+    CreateLicenseConfigurationResponseTypeDef,
+    CreateLicenseConversionTaskForResourceResponseTypeDef,
+    CreateLicenseManagerReportGeneratorResponseTypeDef,
+    CreateLicenseResponseTypeDef,
+    CreateLicenseVersionResponseTypeDef,
+    CreateTokenResponseTypeDef,
+    DeleteGrantResponseTypeDef,
+    DeleteLicenseResponseTypeDef,
+    ExtendLicenseConsumptionResponseTypeDef,
+    GetAccessTokenResponseTypeDef,
+    RejectGrantResponseTypeDef,
     CheckoutLicenseRequestRequestTypeDef,
-    CheckoutBorrowLicenseRequestRequestTypeDef,
     CheckoutLicenseResponseTypeDef,
+    CheckoutBorrowLicenseRequestRequestTypeDef,
     CheckoutBorrowLicenseResponseTypeDef,
     LicenseOperationFailureTypeDef,
-    ConsumptionConfigurationOutputTypeDef,
     ConsumptionConfigurationTypeDef,
     CreateGrantVersionRequestRequestTypeDef,
+    GrantTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateLicenseConversionTaskForResourceRequestRequestTypeDef,
+    GetLicenseConversionTaskResponseTypeDef,
+    LicenseConversionTaskTypeDef,
     CreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     UpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     LicenseUsageTypeDef,
     ListDistributedGrantsRequestRequestTypeDef,
-    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
     ListLicenseConfigurationsRequestRequestTypeDef,
     ListLicenseConversionTasksRequestRequestTypeDef,
     ListLicenseManagerReportGeneratorsRequestRequestTypeDef,
     ListLicensesRequestRequestTypeDef,
     ListReceivedGrantsForOrganizationRequestRequestTypeDef,
     ListReceivedGrantsRequestRequestTypeDef,
     ListReceivedLicensesForOrganizationRequestRequestTypeDef,
     ListReceivedLicensesRequestRequestTypeDef,
     ListTokensRequestRequestTypeDef,
-    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListUsageForLicenseConfigurationRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GetLicenseConversionTaskResponseTypeDef,
-    LicenseConversionTaskTypeDef,
     GetServiceSettingsResponseTypeDef,
-    GrantTypeDef,
-    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
+    UpdateServiceSettingsRequestRequestTypeDef,
     ListResourceInventoryRequestRequestTypeDef,
     ListAssociationsForLicenseConfigurationResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     ListLicenseSpecificationsForResourceResponseTypeDef,
     UpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
+    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
+    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
+    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTokensResponseTypeDef,
-    UpdateServiceSettingsRequestRequestTypeDef,
     ProductInformationOutputTypeDef,
     ProductInformationTypeDef,
     ReportGeneratorTypeDef,
     ListFailuresForLicenseConfigurationOperationsResponseTypeDef,
-    GrantedLicenseTypeDef,
-    LicenseTypeDef,
     CreateLicenseRequestRequestTypeDef,
     CreateLicenseVersionRequestRequestTypeDef,
-    GetLicenseUsageResponseTypeDef,
-    ListLicenseConversionTasksResponseTypeDef,
+    GrantedLicenseTypeDef,
+    LicenseTypeDef,
     GetGrantResponseTypeDef,
     ListDistributedGrantsResponseTypeDef,
     ListReceivedGrantsForOrganizationResponseTypeDef,
     ListReceivedGrantsResponseTypeDef,
+    ListLicenseConversionTasksResponseTypeDef,
+    GetLicenseUsageResponseTypeDef,
     GetLicenseConfigurationResponseTypeDef,
     LicenseConfigurationTypeDef,
     CreateLicenseConfigurationRequestRequestTypeDef,
     UpdateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseManagerReportGeneratorResponseTypeDef,
     ListLicenseManagerReportGeneratorsResponseTypeDef,
     ListReceivedLicensesForOrganizationResponseTypeDef,
```

### Comparing `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/SOURCES.txt` & `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.12/setup.py` & `mypy-boto3-license-manager-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-license-manager",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_license_manager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LicenseManager 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.LicenseManager 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

