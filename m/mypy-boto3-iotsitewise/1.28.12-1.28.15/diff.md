# Comparing `tmp/mypy-boto3-iotsitewise-1.28.12.tar.gz` & `tmp/mypy-boto3-iotsitewise-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotsitewise-1.28.12.tar", last modified: Thu Jul 27 05:34:50 2023, max compression
+gzip compressed data, was "mypy-boto3-iotsitewise-1.28.15.tar", last modified: Fri Jul 28 20:43:01 2023, max compression
```

## Comparing `mypy-boto3-iotsitewise-1.28.12.tar` & `mypy-boto3-iotsitewise-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:50.784478 mypy-boto3-iotsitewise-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29685 2023-07-27 05:34:50.784478 mypy-boto3-iotsitewise-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28182 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:50.784478 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62559 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    62456 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-07-27 05:24:11.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21933 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21913 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   117425 2023-07-27 05:24:14.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   117201 2023-07-27 05:24:13.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:50.784478 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29685 2023-07-27 05:34:50.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-27 05:34:50.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:50.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:50.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:50.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:50.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:50.784478 mypy-boto3-iotsitewise-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:01.917291 mypy-boto3-iotsitewise-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28619 2023-07-28 20:43:01.917291 mypy-boto3-iotsitewise-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27116 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:01.917291 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62559 2023-07-28 20:28:34.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62456 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-07-28 20:28:34.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-07-28 20:28:34.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21899 2023-07-28 20:28:34.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21879 2023-07-28 20:28:34.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   108808 2023-07-28 20:28:39.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108600 2023-07-28 20:28:37.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-28 20:28:34.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-28 20:28:34.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:01.917291 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28619 2023-07-28 20:43:01.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-28 20:43:01.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:01.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:01.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:01.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:43:01.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:01.917291 mypy-boto3-iotsitewise-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/setup.py
```

### Comparing `mypy-boto3-iotsitewise-1.28.12/LICENSE` & `mypy-boto3-iotsitewise-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.12/PKG-INFO` & `mypy-boto3-iotsitewise-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-iotsitewise
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTSiteWise 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotsitewise type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iotsitewise"></a>
 
 # mypy-boto3-iotsitewise
 
 [![PyPI - mypy-boto3-iotsitewise](https://img.shields.io/pypi/v/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsitewise)](https://pepy.tech/project/mypy-boto3-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSiteWise 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[boto3.IoTSiteWise 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
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
 [mypy-boto3-iotsitewise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/).
 
 See how it helps to find and fix potential bugs:
 
@@ -471,57 +439,47 @@
 
 `mypy_boto3_iotsitewise.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotsitewise.type_defs import (
     AggregatesTypeDef,
-    AlarmsOutputTypeDef,
     AlarmsTypeDef,
     AssetErrorDetailsTypeDef,
     AssetHierarchyInfoTypeDef,
     AssetHierarchyTypeDef,
     AssetModelHierarchyDefinitionTypeDef,
-    AssetModelHierarchyOutputTypeDef,
     AssetModelHierarchyTypeDef,
     PropertyNotificationTypeDef,
-    TimeInNanosOutputTypeDef,
-    VariantOutputTypeDef,
     TimeInNanosTypeDef,
     VariantTypeDef,
     AssociateAssetsRequestRequestTypeDef,
     AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
-    AttributeOutputTypeDef,
     AttributeTypeDef,
     BatchAssociateProjectAssetsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     BatchDisassociateProjectAssetsRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesEntryTypeDef,
     BatchGetAssetPropertyAggregatesErrorEntryTypeDef,
     BatchGetAssetPropertyAggregatesErrorInfoTypeDef,
     BatchGetAssetPropertyValueEntryTypeDef,
     BatchGetAssetPropertyValueErrorEntryTypeDef,
     BatchGetAssetPropertyValueErrorInfoTypeDef,
     BatchGetAssetPropertyValueHistoryEntryTypeDef,
     BatchGetAssetPropertyValueHistoryErrorEntryTypeDef,
     BatchGetAssetPropertyValueHistoryErrorInfoTypeDef,
     ConfigurationErrorDetailsTypeDef,
-    CreateAccessPolicyResponseTypeDef,
     CreateAssetRequestRequestTypeDef,
     ErrorReportLocationTypeDef,
     FileTypeDef,
-    CreateBulkImportJobResponseTypeDef,
     CreateDashboardRequestRequestTypeDef,
-    CreateDashboardResponseTypeDef,
-    CreateGatewayResponseTypeDef,
     ImageFileTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
     CsvOutputTypeDef,
     CsvTypeDef,
-    CustomerManagedS3StorageOutputTypeDef,
     CustomerManagedS3StorageTypeDef,
     DashboardSummaryTypeDef,
     DeleteAccessPolicyRequestRequestTypeDef,
     DeleteAssetModelRequestRequestTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeleteDashboardRequestRequestTypeDef,
     DeleteGatewayRequestRequestTypeDef,
@@ -530,204 +488,182 @@
     DeleteTimeSeriesRequestRequestTypeDef,
     DescribeAccessPolicyRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeAssetModelRequestRequestTypeDef,
     DescribeAssetPropertyRequestRequestTypeDef,
     DescribeAssetRequestRequestTypeDef,
     DescribeBulkImportJobRequestRequestTypeDef,
-    ErrorReportLocationOutputTypeDef,
-    FileOutputTypeDef,
     DescribeDashboardRequestRequestTypeDef,
-    DescribeDashboardResponseTypeDef,
     DescribeGatewayCapabilityConfigurationRequestRequestTypeDef,
-    DescribeGatewayCapabilityConfigurationResponseTypeDef,
     DescribeGatewayRequestRequestTypeDef,
     GatewayCapabilitySummaryTypeDef,
-    LoggingOptionsOutputTypeDef,
+    LoggingOptionsTypeDef,
     DescribePortalRequestRequestTypeDef,
     ImageLocationTypeDef,
     DescribeProjectRequestRequestTypeDef,
-    DescribeProjectResponseTypeDef,
-    RetentionPeriodOutputTypeDef,
+    RetentionPeriodTypeDef,
     DescribeTimeSeriesRequestRequestTypeDef,
-    DescribeTimeSeriesResponseTypeDef,
     DetailedErrorTypeDef,
     DisassociateAssetsRequestRequestTypeDef,
     DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    VariableValueOutputTypeDef,
     VariableValueTypeDef,
-    ForwardingConfigOutputTypeDef,
     ForwardingConfigTypeDef,
-    GreengrassOutputTypeDef,
-    GreengrassV2OutputTypeDef,
     GreengrassTypeDef,
     GreengrassV2TypeDef,
-    GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetAssetPropertyAggregatesRequestRequestTypeDef,
-    GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef,
     GetAssetPropertyValueHistoryRequestRequestTypeDef,
     GetAssetPropertyValueRequestRequestTypeDef,
-    GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
     GetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
-    GroupIdentityOutputTypeDef,
     GroupIdentityTypeDef,
-    IAMRoleIdentityOutputTypeDef,
     IAMRoleIdentityTypeDef,
-    IAMUserIdentityOutputTypeDef,
     IAMUserIdentityTypeDef,
-    UserIdentityOutputTypeDef,
     UserIdentityTypeDef,
     JobSummaryTypeDef,
-    ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef,
     ListAccessPoliciesRequestRequestTypeDef,
-    ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
     ListAssetModelPropertiesRequestRequestTypeDef,
-    ListAssetModelsRequestListAssetModelsPaginateTypeDef,
     ListAssetModelsRequestRequestTypeDef,
-    ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
     ListAssetPropertiesRequestRequestTypeDef,
-    ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
     ListAssetRelationshipsRequestRequestTypeDef,
-    ListAssetsRequestListAssetsPaginateTypeDef,
     ListAssetsRequestRequestTypeDef,
-    ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
     ListAssociatedAssetsRequestRequestTypeDef,
-    ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef,
     ListBulkImportJobsRequestRequestTypeDef,
-    ListDashboardsRequestListDashboardsPaginateTypeDef,
     ListDashboardsRequestRequestTypeDef,
-    ListGatewaysRequestListGatewaysPaginateTypeDef,
     ListGatewaysRequestRequestTypeDef,
-    ListPortalsRequestListPortalsPaginateTypeDef,
     ListPortalsRequestRequestTypeDef,
-    ListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
     ListProjectAssetsRequestRequestTypeDef,
-    ListProjectAssetsResponseTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTimeSeriesRequestListTimeSeriesPaginateTypeDef,
     ListTimeSeriesRequestRequestTypeDef,
     TimeSeriesSummaryTypeDef,
-    LoggingOptionsTypeDef,
-    MetricProcessingConfigOutputTypeDef,
     MetricProcessingConfigTypeDef,
-    TumblingWindowOutputTypeDef,
     TumblingWindowTypeDef,
     MonitorErrorDetailsTypeDef,
-    PaginatorConfigTypeDef,
-    PortalResourceOutputTypeDef,
     PortalResourceTypeDef,
-    ProjectResourceOutputTypeDef,
     ProjectResourceTypeDef,
     PutDefaultEncryptionConfigurationRequestRequestTypeDef,
-    RetentionPeriodTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssetPropertyRequestRequestTypeDef,
     UpdateAssetRequestRequestTypeDef,
     UpdateDashboardRequestRequestTypeDef,
     UpdateGatewayCapabilityConfigurationRequestRequestTypeDef,
-    UpdateGatewayCapabilityConfigurationResponseTypeDef,
     UpdateGatewayRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     AggregatedValueTypeDef,
-    BatchAssociateProjectAssetsResponseTypeDef,
-    BatchDisassociateProjectAssetsResponseTypeDef,
     AssetRelationshipSummaryTypeDef,
     AssetPropertySummaryTypeDef,
     AssetPropertyTypeDef,
     BatchPutAssetPropertyErrorTypeDef,
-    AssetPropertyValueOutputTypeDef,
-    InterpolatedAssetPropertyValueTypeDef,
     AssetPropertyValueTypeDef,
+    InterpolatedAssetPropertyValueTypeDef,
+    BatchAssociateProjectAssetsResponseTypeDef,
+    BatchDisassociateProjectAssetsResponseTypeDef,
+    CreateAccessPolicyResponseTypeDef,
+    CreateBulkImportJobResponseTypeDef,
+    CreateDashboardResponseTypeDef,
+    CreateGatewayResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    DescribeDashboardResponseTypeDef,
+    DescribeGatewayCapabilityConfigurationResponseTypeDef,
+    DescribeProjectResponseTypeDef,
+    DescribeTimeSeriesResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListProjectAssetsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateGatewayCapabilityConfigurationResponseTypeDef,
     BatchGetAssetPropertyAggregatesRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesSkippedEntryTypeDef,
     BatchGetAssetPropertyValueRequestRequestTypeDef,
     BatchGetAssetPropertyValueSkippedEntryTypeDef,
     BatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
     BatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
     ConfigurationStatusTypeDef,
     CreatePortalRequestRequestTypeDef,
     ImageTypeDef,
     FileFormatOutputTypeDef,
     FileFormatTypeDef,
-    MultiLayerStorageOutputTypeDef,
     MultiLayerStorageTypeDef,
     ListDashboardsResponseTypeDef,
     DescribeAssetModelRequestAssetModelActiveWaitTypeDef,
     DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef,
     DescribeAssetRequestAssetActiveWaitTypeDef,
     DescribeAssetRequestAssetNotExistsWaitTypeDef,
     DescribePortalRequestPortalActiveWaitTypeDef,
     DescribePortalRequestPortalNotExistsWaitTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
+    PutLoggingOptionsRequestRequestTypeDef,
     ErrorDetailsTypeDef,
-    ExpressionVariableOutputTypeDef,
     ExpressionVariableTypeDef,
-    MeasurementProcessingConfigOutputTypeDef,
-    TransformProcessingConfigOutputTypeDef,
     MeasurementProcessingConfigTypeDef,
     TransformProcessingConfigTypeDef,
-    GatewayPlatformOutputTypeDef,
     GatewayPlatformTypeDef,
-    IdentityOutputTypeDef,
+    GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
+    GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef,
+    GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
+    ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef,
+    ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
+    ListAssetModelsRequestListAssetModelsPaginateTypeDef,
+    ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
+    ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
+    ListAssetsRequestListAssetsPaginateTypeDef,
+    ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
+    ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef,
+    ListDashboardsRequestListDashboardsPaginateTypeDef,
+    ListGatewaysRequestListGatewaysPaginateTypeDef,
+    ListPortalsRequestListPortalsPaginateTypeDef,
+    ListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListTimeSeriesRequestListTimeSeriesPaginateTypeDef,
     IdentityTypeDef,
     ListBulkImportJobsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTimeSeriesResponseTypeDef,
-    PutLoggingOptionsRequestRequestTypeDef,
-    MetricWindowOutputTypeDef,
     MetricWindowTypeDef,
     PortalStatusTypeDef,
-    ResourceOutputTypeDef,
     ResourceTypeDef,
     BatchGetAssetPropertyAggregatesSuccessEntryTypeDef,
     GetAssetPropertyAggregatesResponseTypeDef,
     ListAssetRelationshipsResponseTypeDef,
     ListAssetPropertiesResponseTypeDef,
     AssetCompositeModelTypeDef,
     BatchPutAssetPropertyErrorEntryTypeDef,
     BatchGetAssetPropertyValueHistorySuccessEntryTypeDef,
     BatchGetAssetPropertyValueSuccessEntryTypeDef,
     GetAssetPropertyValueHistoryResponseTypeDef,
     GetAssetPropertyValueResponseTypeDef,
-    GetInterpolatedAssetPropertyValuesResponseTypeDef,
     PutAssetPropertyValueEntryTypeDef,
+    GetInterpolatedAssetPropertyValuesResponseTypeDef,
     DescribeDefaultEncryptionConfigurationResponseTypeDef,
     PutDefaultEncryptionConfigurationResponseTypeDef,
     UpdatePortalRequestRequestTypeDef,
     JobConfigurationOutputTypeDef,
     JobConfigurationTypeDef,
     DescribeStorageConfigurationResponseTypeDef,
-    PutStorageConfigurationResponseTypeDef,
     PutStorageConfigurationRequestRequestTypeDef,
+    PutStorageConfigurationResponseTypeDef,
     AssetModelStatusTypeDef,
     AssetStatusTypeDef,
-    MeasurementOutputTypeDef,
-    TransformOutputTypeDef,
     MeasurementTypeDef,
+    TransformOutputTypeDef,
     TransformTypeDef,
+    CreateGatewayRequestRequestTypeDef,
     DescribeGatewayResponseTypeDef,
     GatewaySummaryTypeDef,
-    CreateGatewayRequestRequestTypeDef,
     MetricOutputTypeDef,
     MetricTypeDef,
     CreatePortalResponseTypeDef,
     DeletePortalResponseTypeDef,
     DescribePortalResponseTypeDef,
     PortalSummaryTypeDef,
     UpdatePortalResponseTypeDef,
     AccessPolicySummaryTypeDef,
-    DescribeAccessPolicyResponseTypeDef,
     CreateAccessPolicyRequestRequestTypeDef,
+    DescribeAccessPolicyResponseTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesResponseTypeDef,
     BatchPutAssetPropertyValueResponseTypeDef,
     BatchGetAssetPropertyValueHistoryResponseTypeDef,
     BatchGetAssetPropertyValueResponseTypeDef,
     BatchPutAssetPropertyValueRequestRequestTypeDef,
     DescribeBulkImportJobResponseTypeDef,
```

### Comparing `mypy-boto3-iotsitewise-1.28.12/README.md` & `mypy-boto3-iotsitewise-1.28.15/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-iotsitewise
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTSiteWise 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 iotsitewise type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iotsitewise"></a>
 
 # mypy-boto3-iotsitewise
 
 [![PyPI - mypy-boto3-iotsitewise](https://img.shields.io/pypi/v/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsitewise)](https://pepy.tech/project/mypy-boto3-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSiteWise 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[boto3.IoTSiteWise 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
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
 [mypy-boto3-iotsitewise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/).
 
 See how it helps to find and fix potential bugs:
 
@@ -439,57 +471,47 @@
 
 `mypy_boto3_iotsitewise.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotsitewise.type_defs import (
     AggregatesTypeDef,
-    AlarmsOutputTypeDef,
     AlarmsTypeDef,
     AssetErrorDetailsTypeDef,
     AssetHierarchyInfoTypeDef,
     AssetHierarchyTypeDef,
     AssetModelHierarchyDefinitionTypeDef,
-    AssetModelHierarchyOutputTypeDef,
     AssetModelHierarchyTypeDef,
     PropertyNotificationTypeDef,
-    TimeInNanosOutputTypeDef,
-    VariantOutputTypeDef,
     TimeInNanosTypeDef,
     VariantTypeDef,
     AssociateAssetsRequestRequestTypeDef,
     AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
-    AttributeOutputTypeDef,
     AttributeTypeDef,
     BatchAssociateProjectAssetsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     BatchDisassociateProjectAssetsRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesEntryTypeDef,
     BatchGetAssetPropertyAggregatesErrorEntryTypeDef,
     BatchGetAssetPropertyAggregatesErrorInfoTypeDef,
     BatchGetAssetPropertyValueEntryTypeDef,
     BatchGetAssetPropertyValueErrorEntryTypeDef,
     BatchGetAssetPropertyValueErrorInfoTypeDef,
     BatchGetAssetPropertyValueHistoryEntryTypeDef,
     BatchGetAssetPropertyValueHistoryErrorEntryTypeDef,
     BatchGetAssetPropertyValueHistoryErrorInfoTypeDef,
     ConfigurationErrorDetailsTypeDef,
-    CreateAccessPolicyResponseTypeDef,
     CreateAssetRequestRequestTypeDef,
     ErrorReportLocationTypeDef,
     FileTypeDef,
-    CreateBulkImportJobResponseTypeDef,
     CreateDashboardRequestRequestTypeDef,
-    CreateDashboardResponseTypeDef,
-    CreateGatewayResponseTypeDef,
     ImageFileTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
     CsvOutputTypeDef,
     CsvTypeDef,
-    CustomerManagedS3StorageOutputTypeDef,
     CustomerManagedS3StorageTypeDef,
     DashboardSummaryTypeDef,
     DeleteAccessPolicyRequestRequestTypeDef,
     DeleteAssetModelRequestRequestTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeleteDashboardRequestRequestTypeDef,
     DeleteGatewayRequestRequestTypeDef,
@@ -498,204 +520,182 @@
     DeleteTimeSeriesRequestRequestTypeDef,
     DescribeAccessPolicyRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeAssetModelRequestRequestTypeDef,
     DescribeAssetPropertyRequestRequestTypeDef,
     DescribeAssetRequestRequestTypeDef,
     DescribeBulkImportJobRequestRequestTypeDef,
-    ErrorReportLocationOutputTypeDef,
-    FileOutputTypeDef,
     DescribeDashboardRequestRequestTypeDef,
-    DescribeDashboardResponseTypeDef,
     DescribeGatewayCapabilityConfigurationRequestRequestTypeDef,
-    DescribeGatewayCapabilityConfigurationResponseTypeDef,
     DescribeGatewayRequestRequestTypeDef,
     GatewayCapabilitySummaryTypeDef,
-    LoggingOptionsOutputTypeDef,
+    LoggingOptionsTypeDef,
     DescribePortalRequestRequestTypeDef,
     ImageLocationTypeDef,
     DescribeProjectRequestRequestTypeDef,
-    DescribeProjectResponseTypeDef,
-    RetentionPeriodOutputTypeDef,
+    RetentionPeriodTypeDef,
     DescribeTimeSeriesRequestRequestTypeDef,
-    DescribeTimeSeriesResponseTypeDef,
     DetailedErrorTypeDef,
     DisassociateAssetsRequestRequestTypeDef,
     DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    VariableValueOutputTypeDef,
     VariableValueTypeDef,
-    ForwardingConfigOutputTypeDef,
     ForwardingConfigTypeDef,
-    GreengrassOutputTypeDef,
-    GreengrassV2OutputTypeDef,
     GreengrassTypeDef,
     GreengrassV2TypeDef,
-    GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetAssetPropertyAggregatesRequestRequestTypeDef,
-    GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef,
     GetAssetPropertyValueHistoryRequestRequestTypeDef,
     GetAssetPropertyValueRequestRequestTypeDef,
-    GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
     GetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
-    GroupIdentityOutputTypeDef,
     GroupIdentityTypeDef,
-    IAMRoleIdentityOutputTypeDef,
     IAMRoleIdentityTypeDef,
-    IAMUserIdentityOutputTypeDef,
     IAMUserIdentityTypeDef,
-    UserIdentityOutputTypeDef,
     UserIdentityTypeDef,
     JobSummaryTypeDef,
-    ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef,
     ListAccessPoliciesRequestRequestTypeDef,
-    ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
     ListAssetModelPropertiesRequestRequestTypeDef,
-    ListAssetModelsRequestListAssetModelsPaginateTypeDef,
     ListAssetModelsRequestRequestTypeDef,
-    ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
     ListAssetPropertiesRequestRequestTypeDef,
-    ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
     ListAssetRelationshipsRequestRequestTypeDef,
-    ListAssetsRequestListAssetsPaginateTypeDef,
     ListAssetsRequestRequestTypeDef,
-    ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
     ListAssociatedAssetsRequestRequestTypeDef,
-    ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef,
     ListBulkImportJobsRequestRequestTypeDef,
-    ListDashboardsRequestListDashboardsPaginateTypeDef,
     ListDashboardsRequestRequestTypeDef,
-    ListGatewaysRequestListGatewaysPaginateTypeDef,
     ListGatewaysRequestRequestTypeDef,
-    ListPortalsRequestListPortalsPaginateTypeDef,
     ListPortalsRequestRequestTypeDef,
-    ListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
     ListProjectAssetsRequestRequestTypeDef,
-    ListProjectAssetsResponseTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTimeSeriesRequestListTimeSeriesPaginateTypeDef,
     ListTimeSeriesRequestRequestTypeDef,
     TimeSeriesSummaryTypeDef,
-    LoggingOptionsTypeDef,
-    MetricProcessingConfigOutputTypeDef,
     MetricProcessingConfigTypeDef,
-    TumblingWindowOutputTypeDef,
     TumblingWindowTypeDef,
     MonitorErrorDetailsTypeDef,
-    PaginatorConfigTypeDef,
-    PortalResourceOutputTypeDef,
     PortalResourceTypeDef,
-    ProjectResourceOutputTypeDef,
     ProjectResourceTypeDef,
     PutDefaultEncryptionConfigurationRequestRequestTypeDef,
-    RetentionPeriodTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssetPropertyRequestRequestTypeDef,
     UpdateAssetRequestRequestTypeDef,
     UpdateDashboardRequestRequestTypeDef,
     UpdateGatewayCapabilityConfigurationRequestRequestTypeDef,
-    UpdateGatewayCapabilityConfigurationResponseTypeDef,
     UpdateGatewayRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     AggregatedValueTypeDef,
-    BatchAssociateProjectAssetsResponseTypeDef,
-    BatchDisassociateProjectAssetsResponseTypeDef,
     AssetRelationshipSummaryTypeDef,
     AssetPropertySummaryTypeDef,
     AssetPropertyTypeDef,
     BatchPutAssetPropertyErrorTypeDef,
-    AssetPropertyValueOutputTypeDef,
-    InterpolatedAssetPropertyValueTypeDef,
     AssetPropertyValueTypeDef,
+    InterpolatedAssetPropertyValueTypeDef,
+    BatchAssociateProjectAssetsResponseTypeDef,
+    BatchDisassociateProjectAssetsResponseTypeDef,
+    CreateAccessPolicyResponseTypeDef,
+    CreateBulkImportJobResponseTypeDef,
+    CreateDashboardResponseTypeDef,
+    CreateGatewayResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    DescribeDashboardResponseTypeDef,
+    DescribeGatewayCapabilityConfigurationResponseTypeDef,
+    DescribeProjectResponseTypeDef,
+    DescribeTimeSeriesResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListProjectAssetsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateGatewayCapabilityConfigurationResponseTypeDef,
     BatchGetAssetPropertyAggregatesRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesSkippedEntryTypeDef,
     BatchGetAssetPropertyValueRequestRequestTypeDef,
     BatchGetAssetPropertyValueSkippedEntryTypeDef,
     BatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
     BatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
     ConfigurationStatusTypeDef,
     CreatePortalRequestRequestTypeDef,
     ImageTypeDef,
     FileFormatOutputTypeDef,
     FileFormatTypeDef,
-    MultiLayerStorageOutputTypeDef,
     MultiLayerStorageTypeDef,
     ListDashboardsResponseTypeDef,
     DescribeAssetModelRequestAssetModelActiveWaitTypeDef,
     DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef,
     DescribeAssetRequestAssetActiveWaitTypeDef,
     DescribeAssetRequestAssetNotExistsWaitTypeDef,
     DescribePortalRequestPortalActiveWaitTypeDef,
     DescribePortalRequestPortalNotExistsWaitTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
+    PutLoggingOptionsRequestRequestTypeDef,
     ErrorDetailsTypeDef,
-    ExpressionVariableOutputTypeDef,
     ExpressionVariableTypeDef,
-    MeasurementProcessingConfigOutputTypeDef,
-    TransformProcessingConfigOutputTypeDef,
     MeasurementProcessingConfigTypeDef,
     TransformProcessingConfigTypeDef,
-    GatewayPlatformOutputTypeDef,
     GatewayPlatformTypeDef,
-    IdentityOutputTypeDef,
+    GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
+    GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef,
+    GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
+    ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef,
+    ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
+    ListAssetModelsRequestListAssetModelsPaginateTypeDef,
+    ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
+    ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
+    ListAssetsRequestListAssetsPaginateTypeDef,
+    ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
+    ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef,
+    ListDashboardsRequestListDashboardsPaginateTypeDef,
+    ListGatewaysRequestListGatewaysPaginateTypeDef,
+    ListPortalsRequestListPortalsPaginateTypeDef,
+    ListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListTimeSeriesRequestListTimeSeriesPaginateTypeDef,
     IdentityTypeDef,
     ListBulkImportJobsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTimeSeriesResponseTypeDef,
-    PutLoggingOptionsRequestRequestTypeDef,
-    MetricWindowOutputTypeDef,
     MetricWindowTypeDef,
     PortalStatusTypeDef,
-    ResourceOutputTypeDef,
     ResourceTypeDef,
     BatchGetAssetPropertyAggregatesSuccessEntryTypeDef,
     GetAssetPropertyAggregatesResponseTypeDef,
     ListAssetRelationshipsResponseTypeDef,
     ListAssetPropertiesResponseTypeDef,
     AssetCompositeModelTypeDef,
     BatchPutAssetPropertyErrorEntryTypeDef,
     BatchGetAssetPropertyValueHistorySuccessEntryTypeDef,
     BatchGetAssetPropertyValueSuccessEntryTypeDef,
     GetAssetPropertyValueHistoryResponseTypeDef,
     GetAssetPropertyValueResponseTypeDef,
-    GetInterpolatedAssetPropertyValuesResponseTypeDef,
     PutAssetPropertyValueEntryTypeDef,
+    GetInterpolatedAssetPropertyValuesResponseTypeDef,
     DescribeDefaultEncryptionConfigurationResponseTypeDef,
     PutDefaultEncryptionConfigurationResponseTypeDef,
     UpdatePortalRequestRequestTypeDef,
     JobConfigurationOutputTypeDef,
     JobConfigurationTypeDef,
     DescribeStorageConfigurationResponseTypeDef,
-    PutStorageConfigurationResponseTypeDef,
     PutStorageConfigurationRequestRequestTypeDef,
+    PutStorageConfigurationResponseTypeDef,
     AssetModelStatusTypeDef,
     AssetStatusTypeDef,
-    MeasurementOutputTypeDef,
-    TransformOutputTypeDef,
     MeasurementTypeDef,
+    TransformOutputTypeDef,
     TransformTypeDef,
+    CreateGatewayRequestRequestTypeDef,
     DescribeGatewayResponseTypeDef,
     GatewaySummaryTypeDef,
-    CreateGatewayRequestRequestTypeDef,
     MetricOutputTypeDef,
     MetricTypeDef,
     CreatePortalResponseTypeDef,
     DeletePortalResponseTypeDef,
     DescribePortalResponseTypeDef,
     PortalSummaryTypeDef,
     UpdatePortalResponseTypeDef,
     AccessPolicySummaryTypeDef,
-    DescribeAccessPolicyResponseTypeDef,
     CreateAccessPolicyRequestRequestTypeDef,
+    DescribeAccessPolicyResponseTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesResponseTypeDef,
     BatchPutAssetPropertyValueResponseTypeDef,
     BatchGetAssetPropertyValueHistoryResponseTypeDef,
     BatchGetAssetPropertyValueResponseTypeDef,
     BatchPutAssetPropertyValueRequestRequestTypeDef,
     DescribeBulkImportJobResponseTypeDef,
```

### Comparing `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/__init__.py` & `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/__init__.pyi` & `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/__main__.py` & `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTSiteWise 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoTSiteWise 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise\nOther"
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

### Comparing `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/client.py` & `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/client.pyi` & `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/literals.py` & `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/literals.pyi` & `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/paginator.py` & `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         startDate: Union[datetime, str],
         endDate: Union[datetime, str],
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAssetPropertyAggregatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyAggregates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getassetpropertyaggregatespaginator)
         """
 
 
@@ -166,15 +166,15 @@
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         startDate: Union[datetime, str] = ...,
         endDate: Union[datetime, str] = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAssetPropertyValueHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyValueHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getassetpropertyvaluehistorypaginator)
         """
 
 
@@ -194,15 +194,15 @@
         type: str,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         startTimeOffsetInNanos: int = ...,
         endTimeOffsetInNanos: int = ...,
         intervalWindowInSeconds: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInterpolatedAssetPropertyValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetInterpolatedAssetPropertyValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getinterpolatedassetpropertyvaluespaginator)
         """
 
 
@@ -216,15 +216,15 @@
         self,
         *,
         identityType: IdentityTypeType = ...,
         identityId: str = ...,
         resourceType: ResourceTypeType = ...,
         resourceId: str = ...,
         iamArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAccessPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listaccesspoliciespaginator)
         """
 
 
@@ -235,30 +235,30 @@
     """
 
     def paginate(
         self,
         *,
         assetModelId: str,
         filter: ListAssetModelPropertiesFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetModelPropertiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModelProperties.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetmodelpropertiespaginator)
         """
 
 
 class ListAssetModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetmodelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetmodelspaginator)
         """
 
 
@@ -269,15 +269,15 @@
     """
 
     def paginate(
         self,
         *,
         assetId: str,
         filter: ListAssetPropertiesFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetPropertiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetProperties.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetpropertiespaginator)
         """
 
 
@@ -288,15 +288,15 @@
     """
 
     def paginate(
         self,
         *,
         assetId: str,
         traversalType: Literal["PATH_TO_ROOT"],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetRelationshipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetRelationships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetrelationshipspaginator)
         """
 
 
@@ -307,15 +307,15 @@
     """
 
     def paginate(
         self,
         *,
         assetModelId: str = ...,
         filter: ListAssetsFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetspaginator)
         """
 
 
@@ -327,15 +327,15 @@
 
     def paginate(
         self,
         *,
         assetId: str,
         hierarchyId: str = ...,
         traversalDirection: TraversalDirectionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociatedAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssociatedAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassociatedassetspaginator)
         """
 
 
@@ -345,90 +345,90 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listbulkimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filter: ListBulkImportJobsFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBulkImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListBulkImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listbulkimportjobspaginator)
         """
 
 
 class ListDashboardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListDashboards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listdashboardspaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDashboardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListDashboards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listdashboardspaginator)
         """
 
 
 class ListGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGatewaysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listgatewayspaginator)
         """
 
 
 class ListPortalsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListPortals)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listportalspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPortalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListPortals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listportalspaginator)
         """
 
 
 class ListProjectAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjectAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectassetspaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjectAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectassetspaginator)
         """
 
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, portalId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, portalId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectspaginator)
         """
 
 
@@ -440,13 +440,13 @@
 
     def paginate(
         self,
         *,
         assetId: str = ...,
         aliasPrefix: str = ...,
         timeSeriesType: ListTimeSeriesTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTimeSeriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListTimeSeries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listtimeseriespaginator)
         """
```

### Comparing `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/paginator.pyi` & `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         startDate: Union[datetime, str],
         endDate: Union[datetime, str],
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAssetPropertyAggregatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyAggregates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getassetpropertyaggregatespaginator)
         """
 
 class GetAssetPropertyValueHistoryPaginator(Paginator):
@@ -161,15 +161,15 @@
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         startDate: Union[datetime, str] = ...,
         endDate: Union[datetime, str] = ...,
         qualities: Sequence[QualityType] = ...,
         timeOrdering: TimeOrderingType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAssetPropertyValueHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyValueHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getassetpropertyvaluehistorypaginator)
         """
 
 class GetInterpolatedAssetPropertyValuesPaginator(Paginator):
@@ -188,15 +188,15 @@
         type: str,
         assetId: str = ...,
         propertyId: str = ...,
         propertyAlias: str = ...,
         startTimeOffsetInNanos: int = ...,
         endTimeOffsetInNanos: int = ...,
         intervalWindowInSeconds: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInterpolatedAssetPropertyValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetInterpolatedAssetPropertyValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#getinterpolatedassetpropertyvaluespaginator)
         """
 
 class ListAccessPoliciesPaginator(Paginator):
@@ -209,15 +209,15 @@
         self,
         *,
         identityType: IdentityTypeType = ...,
         identityId: str = ...,
         resourceType: ResourceTypeType = ...,
         resourceId: str = ...,
         iamArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAccessPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listaccesspoliciespaginator)
         """
 
 class ListAssetModelPropertiesPaginator(Paginator):
@@ -227,29 +227,29 @@
     """
 
     def paginate(
         self,
         *,
         assetModelId: str,
         filter: ListAssetModelPropertiesFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetModelPropertiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModelProperties.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetmodelpropertiespaginator)
         """
 
 class ListAssetModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetmodelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetmodelspaginator)
         """
 
 class ListAssetPropertiesPaginator(Paginator):
@@ -259,15 +259,15 @@
     """
 
     def paginate(
         self,
         *,
         assetId: str,
         filter: ListAssetPropertiesFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetPropertiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetProperties.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetpropertiespaginator)
         """
 
 class ListAssetRelationshipsPaginator(Paginator):
@@ -277,15 +277,15 @@
     """
 
     def paginate(
         self,
         *,
         assetId: str,
         traversalType: Literal["PATH_TO_ROOT"],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetRelationshipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetRelationships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetrelationshipspaginator)
         """
 
 class ListAssetsPaginator(Paginator):
@@ -295,15 +295,15 @@
     """
 
     def paginate(
         self,
         *,
         assetModelId: str = ...,
         filter: ListAssetsFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassetspaginator)
         """
 
 class ListAssociatedAssetsPaginator(Paginator):
@@ -314,15 +314,15 @@
 
     def paginate(
         self,
         *,
         assetId: str,
         hierarchyId: str = ...,
         traversalDirection: TraversalDirectionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociatedAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssociatedAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listassociatedassetspaginator)
         """
 
 class ListBulkImportJobsPaginator(Paginator):
@@ -331,85 +331,85 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listbulkimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filter: ListBulkImportJobsFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBulkImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListBulkImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listbulkimportjobspaginator)
         """
 
 class ListDashboardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListDashboards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listdashboardspaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDashboardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListDashboards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listdashboardspaginator)
         """
 
 class ListGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGatewaysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listgatewayspaginator)
         """
 
 class ListPortalsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListPortals)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listportalspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPortalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListPortals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listportalspaginator)
         """
 
 class ListProjectAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjectAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectassetspaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjectAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectassetspaginator)
         """
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, portalId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, portalId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listprojectspaginator)
         """
 
 class ListTimeSeriesPaginator(Paginator):
@@ -420,13 +420,13 @@
 
     def paginate(
         self,
         *,
         assetId: str = ...,
         aliasPrefix: str = ...,
         timeSeriesType: ListTimeSeriesTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTimeSeriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListTimeSeries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/paginators/#listtimeseriespaginator)
         """
```

### Comparing `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/type_defs.py` & `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,57 +64,47 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AggregatesTypeDef",
-    "AlarmsOutputTypeDef",
     "AlarmsTypeDef",
     "AssetErrorDetailsTypeDef",
     "AssetHierarchyInfoTypeDef",
     "AssetHierarchyTypeDef",
     "AssetModelHierarchyDefinitionTypeDef",
-    "AssetModelHierarchyOutputTypeDef",
     "AssetModelHierarchyTypeDef",
     "PropertyNotificationTypeDef",
-    "TimeInNanosOutputTypeDef",
-    "VariantOutputTypeDef",
     "TimeInNanosTypeDef",
     "VariantTypeDef",
     "AssociateAssetsRequestRequestTypeDef",
     "AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef",
-    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "BatchAssociateProjectAssetsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDisassociateProjectAssetsRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesEntryTypeDef",
     "BatchGetAssetPropertyAggregatesErrorEntryTypeDef",
     "BatchGetAssetPropertyAggregatesErrorInfoTypeDef",
     "BatchGetAssetPropertyValueEntryTypeDef",
     "BatchGetAssetPropertyValueErrorEntryTypeDef",
     "BatchGetAssetPropertyValueErrorInfoTypeDef",
     "BatchGetAssetPropertyValueHistoryEntryTypeDef",
     "BatchGetAssetPropertyValueHistoryErrorEntryTypeDef",
     "BatchGetAssetPropertyValueHistoryErrorInfoTypeDef",
     "ConfigurationErrorDetailsTypeDef",
-    "CreateAccessPolicyResponseTypeDef",
     "CreateAssetRequestRequestTypeDef",
     "ErrorReportLocationTypeDef",
     "FileTypeDef",
-    "CreateBulkImportJobResponseTypeDef",
     "CreateDashboardRequestRequestTypeDef",
-    "CreateDashboardResponseTypeDef",
-    "CreateGatewayResponseTypeDef",
     "ImageFileTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "CreateProjectResponseTypeDef",
     "CsvOutputTypeDef",
     "CsvTypeDef",
-    "CustomerManagedS3StorageOutputTypeDef",
     "CustomerManagedS3StorageTypeDef",
     "DashboardSummaryTypeDef",
     "DeleteAccessPolicyRequestRequestTypeDef",
     "DeleteAssetModelRequestRequestTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeleteDashboardRequestRequestTypeDef",
     "DeleteGatewayRequestRequestTypeDef",
@@ -123,204 +113,182 @@
     "DeleteTimeSeriesRequestRequestTypeDef",
     "DescribeAccessPolicyRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAssetModelRequestRequestTypeDef",
     "DescribeAssetPropertyRequestRequestTypeDef",
     "DescribeAssetRequestRequestTypeDef",
     "DescribeBulkImportJobRequestRequestTypeDef",
-    "ErrorReportLocationOutputTypeDef",
-    "FileOutputTypeDef",
     "DescribeDashboardRequestRequestTypeDef",
-    "DescribeDashboardResponseTypeDef",
     "DescribeGatewayCapabilityConfigurationRequestRequestTypeDef",
-    "DescribeGatewayCapabilityConfigurationResponseTypeDef",
     "DescribeGatewayRequestRequestTypeDef",
     "GatewayCapabilitySummaryTypeDef",
-    "LoggingOptionsOutputTypeDef",
+    "LoggingOptionsTypeDef",
     "DescribePortalRequestRequestTypeDef",
     "ImageLocationTypeDef",
     "DescribeProjectRequestRequestTypeDef",
-    "DescribeProjectResponseTypeDef",
-    "RetentionPeriodOutputTypeDef",
+    "RetentionPeriodTypeDef",
     "DescribeTimeSeriesRequestRequestTypeDef",
-    "DescribeTimeSeriesResponseTypeDef",
     "DetailedErrorTypeDef",
     "DisassociateAssetsRequestRequestTypeDef",
     "DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "VariableValueOutputTypeDef",
     "VariableValueTypeDef",
-    "ForwardingConfigOutputTypeDef",
     "ForwardingConfigTypeDef",
-    "GreengrassOutputTypeDef",
-    "GreengrassV2OutputTypeDef",
     "GreengrassTypeDef",
     "GreengrassV2TypeDef",
-    "GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetAssetPropertyAggregatesRequestRequestTypeDef",
-    "GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef",
     "GetAssetPropertyValueHistoryRequestRequestTypeDef",
     "GetAssetPropertyValueRequestRequestTypeDef",
-    "GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef",
     "GetInterpolatedAssetPropertyValuesRequestRequestTypeDef",
-    "GroupIdentityOutputTypeDef",
     "GroupIdentityTypeDef",
-    "IAMRoleIdentityOutputTypeDef",
     "IAMRoleIdentityTypeDef",
-    "IAMUserIdentityOutputTypeDef",
     "IAMUserIdentityTypeDef",
-    "UserIdentityOutputTypeDef",
     "UserIdentityTypeDef",
     "JobSummaryTypeDef",
-    "ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef",
     "ListAccessPoliciesRequestRequestTypeDef",
-    "ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef",
     "ListAssetModelPropertiesRequestRequestTypeDef",
-    "ListAssetModelsRequestListAssetModelsPaginateTypeDef",
     "ListAssetModelsRequestRequestTypeDef",
-    "ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef",
     "ListAssetPropertiesRequestRequestTypeDef",
-    "ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
     "ListAssetRelationshipsRequestRequestTypeDef",
-    "ListAssetsRequestListAssetsPaginateTypeDef",
     "ListAssetsRequestRequestTypeDef",
-    "ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef",
     "ListAssociatedAssetsRequestRequestTypeDef",
-    "ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef",
     "ListBulkImportJobsRequestRequestTypeDef",
-    "ListDashboardsRequestListDashboardsPaginateTypeDef",
     "ListDashboardsRequestRequestTypeDef",
-    "ListGatewaysRequestListGatewaysPaginateTypeDef",
     "ListGatewaysRequestRequestTypeDef",
-    "ListPortalsRequestListPortalsPaginateTypeDef",
     "ListPortalsRequestRequestTypeDef",
-    "ListProjectAssetsRequestListProjectAssetsPaginateTypeDef",
     "ListProjectAssetsRequestRequestTypeDef",
-    "ListProjectAssetsResponseTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTimeSeriesRequestListTimeSeriesPaginateTypeDef",
     "ListTimeSeriesRequestRequestTypeDef",
     "TimeSeriesSummaryTypeDef",
-    "LoggingOptionsTypeDef",
-    "MetricProcessingConfigOutputTypeDef",
     "MetricProcessingConfigTypeDef",
-    "TumblingWindowOutputTypeDef",
     "TumblingWindowTypeDef",
     "MonitorErrorDetailsTypeDef",
-    "PaginatorConfigTypeDef",
-    "PortalResourceOutputTypeDef",
     "PortalResourceTypeDef",
-    "ProjectResourceOutputTypeDef",
     "ProjectResourceTypeDef",
     "PutDefaultEncryptionConfigurationRequestRequestTypeDef",
-    "RetentionPeriodTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssetPropertyRequestRequestTypeDef",
     "UpdateAssetRequestRequestTypeDef",
     "UpdateDashboardRequestRequestTypeDef",
     "UpdateGatewayCapabilityConfigurationRequestRequestTypeDef",
-    "UpdateGatewayCapabilityConfigurationResponseTypeDef",
     "UpdateGatewayRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "AggregatedValueTypeDef",
-    "BatchAssociateProjectAssetsResponseTypeDef",
-    "BatchDisassociateProjectAssetsResponseTypeDef",
     "AssetRelationshipSummaryTypeDef",
     "AssetPropertySummaryTypeDef",
     "AssetPropertyTypeDef",
     "BatchPutAssetPropertyErrorTypeDef",
-    "AssetPropertyValueOutputTypeDef",
-    "InterpolatedAssetPropertyValueTypeDef",
     "AssetPropertyValueTypeDef",
+    "InterpolatedAssetPropertyValueTypeDef",
+    "BatchAssociateProjectAssetsResponseTypeDef",
+    "BatchDisassociateProjectAssetsResponseTypeDef",
+    "CreateAccessPolicyResponseTypeDef",
+    "CreateBulkImportJobResponseTypeDef",
+    "CreateDashboardResponseTypeDef",
+    "CreateGatewayResponseTypeDef",
+    "CreateProjectResponseTypeDef",
+    "DescribeDashboardResponseTypeDef",
+    "DescribeGatewayCapabilityConfigurationResponseTypeDef",
+    "DescribeProjectResponseTypeDef",
+    "DescribeTimeSeriesResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListProjectAssetsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateGatewayCapabilityConfigurationResponseTypeDef",
     "BatchGetAssetPropertyAggregatesRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesSkippedEntryTypeDef",
     "BatchGetAssetPropertyValueRequestRequestTypeDef",
     "BatchGetAssetPropertyValueSkippedEntryTypeDef",
     "BatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
     "BatchGetAssetPropertyValueHistorySkippedEntryTypeDef",
     "ConfigurationStatusTypeDef",
     "CreatePortalRequestRequestTypeDef",
     "ImageTypeDef",
     "FileFormatOutputTypeDef",
     "FileFormatTypeDef",
-    "MultiLayerStorageOutputTypeDef",
     "MultiLayerStorageTypeDef",
     "ListDashboardsResponseTypeDef",
     "DescribeAssetModelRequestAssetModelActiveWaitTypeDef",
     "DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef",
     "DescribeAssetRequestAssetActiveWaitTypeDef",
     "DescribeAssetRequestAssetNotExistsWaitTypeDef",
     "DescribePortalRequestPortalActiveWaitTypeDef",
     "DescribePortalRequestPortalNotExistsWaitTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
+    "PutLoggingOptionsRequestRequestTypeDef",
     "ErrorDetailsTypeDef",
-    "ExpressionVariableOutputTypeDef",
     "ExpressionVariableTypeDef",
-    "MeasurementProcessingConfigOutputTypeDef",
-    "TransformProcessingConfigOutputTypeDef",
     "MeasurementProcessingConfigTypeDef",
     "TransformProcessingConfigTypeDef",
-    "GatewayPlatformOutputTypeDef",
     "GatewayPlatformTypeDef",
-    "IdentityOutputTypeDef",
+    "GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
+    "GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef",
+    "GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef",
+    "ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef",
+    "ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef",
+    "ListAssetModelsRequestListAssetModelsPaginateTypeDef",
+    "ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef",
+    "ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
+    "ListAssetsRequestListAssetsPaginateTypeDef",
+    "ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef",
+    "ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef",
+    "ListDashboardsRequestListDashboardsPaginateTypeDef",
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
+    "ListPortalsRequestListPortalsPaginateTypeDef",
+    "ListProjectAssetsRequestListProjectAssetsPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListTimeSeriesRequestListTimeSeriesPaginateTypeDef",
     "IdentityTypeDef",
     "ListBulkImportJobsResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "ListTimeSeriesResponseTypeDef",
-    "PutLoggingOptionsRequestRequestTypeDef",
-    "MetricWindowOutputTypeDef",
     "MetricWindowTypeDef",
     "PortalStatusTypeDef",
-    "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "BatchGetAssetPropertyAggregatesSuccessEntryTypeDef",
     "GetAssetPropertyAggregatesResponseTypeDef",
     "ListAssetRelationshipsResponseTypeDef",
     "ListAssetPropertiesResponseTypeDef",
     "AssetCompositeModelTypeDef",
     "BatchPutAssetPropertyErrorEntryTypeDef",
     "BatchGetAssetPropertyValueHistorySuccessEntryTypeDef",
     "BatchGetAssetPropertyValueSuccessEntryTypeDef",
     "GetAssetPropertyValueHistoryResponseTypeDef",
     "GetAssetPropertyValueResponseTypeDef",
-    "GetInterpolatedAssetPropertyValuesResponseTypeDef",
     "PutAssetPropertyValueEntryTypeDef",
+    "GetInterpolatedAssetPropertyValuesResponseTypeDef",
     "DescribeDefaultEncryptionConfigurationResponseTypeDef",
     "PutDefaultEncryptionConfigurationResponseTypeDef",
     "UpdatePortalRequestRequestTypeDef",
     "JobConfigurationOutputTypeDef",
     "JobConfigurationTypeDef",
     "DescribeStorageConfigurationResponseTypeDef",
-    "PutStorageConfigurationResponseTypeDef",
     "PutStorageConfigurationRequestRequestTypeDef",
+    "PutStorageConfigurationResponseTypeDef",
     "AssetModelStatusTypeDef",
     "AssetStatusTypeDef",
-    "MeasurementOutputTypeDef",
-    "TransformOutputTypeDef",
     "MeasurementTypeDef",
+    "TransformOutputTypeDef",
     "TransformTypeDef",
+    "CreateGatewayRequestRequestTypeDef",
     "DescribeGatewayResponseTypeDef",
     "GatewaySummaryTypeDef",
-    "CreateGatewayRequestRequestTypeDef",
     "MetricOutputTypeDef",
     "MetricTypeDef",
     "CreatePortalResponseTypeDef",
     "DeletePortalResponseTypeDef",
     "DescribePortalResponseTypeDef",
     "PortalSummaryTypeDef",
     "UpdatePortalResponseTypeDef",
     "AccessPolicySummaryTypeDef",
-    "DescribeAccessPolicyResponseTypeDef",
     "CreateAccessPolicyRequestRequestTypeDef",
+    "DescribeAccessPolicyResponseTypeDef",
     "UpdateAccessPolicyRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesResponseTypeDef",
     "BatchPutAssetPropertyValueResponseTypeDef",
     "BatchGetAssetPropertyValueHistoryResponseTypeDef",
     "BatchGetAssetPropertyValueResponseTypeDef",
     "BatchPutAssetPropertyValueRequestRequestTypeDef",
     "DescribeBulkImportJobResponseTypeDef",
@@ -368,33 +336,14 @@
         "minimum": float,
         "sum": float,
         "standardDeviation": float,
     },
     total=False,
 )
 
-_RequiredAlarmsOutputTypeDef = TypedDict(
-    "_RequiredAlarmsOutputTypeDef",
-    {
-        "alarmRoleArn": str,
-    },
-)
-_OptionalAlarmsOutputTypeDef = TypedDict(
-    "_OptionalAlarmsOutputTypeDef",
-    {
-        "notificationLambdaArn": str,
-    },
-    total=False,
-)
-
-
-class AlarmsOutputTypeDef(_RequiredAlarmsOutputTypeDef, _OptionalAlarmsOutputTypeDef):
-    pass
-
-
 _RequiredAlarmsTypeDef = TypedDict(
     "_RequiredAlarmsTypeDef",
     {
         "alarmRoleArn": str,
     },
 )
 _OptionalAlarmsTypeDef = TypedDict(
@@ -451,36 +400,14 @@
     "AssetModelHierarchyDefinitionTypeDef",
     {
         "name": str,
         "childAssetModelId": str,
     },
 )
 
-_RequiredAssetModelHierarchyOutputTypeDef = TypedDict(
-    "_RequiredAssetModelHierarchyOutputTypeDef",
-    {
-        "name": str,
-        "childAssetModelId": str,
-    },
-)
-_OptionalAssetModelHierarchyOutputTypeDef = TypedDict(
-    "_OptionalAssetModelHierarchyOutputTypeDef",
-    {
-        "id": str,
-    },
-    total=False,
-)
-
-
-class AssetModelHierarchyOutputTypeDef(
-    _RequiredAssetModelHierarchyOutputTypeDef, _OptionalAssetModelHierarchyOutputTypeDef
-):
-    pass
-
-
 _RequiredAssetModelHierarchyTypeDef = TypedDict(
     "_RequiredAssetModelHierarchyTypeDef",
     {
         "name": str,
         "childAssetModelId": str,
     },
 )
@@ -503,46 +430,14 @@
     "PropertyNotificationTypeDef",
     {
         "topic": str,
         "state": PropertyNotificationStateType,
     },
 )
 
-_RequiredTimeInNanosOutputTypeDef = TypedDict(
-    "_RequiredTimeInNanosOutputTypeDef",
-    {
-        "timeInSeconds": int,
-    },
-)
-_OptionalTimeInNanosOutputTypeDef = TypedDict(
-    "_OptionalTimeInNanosOutputTypeDef",
-    {
-        "offsetInNanos": int,
-    },
-    total=False,
-)
-
-
-class TimeInNanosOutputTypeDef(
-    _RequiredTimeInNanosOutputTypeDef, _OptionalTimeInNanosOutputTypeDef
-):
-    pass
-
-
-VariantOutputTypeDef = TypedDict(
-    "VariantOutputTypeDef",
-    {
-        "stringValue": str,
-        "integerValue": int,
-        "doubleValue": float,
-        "booleanValue": bool,
-    },
-    total=False,
-)
-
 _RequiredTimeInNanosTypeDef = TypedDict(
     "_RequiredTimeInNanosTypeDef",
     {
         "timeInSeconds": int,
     },
 )
 _OptionalTimeInNanosTypeDef = TypedDict(
@@ -612,22 +507,14 @@
 class AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef(
     _RequiredAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
     _OptionalAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
 ):
     pass
 
 
-AttributeOutputTypeDef = TypedDict(
-    "AttributeOutputTypeDef",
-    {
-        "defaultValue": str,
-    },
-    total=False,
-)
-
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "defaultValue": str,
     },
     total=False,
 )
@@ -651,14 +538,25 @@
 class BatchAssociateProjectAssetsRequestRequestTypeDef(
     _RequiredBatchAssociateProjectAssetsRequestRequestTypeDef,
     _OptionalBatchAssociateProjectAssetsRequestRequestTypeDef,
 ):
     pass
 
 
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
 _RequiredBatchDisassociateProjectAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDisassociateProjectAssetsRequestRequestTypeDef",
     {
         "projectId": str,
         "assetIds": Sequence[str],
     },
 )
@@ -814,23 +712,14 @@
     "ConfigurationErrorDetailsTypeDef",
     {
         "code": ErrorCodeType,
         "message": str,
     },
 )
 
-CreateAccessPolicyResponseTypeDef = TypedDict(
-    "CreateAccessPolicyResponseTypeDef",
-    {
-        "accessPolicyId": str,
-        "accessPolicyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateAssetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssetRequestRequestTypeDef",
     {
         "assetName": str,
         "assetModelId": str,
     },
 )
@@ -875,24 +764,14 @@
 )
 
 
 class FileTypeDef(_RequiredFileTypeDef, _OptionalFileTypeDef):
     pass
 
 
-CreateBulkImportJobResponseTypeDef = TypedDict(
-    "CreateBulkImportJobResponseTypeDef",
-    {
-        "jobId": str,
-        "jobName": str,
-        "jobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateDashboardRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDashboardRequestRequestTypeDef",
     {
         "projectId": str,
         "dashboardName": str,
         "dashboardDefinition": str,
     },
@@ -910,32 +789,14 @@
 
 class CreateDashboardRequestRequestTypeDef(
     _RequiredCreateDashboardRequestRequestTypeDef, _OptionalCreateDashboardRequestRequestTypeDef
 ):
     pass
 
 
-CreateDashboardResponseTypeDef = TypedDict(
-    "CreateDashboardResponseTypeDef",
-    {
-        "dashboardId": str,
-        "dashboardArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateGatewayResponseTypeDef = TypedDict(
-    "CreateGatewayResponseTypeDef",
-    {
-        "gatewayId": str,
-        "gatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImageFileTypeDef = TypedDict(
     "ImageFileTypeDef",
     {
         "data": Union[str, bytes, IO[Any], StreamingBody],
         "type": Literal["PNG"],
     },
 )
@@ -960,23 +821,14 @@
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "projectId": str,
-        "projectArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CsvOutputTypeDef = TypedDict(
     "CsvOutputTypeDef",
     {
         "columnNames": List[ColumnNameType],
     },
     total=False,
 )
@@ -985,22 +837,14 @@
     "CsvTypeDef",
     {
         "columnNames": Sequence[ColumnNameType],
     },
     total=False,
 )
 
-CustomerManagedS3StorageOutputTypeDef = TypedDict(
-    "CustomerManagedS3StorageOutputTypeDef",
-    {
-        "s3ResourceArn": str,
-        "roleArn": str,
-    },
-)
-
 CustomerManagedS3StorageTypeDef = TypedDict(
     "CustomerManagedS3StorageTypeDef",
     {
         "s3ResourceArn": str,
         "roleArn": str,
     },
 )
@@ -1242,83 +1086,29 @@
 DescribeBulkImportJobRequestRequestTypeDef = TypedDict(
     "DescribeBulkImportJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
-ErrorReportLocationOutputTypeDef = TypedDict(
-    "ErrorReportLocationOutputTypeDef",
-    {
-        "bucket": str,
-        "prefix": str,
-    },
-)
-
-_RequiredFileOutputTypeDef = TypedDict(
-    "_RequiredFileOutputTypeDef",
-    {
-        "bucket": str,
-        "key": str,
-    },
-)
-_OptionalFileOutputTypeDef = TypedDict(
-    "_OptionalFileOutputTypeDef",
-    {
-        "versionId": str,
-    },
-    total=False,
-)
-
-
-class FileOutputTypeDef(_RequiredFileOutputTypeDef, _OptionalFileOutputTypeDef):
-    pass
-
-
 DescribeDashboardRequestRequestTypeDef = TypedDict(
     "DescribeDashboardRequestRequestTypeDef",
     {
         "dashboardId": str,
     },
 )
 
-DescribeDashboardResponseTypeDef = TypedDict(
-    "DescribeDashboardResponseTypeDef",
-    {
-        "dashboardId": str,
-        "dashboardArn": str,
-        "dashboardName": str,
-        "projectId": str,
-        "dashboardDescription": str,
-        "dashboardDefinition": str,
-        "dashboardCreationDate": datetime,
-        "dashboardLastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeGatewayCapabilityConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeGatewayCapabilityConfigurationRequestRequestTypeDef",
     {
         "gatewayId": str,
         "capabilityNamespace": str,
     },
 )
 
-DescribeGatewayCapabilityConfigurationResponseTypeDef = TypedDict(
-    "DescribeGatewayCapabilityConfigurationResponseTypeDef",
-    {
-        "gatewayId": str,
-        "capabilityNamespace": str,
-        "capabilityConfiguration": str,
-        "capabilitySyncStatus": CapabilitySyncStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeGatewayRequestRequestTypeDef = TypedDict(
     "DescribeGatewayRequestRequestTypeDef",
     {
         "gatewayId": str,
     },
 )
 
@@ -1326,16 +1116,16 @@
     "GatewayCapabilitySummaryTypeDef",
     {
         "capabilityNamespace": str,
         "capabilitySyncStatus": CapabilitySyncStatusType,
     },
 )
 
-LoggingOptionsOutputTypeDef = TypedDict(
-    "LoggingOptionsOutputTypeDef",
+LoggingOptionsTypeDef = TypedDict(
+    "LoggingOptionsTypeDef",
     {
         "level": LoggingLevelType,
     },
 )
 
 DescribePortalRequestRequestTypeDef = TypedDict(
     "DescribePortalRequestRequestTypeDef",
@@ -1355,30 +1145,16 @@
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 
-DescribeProjectResponseTypeDef = TypedDict(
-    "DescribeProjectResponseTypeDef",
-    {
-        "projectId": str,
-        "projectArn": str,
-        "projectName": str,
-        "portalId": str,
-        "projectDescription": str,
-        "projectCreationDate": datetime,
-        "projectLastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RetentionPeriodOutputTypeDef = TypedDict(
-    "RetentionPeriodOutputTypeDef",
+RetentionPeriodTypeDef = TypedDict(
+    "RetentionPeriodTypeDef",
     {
         "numberOfDays": int,
         "unlimited": bool,
     },
     total=False,
 )
 
@@ -1388,30 +1164,14 @@
         "alias": str,
         "assetId": str,
         "propertyId": str,
     },
     total=False,
 )
 
-DescribeTimeSeriesResponseTypeDef = TypedDict(
-    "DescribeTimeSeriesResponseTypeDef",
-    {
-        "assetId": str,
-        "propertyId": str,
-        "alias": str,
-        "timeSeriesId": str,
-        "dataType": PropertyDataTypeType,
-        "dataTypeSpec": str,
-        "timeSeriesCreationDate": datetime,
-        "timeSeriesLastUpdateDate": datetime,
-        "timeSeriesArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DetailedErrorTypeDef = TypedDict(
     "DetailedErrorTypeDef",
     {
         "code": DetailedErrorCodeType,
         "message": str,
     },
 )
@@ -1460,42 +1220,14 @@
 class DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef(
     _RequiredDisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
     _OptionalDisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredVariableValueOutputTypeDef = TypedDict(
-    "_RequiredVariableValueOutputTypeDef",
-    {
-        "propertyId": str,
-    },
-)
-_OptionalVariableValueOutputTypeDef = TypedDict(
-    "_OptionalVariableValueOutputTypeDef",
-    {
-        "hierarchyId": str,
-    },
-    total=False,
-)
-
-
-class VariableValueOutputTypeDef(
-    _RequiredVariableValueOutputTypeDef, _OptionalVariableValueOutputTypeDef
-):
-    pass
-
-
 _RequiredVariableValueTypeDef = TypedDict(
     "_RequiredVariableValueTypeDef",
     {
         "propertyId": str,
     },
 )
 _OptionalVariableValueTypeDef = TypedDict(
@@ -1507,86 +1239,45 @@
 )
 
 
 class VariableValueTypeDef(_RequiredVariableValueTypeDef, _OptionalVariableValueTypeDef):
     pass
 
 
-ForwardingConfigOutputTypeDef = TypedDict(
-    "ForwardingConfigOutputTypeDef",
-    {
-        "state": ForwardingConfigStateType,
-    },
-)
-
 ForwardingConfigTypeDef = TypedDict(
     "ForwardingConfigTypeDef",
     {
         "state": ForwardingConfigStateType,
     },
 )
 
-GreengrassOutputTypeDef = TypedDict(
-    "GreengrassOutputTypeDef",
-    {
-        "groupArn": str,
-    },
-)
-
-GreengrassV2OutputTypeDef = TypedDict(
-    "GreengrassV2OutputTypeDef",
-    {
-        "coreDeviceThingName": str,
-    },
-)
-
 GreengrassTypeDef = TypedDict(
     "GreengrassTypeDef",
     {
         "groupArn": str,
     },
 )
 
 GreengrassV2TypeDef = TypedDict(
     "GreengrassV2TypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 
-_RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef = TypedDict(
-    "_RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
-    {
-        "aggregateTypes": Sequence[AggregateTypeType],
-        "resolution": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-    },
-)
-_OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef = TypedDict(
-    "_OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "qualities": Sequence[QualityType],
-        "timeOrdering": TimeOrderingType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef(
-    _RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
-    _OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAssetPropertyAggregatesRequestRequestTypeDef",
     {
         "aggregateTypes": Sequence[AggregateTypeType],
         "resolution": str,
         "startDate": Union[datetime, str],
         "endDate": Union[datetime, str],
@@ -1610,29 +1301,14 @@
 class GetAssetPropertyAggregatesRequestRequestTypeDef(
     _RequiredGetAssetPropertyAggregatesRequestRequestTypeDef,
     _OptionalGetAssetPropertyAggregatesRequestRequestTypeDef,
 ):
     pass
 
 
-GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef = TypedDict(
-    "GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef",
-    {
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-        "qualities": Sequence[QualityType],
-        "timeOrdering": TimeOrderingType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "GetAssetPropertyValueHistoryRequestRequestTypeDef",
     {
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
         "startDate": Union[datetime, str],
@@ -1651,46 +1327,14 @@
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
     },
     total=False,
 )
 
-_RequiredGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef = TypedDict(
-    "_RequiredGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef",
-    {
-        "startTimeInSeconds": int,
-        "endTimeInSeconds": int,
-        "quality": QualityType,
-        "intervalInSeconds": int,
-        "type": str,
-    },
-)
-_OptionalGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef = TypedDict(
-    "_OptionalGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef",
-    {
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "startTimeOffsetInNanos": int,
-        "endTimeOffsetInNanos": int,
-        "intervalWindowInSeconds": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef(
-    _RequiredGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
-    _OptionalGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetInterpolatedAssetPropertyValuesRequestRequestTypeDef = TypedDict(
     "_RequiredGetInterpolatedAssetPropertyValuesRequestRequestTypeDef",
     {
         "startTimeInSeconds": int,
         "endTimeInSeconds": int,
         "quality": QualityType,
         "intervalInSeconds": int,
@@ -1716,63 +1360,35 @@
 class GetInterpolatedAssetPropertyValuesRequestRequestTypeDef(
     _RequiredGetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
     _OptionalGetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
 ):
     pass
 
 
-GroupIdentityOutputTypeDef = TypedDict(
-    "GroupIdentityOutputTypeDef",
-    {
-        "id": str,
-    },
-)
-
 GroupIdentityTypeDef = TypedDict(
     "GroupIdentityTypeDef",
     {
         "id": str,
     },
 )
 
-IAMRoleIdentityOutputTypeDef = TypedDict(
-    "IAMRoleIdentityOutputTypeDef",
-    {
-        "arn": str,
-    },
-)
-
 IAMRoleIdentityTypeDef = TypedDict(
     "IAMRoleIdentityTypeDef",
     {
         "arn": str,
     },
 )
 
-IAMUserIdentityOutputTypeDef = TypedDict(
-    "IAMUserIdentityOutputTypeDef",
-    {
-        "arn": str,
-    },
-)
-
 IAMUserIdentityTypeDef = TypedDict(
     "IAMUserIdentityTypeDef",
     {
         "arn": str,
     },
 )
 
-UserIdentityOutputTypeDef = TypedDict(
-    "UserIdentityOutputTypeDef",
-    {
-        "id": str,
-    },
-)
-
 UserIdentityTypeDef = TypedDict(
     "UserIdentityTypeDef",
     {
         "id": str,
     },
 )
 
@@ -1781,64 +1397,28 @@
     {
         "id": str,
         "name": str,
         "status": JobStatusType,
     },
 )
 
-ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef = TypedDict(
-    "ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef",
-    {
-        "identityType": IdentityTypeType,
-        "identityId": str,
-        "resourceType": ResourceTypeType,
-        "resourceId": str,
-        "iamArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAccessPoliciesRequestRequestTypeDef = TypedDict(
     "ListAccessPoliciesRequestRequestTypeDef",
     {
         "identityType": IdentityTypeType,
         "identityId": str,
         "resourceType": ResourceTypeType,
         "resourceId": str,
         "iamArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef = TypedDict(
-    "_RequiredListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef",
-    {
-        "assetModelId": str,
-    },
-)
-_OptionalListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef = TypedDict(
-    "_OptionalListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef",
-    {
-        "filter": ListAssetModelPropertiesFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef(
-    _RequiredListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
-    _OptionalListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssetModelPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredListAssetModelPropertiesRequestRequestTypeDef",
     {
         "assetModelId": str,
     },
 )
 _OptionalListAssetModelPropertiesRequestRequestTypeDef = TypedDict(
@@ -1855,54 +1435,23 @@
 class ListAssetModelPropertiesRequestRequestTypeDef(
     _RequiredListAssetModelPropertiesRequestRequestTypeDef,
     _OptionalListAssetModelPropertiesRequestRequestTypeDef,
 ):
     pass
 
 
-ListAssetModelsRequestListAssetModelsPaginateTypeDef = TypedDict(
-    "ListAssetModelsRequestListAssetModelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAssetModelsRequestRequestTypeDef = TypedDict(
     "ListAssetModelsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef = TypedDict(
-    "_RequiredListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef",
-    {
-        "assetId": str,
-    },
-)
-_OptionalListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef = TypedDict(
-    "_OptionalListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef",
-    {
-        "filter": ListAssetPropertiesFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef(
-    _RequiredListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
-    _OptionalListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssetPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredListAssetPropertiesRequestRequestTypeDef",
     {
         "assetId": str,
     },
 )
 _OptionalListAssetPropertiesRequestRequestTypeDef = TypedDict(
@@ -1919,37 +1468,14 @@
 class ListAssetPropertiesRequestRequestTypeDef(
     _RequiredListAssetPropertiesRequestRequestTypeDef,
     _OptionalListAssetPropertiesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef = TypedDict(
-    "_RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
-    {
-        "assetId": str,
-        "traversalType": Literal["PATH_TO_ROOT"],
-    },
-)
-_OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef = TypedDict(
-    "_OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef(
-    _RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
-    _OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssetRelationshipsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssetRelationshipsRequestRequestTypeDef",
     {
         "assetId": str,
         "traversalType": Literal["PATH_TO_ROOT"],
     },
 )
@@ -1966,59 +1492,25 @@
 class ListAssetRelationshipsRequestRequestTypeDef(
     _RequiredListAssetRelationshipsRequestRequestTypeDef,
     _OptionalListAssetRelationshipsRequestRequestTypeDef,
 ):
     pass
 
 
-ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
-    "ListAssetsRequestListAssetsPaginateTypeDef",
-    {
-        "assetModelId": str,
-        "filter": ListAssetsFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAssetsRequestRequestTypeDef = TypedDict(
     "ListAssetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "assetModelId": str,
         "filter": ListAssetsFilterType,
     },
     total=False,
 )
 
-_RequiredListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef",
-    {
-        "assetId": str,
-    },
-)
-_OptionalListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef",
-    {
-        "hierarchyId": str,
-        "traversalDirection": TraversalDirectionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef(
-    _RequiredListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
-    _OptionalListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssociatedAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedAssetsRequestRequestTypeDef",
     {
         "assetId": str,
     },
 )
 _OptionalListAssociatedAssetsRequestRequestTypeDef = TypedDict(
@@ -2036,55 +1528,24 @@
 class ListAssociatedAssetsRequestRequestTypeDef(
     _RequiredListAssociatedAssetsRequestRequestTypeDef,
     _OptionalListAssociatedAssetsRequestRequestTypeDef,
 ):
     pass
 
 
-ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef = TypedDict(
-    "ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef",
-    {
-        "filter": ListBulkImportJobsFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBulkImportJobsRequestRequestTypeDef = TypedDict(
     "ListBulkImportJobsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filter": ListBulkImportJobsFilterType,
     },
     total=False,
 )
 
-_RequiredListDashboardsRequestListDashboardsPaginateTypeDef = TypedDict(
-    "_RequiredListDashboardsRequestListDashboardsPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListDashboardsRequestListDashboardsPaginateTypeDef = TypedDict(
-    "_OptionalListDashboardsRequestListDashboardsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDashboardsRequestListDashboardsPaginateTypeDef(
-    _RequiredListDashboardsRequestListDashboardsPaginateTypeDef,
-    _OptionalListDashboardsRequestListDashboardsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDashboardsRequestRequestTypeDef = TypedDict(
     "_RequiredListDashboardsRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalListDashboardsRequestRequestTypeDef = TypedDict(
@@ -2099,70 +1560,32 @@
 
 class ListDashboardsRequestRequestTypeDef(
     _RequiredListDashboardsRequestRequestTypeDef, _OptionalListDashboardsRequestRequestTypeDef
 ):
     pass
 
 
-ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
-    "ListGatewaysRequestListGatewaysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGatewaysRequestRequestTypeDef = TypedDict(
     "ListGatewaysRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListPortalsRequestListPortalsPaginateTypeDef = TypedDict(
-    "ListPortalsRequestListPortalsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPortalsRequestRequestTypeDef = TypedDict(
     "ListPortalsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListProjectAssetsRequestListProjectAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListProjectAssetsRequestListProjectAssetsPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListProjectAssetsRequestListProjectAssetsPaginateTypeDef(
-    _RequiredListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
-    _OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListProjectAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectAssetsRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalListProjectAssetsRequestRequestTypeDef = TypedDict(
@@ -2177,45 +1600,14 @@
 
 class ListProjectAssetsRequestRequestTypeDef(
     _RequiredListProjectAssetsRequestRequestTypeDef, _OptionalListProjectAssetsRequestRequestTypeDef
 ):
     pass
 
 
-ListProjectAssetsResponseTypeDef = TypedDict(
-    "ListProjectAssetsResponseTypeDef",
-    {
-        "assetIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "_RequiredListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "portalId": str,
-    },
-)
-_OptionalListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "_OptionalListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListProjectsRequestListProjectsPaginateTypeDef(
-    _RequiredListProjectsRequestListProjectsPaginateTypeDef,
-    _OptionalListProjectsRequestListProjectsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListProjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectsRequestRequestTypeDef",
     {
         "portalId": str,
     },
 )
 _OptionalListProjectsRequestRequestTypeDef = TypedDict(
@@ -2259,33 +1651,14 @@
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
-ListTimeSeriesRequestListTimeSeriesPaginateTypeDef = TypedDict(
-    "ListTimeSeriesRequestListTimeSeriesPaginateTypeDef",
-    {
-        "assetId": str,
-        "aliasPrefix": str,
-        "timeSeriesType": ListTimeSeriesTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTimeSeriesRequestRequestTypeDef = TypedDict(
     "ListTimeSeriesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "assetId": str,
         "aliasPrefix": str,
@@ -2318,56 +1691,21 @@
 
 class TimeSeriesSummaryTypeDef(
     _RequiredTimeSeriesSummaryTypeDef, _OptionalTimeSeriesSummaryTypeDef
 ):
     pass
 
 
-LoggingOptionsTypeDef = TypedDict(
-    "LoggingOptionsTypeDef",
-    {
-        "level": LoggingLevelType,
-    },
-)
-
-MetricProcessingConfigOutputTypeDef = TypedDict(
-    "MetricProcessingConfigOutputTypeDef",
-    {
-        "computeLocation": ComputeLocationType,
-    },
-)
-
 MetricProcessingConfigTypeDef = TypedDict(
     "MetricProcessingConfigTypeDef",
     {
         "computeLocation": ComputeLocationType,
     },
 )
 
-_RequiredTumblingWindowOutputTypeDef = TypedDict(
-    "_RequiredTumblingWindowOutputTypeDef",
-    {
-        "interval": str,
-    },
-)
-_OptionalTumblingWindowOutputTypeDef = TypedDict(
-    "_OptionalTumblingWindowOutputTypeDef",
-    {
-        "offset": str,
-    },
-    total=False,
-)
-
-
-class TumblingWindowOutputTypeDef(
-    _RequiredTumblingWindowOutputTypeDef, _OptionalTumblingWindowOutputTypeDef
-):
-    pass
-
-
 _RequiredTumblingWindowTypeDef = TypedDict(
     "_RequiredTumblingWindowTypeDef",
     {
         "interval": str,
     },
 )
 _OptionalTumblingWindowTypeDef = TypedDict(
@@ -2388,45 +1726,21 @@
     {
         "code": MonitorErrorCodeType,
         "message": str,
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
-PortalResourceOutputTypeDef = TypedDict(
-    "PortalResourceOutputTypeDef",
-    {
-        "id": str,
-    },
-)
-
 PortalResourceTypeDef = TypedDict(
     "PortalResourceTypeDef",
     {
         "id": str,
     },
 )
 
-ProjectResourceOutputTypeDef = TypedDict(
-    "ProjectResourceOutputTypeDef",
-    {
-        "id": str,
-    },
-)
-
 ProjectResourceTypeDef = TypedDict(
     "ProjectResourceTypeDef",
     {
         "id": str,
     },
 )
 
@@ -2448,34 +1762,14 @@
 class PutDefaultEncryptionConfigurationRequestRequestTypeDef(
     _RequiredPutDefaultEncryptionConfigurationRequestRequestTypeDef,
     _OptionalPutDefaultEncryptionConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-RetentionPeriodTypeDef = TypedDict(
-    "RetentionPeriodTypeDef",
-    {
-        "numberOfDays": int,
-        "unlimited": bool,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -2566,23 +1860,14 @@
     {
         "gatewayId": str,
         "capabilityNamespace": str,
         "capabilityConfiguration": str,
     },
 )
 
-UpdateGatewayCapabilityConfigurationResponseTypeDef = TypedDict(
-    "UpdateGatewayCapabilityConfigurationResponseTypeDef",
-    {
-        "capabilityNamespace": str,
-        "capabilitySyncStatus": CapabilitySyncStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateGatewayRequestRequestTypeDef = TypedDict(
     "UpdateGatewayRequestRequestTypeDef",
     {
         "gatewayId": str,
         "gatewayName": str,
     },
 )
@@ -2626,30 +1911,14 @@
 )
 
 
 class AggregatedValueTypeDef(_RequiredAggregatedValueTypeDef, _OptionalAggregatedValueTypeDef):
     pass
 
 
-BatchAssociateProjectAssetsResponseTypeDef = TypedDict(
-    "BatchAssociateProjectAssetsResponseTypeDef",
-    {
-        "errors": List[AssetErrorDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchDisassociateProjectAssetsResponseTypeDef = TypedDict(
-    "BatchDisassociateProjectAssetsResponseTypeDef",
-    {
-        "errors": List[AssetErrorDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssetRelationshipSummaryTypeDef = TypedDict(
     "_RequiredAssetRelationshipSummaryTypeDef",
     {
         "relationshipType": Literal["HIERARCHY"],
     },
 )
 _OptionalAssetRelationshipSummaryTypeDef = TypedDict(
@@ -2704,69 +1973,198 @@
 
 
 BatchPutAssetPropertyErrorTypeDef = TypedDict(
     "BatchPutAssetPropertyErrorTypeDef",
     {
         "errorCode": BatchPutAssetPropertyValueErrorCodeType,
         "errorMessage": str,
-        "timestamps": List[TimeInNanosOutputTypeDef],
+        "timestamps": List[TimeInNanosTypeDef],
     },
 )
 
-_RequiredAssetPropertyValueOutputTypeDef = TypedDict(
-    "_RequiredAssetPropertyValueOutputTypeDef",
+_RequiredAssetPropertyValueTypeDef = TypedDict(
+    "_RequiredAssetPropertyValueTypeDef",
     {
-        "value": VariantOutputTypeDef,
-        "timestamp": TimeInNanosOutputTypeDef,
+        "value": VariantTypeDef,
+        "timestamp": TimeInNanosTypeDef,
     },
 )
-_OptionalAssetPropertyValueOutputTypeDef = TypedDict(
-    "_OptionalAssetPropertyValueOutputTypeDef",
+_OptionalAssetPropertyValueTypeDef = TypedDict(
+    "_OptionalAssetPropertyValueTypeDef",
     {
         "quality": QualityType,
     },
     total=False,
 )
 
 
-class AssetPropertyValueOutputTypeDef(
-    _RequiredAssetPropertyValueOutputTypeDef, _OptionalAssetPropertyValueOutputTypeDef
+class AssetPropertyValueTypeDef(
+    _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
 ):
     pass
 
 
 InterpolatedAssetPropertyValueTypeDef = TypedDict(
     "InterpolatedAssetPropertyValueTypeDef",
     {
-        "timestamp": TimeInNanosOutputTypeDef,
-        "value": VariantOutputTypeDef,
+        "timestamp": TimeInNanosTypeDef,
+        "value": VariantTypeDef,
     },
 )
 
-_RequiredAssetPropertyValueTypeDef = TypedDict(
-    "_RequiredAssetPropertyValueTypeDef",
+BatchAssociateProjectAssetsResponseTypeDef = TypedDict(
+    "BatchAssociateProjectAssetsResponseTypeDef",
     {
-        "value": VariantTypeDef,
-        "timestamp": TimeInNanosTypeDef,
+        "errors": List[AssetErrorDetailsTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAssetPropertyValueTypeDef = TypedDict(
-    "_OptionalAssetPropertyValueTypeDef",
+
+BatchDisassociateProjectAssetsResponseTypeDef = TypedDict(
+    "BatchDisassociateProjectAssetsResponseTypeDef",
     {
-        "quality": QualityType,
+        "errors": List[AssetErrorDetailsTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+CreateAccessPolicyResponseTypeDef = TypedDict(
+    "CreateAccessPolicyResponseTypeDef",
+    {
+        "accessPolicyId": str,
+        "accessPolicyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class AssetPropertyValueTypeDef(
-    _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
-):
-    pass
+CreateBulkImportJobResponseTypeDef = TypedDict(
+    "CreateBulkImportJobResponseTypeDef",
+    {
+        "jobId": str,
+        "jobName": str,
+        "jobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+CreateDashboardResponseTypeDef = TypedDict(
+    "CreateDashboardResponseTypeDef",
+    {
+        "dashboardId": str,
+        "dashboardArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGatewayResponseTypeDef = TypedDict(
+    "CreateGatewayResponseTypeDef",
+    {
+        "gatewayId": str,
+        "gatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "projectId": str,
+        "projectArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDashboardResponseTypeDef = TypedDict(
+    "DescribeDashboardResponseTypeDef",
+    {
+        "dashboardId": str,
+        "dashboardArn": str,
+        "dashboardName": str,
+        "projectId": str,
+        "dashboardDescription": str,
+        "dashboardDefinition": str,
+        "dashboardCreationDate": datetime,
+        "dashboardLastUpdateDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGatewayCapabilityConfigurationResponseTypeDef = TypedDict(
+    "DescribeGatewayCapabilityConfigurationResponseTypeDef",
+    {
+        "gatewayId": str,
+        "capabilityNamespace": str,
+        "capabilityConfiguration": str,
+        "capabilitySyncStatus": CapabilitySyncStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeProjectResponseTypeDef = TypedDict(
+    "DescribeProjectResponseTypeDef",
+    {
+        "projectId": str,
+        "projectArn": str,
+        "projectName": str,
+        "portalId": str,
+        "projectDescription": str,
+        "projectCreationDate": datetime,
+        "projectLastUpdateDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTimeSeriesResponseTypeDef = TypedDict(
+    "DescribeTimeSeriesResponseTypeDef",
+    {
+        "assetId": str,
+        "propertyId": str,
+        "alias": str,
+        "timeSeriesId": str,
+        "dataType": PropertyDataTypeType,
+        "dataTypeSpec": str,
+        "timeSeriesCreationDate": datetime,
+        "timeSeriesLastUpdateDate": datetime,
+        "timeSeriesArn": str,
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
+ListProjectAssetsResponseTypeDef = TypedDict(
+    "ListProjectAssetsResponseTypeDef",
+    {
+        "assetIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewayCapabilityConfigurationResponseTypeDef = TypedDict(
+    "UpdateGatewayCapabilityConfigurationResponseTypeDef",
+    {
+        "capabilityNamespace": str,
+        "capabilitySyncStatus": CapabilitySyncStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef",
     {
         "entries": Sequence[BatchGetAssetPropertyAggregatesEntryTypeDef],
     },
 )
@@ -2972,34 +2370,27 @@
     "FileFormatTypeDef",
     {
         "csv": CsvTypeDef,
     },
     total=False,
 )
 
-MultiLayerStorageOutputTypeDef = TypedDict(
-    "MultiLayerStorageOutputTypeDef",
-    {
-        "customerManagedS3Storage": CustomerManagedS3StorageOutputTypeDef,
-    },
-)
-
 MultiLayerStorageTypeDef = TypedDict(
     "MultiLayerStorageTypeDef",
     {
         "customerManagedS3Storage": CustomerManagedS3StorageTypeDef,
     },
 )
 
 ListDashboardsResponseTypeDef = TypedDict(
     "ListDashboardsResponseTypeDef",
     {
         "dashboardSummaries": List[DashboardSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeAssetModelRequestAssetModelActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeAssetModelRequestAssetModelActiveWaitTypeDef",
     {
         "assetModelId": str,
@@ -3134,16 +2525,23 @@
 ):
     pass
 
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
-        "loggingOptions": LoggingOptionsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "loggingOptions": LoggingOptionsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutLoggingOptionsRequestRequestTypeDef = TypedDict(
+    "PutLoggingOptionsRequestRequestTypeDef",
+    {
+        "loggingOptions": LoggingOptionsTypeDef,
     },
 )
 
 _RequiredErrorDetailsTypeDef = TypedDict(
     "_RequiredErrorDetailsTypeDef",
     {
         "code": ErrorCodeType,
@@ -3159,111 +2557,358 @@
 )
 
 
 class ErrorDetailsTypeDef(_RequiredErrorDetailsTypeDef, _OptionalErrorDetailsTypeDef):
     pass
 
 
-ExpressionVariableOutputTypeDef = TypedDict(
-    "ExpressionVariableOutputTypeDef",
-    {
-        "name": str,
-        "value": VariableValueOutputTypeDef,
-    },
-)
-
 ExpressionVariableTypeDef = TypedDict(
     "ExpressionVariableTypeDef",
     {
         "name": str,
         "value": VariableValueTypeDef,
     },
 )
 
-MeasurementProcessingConfigOutputTypeDef = TypedDict(
-    "MeasurementProcessingConfigOutputTypeDef",
+MeasurementProcessingConfigTypeDef = TypedDict(
+    "MeasurementProcessingConfigTypeDef",
     {
-        "forwardingConfig": ForwardingConfigOutputTypeDef,
+        "forwardingConfig": ForwardingConfigTypeDef,
     },
 )
 
-_RequiredTransformProcessingConfigOutputTypeDef = TypedDict(
-    "_RequiredTransformProcessingConfigOutputTypeDef",
+_RequiredTransformProcessingConfigTypeDef = TypedDict(
+    "_RequiredTransformProcessingConfigTypeDef",
     {
         "computeLocation": ComputeLocationType,
     },
 )
-_OptionalTransformProcessingConfigOutputTypeDef = TypedDict(
-    "_OptionalTransformProcessingConfigOutputTypeDef",
+_OptionalTransformProcessingConfigTypeDef = TypedDict(
+    "_OptionalTransformProcessingConfigTypeDef",
     {
-        "forwardingConfig": ForwardingConfigOutputTypeDef,
+        "forwardingConfig": ForwardingConfigTypeDef,
     },
     total=False,
 )
 
 
-class TransformProcessingConfigOutputTypeDef(
-    _RequiredTransformProcessingConfigOutputTypeDef, _OptionalTransformProcessingConfigOutputTypeDef
+class TransformProcessingConfigTypeDef(
+    _RequiredTransformProcessingConfigTypeDef, _OptionalTransformProcessingConfigTypeDef
 ):
     pass
 
 
-MeasurementProcessingConfigTypeDef = TypedDict(
-    "MeasurementProcessingConfigTypeDef",
+GatewayPlatformTypeDef = TypedDict(
+    "GatewayPlatformTypeDef",
     {
-        "forwardingConfig": ForwardingConfigTypeDef,
+        "greengrass": GreengrassTypeDef,
+        "greengrassV2": GreengrassV2TypeDef,
     },
+    total=False,
 )
 
-_RequiredTransformProcessingConfigTypeDef = TypedDict(
-    "_RequiredTransformProcessingConfigTypeDef",
+_RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef = TypedDict(
+    "_RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
     {
-        "computeLocation": ComputeLocationType,
+        "aggregateTypes": Sequence[AggregateTypeType],
+        "resolution": str,
+        "startDate": Union[datetime, str],
+        "endDate": Union[datetime, str],
     },
 )
-_OptionalTransformProcessingConfigTypeDef = TypedDict(
-    "_OptionalTransformProcessingConfigTypeDef",
+_OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef = TypedDict(
+    "_OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
     {
-        "forwardingConfig": ForwardingConfigTypeDef,
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+        "qualities": Sequence[QualityType],
+        "timeOrdering": TimeOrderingType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class TransformProcessingConfigTypeDef(
-    _RequiredTransformProcessingConfigTypeDef, _OptionalTransformProcessingConfigTypeDef
+class GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef(
+    _RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
+    _OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
 ):
     pass
 
 
-GatewayPlatformOutputTypeDef = TypedDict(
-    "GatewayPlatformOutputTypeDef",
+GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef = TypedDict(
+    "GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef",
     {
-        "greengrass": GreengrassOutputTypeDef,
-        "greengrassV2": GreengrassV2OutputTypeDef,
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+        "startDate": Union[datetime, str],
+        "endDate": Union[datetime, str],
+        "qualities": Sequence[QualityType],
+        "timeOrdering": TimeOrderingType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-GatewayPlatformTypeDef = TypedDict(
-    "GatewayPlatformTypeDef",
+_RequiredGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef = TypedDict(
+    "_RequiredGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef",
     {
-        "greengrass": GreengrassTypeDef,
-        "greengrassV2": GreengrassV2TypeDef,
+        "startTimeInSeconds": int,
+        "endTimeInSeconds": int,
+        "quality": QualityType,
+        "intervalInSeconds": int,
+        "type": str,
+    },
+)
+_OptionalGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef = TypedDict(
+    "_OptionalGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef",
+    {
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+        "startTimeOffsetInNanos": int,
+        "endTimeOffsetInNanos": int,
+        "intervalWindowInSeconds": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-IdentityOutputTypeDef = TypedDict(
-    "IdentityOutputTypeDef",
+
+class GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef(
+    _RequiredGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
+    _OptionalGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
+):
+    pass
+
+
+ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef = TypedDict(
+    "ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef",
     {
-        "user": UserIdentityOutputTypeDef,
-        "group": GroupIdentityOutputTypeDef,
-        "iamUser": IAMUserIdentityOutputTypeDef,
-        "iamRole": IAMRoleIdentityOutputTypeDef,
+        "identityType": IdentityTypeType,
+        "identityId": str,
+        "resourceType": ResourceTypeType,
+        "resourceId": str,
+        "iamArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef = TypedDict(
+    "_RequiredListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef",
+    {
+        "assetModelId": str,
+    },
+)
+_OptionalListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef = TypedDict(
+    "_OptionalListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef",
+    {
+        "filter": ListAssetModelPropertiesFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef(
+    _RequiredListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
+    _OptionalListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
+):
+    pass
+
+
+ListAssetModelsRequestListAssetModelsPaginateTypeDef = TypedDict(
+    "ListAssetModelsRequestListAssetModelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef = TypedDict(
+    "_RequiredListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef",
+    {
+        "assetId": str,
+    },
+)
+_OptionalListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef = TypedDict(
+    "_OptionalListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef",
+    {
+        "filter": ListAssetPropertiesFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef(
+    _RequiredListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
+    _OptionalListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef = TypedDict(
+    "_RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
+    {
+        "assetId": str,
+        "traversalType": Literal["PATH_TO_ROOT"],
+    },
+)
+_OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef = TypedDict(
+    "_OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef(
+    _RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
+    _OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
+):
+    pass
+
+
+ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
+    "ListAssetsRequestListAssetsPaginateTypeDef",
+    {
+        "assetModelId": str,
+        "filter": ListAssetsFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef",
+    {
+        "assetId": str,
+    },
+)
+_OptionalListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef",
+    {
+        "hierarchyId": str,
+        "traversalDirection": TraversalDirectionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef(
+    _RequiredListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
+    _OptionalListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
+):
+    pass
+
+
+ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef = TypedDict(
+    "ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef",
+    {
+        "filter": ListBulkImportJobsFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDashboardsRequestListDashboardsPaginateTypeDef = TypedDict(
+    "_RequiredListDashboardsRequestListDashboardsPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListDashboardsRequestListDashboardsPaginateTypeDef = TypedDict(
+    "_OptionalListDashboardsRequestListDashboardsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDashboardsRequestListDashboardsPaginateTypeDef(
+    _RequiredListDashboardsRequestListDashboardsPaginateTypeDef,
+    _OptionalListDashboardsRequestListDashboardsPaginateTypeDef,
+):
+    pass
+
+
+ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPortalsRequestListPortalsPaginateTypeDef = TypedDict(
+    "ListPortalsRequestListPortalsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListProjectAssetsRequestListProjectAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListProjectAssetsRequestListProjectAssetsPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListProjectAssetsRequestListProjectAssetsPaginateTypeDef(
+    _RequiredListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
+    _OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "_RequiredListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "portalId": str,
+    },
+)
+_OptionalListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "_OptionalListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListProjectsRequestListProjectsPaginateTypeDef(
+    _RequiredListProjectsRequestListProjectsPaginateTypeDef,
+    _OptionalListProjectsRequestListProjectsPaginateTypeDef,
+):
+    pass
+
+
+ListTimeSeriesRequestListTimeSeriesPaginateTypeDef = TypedDict(
+    "ListTimeSeriesRequestListTimeSeriesPaginateTypeDef",
+    {
+        "assetId": str,
+        "aliasPrefix": str,
+        "timeSeriesType": ListTimeSeriesTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 IdentityTypeDef = TypedDict(
     "IdentityTypeDef",
     {
@@ -3276,51 +2921,36 @@
 )
 
 ListBulkImportJobsResponseTypeDef = TypedDict(
     "ListBulkImportJobsResponseTypeDef",
     {
         "jobSummaries": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "projectSummaries": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTimeSeriesResponseTypeDef = TypedDict(
     "ListTimeSeriesResponseTypeDef",
     {
         "TimeSeriesSummaries": List[TimeSeriesSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutLoggingOptionsRequestRequestTypeDef = TypedDict(
-    "PutLoggingOptionsRequestRequestTypeDef",
-    {
-        "loggingOptions": LoggingOptionsTypeDef,
-    },
-)
-
-MetricWindowOutputTypeDef = TypedDict(
-    "MetricWindowOutputTypeDef",
-    {
-        "tumbling": TumblingWindowOutputTypeDef,
-    },
-    total=False,
-)
-
 MetricWindowTypeDef = TypedDict(
     "MetricWindowTypeDef",
     {
         "tumbling": TumblingWindowTypeDef,
     },
     total=False,
 )
@@ -3340,23 +2970,14 @@
 )
 
 
 class PortalStatusTypeDef(_RequiredPortalStatusTypeDef, _OptionalPortalStatusTypeDef):
     pass
 
 
-ResourceOutputTypeDef = TypedDict(
-    "ResourceOutputTypeDef",
-    {
-        "portal": PortalResourceOutputTypeDef,
-        "project": ProjectResourceOutputTypeDef,
-    },
-    total=False,
-)
-
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "portal": PortalResourceTypeDef,
         "project": ProjectResourceTypeDef,
     },
     total=False,
@@ -3371,33 +2992,33 @@
 )
 
 GetAssetPropertyAggregatesResponseTypeDef = TypedDict(
     "GetAssetPropertyAggregatesResponseTypeDef",
     {
         "aggregatedValues": List[AggregatedValueTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssetRelationshipsResponseTypeDef = TypedDict(
     "ListAssetRelationshipsResponseTypeDef",
     {
         "assetRelationshipSummaries": List[AssetRelationshipSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssetPropertiesResponseTypeDef = TypedDict(
     "ListAssetPropertiesResponseTypeDef",
     {
         "assetPropertySummaries": List[AssetPropertySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssetCompositeModelTypeDef = TypedDict(
     "_RequiredAssetCompositeModelTypeDef",
     {
         "name": str,
@@ -3429,28 +3050,28 @@
     },
 )
 
 BatchGetAssetPropertyValueHistorySuccessEntryTypeDef = TypedDict(
     "BatchGetAssetPropertyValueHistorySuccessEntryTypeDef",
     {
         "entryId": str,
-        "assetPropertyValueHistory": List[AssetPropertyValueOutputTypeDef],
+        "assetPropertyValueHistory": List[AssetPropertyValueTypeDef],
     },
 )
 
 _RequiredBatchGetAssetPropertyValueSuccessEntryTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueSuccessEntryTypeDef",
     {
         "entryId": str,
     },
 )
 _OptionalBatchGetAssetPropertyValueSuccessEntryTypeDef = TypedDict(
     "_OptionalBatchGetAssetPropertyValueSuccessEntryTypeDef",
     {
-        "assetPropertyValue": AssetPropertyValueOutputTypeDef,
+        "assetPropertyValue": AssetPropertyValueTypeDef,
     },
     total=False,
 )
 
 
 class BatchGetAssetPropertyValueSuccessEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueSuccessEntryTypeDef,
@@ -3458,34 +3079,25 @@
 ):
     pass
 
 
 GetAssetPropertyValueHistoryResponseTypeDef = TypedDict(
     "GetAssetPropertyValueHistoryResponseTypeDef",
     {
-        "assetPropertyValueHistory": List[AssetPropertyValueOutputTypeDef],
+        "assetPropertyValueHistory": List[AssetPropertyValueTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssetPropertyValueResponseTypeDef = TypedDict(
     "GetAssetPropertyValueResponseTypeDef",
     {
-        "propertyValue": AssetPropertyValueOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetInterpolatedAssetPropertyValuesResponseTypeDef = TypedDict(
-    "GetInterpolatedAssetPropertyValuesResponseTypeDef",
-    {
-        "interpolatedAssetPropertyValues": List[InterpolatedAssetPropertyValueTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "propertyValue": AssetPropertyValueTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutAssetPropertyValueEntryTypeDef = TypedDict(
     "_RequiredPutAssetPropertyValueEntryTypeDef",
     {
         "entryId": str,
@@ -3505,31 +3117,40 @@
 
 class PutAssetPropertyValueEntryTypeDef(
     _RequiredPutAssetPropertyValueEntryTypeDef, _OptionalPutAssetPropertyValueEntryTypeDef
 ):
     pass
 
 
+GetInterpolatedAssetPropertyValuesResponseTypeDef = TypedDict(
+    "GetInterpolatedAssetPropertyValuesResponseTypeDef",
+    {
+        "interpolatedAssetPropertyValues": List[InterpolatedAssetPropertyValueTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeDefaultEncryptionConfigurationResponseTypeDef = TypedDict(
     "DescribeDefaultEncryptionConfigurationResponseTypeDef",
     {
         "encryptionType": EncryptionTypeType,
         "kmsKeyArn": str,
         "configurationStatus": ConfigurationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDefaultEncryptionConfigurationResponseTypeDef = TypedDict(
     "PutDefaultEncryptionConfigurationResponseTypeDef",
     {
         "encryptionType": EncryptionTypeType,
         "kmsKeyArn": str,
         "configurationStatus": ConfigurationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdatePortalRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePortalRequestRequestTypeDef",
     {
         "portalId": str,
@@ -3571,32 +3192,20 @@
     },
 )
 
 DescribeStorageConfigurationResponseTypeDef = TypedDict(
     "DescribeStorageConfigurationResponseTypeDef",
     {
         "storageType": StorageTypeType,
-        "multiLayerStorage": MultiLayerStorageOutputTypeDef,
+        "multiLayerStorage": MultiLayerStorageTypeDef,
         "disassociatedDataStorage": DisassociatedDataStorageStateType,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
+        "retentionPeriod": RetentionPeriodTypeDef,
         "configurationStatus": ConfigurationStatusTypeDef,
         "lastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutStorageConfigurationResponseTypeDef = TypedDict(
-    "PutStorageConfigurationResponseTypeDef",
-    {
-        "storageType": StorageTypeType,
-        "multiLayerStorage": MultiLayerStorageOutputTypeDef,
-        "disassociatedDataStorage": DisassociatedDataStorageStateType,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
-        "configurationStatus": ConfigurationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutStorageConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutStorageConfigurationRequestRequestTypeDef",
     {
         "storageType": StorageTypeType,
@@ -3616,14 +3225,26 @@
 class PutStorageConfigurationRequestRequestTypeDef(
     _RequiredPutStorageConfigurationRequestRequestTypeDef,
     _OptionalPutStorageConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+PutStorageConfigurationResponseTypeDef = TypedDict(
+    "PutStorageConfigurationResponseTypeDef",
+    {
+        "storageType": StorageTypeType,
+        "multiLayerStorage": MultiLayerStorageTypeDef,
+        "disassociatedDataStorage": DisassociatedDataStorageStateType,
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "configurationStatus": ConfigurationStatusTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredAssetModelStatusTypeDef = TypedDict(
     "_RequiredAssetModelStatusTypeDef",
     {
         "state": AssetModelStateType,
     },
 )
 _OptionalAssetModelStatusTypeDef = TypedDict(
@@ -3654,50 +3275,42 @@
 )
 
 
 class AssetStatusTypeDef(_RequiredAssetStatusTypeDef, _OptionalAssetStatusTypeDef):
     pass
 
 
-MeasurementOutputTypeDef = TypedDict(
-    "MeasurementOutputTypeDef",
+MeasurementTypeDef = TypedDict(
+    "MeasurementTypeDef",
     {
-        "processingConfig": MeasurementProcessingConfigOutputTypeDef,
+        "processingConfig": MeasurementProcessingConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredTransformOutputTypeDef = TypedDict(
     "_RequiredTransformOutputTypeDef",
     {
         "expression": str,
-        "variables": List[ExpressionVariableOutputTypeDef],
+        "variables": List[ExpressionVariableTypeDef],
     },
 )
 _OptionalTransformOutputTypeDef = TypedDict(
     "_OptionalTransformOutputTypeDef",
     {
-        "processingConfig": TransformProcessingConfigOutputTypeDef,
+        "processingConfig": TransformProcessingConfigTypeDef,
     },
     total=False,
 )
 
 
 class TransformOutputTypeDef(_RequiredTransformOutputTypeDef, _OptionalTransformOutputTypeDef):
     pass
 
 
-MeasurementTypeDef = TypedDict(
-    "MeasurementTypeDef",
-    {
-        "processingConfig": MeasurementProcessingConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredTransformTypeDef = TypedDict(
     "_RequiredTransformTypeDef",
     {
         "expression": str,
         "variables": Sequence[ExpressionVariableTypeDef],
     },
 )
@@ -3710,25 +3323,47 @@
 )
 
 
 class TransformTypeDef(_RequiredTransformTypeDef, _OptionalTransformTypeDef):
     pass
 
 
+_RequiredCreateGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateGatewayRequestRequestTypeDef",
+    {
+        "gatewayName": str,
+        "gatewayPlatform": GatewayPlatformTypeDef,
+    },
+)
+_OptionalCreateGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateGatewayRequestRequestTypeDef",
+    {
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateGatewayRequestRequestTypeDef(
+    _RequiredCreateGatewayRequestRequestTypeDef, _OptionalCreateGatewayRequestRequestTypeDef
+):
+    pass
+
+
 DescribeGatewayResponseTypeDef = TypedDict(
     "DescribeGatewayResponseTypeDef",
     {
         "gatewayId": str,
         "gatewayName": str,
         "gatewayArn": str,
-        "gatewayPlatform": GatewayPlatformOutputTypeDef,
+        "gatewayPlatform": GatewayPlatformTypeDef,
         "gatewayCapabilitySummaries": List[GatewayCapabilitySummaryTypeDef],
         "creationDate": datetime,
         "lastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGatewaySummaryTypeDef = TypedDict(
     "_RequiredGatewaySummaryTypeDef",
     {
         "gatewayId": str,
@@ -3736,59 +3371,37 @@
         "creationDate": datetime,
         "lastUpdateDate": datetime,
     },
 )
 _OptionalGatewaySummaryTypeDef = TypedDict(
     "_OptionalGatewaySummaryTypeDef",
     {
-        "gatewayPlatform": GatewayPlatformOutputTypeDef,
+        "gatewayPlatform": GatewayPlatformTypeDef,
         "gatewayCapabilitySummaries": List[GatewayCapabilitySummaryTypeDef],
     },
     total=False,
 )
 
 
 class GatewaySummaryTypeDef(_RequiredGatewaySummaryTypeDef, _OptionalGatewaySummaryTypeDef):
     pass
 
 
-_RequiredCreateGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateGatewayRequestRequestTypeDef",
-    {
-        "gatewayName": str,
-        "gatewayPlatform": GatewayPlatformTypeDef,
-    },
-)
-_OptionalCreateGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateGatewayRequestRequestTypeDef",
-    {
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateGatewayRequestRequestTypeDef(
-    _RequiredCreateGatewayRequestRequestTypeDef, _OptionalCreateGatewayRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredMetricOutputTypeDef = TypedDict(
     "_RequiredMetricOutputTypeDef",
     {
         "expression": str,
-        "variables": List[ExpressionVariableOutputTypeDef],
-        "window": MetricWindowOutputTypeDef,
+        "variables": List[ExpressionVariableTypeDef],
+        "window": MetricWindowTypeDef,
     },
 )
 _OptionalMetricOutputTypeDef = TypedDict(
     "_OptionalMetricOutputTypeDef",
     {
-        "processingConfig": MetricProcessingConfigOutputTypeDef,
+        "processingConfig": MetricProcessingConfigTypeDef,
     },
     total=False,
 )
 
 
 class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
     pass
@@ -3819,23 +3432,23 @@
     "CreatePortalResponseTypeDef",
     {
         "portalId": str,
         "portalArn": str,
         "portalStartUrl": str,
         "portalStatus": PortalStatusTypeDef,
         "ssoApplicationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePortalResponseTypeDef = TypedDict(
     "DeletePortalResponseTypeDef",
     {
         "portalStatus": PortalStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePortalResponseTypeDef = TypedDict(
     "DescribePortalResponseTypeDef",
     {
         "portalId": str,
@@ -3848,16 +3461,16 @@
         "portalStatus": PortalStatusTypeDef,
         "portalCreationDate": datetime,
         "portalLastUpdateDate": datetime,
         "portalLogoImageLocation": ImageLocationTypeDef,
         "roleArn": str,
         "portalAuthMode": AuthModeType,
         "notificationSenderEmail": str,
-        "alarms": AlarmsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "alarms": AlarmsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPortalSummaryTypeDef = TypedDict(
     "_RequiredPortalSummaryTypeDef",
     {
         "id": str,
@@ -3882,24 +3495,24 @@
     pass
 
 
 UpdatePortalResponseTypeDef = TypedDict(
     "UpdatePortalResponseTypeDef",
     {
         "portalStatus": PortalStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAccessPolicySummaryTypeDef = TypedDict(
     "_RequiredAccessPolicySummaryTypeDef",
     {
         "id": str,
-        "identity": IdentityOutputTypeDef,
-        "resource": ResourceOutputTypeDef,
+        "identity": IdentityTypeDef,
+        "resource": ResourceTypeDef,
         "permission": PermissionType,
     },
 )
 _OptionalAccessPolicySummaryTypeDef = TypedDict(
     "_OptionalAccessPolicySummaryTypeDef",
     {
         "creationDate": datetime,
@@ -3911,28 +3524,14 @@
 
 class AccessPolicySummaryTypeDef(
     _RequiredAccessPolicySummaryTypeDef, _OptionalAccessPolicySummaryTypeDef
 ):
     pass
 
 
-DescribeAccessPolicyResponseTypeDef = TypedDict(
-    "DescribeAccessPolicyResponseTypeDef",
-    {
-        "accessPolicyId": str,
-        "accessPolicyArn": str,
-        "accessPolicyIdentity": IdentityOutputTypeDef,
-        "accessPolicyResource": ResourceOutputTypeDef,
-        "accessPolicyPermission": PermissionType,
-        "accessPolicyCreationDate": datetime,
-        "accessPolicyLastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateAccessPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPolicyRequestRequestTypeDef",
     {
         "accessPolicyIdentity": IdentityTypeDef,
         "accessPolicyResource": ResourceTypeDef,
         "accessPolicyPermission": PermissionType,
     },
@@ -3950,14 +3549,28 @@
 class CreateAccessPolicyRequestRequestTypeDef(
     _RequiredCreateAccessPolicyRequestRequestTypeDef,
     _OptionalCreateAccessPolicyRequestRequestTypeDef,
 ):
     pass
 
 
+DescribeAccessPolicyResponseTypeDef = TypedDict(
+    "DescribeAccessPolicyResponseTypeDef",
+    {
+        "accessPolicyId": str,
+        "accessPolicyArn": str,
+        "accessPolicyIdentity": IdentityTypeDef,
+        "accessPolicyResource": ResourceTypeDef,
+        "accessPolicyPermission": PermissionType,
+        "accessPolicyCreationDate": datetime,
+        "accessPolicyLastUpdateDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateAccessPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAccessPolicyRequestRequestTypeDef",
     {
         "accessPolicyId": str,
         "accessPolicyIdentity": IdentityTypeDef,
         "accessPolicyResource": ResourceTypeDef,
         "accessPolicyPermission": PermissionType,
@@ -3982,45 +3595,45 @@
 BatchGetAssetPropertyAggregatesResponseTypeDef = TypedDict(
     "BatchGetAssetPropertyAggregatesResponseTypeDef",
     {
         "errorEntries": List[BatchGetAssetPropertyAggregatesErrorEntryTypeDef],
         "successEntries": List[BatchGetAssetPropertyAggregatesSuccessEntryTypeDef],
         "skippedEntries": List[BatchGetAssetPropertyAggregatesSkippedEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutAssetPropertyValueResponseTypeDef = TypedDict(
     "BatchPutAssetPropertyValueResponseTypeDef",
     {
         "errorEntries": List[BatchPutAssetPropertyErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetAssetPropertyValueHistoryResponseTypeDef = TypedDict(
     "BatchGetAssetPropertyValueHistoryResponseTypeDef",
     {
         "errorEntries": List[BatchGetAssetPropertyValueHistoryErrorEntryTypeDef],
         "successEntries": List[BatchGetAssetPropertyValueHistorySuccessEntryTypeDef],
         "skippedEntries": List[BatchGetAssetPropertyValueHistorySkippedEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetAssetPropertyValueResponseTypeDef = TypedDict(
     "BatchGetAssetPropertyValueResponseTypeDef",
     {
         "errorEntries": List[BatchGetAssetPropertyValueErrorEntryTypeDef],
         "successEntries": List[BatchGetAssetPropertyValueSuccessEntryTypeDef],
         "skippedEntries": List[BatchGetAssetPropertyValueSkippedEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutAssetPropertyValueRequestRequestTypeDef = TypedDict(
     "BatchPutAssetPropertyValueRequestRequestTypeDef",
     {
         "entries": Sequence[PutAssetPropertyValueEntryTypeDef],
@@ -4030,20 +3643,20 @@
 DescribeBulkImportJobResponseTypeDef = TypedDict(
     "DescribeBulkImportJobResponseTypeDef",
     {
         "jobId": str,
         "jobName": str,
         "jobStatus": JobStatusType,
         "jobRoleArn": str,
-        "files": List[FileOutputTypeDef],
-        "errorReportLocation": ErrorReportLocationOutputTypeDef,
+        "files": List[FileTypeDef],
+        "errorReportLocation": ErrorReportLocationTypeDef,
         "jobConfiguration": JobConfigurationOutputTypeDef,
         "jobCreationDate": datetime,
         "jobLastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBulkImportJobRequestRequestTypeDef = TypedDict(
     "CreateBulkImportJobRequestRequestTypeDef",
     {
         "jobName": str,
@@ -4069,31 +3682,31 @@
 
 CreateAssetModelResponseTypeDef = TypedDict(
     "CreateAssetModelResponseTypeDef",
     {
         "assetModelId": str,
         "assetModelArn": str,
         "assetModelStatus": AssetModelStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAssetModelResponseTypeDef = TypedDict(
     "DeleteAssetModelResponseTypeDef",
     {
         "assetModelStatus": AssetModelStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssetModelResponseTypeDef = TypedDict(
     "UpdateAssetModelResponseTypeDef",
     {
         "assetModelStatus": AssetModelStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssetSummaryTypeDef = TypedDict(
     "_RequiredAssetSummaryTypeDef",
     {
         "id": str,
@@ -4149,23 +3762,23 @@
 
 CreateAssetResponseTypeDef = TypedDict(
     "CreateAssetResponseTypeDef",
     {
         "assetId": str,
         "assetArn": str,
         "assetStatus": AssetStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAssetResponseTypeDef = TypedDict(
     "DeleteAssetResponseTypeDef",
     {
         "assetStatus": AssetStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssetResponseTypeDef = TypedDict(
     "DescribeAssetResponseTypeDef",
     {
         "assetId": str,
@@ -4175,40 +3788,40 @@
         "assetProperties": List[AssetPropertyTypeDef],
         "assetHierarchies": List[AssetHierarchyTypeDef],
         "assetCompositeModels": List[AssetCompositeModelTypeDef],
         "assetCreationDate": datetime,
         "assetLastUpdateDate": datetime,
         "assetStatus": AssetStatusTypeDef,
         "assetDescription": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssetResponseTypeDef = TypedDict(
     "UpdateAssetResponseTypeDef",
     {
         "assetStatus": AssetStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGatewaysResponseTypeDef = TypedDict(
     "ListGatewaysResponseTypeDef",
     {
         "gatewaySummaries": List[GatewaySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PropertyTypeOutputTypeDef = TypedDict(
     "PropertyTypeOutputTypeDef",
     {
-        "attribute": AttributeOutputTypeDef,
-        "measurement": MeasurementOutputTypeDef,
+        "attribute": AttributeTypeDef,
+        "measurement": MeasurementTypeDef,
         "transform": TransformOutputTypeDef,
         "metric": MetricOutputTypeDef,
     },
     total=False,
 )
 
 PropertyTypeTypeDef = TypedDict(
@@ -4223,51 +3836,51 @@
 )
 
 ListPortalsResponseTypeDef = TypedDict(
     "ListPortalsResponseTypeDef",
     {
         "portalSummaries": List[PortalSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccessPoliciesResponseTypeDef = TypedDict(
     "ListAccessPoliciesResponseTypeDef",
     {
         "accessPolicySummaries": List[AccessPolicySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssetModelsResponseTypeDef = TypedDict(
     "ListAssetModelsResponseTypeDef",
     {
         "assetModelSummaries": List[AssetModelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssetsResponseTypeDef = TypedDict(
     "ListAssetsResponseTypeDef",
     {
         "assetSummaries": List[AssetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssociatedAssetsResponseTypeDef = TypedDict(
     "ListAssociatedAssetsResponseTypeDef",
     {
         "assetSummaries": List[AssociatedAssetsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssetModelPropertyOutputTypeDef = TypedDict(
     "_RequiredAssetModelPropertyOutputTypeDef",
     {
         "name": str,
@@ -4416,15 +4029,15 @@
 
 
 ListAssetModelPropertiesResponseTypeDef = TypedDict(
     "ListAssetModelPropertiesResponseTypeDef",
     {
         "assetModelPropertySummaries": List[AssetModelPropertySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCompositeModelPropertyTypeDef = TypedDict(
     "_RequiredCompositeModelPropertyTypeDef",
     {
         "name": str,
@@ -4499,32 +4112,32 @@
     "DescribeAssetModelResponseTypeDef",
     {
         "assetModelId": str,
         "assetModelArn": str,
         "assetModelName": str,
         "assetModelDescription": str,
         "assetModelProperties": List[AssetModelPropertyOutputTypeDef],
-        "assetModelHierarchies": List[AssetModelHierarchyOutputTypeDef],
+        "assetModelHierarchies": List[AssetModelHierarchyTypeDef],
         "assetModelCompositeModels": List[AssetModelCompositeModelOutputTypeDef],
         "assetModelCreationDate": datetime,
         "assetModelLastUpdateDate": datetime,
         "assetModelStatus": AssetModelStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssetPropertyResponseTypeDef = TypedDict(
     "DescribeAssetPropertyResponseTypeDef",
     {
         "assetId": str,
         "assetName": str,
         "assetModelId": str,
         "assetProperty": PropertyTypeDef,
         "compositeModel": CompositeModelPropertyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAssetModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssetModelRequestRequestTypeDef",
     {
         "assetModelName": str,
```

### Comparing `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/type_defs.pyi` & `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -63,57 +63,47 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AggregatesTypeDef",
-    "AlarmsOutputTypeDef",
     "AlarmsTypeDef",
     "AssetErrorDetailsTypeDef",
     "AssetHierarchyInfoTypeDef",
     "AssetHierarchyTypeDef",
     "AssetModelHierarchyDefinitionTypeDef",
-    "AssetModelHierarchyOutputTypeDef",
     "AssetModelHierarchyTypeDef",
     "PropertyNotificationTypeDef",
-    "TimeInNanosOutputTypeDef",
-    "VariantOutputTypeDef",
     "TimeInNanosTypeDef",
     "VariantTypeDef",
     "AssociateAssetsRequestRequestTypeDef",
     "AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef",
-    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "BatchAssociateProjectAssetsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDisassociateProjectAssetsRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesEntryTypeDef",
     "BatchGetAssetPropertyAggregatesErrorEntryTypeDef",
     "BatchGetAssetPropertyAggregatesErrorInfoTypeDef",
     "BatchGetAssetPropertyValueEntryTypeDef",
     "BatchGetAssetPropertyValueErrorEntryTypeDef",
     "BatchGetAssetPropertyValueErrorInfoTypeDef",
     "BatchGetAssetPropertyValueHistoryEntryTypeDef",
     "BatchGetAssetPropertyValueHistoryErrorEntryTypeDef",
     "BatchGetAssetPropertyValueHistoryErrorInfoTypeDef",
     "ConfigurationErrorDetailsTypeDef",
-    "CreateAccessPolicyResponseTypeDef",
     "CreateAssetRequestRequestTypeDef",
     "ErrorReportLocationTypeDef",
     "FileTypeDef",
-    "CreateBulkImportJobResponseTypeDef",
     "CreateDashboardRequestRequestTypeDef",
-    "CreateDashboardResponseTypeDef",
-    "CreateGatewayResponseTypeDef",
     "ImageFileTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "CreateProjectResponseTypeDef",
     "CsvOutputTypeDef",
     "CsvTypeDef",
-    "CustomerManagedS3StorageOutputTypeDef",
     "CustomerManagedS3StorageTypeDef",
     "DashboardSummaryTypeDef",
     "DeleteAccessPolicyRequestRequestTypeDef",
     "DeleteAssetModelRequestRequestTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeleteDashboardRequestRequestTypeDef",
     "DeleteGatewayRequestRequestTypeDef",
@@ -122,204 +112,182 @@
     "DeleteTimeSeriesRequestRequestTypeDef",
     "DescribeAccessPolicyRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAssetModelRequestRequestTypeDef",
     "DescribeAssetPropertyRequestRequestTypeDef",
     "DescribeAssetRequestRequestTypeDef",
     "DescribeBulkImportJobRequestRequestTypeDef",
-    "ErrorReportLocationOutputTypeDef",
-    "FileOutputTypeDef",
     "DescribeDashboardRequestRequestTypeDef",
-    "DescribeDashboardResponseTypeDef",
     "DescribeGatewayCapabilityConfigurationRequestRequestTypeDef",
-    "DescribeGatewayCapabilityConfigurationResponseTypeDef",
     "DescribeGatewayRequestRequestTypeDef",
     "GatewayCapabilitySummaryTypeDef",
-    "LoggingOptionsOutputTypeDef",
+    "LoggingOptionsTypeDef",
     "DescribePortalRequestRequestTypeDef",
     "ImageLocationTypeDef",
     "DescribeProjectRequestRequestTypeDef",
-    "DescribeProjectResponseTypeDef",
-    "RetentionPeriodOutputTypeDef",
+    "RetentionPeriodTypeDef",
     "DescribeTimeSeriesRequestRequestTypeDef",
-    "DescribeTimeSeriesResponseTypeDef",
     "DetailedErrorTypeDef",
     "DisassociateAssetsRequestRequestTypeDef",
     "DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "VariableValueOutputTypeDef",
     "VariableValueTypeDef",
-    "ForwardingConfigOutputTypeDef",
     "ForwardingConfigTypeDef",
-    "GreengrassOutputTypeDef",
-    "GreengrassV2OutputTypeDef",
     "GreengrassTypeDef",
     "GreengrassV2TypeDef",
-    "GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetAssetPropertyAggregatesRequestRequestTypeDef",
-    "GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef",
     "GetAssetPropertyValueHistoryRequestRequestTypeDef",
     "GetAssetPropertyValueRequestRequestTypeDef",
-    "GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef",
     "GetInterpolatedAssetPropertyValuesRequestRequestTypeDef",
-    "GroupIdentityOutputTypeDef",
     "GroupIdentityTypeDef",
-    "IAMRoleIdentityOutputTypeDef",
     "IAMRoleIdentityTypeDef",
-    "IAMUserIdentityOutputTypeDef",
     "IAMUserIdentityTypeDef",
-    "UserIdentityOutputTypeDef",
     "UserIdentityTypeDef",
     "JobSummaryTypeDef",
-    "ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef",
     "ListAccessPoliciesRequestRequestTypeDef",
-    "ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef",
     "ListAssetModelPropertiesRequestRequestTypeDef",
-    "ListAssetModelsRequestListAssetModelsPaginateTypeDef",
     "ListAssetModelsRequestRequestTypeDef",
-    "ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef",
     "ListAssetPropertiesRequestRequestTypeDef",
-    "ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
     "ListAssetRelationshipsRequestRequestTypeDef",
-    "ListAssetsRequestListAssetsPaginateTypeDef",
     "ListAssetsRequestRequestTypeDef",
-    "ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef",
     "ListAssociatedAssetsRequestRequestTypeDef",
-    "ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef",
     "ListBulkImportJobsRequestRequestTypeDef",
-    "ListDashboardsRequestListDashboardsPaginateTypeDef",
     "ListDashboardsRequestRequestTypeDef",
-    "ListGatewaysRequestListGatewaysPaginateTypeDef",
     "ListGatewaysRequestRequestTypeDef",
-    "ListPortalsRequestListPortalsPaginateTypeDef",
     "ListPortalsRequestRequestTypeDef",
-    "ListProjectAssetsRequestListProjectAssetsPaginateTypeDef",
     "ListProjectAssetsRequestRequestTypeDef",
-    "ListProjectAssetsResponseTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTimeSeriesRequestListTimeSeriesPaginateTypeDef",
     "ListTimeSeriesRequestRequestTypeDef",
     "TimeSeriesSummaryTypeDef",
-    "LoggingOptionsTypeDef",
-    "MetricProcessingConfigOutputTypeDef",
     "MetricProcessingConfigTypeDef",
-    "TumblingWindowOutputTypeDef",
     "TumblingWindowTypeDef",
     "MonitorErrorDetailsTypeDef",
-    "PaginatorConfigTypeDef",
-    "PortalResourceOutputTypeDef",
     "PortalResourceTypeDef",
-    "ProjectResourceOutputTypeDef",
     "ProjectResourceTypeDef",
     "PutDefaultEncryptionConfigurationRequestRequestTypeDef",
-    "RetentionPeriodTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssetPropertyRequestRequestTypeDef",
     "UpdateAssetRequestRequestTypeDef",
     "UpdateDashboardRequestRequestTypeDef",
     "UpdateGatewayCapabilityConfigurationRequestRequestTypeDef",
-    "UpdateGatewayCapabilityConfigurationResponseTypeDef",
     "UpdateGatewayRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "AggregatedValueTypeDef",
-    "BatchAssociateProjectAssetsResponseTypeDef",
-    "BatchDisassociateProjectAssetsResponseTypeDef",
     "AssetRelationshipSummaryTypeDef",
     "AssetPropertySummaryTypeDef",
     "AssetPropertyTypeDef",
     "BatchPutAssetPropertyErrorTypeDef",
-    "AssetPropertyValueOutputTypeDef",
-    "InterpolatedAssetPropertyValueTypeDef",
     "AssetPropertyValueTypeDef",
+    "InterpolatedAssetPropertyValueTypeDef",
+    "BatchAssociateProjectAssetsResponseTypeDef",
+    "BatchDisassociateProjectAssetsResponseTypeDef",
+    "CreateAccessPolicyResponseTypeDef",
+    "CreateBulkImportJobResponseTypeDef",
+    "CreateDashboardResponseTypeDef",
+    "CreateGatewayResponseTypeDef",
+    "CreateProjectResponseTypeDef",
+    "DescribeDashboardResponseTypeDef",
+    "DescribeGatewayCapabilityConfigurationResponseTypeDef",
+    "DescribeProjectResponseTypeDef",
+    "DescribeTimeSeriesResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListProjectAssetsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateGatewayCapabilityConfigurationResponseTypeDef",
     "BatchGetAssetPropertyAggregatesRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesSkippedEntryTypeDef",
     "BatchGetAssetPropertyValueRequestRequestTypeDef",
     "BatchGetAssetPropertyValueSkippedEntryTypeDef",
     "BatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
     "BatchGetAssetPropertyValueHistorySkippedEntryTypeDef",
     "ConfigurationStatusTypeDef",
     "CreatePortalRequestRequestTypeDef",
     "ImageTypeDef",
     "FileFormatOutputTypeDef",
     "FileFormatTypeDef",
-    "MultiLayerStorageOutputTypeDef",
     "MultiLayerStorageTypeDef",
     "ListDashboardsResponseTypeDef",
     "DescribeAssetModelRequestAssetModelActiveWaitTypeDef",
     "DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef",
     "DescribeAssetRequestAssetActiveWaitTypeDef",
     "DescribeAssetRequestAssetNotExistsWaitTypeDef",
     "DescribePortalRequestPortalActiveWaitTypeDef",
     "DescribePortalRequestPortalNotExistsWaitTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
+    "PutLoggingOptionsRequestRequestTypeDef",
     "ErrorDetailsTypeDef",
-    "ExpressionVariableOutputTypeDef",
     "ExpressionVariableTypeDef",
-    "MeasurementProcessingConfigOutputTypeDef",
-    "TransformProcessingConfigOutputTypeDef",
     "MeasurementProcessingConfigTypeDef",
     "TransformProcessingConfigTypeDef",
-    "GatewayPlatformOutputTypeDef",
     "GatewayPlatformTypeDef",
-    "IdentityOutputTypeDef",
+    "GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
+    "GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef",
+    "GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef",
+    "ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef",
+    "ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef",
+    "ListAssetModelsRequestListAssetModelsPaginateTypeDef",
+    "ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef",
+    "ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
+    "ListAssetsRequestListAssetsPaginateTypeDef",
+    "ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef",
+    "ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef",
+    "ListDashboardsRequestListDashboardsPaginateTypeDef",
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
+    "ListPortalsRequestListPortalsPaginateTypeDef",
+    "ListProjectAssetsRequestListProjectAssetsPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListTimeSeriesRequestListTimeSeriesPaginateTypeDef",
     "IdentityTypeDef",
     "ListBulkImportJobsResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "ListTimeSeriesResponseTypeDef",
-    "PutLoggingOptionsRequestRequestTypeDef",
-    "MetricWindowOutputTypeDef",
     "MetricWindowTypeDef",
     "PortalStatusTypeDef",
-    "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "BatchGetAssetPropertyAggregatesSuccessEntryTypeDef",
     "GetAssetPropertyAggregatesResponseTypeDef",
     "ListAssetRelationshipsResponseTypeDef",
     "ListAssetPropertiesResponseTypeDef",
     "AssetCompositeModelTypeDef",
     "BatchPutAssetPropertyErrorEntryTypeDef",
     "BatchGetAssetPropertyValueHistorySuccessEntryTypeDef",
     "BatchGetAssetPropertyValueSuccessEntryTypeDef",
     "GetAssetPropertyValueHistoryResponseTypeDef",
     "GetAssetPropertyValueResponseTypeDef",
-    "GetInterpolatedAssetPropertyValuesResponseTypeDef",
     "PutAssetPropertyValueEntryTypeDef",
+    "GetInterpolatedAssetPropertyValuesResponseTypeDef",
     "DescribeDefaultEncryptionConfigurationResponseTypeDef",
     "PutDefaultEncryptionConfigurationResponseTypeDef",
     "UpdatePortalRequestRequestTypeDef",
     "JobConfigurationOutputTypeDef",
     "JobConfigurationTypeDef",
     "DescribeStorageConfigurationResponseTypeDef",
-    "PutStorageConfigurationResponseTypeDef",
     "PutStorageConfigurationRequestRequestTypeDef",
+    "PutStorageConfigurationResponseTypeDef",
     "AssetModelStatusTypeDef",
     "AssetStatusTypeDef",
-    "MeasurementOutputTypeDef",
-    "TransformOutputTypeDef",
     "MeasurementTypeDef",
+    "TransformOutputTypeDef",
     "TransformTypeDef",
+    "CreateGatewayRequestRequestTypeDef",
     "DescribeGatewayResponseTypeDef",
     "GatewaySummaryTypeDef",
-    "CreateGatewayRequestRequestTypeDef",
     "MetricOutputTypeDef",
     "MetricTypeDef",
     "CreatePortalResponseTypeDef",
     "DeletePortalResponseTypeDef",
     "DescribePortalResponseTypeDef",
     "PortalSummaryTypeDef",
     "UpdatePortalResponseTypeDef",
     "AccessPolicySummaryTypeDef",
-    "DescribeAccessPolicyResponseTypeDef",
     "CreateAccessPolicyRequestRequestTypeDef",
+    "DescribeAccessPolicyResponseTypeDef",
     "UpdateAccessPolicyRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesResponseTypeDef",
     "BatchPutAssetPropertyValueResponseTypeDef",
     "BatchGetAssetPropertyValueHistoryResponseTypeDef",
     "BatchGetAssetPropertyValueResponseTypeDef",
     "BatchPutAssetPropertyValueRequestRequestTypeDef",
     "DescribeBulkImportJobResponseTypeDef",
@@ -367,31 +335,14 @@
         "minimum": float,
         "sum": float,
         "standardDeviation": float,
     },
     total=False,
 )
 
-_RequiredAlarmsOutputTypeDef = TypedDict(
-    "_RequiredAlarmsOutputTypeDef",
-    {
-        "alarmRoleArn": str,
-    },
-)
-_OptionalAlarmsOutputTypeDef = TypedDict(
-    "_OptionalAlarmsOutputTypeDef",
-    {
-        "notificationLambdaArn": str,
-    },
-    total=False,
-)
-
-class AlarmsOutputTypeDef(_RequiredAlarmsOutputTypeDef, _OptionalAlarmsOutputTypeDef):
-    pass
-
 _RequiredAlarmsTypeDef = TypedDict(
     "_RequiredAlarmsTypeDef",
     {
         "alarmRoleArn": str,
     },
 )
 _OptionalAlarmsTypeDef = TypedDict(
@@ -444,34 +395,14 @@
     "AssetModelHierarchyDefinitionTypeDef",
     {
         "name": str,
         "childAssetModelId": str,
     },
 )
 
-_RequiredAssetModelHierarchyOutputTypeDef = TypedDict(
-    "_RequiredAssetModelHierarchyOutputTypeDef",
-    {
-        "name": str,
-        "childAssetModelId": str,
-    },
-)
-_OptionalAssetModelHierarchyOutputTypeDef = TypedDict(
-    "_OptionalAssetModelHierarchyOutputTypeDef",
-    {
-        "id": str,
-    },
-    total=False,
-)
-
-class AssetModelHierarchyOutputTypeDef(
-    _RequiredAssetModelHierarchyOutputTypeDef, _OptionalAssetModelHierarchyOutputTypeDef
-):
-    pass
-
 _RequiredAssetModelHierarchyTypeDef = TypedDict(
     "_RequiredAssetModelHierarchyTypeDef",
     {
         "name": str,
         "childAssetModelId": str,
     },
 )
@@ -492,44 +423,14 @@
     "PropertyNotificationTypeDef",
     {
         "topic": str,
         "state": PropertyNotificationStateType,
     },
 )
 
-_RequiredTimeInNanosOutputTypeDef = TypedDict(
-    "_RequiredTimeInNanosOutputTypeDef",
-    {
-        "timeInSeconds": int,
-    },
-)
-_OptionalTimeInNanosOutputTypeDef = TypedDict(
-    "_OptionalTimeInNanosOutputTypeDef",
-    {
-        "offsetInNanos": int,
-    },
-    total=False,
-)
-
-class TimeInNanosOutputTypeDef(
-    _RequiredTimeInNanosOutputTypeDef, _OptionalTimeInNanosOutputTypeDef
-):
-    pass
-
-VariantOutputTypeDef = TypedDict(
-    "VariantOutputTypeDef",
-    {
-        "stringValue": str,
-        "integerValue": int,
-        "doubleValue": float,
-        "booleanValue": bool,
-    },
-    total=False,
-)
-
 _RequiredTimeInNanosTypeDef = TypedDict(
     "_RequiredTimeInNanosTypeDef",
     {
         "timeInSeconds": int,
     },
 )
 _OptionalTimeInNanosTypeDef = TypedDict(
@@ -593,22 +494,14 @@
 
 class AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef(
     _RequiredAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
     _OptionalAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
 ):
     pass
 
-AttributeOutputTypeDef = TypedDict(
-    "AttributeOutputTypeDef",
-    {
-        "defaultValue": str,
-    },
-    total=False,
-)
-
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "defaultValue": str,
     },
     total=False,
 )
@@ -630,14 +523,25 @@
 
 class BatchAssociateProjectAssetsRequestRequestTypeDef(
     _RequiredBatchAssociateProjectAssetsRequestRequestTypeDef,
     _OptionalBatchAssociateProjectAssetsRequestRequestTypeDef,
 ):
     pass
 
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
 _RequiredBatchDisassociateProjectAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDisassociateProjectAssetsRequestRequestTypeDef",
     {
         "projectId": str,
         "assetIds": Sequence[str],
     },
 )
@@ -785,23 +689,14 @@
     "ConfigurationErrorDetailsTypeDef",
     {
         "code": ErrorCodeType,
         "message": str,
     },
 )
 
-CreateAccessPolicyResponseTypeDef = TypedDict(
-    "CreateAccessPolicyResponseTypeDef",
-    {
-        "accessPolicyId": str,
-        "accessPolicyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateAssetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssetRequestRequestTypeDef",
     {
         "assetName": str,
         "assetModelId": str,
     },
 )
@@ -842,24 +737,14 @@
     },
     total=False,
 )
 
 class FileTypeDef(_RequiredFileTypeDef, _OptionalFileTypeDef):
     pass
 
-CreateBulkImportJobResponseTypeDef = TypedDict(
-    "CreateBulkImportJobResponseTypeDef",
-    {
-        "jobId": str,
-        "jobName": str,
-        "jobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateDashboardRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDashboardRequestRequestTypeDef",
     {
         "projectId": str,
         "dashboardName": str,
         "dashboardDefinition": str,
     },
@@ -875,32 +760,14 @@
 )
 
 class CreateDashboardRequestRequestTypeDef(
     _RequiredCreateDashboardRequestRequestTypeDef, _OptionalCreateDashboardRequestRequestTypeDef
 ):
     pass
 
-CreateDashboardResponseTypeDef = TypedDict(
-    "CreateDashboardResponseTypeDef",
-    {
-        "dashboardId": str,
-        "dashboardArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateGatewayResponseTypeDef = TypedDict(
-    "CreateGatewayResponseTypeDef",
-    {
-        "gatewayId": str,
-        "gatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImageFileTypeDef = TypedDict(
     "ImageFileTypeDef",
     {
         "data": Union[str, bytes, IO[Any], StreamingBody],
         "type": Literal["PNG"],
     },
 )
@@ -923,23 +790,14 @@
 )
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "projectId": str,
-        "projectArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CsvOutputTypeDef = TypedDict(
     "CsvOutputTypeDef",
     {
         "columnNames": List[ColumnNameType],
     },
     total=False,
 )
@@ -948,22 +806,14 @@
     "CsvTypeDef",
     {
         "columnNames": Sequence[ColumnNameType],
     },
     total=False,
 )
 
-CustomerManagedS3StorageOutputTypeDef = TypedDict(
-    "CustomerManagedS3StorageOutputTypeDef",
-    {
-        "s3ResourceArn": str,
-        "roleArn": str,
-    },
-)
-
 CustomerManagedS3StorageTypeDef = TypedDict(
     "CustomerManagedS3StorageTypeDef",
     {
         "s3ResourceArn": str,
         "roleArn": str,
     },
 )
@@ -1187,81 +1037,29 @@
 DescribeBulkImportJobRequestRequestTypeDef = TypedDict(
     "DescribeBulkImportJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
-ErrorReportLocationOutputTypeDef = TypedDict(
-    "ErrorReportLocationOutputTypeDef",
-    {
-        "bucket": str,
-        "prefix": str,
-    },
-)
-
-_RequiredFileOutputTypeDef = TypedDict(
-    "_RequiredFileOutputTypeDef",
-    {
-        "bucket": str,
-        "key": str,
-    },
-)
-_OptionalFileOutputTypeDef = TypedDict(
-    "_OptionalFileOutputTypeDef",
-    {
-        "versionId": str,
-    },
-    total=False,
-)
-
-class FileOutputTypeDef(_RequiredFileOutputTypeDef, _OptionalFileOutputTypeDef):
-    pass
-
 DescribeDashboardRequestRequestTypeDef = TypedDict(
     "DescribeDashboardRequestRequestTypeDef",
     {
         "dashboardId": str,
     },
 )
 
-DescribeDashboardResponseTypeDef = TypedDict(
-    "DescribeDashboardResponseTypeDef",
-    {
-        "dashboardId": str,
-        "dashboardArn": str,
-        "dashboardName": str,
-        "projectId": str,
-        "dashboardDescription": str,
-        "dashboardDefinition": str,
-        "dashboardCreationDate": datetime,
-        "dashboardLastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeGatewayCapabilityConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeGatewayCapabilityConfigurationRequestRequestTypeDef",
     {
         "gatewayId": str,
         "capabilityNamespace": str,
     },
 )
 
-DescribeGatewayCapabilityConfigurationResponseTypeDef = TypedDict(
-    "DescribeGatewayCapabilityConfigurationResponseTypeDef",
-    {
-        "gatewayId": str,
-        "capabilityNamespace": str,
-        "capabilityConfiguration": str,
-        "capabilitySyncStatus": CapabilitySyncStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeGatewayRequestRequestTypeDef = TypedDict(
     "DescribeGatewayRequestRequestTypeDef",
     {
         "gatewayId": str,
     },
 )
 
@@ -1269,16 +1067,16 @@
     "GatewayCapabilitySummaryTypeDef",
     {
         "capabilityNamespace": str,
         "capabilitySyncStatus": CapabilitySyncStatusType,
     },
 )
 
-LoggingOptionsOutputTypeDef = TypedDict(
-    "LoggingOptionsOutputTypeDef",
+LoggingOptionsTypeDef = TypedDict(
+    "LoggingOptionsTypeDef",
     {
         "level": LoggingLevelType,
     },
 )
 
 DescribePortalRequestRequestTypeDef = TypedDict(
     "DescribePortalRequestRequestTypeDef",
@@ -1298,30 +1096,16 @@
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 
-DescribeProjectResponseTypeDef = TypedDict(
-    "DescribeProjectResponseTypeDef",
-    {
-        "projectId": str,
-        "projectArn": str,
-        "projectName": str,
-        "portalId": str,
-        "projectDescription": str,
-        "projectCreationDate": datetime,
-        "projectLastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RetentionPeriodOutputTypeDef = TypedDict(
-    "RetentionPeriodOutputTypeDef",
+RetentionPeriodTypeDef = TypedDict(
+    "RetentionPeriodTypeDef",
     {
         "numberOfDays": int,
         "unlimited": bool,
     },
     total=False,
 )
 
@@ -1331,30 +1115,14 @@
         "alias": str,
         "assetId": str,
         "propertyId": str,
     },
     total=False,
 )
 
-DescribeTimeSeriesResponseTypeDef = TypedDict(
-    "DescribeTimeSeriesResponseTypeDef",
-    {
-        "assetId": str,
-        "propertyId": str,
-        "alias": str,
-        "timeSeriesId": str,
-        "dataType": PropertyDataTypeType,
-        "dataTypeSpec": str,
-        "timeSeriesCreationDate": datetime,
-        "timeSeriesLastUpdateDate": datetime,
-        "timeSeriesArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DetailedErrorTypeDef = TypedDict(
     "DetailedErrorTypeDef",
     {
         "code": DetailedErrorCodeType,
         "message": str,
     },
 )
@@ -1399,40 +1167,14 @@
 
 class DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef(
     _RequiredDisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
     _OptionalDisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredVariableValueOutputTypeDef = TypedDict(
-    "_RequiredVariableValueOutputTypeDef",
-    {
-        "propertyId": str,
-    },
-)
-_OptionalVariableValueOutputTypeDef = TypedDict(
-    "_OptionalVariableValueOutputTypeDef",
-    {
-        "hierarchyId": str,
-    },
-    total=False,
-)
-
-class VariableValueOutputTypeDef(
-    _RequiredVariableValueOutputTypeDef, _OptionalVariableValueOutputTypeDef
-):
-    pass
-
 _RequiredVariableValueTypeDef = TypedDict(
     "_RequiredVariableValueTypeDef",
     {
         "propertyId": str,
     },
 )
 _OptionalVariableValueTypeDef = TypedDict(
@@ -1442,84 +1184,45 @@
     },
     total=False,
 )
 
 class VariableValueTypeDef(_RequiredVariableValueTypeDef, _OptionalVariableValueTypeDef):
     pass
 
-ForwardingConfigOutputTypeDef = TypedDict(
-    "ForwardingConfigOutputTypeDef",
-    {
-        "state": ForwardingConfigStateType,
-    },
-)
-
 ForwardingConfigTypeDef = TypedDict(
     "ForwardingConfigTypeDef",
     {
         "state": ForwardingConfigStateType,
     },
 )
 
-GreengrassOutputTypeDef = TypedDict(
-    "GreengrassOutputTypeDef",
-    {
-        "groupArn": str,
-    },
-)
-
-GreengrassV2OutputTypeDef = TypedDict(
-    "GreengrassV2OutputTypeDef",
-    {
-        "coreDeviceThingName": str,
-    },
-)
-
 GreengrassTypeDef = TypedDict(
     "GreengrassTypeDef",
     {
         "groupArn": str,
     },
 )
 
 GreengrassV2TypeDef = TypedDict(
     "GreengrassV2TypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 
-_RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef = TypedDict(
-    "_RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
-    {
-        "aggregateTypes": Sequence[AggregateTypeType],
-        "resolution": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-    },
-)
-_OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef = TypedDict(
-    "_OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "qualities": Sequence[QualityType],
-        "timeOrdering": TimeOrderingType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef(
-    _RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
-    _OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAssetPropertyAggregatesRequestRequestTypeDef",
     {
         "aggregateTypes": Sequence[AggregateTypeType],
         "resolution": str,
         "startDate": Union[datetime, str],
         "endDate": Union[datetime, str],
@@ -1541,29 +1244,14 @@
 
 class GetAssetPropertyAggregatesRequestRequestTypeDef(
     _RequiredGetAssetPropertyAggregatesRequestRequestTypeDef,
     _OptionalGetAssetPropertyAggregatesRequestRequestTypeDef,
 ):
     pass
 
-GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef = TypedDict(
-    "GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef",
-    {
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "startDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-        "qualities": Sequence[QualityType],
-        "timeOrdering": TimeOrderingType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "GetAssetPropertyValueHistoryRequestRequestTypeDef",
     {
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
         "startDate": Union[datetime, str],
@@ -1582,44 +1270,14 @@
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
     },
     total=False,
 )
 
-_RequiredGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef = TypedDict(
-    "_RequiredGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef",
-    {
-        "startTimeInSeconds": int,
-        "endTimeInSeconds": int,
-        "quality": QualityType,
-        "intervalInSeconds": int,
-        "type": str,
-    },
-)
-_OptionalGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef = TypedDict(
-    "_OptionalGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef",
-    {
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "startTimeOffsetInNanos": int,
-        "endTimeOffsetInNanos": int,
-        "intervalWindowInSeconds": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef(
-    _RequiredGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
-    _OptionalGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetInterpolatedAssetPropertyValuesRequestRequestTypeDef = TypedDict(
     "_RequiredGetInterpolatedAssetPropertyValuesRequestRequestTypeDef",
     {
         "startTimeInSeconds": int,
         "endTimeInSeconds": int,
         "quality": QualityType,
         "intervalInSeconds": int,
@@ -1643,63 +1301,35 @@
 
 class GetInterpolatedAssetPropertyValuesRequestRequestTypeDef(
     _RequiredGetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
     _OptionalGetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
 ):
     pass
 
-GroupIdentityOutputTypeDef = TypedDict(
-    "GroupIdentityOutputTypeDef",
-    {
-        "id": str,
-    },
-)
-
 GroupIdentityTypeDef = TypedDict(
     "GroupIdentityTypeDef",
     {
         "id": str,
     },
 )
 
-IAMRoleIdentityOutputTypeDef = TypedDict(
-    "IAMRoleIdentityOutputTypeDef",
-    {
-        "arn": str,
-    },
-)
-
 IAMRoleIdentityTypeDef = TypedDict(
     "IAMRoleIdentityTypeDef",
     {
         "arn": str,
     },
 )
 
-IAMUserIdentityOutputTypeDef = TypedDict(
-    "IAMUserIdentityOutputTypeDef",
-    {
-        "arn": str,
-    },
-)
-
 IAMUserIdentityTypeDef = TypedDict(
     "IAMUserIdentityTypeDef",
     {
         "arn": str,
     },
 )
 
-UserIdentityOutputTypeDef = TypedDict(
-    "UserIdentityOutputTypeDef",
-    {
-        "id": str,
-    },
-)
-
 UserIdentityTypeDef = TypedDict(
     "UserIdentityTypeDef",
     {
         "id": str,
     },
 )
 
@@ -1708,62 +1338,28 @@
     {
         "id": str,
         "name": str,
         "status": JobStatusType,
     },
 )
 
-ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef = TypedDict(
-    "ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef",
-    {
-        "identityType": IdentityTypeType,
-        "identityId": str,
-        "resourceType": ResourceTypeType,
-        "resourceId": str,
-        "iamArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAccessPoliciesRequestRequestTypeDef = TypedDict(
     "ListAccessPoliciesRequestRequestTypeDef",
     {
         "identityType": IdentityTypeType,
         "identityId": str,
         "resourceType": ResourceTypeType,
         "resourceId": str,
         "iamArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef = TypedDict(
-    "_RequiredListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef",
-    {
-        "assetModelId": str,
-    },
-)
-_OptionalListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef = TypedDict(
-    "_OptionalListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef",
-    {
-        "filter": ListAssetModelPropertiesFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef(
-    _RequiredListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
-    _OptionalListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssetModelPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredListAssetModelPropertiesRequestRequestTypeDef",
     {
         "assetModelId": str,
     },
 )
 _OptionalListAssetModelPropertiesRequestRequestTypeDef = TypedDict(
@@ -1778,52 +1374,23 @@
 
 class ListAssetModelPropertiesRequestRequestTypeDef(
     _RequiredListAssetModelPropertiesRequestRequestTypeDef,
     _OptionalListAssetModelPropertiesRequestRequestTypeDef,
 ):
     pass
 
-ListAssetModelsRequestListAssetModelsPaginateTypeDef = TypedDict(
-    "ListAssetModelsRequestListAssetModelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAssetModelsRequestRequestTypeDef = TypedDict(
     "ListAssetModelsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef = TypedDict(
-    "_RequiredListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef",
-    {
-        "assetId": str,
-    },
-)
-_OptionalListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef = TypedDict(
-    "_OptionalListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef",
-    {
-        "filter": ListAssetPropertiesFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef(
-    _RequiredListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
-    _OptionalListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssetPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredListAssetPropertiesRequestRequestTypeDef",
     {
         "assetId": str,
     },
 )
 _OptionalListAssetPropertiesRequestRequestTypeDef = TypedDict(
@@ -1838,35 +1405,14 @@
 
 class ListAssetPropertiesRequestRequestTypeDef(
     _RequiredListAssetPropertiesRequestRequestTypeDef,
     _OptionalListAssetPropertiesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef = TypedDict(
-    "_RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
-    {
-        "assetId": str,
-        "traversalType": Literal["PATH_TO_ROOT"],
-    },
-)
-_OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef = TypedDict(
-    "_OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef(
-    _RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
-    _OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssetRelationshipsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssetRelationshipsRequestRequestTypeDef",
     {
         "assetId": str,
         "traversalType": Literal["PATH_TO_ROOT"],
     },
 )
@@ -1881,57 +1427,25 @@
 
 class ListAssetRelationshipsRequestRequestTypeDef(
     _RequiredListAssetRelationshipsRequestRequestTypeDef,
     _OptionalListAssetRelationshipsRequestRequestTypeDef,
 ):
     pass
 
-ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
-    "ListAssetsRequestListAssetsPaginateTypeDef",
-    {
-        "assetModelId": str,
-        "filter": ListAssetsFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAssetsRequestRequestTypeDef = TypedDict(
     "ListAssetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "assetModelId": str,
         "filter": ListAssetsFilterType,
     },
     total=False,
 )
 
-_RequiredListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef",
-    {
-        "assetId": str,
-    },
-)
-_OptionalListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef",
-    {
-        "hierarchyId": str,
-        "traversalDirection": TraversalDirectionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef(
-    _RequiredListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
-    _OptionalListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssociatedAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedAssetsRequestRequestTypeDef",
     {
         "assetId": str,
     },
 )
 _OptionalListAssociatedAssetsRequestRequestTypeDef = TypedDict(
@@ -1947,53 +1461,24 @@
 
 class ListAssociatedAssetsRequestRequestTypeDef(
     _RequiredListAssociatedAssetsRequestRequestTypeDef,
     _OptionalListAssociatedAssetsRequestRequestTypeDef,
 ):
     pass
 
-ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef = TypedDict(
-    "ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef",
-    {
-        "filter": ListBulkImportJobsFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBulkImportJobsRequestRequestTypeDef = TypedDict(
     "ListBulkImportJobsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filter": ListBulkImportJobsFilterType,
     },
     total=False,
 )
 
-_RequiredListDashboardsRequestListDashboardsPaginateTypeDef = TypedDict(
-    "_RequiredListDashboardsRequestListDashboardsPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListDashboardsRequestListDashboardsPaginateTypeDef = TypedDict(
-    "_OptionalListDashboardsRequestListDashboardsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDashboardsRequestListDashboardsPaginateTypeDef(
-    _RequiredListDashboardsRequestListDashboardsPaginateTypeDef,
-    _OptionalListDashboardsRequestListDashboardsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDashboardsRequestRequestTypeDef = TypedDict(
     "_RequiredListDashboardsRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalListDashboardsRequestRequestTypeDef = TypedDict(
@@ -2006,68 +1491,32 @@
 )
 
 class ListDashboardsRequestRequestTypeDef(
     _RequiredListDashboardsRequestRequestTypeDef, _OptionalListDashboardsRequestRequestTypeDef
 ):
     pass
 
-ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
-    "ListGatewaysRequestListGatewaysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGatewaysRequestRequestTypeDef = TypedDict(
     "ListGatewaysRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListPortalsRequestListPortalsPaginateTypeDef = TypedDict(
-    "ListPortalsRequestListPortalsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPortalsRequestRequestTypeDef = TypedDict(
     "ListPortalsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListProjectAssetsRequestListProjectAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListProjectAssetsRequestListProjectAssetsPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListProjectAssetsRequestListProjectAssetsPaginateTypeDef(
-    _RequiredListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
-    _OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListProjectAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectAssetsRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalListProjectAssetsRequestRequestTypeDef = TypedDict(
@@ -2080,43 +1529,14 @@
 )
 
 class ListProjectAssetsRequestRequestTypeDef(
     _RequiredListProjectAssetsRequestRequestTypeDef, _OptionalListProjectAssetsRequestRequestTypeDef
 ):
     pass
 
-ListProjectAssetsResponseTypeDef = TypedDict(
-    "ListProjectAssetsResponseTypeDef",
-    {
-        "assetIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "_RequiredListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "portalId": str,
-    },
-)
-_OptionalListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "_OptionalListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListProjectsRequestListProjectsPaginateTypeDef(
-    _RequiredListProjectsRequestListProjectsPaginateTypeDef,
-    _OptionalListProjectsRequestListProjectsPaginateTypeDef,
-):
-    pass
-
 _RequiredListProjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectsRequestRequestTypeDef",
     {
         "portalId": str,
     },
 )
 _OptionalListProjectsRequestRequestTypeDef = TypedDict(
@@ -2156,33 +1576,14 @@
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
-ListTimeSeriesRequestListTimeSeriesPaginateTypeDef = TypedDict(
-    "ListTimeSeriesRequestListTimeSeriesPaginateTypeDef",
-    {
-        "assetId": str,
-        "aliasPrefix": str,
-        "timeSeriesType": ListTimeSeriesTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTimeSeriesRequestRequestTypeDef = TypedDict(
     "ListTimeSeriesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "assetId": str,
         "aliasPrefix": str,
@@ -2213,54 +1614,21 @@
 )
 
 class TimeSeriesSummaryTypeDef(
     _RequiredTimeSeriesSummaryTypeDef, _OptionalTimeSeriesSummaryTypeDef
 ):
     pass
 
-LoggingOptionsTypeDef = TypedDict(
-    "LoggingOptionsTypeDef",
-    {
-        "level": LoggingLevelType,
-    },
-)
-
-MetricProcessingConfigOutputTypeDef = TypedDict(
-    "MetricProcessingConfigOutputTypeDef",
-    {
-        "computeLocation": ComputeLocationType,
-    },
-)
-
 MetricProcessingConfigTypeDef = TypedDict(
     "MetricProcessingConfigTypeDef",
     {
         "computeLocation": ComputeLocationType,
     },
 )
 
-_RequiredTumblingWindowOutputTypeDef = TypedDict(
-    "_RequiredTumblingWindowOutputTypeDef",
-    {
-        "interval": str,
-    },
-)
-_OptionalTumblingWindowOutputTypeDef = TypedDict(
-    "_OptionalTumblingWindowOutputTypeDef",
-    {
-        "offset": str,
-    },
-    total=False,
-)
-
-class TumblingWindowOutputTypeDef(
-    _RequiredTumblingWindowOutputTypeDef, _OptionalTumblingWindowOutputTypeDef
-):
-    pass
-
 _RequiredTumblingWindowTypeDef = TypedDict(
     "_RequiredTumblingWindowTypeDef",
     {
         "interval": str,
     },
 )
 _OptionalTumblingWindowTypeDef = TypedDict(
@@ -2279,45 +1647,21 @@
     {
         "code": MonitorErrorCodeType,
         "message": str,
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
-PortalResourceOutputTypeDef = TypedDict(
-    "PortalResourceOutputTypeDef",
-    {
-        "id": str,
-    },
-)
-
 PortalResourceTypeDef = TypedDict(
     "PortalResourceTypeDef",
     {
         "id": str,
     },
 )
 
-ProjectResourceOutputTypeDef = TypedDict(
-    "ProjectResourceOutputTypeDef",
-    {
-        "id": str,
-    },
-)
-
 ProjectResourceTypeDef = TypedDict(
     "ProjectResourceTypeDef",
     {
         "id": str,
     },
 )
 
@@ -2337,34 +1681,14 @@
 
 class PutDefaultEncryptionConfigurationRequestRequestTypeDef(
     _RequiredPutDefaultEncryptionConfigurationRequestRequestTypeDef,
     _OptionalPutDefaultEncryptionConfigurationRequestRequestTypeDef,
 ):
     pass
 
-RetentionPeriodTypeDef = TypedDict(
-    "RetentionPeriodTypeDef",
-    {
-        "numberOfDays": int,
-        "unlimited": bool,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -2449,23 +1773,14 @@
     {
         "gatewayId": str,
         "capabilityNamespace": str,
         "capabilityConfiguration": str,
     },
 )
 
-UpdateGatewayCapabilityConfigurationResponseTypeDef = TypedDict(
-    "UpdateGatewayCapabilityConfigurationResponseTypeDef",
-    {
-        "capabilityNamespace": str,
-        "capabilitySyncStatus": CapabilitySyncStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateGatewayRequestRequestTypeDef = TypedDict(
     "UpdateGatewayRequestRequestTypeDef",
     {
         "gatewayId": str,
         "gatewayName": str,
     },
 )
@@ -2505,30 +1820,14 @@
     },
     total=False,
 )
 
 class AggregatedValueTypeDef(_RequiredAggregatedValueTypeDef, _OptionalAggregatedValueTypeDef):
     pass
 
-BatchAssociateProjectAssetsResponseTypeDef = TypedDict(
-    "BatchAssociateProjectAssetsResponseTypeDef",
-    {
-        "errors": List[AssetErrorDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchDisassociateProjectAssetsResponseTypeDef = TypedDict(
-    "BatchDisassociateProjectAssetsResponseTypeDef",
-    {
-        "errors": List[AssetErrorDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssetRelationshipSummaryTypeDef = TypedDict(
     "_RequiredAssetRelationshipSummaryTypeDef",
     {
         "relationshipType": Literal["HIERARCHY"],
     },
 )
 _OptionalAssetRelationshipSummaryTypeDef = TypedDict(
@@ -2579,65 +1878,196 @@
     pass
 
 BatchPutAssetPropertyErrorTypeDef = TypedDict(
     "BatchPutAssetPropertyErrorTypeDef",
     {
         "errorCode": BatchPutAssetPropertyValueErrorCodeType,
         "errorMessage": str,
-        "timestamps": List[TimeInNanosOutputTypeDef],
+        "timestamps": List[TimeInNanosTypeDef],
     },
 )
 
-_RequiredAssetPropertyValueOutputTypeDef = TypedDict(
-    "_RequiredAssetPropertyValueOutputTypeDef",
+_RequiredAssetPropertyValueTypeDef = TypedDict(
+    "_RequiredAssetPropertyValueTypeDef",
     {
-        "value": VariantOutputTypeDef,
-        "timestamp": TimeInNanosOutputTypeDef,
+        "value": VariantTypeDef,
+        "timestamp": TimeInNanosTypeDef,
     },
 )
-_OptionalAssetPropertyValueOutputTypeDef = TypedDict(
-    "_OptionalAssetPropertyValueOutputTypeDef",
+_OptionalAssetPropertyValueTypeDef = TypedDict(
+    "_OptionalAssetPropertyValueTypeDef",
     {
         "quality": QualityType,
     },
     total=False,
 )
 
-class AssetPropertyValueOutputTypeDef(
-    _RequiredAssetPropertyValueOutputTypeDef, _OptionalAssetPropertyValueOutputTypeDef
+class AssetPropertyValueTypeDef(
+    _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
 ):
     pass
 
 InterpolatedAssetPropertyValueTypeDef = TypedDict(
     "InterpolatedAssetPropertyValueTypeDef",
     {
-        "timestamp": TimeInNanosOutputTypeDef,
-        "value": VariantOutputTypeDef,
+        "timestamp": TimeInNanosTypeDef,
+        "value": VariantTypeDef,
     },
 )
 
-_RequiredAssetPropertyValueTypeDef = TypedDict(
-    "_RequiredAssetPropertyValueTypeDef",
+BatchAssociateProjectAssetsResponseTypeDef = TypedDict(
+    "BatchAssociateProjectAssetsResponseTypeDef",
     {
-        "value": VariantTypeDef,
-        "timestamp": TimeInNanosTypeDef,
+        "errors": List[AssetErrorDetailsTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAssetPropertyValueTypeDef = TypedDict(
-    "_OptionalAssetPropertyValueTypeDef",
+
+BatchDisassociateProjectAssetsResponseTypeDef = TypedDict(
+    "BatchDisassociateProjectAssetsResponseTypeDef",
     {
-        "quality": QualityType,
+        "errors": List[AssetErrorDetailsTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class AssetPropertyValueTypeDef(
-    _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
-):
-    pass
+CreateAccessPolicyResponseTypeDef = TypedDict(
+    "CreateAccessPolicyResponseTypeDef",
+    {
+        "accessPolicyId": str,
+        "accessPolicyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBulkImportJobResponseTypeDef = TypedDict(
+    "CreateBulkImportJobResponseTypeDef",
+    {
+        "jobId": str,
+        "jobName": str,
+        "jobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDashboardResponseTypeDef = TypedDict(
+    "CreateDashboardResponseTypeDef",
+    {
+        "dashboardId": str,
+        "dashboardArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGatewayResponseTypeDef = TypedDict(
+    "CreateGatewayResponseTypeDef",
+    {
+        "gatewayId": str,
+        "gatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "projectId": str,
+        "projectArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDashboardResponseTypeDef = TypedDict(
+    "DescribeDashboardResponseTypeDef",
+    {
+        "dashboardId": str,
+        "dashboardArn": str,
+        "dashboardName": str,
+        "projectId": str,
+        "dashboardDescription": str,
+        "dashboardDefinition": str,
+        "dashboardCreationDate": datetime,
+        "dashboardLastUpdateDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGatewayCapabilityConfigurationResponseTypeDef = TypedDict(
+    "DescribeGatewayCapabilityConfigurationResponseTypeDef",
+    {
+        "gatewayId": str,
+        "capabilityNamespace": str,
+        "capabilityConfiguration": str,
+        "capabilitySyncStatus": CapabilitySyncStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeProjectResponseTypeDef = TypedDict(
+    "DescribeProjectResponseTypeDef",
+    {
+        "projectId": str,
+        "projectArn": str,
+        "projectName": str,
+        "portalId": str,
+        "projectDescription": str,
+        "projectCreationDate": datetime,
+        "projectLastUpdateDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTimeSeriesResponseTypeDef = TypedDict(
+    "DescribeTimeSeriesResponseTypeDef",
+    {
+        "assetId": str,
+        "propertyId": str,
+        "alias": str,
+        "timeSeriesId": str,
+        "dataType": PropertyDataTypeType,
+        "dataTypeSpec": str,
+        "timeSeriesCreationDate": datetime,
+        "timeSeriesLastUpdateDate": datetime,
+        "timeSeriesArn": str,
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
+ListProjectAssetsResponseTypeDef = TypedDict(
+    "ListProjectAssetsResponseTypeDef",
+    {
+        "assetIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewayCapabilityConfigurationResponseTypeDef = TypedDict(
+    "UpdateGatewayCapabilityConfigurationResponseTypeDef",
+    {
+        "capabilityNamespace": str,
+        "capabilitySyncStatus": CapabilitySyncStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef",
     {
         "entries": Sequence[BatchGetAssetPropertyAggregatesEntryTypeDef],
     },
 )
@@ -2827,34 +2257,27 @@
     "FileFormatTypeDef",
     {
         "csv": CsvTypeDef,
     },
     total=False,
 )
 
-MultiLayerStorageOutputTypeDef = TypedDict(
-    "MultiLayerStorageOutputTypeDef",
-    {
-        "customerManagedS3Storage": CustomerManagedS3StorageOutputTypeDef,
-    },
-)
-
 MultiLayerStorageTypeDef = TypedDict(
     "MultiLayerStorageTypeDef",
     {
         "customerManagedS3Storage": CustomerManagedS3StorageTypeDef,
     },
 )
 
 ListDashboardsResponseTypeDef = TypedDict(
     "ListDashboardsResponseTypeDef",
     {
         "dashboardSummaries": List[DashboardSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeAssetModelRequestAssetModelActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeAssetModelRequestAssetModelActiveWaitTypeDef",
     {
         "assetModelId": str,
@@ -2977,16 +2400,23 @@
     _OptionalDescribePortalRequestPortalNotExistsWaitTypeDef,
 ):
     pass
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
-        "loggingOptions": LoggingOptionsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "loggingOptions": LoggingOptionsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutLoggingOptionsRequestRequestTypeDef = TypedDict(
+    "PutLoggingOptionsRequestRequestTypeDef",
+    {
+        "loggingOptions": LoggingOptionsTypeDef,
     },
 )
 
 _RequiredErrorDetailsTypeDef = TypedDict(
     "_RequiredErrorDetailsTypeDef",
     {
         "code": ErrorCodeType,
@@ -3000,107 +2430,338 @@
     },
     total=False,
 )
 
 class ErrorDetailsTypeDef(_RequiredErrorDetailsTypeDef, _OptionalErrorDetailsTypeDef):
     pass
 
-ExpressionVariableOutputTypeDef = TypedDict(
-    "ExpressionVariableOutputTypeDef",
-    {
-        "name": str,
-        "value": VariableValueOutputTypeDef,
-    },
-)
-
 ExpressionVariableTypeDef = TypedDict(
     "ExpressionVariableTypeDef",
     {
         "name": str,
         "value": VariableValueTypeDef,
     },
 )
 
-MeasurementProcessingConfigOutputTypeDef = TypedDict(
-    "MeasurementProcessingConfigOutputTypeDef",
+MeasurementProcessingConfigTypeDef = TypedDict(
+    "MeasurementProcessingConfigTypeDef",
     {
-        "forwardingConfig": ForwardingConfigOutputTypeDef,
+        "forwardingConfig": ForwardingConfigTypeDef,
     },
 )
 
-_RequiredTransformProcessingConfigOutputTypeDef = TypedDict(
-    "_RequiredTransformProcessingConfigOutputTypeDef",
+_RequiredTransformProcessingConfigTypeDef = TypedDict(
+    "_RequiredTransformProcessingConfigTypeDef",
     {
         "computeLocation": ComputeLocationType,
     },
 )
-_OptionalTransformProcessingConfigOutputTypeDef = TypedDict(
-    "_OptionalTransformProcessingConfigOutputTypeDef",
+_OptionalTransformProcessingConfigTypeDef = TypedDict(
+    "_OptionalTransformProcessingConfigTypeDef",
     {
-        "forwardingConfig": ForwardingConfigOutputTypeDef,
+        "forwardingConfig": ForwardingConfigTypeDef,
     },
     total=False,
 )
 
-class TransformProcessingConfigOutputTypeDef(
-    _RequiredTransformProcessingConfigOutputTypeDef, _OptionalTransformProcessingConfigOutputTypeDef
+class TransformProcessingConfigTypeDef(
+    _RequiredTransformProcessingConfigTypeDef, _OptionalTransformProcessingConfigTypeDef
 ):
     pass
 
-MeasurementProcessingConfigTypeDef = TypedDict(
-    "MeasurementProcessingConfigTypeDef",
+GatewayPlatformTypeDef = TypedDict(
+    "GatewayPlatformTypeDef",
     {
-        "forwardingConfig": ForwardingConfigTypeDef,
+        "greengrass": GreengrassTypeDef,
+        "greengrassV2": GreengrassV2TypeDef,
     },
+    total=False,
 )
 
-_RequiredTransformProcessingConfigTypeDef = TypedDict(
-    "_RequiredTransformProcessingConfigTypeDef",
+_RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef = TypedDict(
+    "_RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
     {
-        "computeLocation": ComputeLocationType,
+        "aggregateTypes": Sequence[AggregateTypeType],
+        "resolution": str,
+        "startDate": Union[datetime, str],
+        "endDate": Union[datetime, str],
     },
 )
-_OptionalTransformProcessingConfigTypeDef = TypedDict(
-    "_OptionalTransformProcessingConfigTypeDef",
+_OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef = TypedDict(
+    "_OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
     {
-        "forwardingConfig": ForwardingConfigTypeDef,
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+        "qualities": Sequence[QualityType],
+        "timeOrdering": TimeOrderingType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class TransformProcessingConfigTypeDef(
-    _RequiredTransformProcessingConfigTypeDef, _OptionalTransformProcessingConfigTypeDef
+class GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef(
+    _RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
+    _OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
 ):
     pass
 
-GatewayPlatformOutputTypeDef = TypedDict(
-    "GatewayPlatformOutputTypeDef",
+GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef = TypedDict(
+    "GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef",
     {
-        "greengrass": GreengrassOutputTypeDef,
-        "greengrassV2": GreengrassV2OutputTypeDef,
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+        "startDate": Union[datetime, str],
+        "endDate": Union[datetime, str],
+        "qualities": Sequence[QualityType],
+        "timeOrdering": TimeOrderingType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-GatewayPlatformTypeDef = TypedDict(
-    "GatewayPlatformTypeDef",
+_RequiredGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef = TypedDict(
+    "_RequiredGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef",
     {
-        "greengrass": GreengrassTypeDef,
-        "greengrassV2": GreengrassV2TypeDef,
+        "startTimeInSeconds": int,
+        "endTimeInSeconds": int,
+        "quality": QualityType,
+        "intervalInSeconds": int,
+        "type": str,
+    },
+)
+_OptionalGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef = TypedDict(
+    "_OptionalGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef",
+    {
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+        "startTimeOffsetInNanos": int,
+        "endTimeOffsetInNanos": int,
+        "intervalWindowInSeconds": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-IdentityOutputTypeDef = TypedDict(
-    "IdentityOutputTypeDef",
+class GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef(
+    _RequiredGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
+    _OptionalGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
+):
+    pass
+
+ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef = TypedDict(
+    "ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef",
     {
-        "user": UserIdentityOutputTypeDef,
-        "group": GroupIdentityOutputTypeDef,
-        "iamUser": IAMUserIdentityOutputTypeDef,
-        "iamRole": IAMRoleIdentityOutputTypeDef,
+        "identityType": IdentityTypeType,
+        "identityId": str,
+        "resourceType": ResourceTypeType,
+        "resourceId": str,
+        "iamArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef = TypedDict(
+    "_RequiredListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef",
+    {
+        "assetModelId": str,
+    },
+)
+_OptionalListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef = TypedDict(
+    "_OptionalListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef",
+    {
+        "filter": ListAssetModelPropertiesFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef(
+    _RequiredListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
+    _OptionalListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
+):
+    pass
+
+ListAssetModelsRequestListAssetModelsPaginateTypeDef = TypedDict(
+    "ListAssetModelsRequestListAssetModelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef = TypedDict(
+    "_RequiredListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef",
+    {
+        "assetId": str,
+    },
+)
+_OptionalListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef = TypedDict(
+    "_OptionalListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef",
+    {
+        "filter": ListAssetPropertiesFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef(
+    _RequiredListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
+    _OptionalListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef = TypedDict(
+    "_RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
+    {
+        "assetId": str,
+        "traversalType": Literal["PATH_TO_ROOT"],
+    },
+)
+_OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef = TypedDict(
+    "_OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef(
+    _RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
+    _OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
+):
+    pass
+
+ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
+    "ListAssetsRequestListAssetsPaginateTypeDef",
+    {
+        "assetModelId": str,
+        "filter": ListAssetsFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef",
+    {
+        "assetId": str,
+    },
+)
+_OptionalListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef",
+    {
+        "hierarchyId": str,
+        "traversalDirection": TraversalDirectionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef(
+    _RequiredListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
+    _OptionalListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
+):
+    pass
+
+ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef = TypedDict(
+    "ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef",
+    {
+        "filter": ListBulkImportJobsFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDashboardsRequestListDashboardsPaginateTypeDef = TypedDict(
+    "_RequiredListDashboardsRequestListDashboardsPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListDashboardsRequestListDashboardsPaginateTypeDef = TypedDict(
+    "_OptionalListDashboardsRequestListDashboardsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDashboardsRequestListDashboardsPaginateTypeDef(
+    _RequiredListDashboardsRequestListDashboardsPaginateTypeDef,
+    _OptionalListDashboardsRequestListDashboardsPaginateTypeDef,
+):
+    pass
+
+ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPortalsRequestListPortalsPaginateTypeDef = TypedDict(
+    "ListPortalsRequestListPortalsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListProjectAssetsRequestListProjectAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListProjectAssetsRequestListProjectAssetsPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListProjectAssetsRequestListProjectAssetsPaginateTypeDef(
+    _RequiredListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
+    _OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
+):
+    pass
+
+_RequiredListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "_RequiredListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "portalId": str,
+    },
+)
+_OptionalListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "_OptionalListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListProjectsRequestListProjectsPaginateTypeDef(
+    _RequiredListProjectsRequestListProjectsPaginateTypeDef,
+    _OptionalListProjectsRequestListProjectsPaginateTypeDef,
+):
+    pass
+
+ListTimeSeriesRequestListTimeSeriesPaginateTypeDef = TypedDict(
+    "ListTimeSeriesRequestListTimeSeriesPaginateTypeDef",
+    {
+        "assetId": str,
+        "aliasPrefix": str,
+        "timeSeriesType": ListTimeSeriesTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 IdentityTypeDef = TypedDict(
     "IdentityTypeDef",
     {
@@ -3113,51 +2774,36 @@
 )
 
 ListBulkImportJobsResponseTypeDef = TypedDict(
     "ListBulkImportJobsResponseTypeDef",
     {
         "jobSummaries": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "projectSummaries": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTimeSeriesResponseTypeDef = TypedDict(
     "ListTimeSeriesResponseTypeDef",
     {
         "TimeSeriesSummaries": List[TimeSeriesSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutLoggingOptionsRequestRequestTypeDef = TypedDict(
-    "PutLoggingOptionsRequestRequestTypeDef",
-    {
-        "loggingOptions": LoggingOptionsTypeDef,
-    },
-)
-
-MetricWindowOutputTypeDef = TypedDict(
-    "MetricWindowOutputTypeDef",
-    {
-        "tumbling": TumblingWindowOutputTypeDef,
-    },
-    total=False,
-)
-
 MetricWindowTypeDef = TypedDict(
     "MetricWindowTypeDef",
     {
         "tumbling": TumblingWindowTypeDef,
     },
     total=False,
 )
@@ -3175,23 +2821,14 @@
     },
     total=False,
 )
 
 class PortalStatusTypeDef(_RequiredPortalStatusTypeDef, _OptionalPortalStatusTypeDef):
     pass
 
-ResourceOutputTypeDef = TypedDict(
-    "ResourceOutputTypeDef",
-    {
-        "portal": PortalResourceOutputTypeDef,
-        "project": ProjectResourceOutputTypeDef,
-    },
-    total=False,
-)
-
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "portal": PortalResourceTypeDef,
         "project": ProjectResourceTypeDef,
     },
     total=False,
@@ -3206,33 +2843,33 @@
 )
 
 GetAssetPropertyAggregatesResponseTypeDef = TypedDict(
     "GetAssetPropertyAggregatesResponseTypeDef",
     {
         "aggregatedValues": List[AggregatedValueTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssetRelationshipsResponseTypeDef = TypedDict(
     "ListAssetRelationshipsResponseTypeDef",
     {
         "assetRelationshipSummaries": List[AssetRelationshipSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssetPropertiesResponseTypeDef = TypedDict(
     "ListAssetPropertiesResponseTypeDef",
     {
         "assetPropertySummaries": List[AssetPropertySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssetCompositeModelTypeDef = TypedDict(
     "_RequiredAssetCompositeModelTypeDef",
     {
         "name": str,
@@ -3262,61 +2899,52 @@
     },
 )
 
 BatchGetAssetPropertyValueHistorySuccessEntryTypeDef = TypedDict(
     "BatchGetAssetPropertyValueHistorySuccessEntryTypeDef",
     {
         "entryId": str,
-        "assetPropertyValueHistory": List[AssetPropertyValueOutputTypeDef],
+        "assetPropertyValueHistory": List[AssetPropertyValueTypeDef],
     },
 )
 
 _RequiredBatchGetAssetPropertyValueSuccessEntryTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueSuccessEntryTypeDef",
     {
         "entryId": str,
     },
 )
 _OptionalBatchGetAssetPropertyValueSuccessEntryTypeDef = TypedDict(
     "_OptionalBatchGetAssetPropertyValueSuccessEntryTypeDef",
     {
-        "assetPropertyValue": AssetPropertyValueOutputTypeDef,
+        "assetPropertyValue": AssetPropertyValueTypeDef,
     },
     total=False,
 )
 
 class BatchGetAssetPropertyValueSuccessEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueSuccessEntryTypeDef,
     _OptionalBatchGetAssetPropertyValueSuccessEntryTypeDef,
 ):
     pass
 
 GetAssetPropertyValueHistoryResponseTypeDef = TypedDict(
     "GetAssetPropertyValueHistoryResponseTypeDef",
     {
-        "assetPropertyValueHistory": List[AssetPropertyValueOutputTypeDef],
+        "assetPropertyValueHistory": List[AssetPropertyValueTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssetPropertyValueResponseTypeDef = TypedDict(
     "GetAssetPropertyValueResponseTypeDef",
     {
-        "propertyValue": AssetPropertyValueOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetInterpolatedAssetPropertyValuesResponseTypeDef = TypedDict(
-    "GetInterpolatedAssetPropertyValuesResponseTypeDef",
-    {
-        "interpolatedAssetPropertyValues": List[InterpolatedAssetPropertyValueTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "propertyValue": AssetPropertyValueTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutAssetPropertyValueEntryTypeDef = TypedDict(
     "_RequiredPutAssetPropertyValueEntryTypeDef",
     {
         "entryId": str,
@@ -3334,31 +2962,40 @@
 )
 
 class PutAssetPropertyValueEntryTypeDef(
     _RequiredPutAssetPropertyValueEntryTypeDef, _OptionalPutAssetPropertyValueEntryTypeDef
 ):
     pass
 
+GetInterpolatedAssetPropertyValuesResponseTypeDef = TypedDict(
+    "GetInterpolatedAssetPropertyValuesResponseTypeDef",
+    {
+        "interpolatedAssetPropertyValues": List[InterpolatedAssetPropertyValueTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeDefaultEncryptionConfigurationResponseTypeDef = TypedDict(
     "DescribeDefaultEncryptionConfigurationResponseTypeDef",
     {
         "encryptionType": EncryptionTypeType,
         "kmsKeyArn": str,
         "configurationStatus": ConfigurationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDefaultEncryptionConfigurationResponseTypeDef = TypedDict(
     "PutDefaultEncryptionConfigurationResponseTypeDef",
     {
         "encryptionType": EncryptionTypeType,
         "kmsKeyArn": str,
         "configurationStatus": ConfigurationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdatePortalRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePortalRequestRequestTypeDef",
     {
         "portalId": str,
@@ -3398,32 +3035,20 @@
     },
 )
 
 DescribeStorageConfigurationResponseTypeDef = TypedDict(
     "DescribeStorageConfigurationResponseTypeDef",
     {
         "storageType": StorageTypeType,
-        "multiLayerStorage": MultiLayerStorageOutputTypeDef,
+        "multiLayerStorage": MultiLayerStorageTypeDef,
         "disassociatedDataStorage": DisassociatedDataStorageStateType,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
+        "retentionPeriod": RetentionPeriodTypeDef,
         "configurationStatus": ConfigurationStatusTypeDef,
         "lastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutStorageConfigurationResponseTypeDef = TypedDict(
-    "PutStorageConfigurationResponseTypeDef",
-    {
-        "storageType": StorageTypeType,
-        "multiLayerStorage": MultiLayerStorageOutputTypeDef,
-        "disassociatedDataStorage": DisassociatedDataStorageStateType,
-        "retentionPeriod": RetentionPeriodOutputTypeDef,
-        "configurationStatus": ConfigurationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutStorageConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutStorageConfigurationRequestRequestTypeDef",
     {
         "storageType": StorageTypeType,
@@ -3441,14 +3066,26 @@
 
 class PutStorageConfigurationRequestRequestTypeDef(
     _RequiredPutStorageConfigurationRequestRequestTypeDef,
     _OptionalPutStorageConfigurationRequestRequestTypeDef,
 ):
     pass
 
+PutStorageConfigurationResponseTypeDef = TypedDict(
+    "PutStorageConfigurationResponseTypeDef",
+    {
+        "storageType": StorageTypeType,
+        "multiLayerStorage": MultiLayerStorageTypeDef,
+        "disassociatedDataStorage": DisassociatedDataStorageStateType,
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "configurationStatus": ConfigurationStatusTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredAssetModelStatusTypeDef = TypedDict(
     "_RequiredAssetModelStatusTypeDef",
     {
         "state": AssetModelStateType,
     },
 )
 _OptionalAssetModelStatusTypeDef = TypedDict(
@@ -3475,48 +3112,40 @@
     },
     total=False,
 )
 
 class AssetStatusTypeDef(_RequiredAssetStatusTypeDef, _OptionalAssetStatusTypeDef):
     pass
 
-MeasurementOutputTypeDef = TypedDict(
-    "MeasurementOutputTypeDef",
+MeasurementTypeDef = TypedDict(
+    "MeasurementTypeDef",
     {
-        "processingConfig": MeasurementProcessingConfigOutputTypeDef,
+        "processingConfig": MeasurementProcessingConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredTransformOutputTypeDef = TypedDict(
     "_RequiredTransformOutputTypeDef",
     {
         "expression": str,
-        "variables": List[ExpressionVariableOutputTypeDef],
+        "variables": List[ExpressionVariableTypeDef],
     },
 )
 _OptionalTransformOutputTypeDef = TypedDict(
     "_OptionalTransformOutputTypeDef",
     {
-        "processingConfig": TransformProcessingConfigOutputTypeDef,
+        "processingConfig": TransformProcessingConfigTypeDef,
     },
     total=False,
 )
 
 class TransformOutputTypeDef(_RequiredTransformOutputTypeDef, _OptionalTransformOutputTypeDef):
     pass
 
-MeasurementTypeDef = TypedDict(
-    "MeasurementTypeDef",
-    {
-        "processingConfig": MeasurementProcessingConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredTransformTypeDef = TypedDict(
     "_RequiredTransformTypeDef",
     {
         "expression": str,
         "variables": Sequence[ExpressionVariableTypeDef],
     },
 )
@@ -3527,25 +3156,45 @@
     },
     total=False,
 )
 
 class TransformTypeDef(_RequiredTransformTypeDef, _OptionalTransformTypeDef):
     pass
 
+_RequiredCreateGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateGatewayRequestRequestTypeDef",
+    {
+        "gatewayName": str,
+        "gatewayPlatform": GatewayPlatformTypeDef,
+    },
+)
+_OptionalCreateGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateGatewayRequestRequestTypeDef",
+    {
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateGatewayRequestRequestTypeDef(
+    _RequiredCreateGatewayRequestRequestTypeDef, _OptionalCreateGatewayRequestRequestTypeDef
+):
+    pass
+
 DescribeGatewayResponseTypeDef = TypedDict(
     "DescribeGatewayResponseTypeDef",
     {
         "gatewayId": str,
         "gatewayName": str,
         "gatewayArn": str,
-        "gatewayPlatform": GatewayPlatformOutputTypeDef,
+        "gatewayPlatform": GatewayPlatformTypeDef,
         "gatewayCapabilitySummaries": List[GatewayCapabilitySummaryTypeDef],
         "creationDate": datetime,
         "lastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGatewaySummaryTypeDef = TypedDict(
     "_RequiredGatewaySummaryTypeDef",
     {
         "gatewayId": str,
@@ -3553,55 +3202,35 @@
         "creationDate": datetime,
         "lastUpdateDate": datetime,
     },
 )
 _OptionalGatewaySummaryTypeDef = TypedDict(
     "_OptionalGatewaySummaryTypeDef",
     {
-        "gatewayPlatform": GatewayPlatformOutputTypeDef,
+        "gatewayPlatform": GatewayPlatformTypeDef,
         "gatewayCapabilitySummaries": List[GatewayCapabilitySummaryTypeDef],
     },
     total=False,
 )
 
 class GatewaySummaryTypeDef(_RequiredGatewaySummaryTypeDef, _OptionalGatewaySummaryTypeDef):
     pass
 
-_RequiredCreateGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateGatewayRequestRequestTypeDef",
-    {
-        "gatewayName": str,
-        "gatewayPlatform": GatewayPlatformTypeDef,
-    },
-)
-_OptionalCreateGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateGatewayRequestRequestTypeDef",
-    {
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateGatewayRequestRequestTypeDef(
-    _RequiredCreateGatewayRequestRequestTypeDef, _OptionalCreateGatewayRequestRequestTypeDef
-):
-    pass
-
 _RequiredMetricOutputTypeDef = TypedDict(
     "_RequiredMetricOutputTypeDef",
     {
         "expression": str,
-        "variables": List[ExpressionVariableOutputTypeDef],
-        "window": MetricWindowOutputTypeDef,
+        "variables": List[ExpressionVariableTypeDef],
+        "window": MetricWindowTypeDef,
     },
 )
 _OptionalMetricOutputTypeDef = TypedDict(
     "_OptionalMetricOutputTypeDef",
     {
-        "processingConfig": MetricProcessingConfigOutputTypeDef,
+        "processingConfig": MetricProcessingConfigTypeDef,
     },
     total=False,
 )
 
 class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
     pass
 
@@ -3628,23 +3257,23 @@
     "CreatePortalResponseTypeDef",
     {
         "portalId": str,
         "portalArn": str,
         "portalStartUrl": str,
         "portalStatus": PortalStatusTypeDef,
         "ssoApplicationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePortalResponseTypeDef = TypedDict(
     "DeletePortalResponseTypeDef",
     {
         "portalStatus": PortalStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePortalResponseTypeDef = TypedDict(
     "DescribePortalResponseTypeDef",
     {
         "portalId": str,
@@ -3657,16 +3286,16 @@
         "portalStatus": PortalStatusTypeDef,
         "portalCreationDate": datetime,
         "portalLastUpdateDate": datetime,
         "portalLogoImageLocation": ImageLocationTypeDef,
         "roleArn": str,
         "portalAuthMode": AuthModeType,
         "notificationSenderEmail": str,
-        "alarms": AlarmsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "alarms": AlarmsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPortalSummaryTypeDef = TypedDict(
     "_RequiredPortalSummaryTypeDef",
     {
         "id": str,
@@ -3689,24 +3318,24 @@
 class PortalSummaryTypeDef(_RequiredPortalSummaryTypeDef, _OptionalPortalSummaryTypeDef):
     pass
 
 UpdatePortalResponseTypeDef = TypedDict(
     "UpdatePortalResponseTypeDef",
     {
         "portalStatus": PortalStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAccessPolicySummaryTypeDef = TypedDict(
     "_RequiredAccessPolicySummaryTypeDef",
     {
         "id": str,
-        "identity": IdentityOutputTypeDef,
-        "resource": ResourceOutputTypeDef,
+        "identity": IdentityTypeDef,
+        "resource": ResourceTypeDef,
         "permission": PermissionType,
     },
 )
 _OptionalAccessPolicySummaryTypeDef = TypedDict(
     "_OptionalAccessPolicySummaryTypeDef",
     {
         "creationDate": datetime,
@@ -3716,28 +3345,14 @@
 )
 
 class AccessPolicySummaryTypeDef(
     _RequiredAccessPolicySummaryTypeDef, _OptionalAccessPolicySummaryTypeDef
 ):
     pass
 
-DescribeAccessPolicyResponseTypeDef = TypedDict(
-    "DescribeAccessPolicyResponseTypeDef",
-    {
-        "accessPolicyId": str,
-        "accessPolicyArn": str,
-        "accessPolicyIdentity": IdentityOutputTypeDef,
-        "accessPolicyResource": ResourceOutputTypeDef,
-        "accessPolicyPermission": PermissionType,
-        "accessPolicyCreationDate": datetime,
-        "accessPolicyLastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateAccessPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPolicyRequestRequestTypeDef",
     {
         "accessPolicyIdentity": IdentityTypeDef,
         "accessPolicyResource": ResourceTypeDef,
         "accessPolicyPermission": PermissionType,
     },
@@ -3753,14 +3368,28 @@
 
 class CreateAccessPolicyRequestRequestTypeDef(
     _RequiredCreateAccessPolicyRequestRequestTypeDef,
     _OptionalCreateAccessPolicyRequestRequestTypeDef,
 ):
     pass
 
+DescribeAccessPolicyResponseTypeDef = TypedDict(
+    "DescribeAccessPolicyResponseTypeDef",
+    {
+        "accessPolicyId": str,
+        "accessPolicyArn": str,
+        "accessPolicyIdentity": IdentityTypeDef,
+        "accessPolicyResource": ResourceTypeDef,
+        "accessPolicyPermission": PermissionType,
+        "accessPolicyCreationDate": datetime,
+        "accessPolicyLastUpdateDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateAccessPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAccessPolicyRequestRequestTypeDef",
     {
         "accessPolicyId": str,
         "accessPolicyIdentity": IdentityTypeDef,
         "accessPolicyResource": ResourceTypeDef,
         "accessPolicyPermission": PermissionType,
@@ -3783,45 +3412,45 @@
 BatchGetAssetPropertyAggregatesResponseTypeDef = TypedDict(
     "BatchGetAssetPropertyAggregatesResponseTypeDef",
     {
         "errorEntries": List[BatchGetAssetPropertyAggregatesErrorEntryTypeDef],
         "successEntries": List[BatchGetAssetPropertyAggregatesSuccessEntryTypeDef],
         "skippedEntries": List[BatchGetAssetPropertyAggregatesSkippedEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutAssetPropertyValueResponseTypeDef = TypedDict(
     "BatchPutAssetPropertyValueResponseTypeDef",
     {
         "errorEntries": List[BatchPutAssetPropertyErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetAssetPropertyValueHistoryResponseTypeDef = TypedDict(
     "BatchGetAssetPropertyValueHistoryResponseTypeDef",
     {
         "errorEntries": List[BatchGetAssetPropertyValueHistoryErrorEntryTypeDef],
         "successEntries": List[BatchGetAssetPropertyValueHistorySuccessEntryTypeDef],
         "skippedEntries": List[BatchGetAssetPropertyValueHistorySkippedEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetAssetPropertyValueResponseTypeDef = TypedDict(
     "BatchGetAssetPropertyValueResponseTypeDef",
     {
         "errorEntries": List[BatchGetAssetPropertyValueErrorEntryTypeDef],
         "successEntries": List[BatchGetAssetPropertyValueSuccessEntryTypeDef],
         "skippedEntries": List[BatchGetAssetPropertyValueSkippedEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutAssetPropertyValueRequestRequestTypeDef = TypedDict(
     "BatchPutAssetPropertyValueRequestRequestTypeDef",
     {
         "entries": Sequence[PutAssetPropertyValueEntryTypeDef],
@@ -3831,20 +3460,20 @@
 DescribeBulkImportJobResponseTypeDef = TypedDict(
     "DescribeBulkImportJobResponseTypeDef",
     {
         "jobId": str,
         "jobName": str,
         "jobStatus": JobStatusType,
         "jobRoleArn": str,
-        "files": List[FileOutputTypeDef],
-        "errorReportLocation": ErrorReportLocationOutputTypeDef,
+        "files": List[FileTypeDef],
+        "errorReportLocation": ErrorReportLocationTypeDef,
         "jobConfiguration": JobConfigurationOutputTypeDef,
         "jobCreationDate": datetime,
         "jobLastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBulkImportJobRequestRequestTypeDef = TypedDict(
     "CreateBulkImportJobRequestRequestTypeDef",
     {
         "jobName": str,
@@ -3870,31 +3499,31 @@
 
 CreateAssetModelResponseTypeDef = TypedDict(
     "CreateAssetModelResponseTypeDef",
     {
         "assetModelId": str,
         "assetModelArn": str,
         "assetModelStatus": AssetModelStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAssetModelResponseTypeDef = TypedDict(
     "DeleteAssetModelResponseTypeDef",
     {
         "assetModelStatus": AssetModelStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssetModelResponseTypeDef = TypedDict(
     "UpdateAssetModelResponseTypeDef",
     {
         "assetModelStatus": AssetModelStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssetSummaryTypeDef = TypedDict(
     "_RequiredAssetSummaryTypeDef",
     {
         "id": str,
@@ -3946,23 +3575,23 @@
 
 CreateAssetResponseTypeDef = TypedDict(
     "CreateAssetResponseTypeDef",
     {
         "assetId": str,
         "assetArn": str,
         "assetStatus": AssetStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAssetResponseTypeDef = TypedDict(
     "DeleteAssetResponseTypeDef",
     {
         "assetStatus": AssetStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssetResponseTypeDef = TypedDict(
     "DescribeAssetResponseTypeDef",
     {
         "assetId": str,
@@ -3972,40 +3601,40 @@
         "assetProperties": List[AssetPropertyTypeDef],
         "assetHierarchies": List[AssetHierarchyTypeDef],
         "assetCompositeModels": List[AssetCompositeModelTypeDef],
         "assetCreationDate": datetime,
         "assetLastUpdateDate": datetime,
         "assetStatus": AssetStatusTypeDef,
         "assetDescription": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssetResponseTypeDef = TypedDict(
     "UpdateAssetResponseTypeDef",
     {
         "assetStatus": AssetStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGatewaysResponseTypeDef = TypedDict(
     "ListGatewaysResponseTypeDef",
     {
         "gatewaySummaries": List[GatewaySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PropertyTypeOutputTypeDef = TypedDict(
     "PropertyTypeOutputTypeDef",
     {
-        "attribute": AttributeOutputTypeDef,
-        "measurement": MeasurementOutputTypeDef,
+        "attribute": AttributeTypeDef,
+        "measurement": MeasurementTypeDef,
         "transform": TransformOutputTypeDef,
         "metric": MetricOutputTypeDef,
     },
     total=False,
 )
 
 PropertyTypeTypeDef = TypedDict(
@@ -4020,51 +3649,51 @@
 )
 
 ListPortalsResponseTypeDef = TypedDict(
     "ListPortalsResponseTypeDef",
     {
         "portalSummaries": List[PortalSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccessPoliciesResponseTypeDef = TypedDict(
     "ListAccessPoliciesResponseTypeDef",
     {
         "accessPolicySummaries": List[AccessPolicySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssetModelsResponseTypeDef = TypedDict(
     "ListAssetModelsResponseTypeDef",
     {
         "assetModelSummaries": List[AssetModelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssetsResponseTypeDef = TypedDict(
     "ListAssetsResponseTypeDef",
     {
         "assetSummaries": List[AssetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssociatedAssetsResponseTypeDef = TypedDict(
     "ListAssociatedAssetsResponseTypeDef",
     {
         "assetSummaries": List[AssociatedAssetsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssetModelPropertyOutputTypeDef = TypedDict(
     "_RequiredAssetModelPropertyOutputTypeDef",
     {
         "name": str,
@@ -4201,15 +3830,15 @@
     pass
 
 ListAssetModelPropertiesResponseTypeDef = TypedDict(
     "ListAssetModelPropertiesResponseTypeDef",
     {
         "assetModelPropertySummaries": List[AssetModelPropertySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCompositeModelPropertyTypeDef = TypedDict(
     "_RequiredCompositeModelPropertyTypeDef",
     {
         "name": str,
@@ -4278,32 +3907,32 @@
     "DescribeAssetModelResponseTypeDef",
     {
         "assetModelId": str,
         "assetModelArn": str,
         "assetModelName": str,
         "assetModelDescription": str,
         "assetModelProperties": List[AssetModelPropertyOutputTypeDef],
-        "assetModelHierarchies": List[AssetModelHierarchyOutputTypeDef],
+        "assetModelHierarchies": List[AssetModelHierarchyTypeDef],
         "assetModelCompositeModels": List[AssetModelCompositeModelOutputTypeDef],
         "assetModelCreationDate": datetime,
         "assetModelLastUpdateDate": datetime,
         "assetModelStatus": AssetModelStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssetPropertyResponseTypeDef = TypedDict(
     "DescribeAssetPropertyResponseTypeDef",
     {
         "assetId": str,
         "assetName": str,
         "assetModelId": str,
         "assetProperty": PropertyTypeDef,
         "compositeModel": CompositeModelPropertyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAssetModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssetModelRequestRequestTypeDef",
     {
         "assetModelName": str,
```

### Comparing `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/waiter.py` & `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/waiter.pyi` & `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/PKG-INFO` & `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsitewise
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTSiteWise 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTSiteWise 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsitewise)](https://pepy.tech/project/mypy-boto3-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSiteWise 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[boto3.IoTSiteWise 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
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
 [mypy-boto3-iotsitewise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/).
 
 See how it helps to find and fix potential bugs:
 
@@ -471,57 +471,47 @@
 
 `mypy_boto3_iotsitewise.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotsitewise.type_defs import (
     AggregatesTypeDef,
-    AlarmsOutputTypeDef,
     AlarmsTypeDef,
     AssetErrorDetailsTypeDef,
     AssetHierarchyInfoTypeDef,
     AssetHierarchyTypeDef,
     AssetModelHierarchyDefinitionTypeDef,
-    AssetModelHierarchyOutputTypeDef,
     AssetModelHierarchyTypeDef,
     PropertyNotificationTypeDef,
-    TimeInNanosOutputTypeDef,
-    VariantOutputTypeDef,
     TimeInNanosTypeDef,
     VariantTypeDef,
     AssociateAssetsRequestRequestTypeDef,
     AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
-    AttributeOutputTypeDef,
     AttributeTypeDef,
     BatchAssociateProjectAssetsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     BatchDisassociateProjectAssetsRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesEntryTypeDef,
     BatchGetAssetPropertyAggregatesErrorEntryTypeDef,
     BatchGetAssetPropertyAggregatesErrorInfoTypeDef,
     BatchGetAssetPropertyValueEntryTypeDef,
     BatchGetAssetPropertyValueErrorEntryTypeDef,
     BatchGetAssetPropertyValueErrorInfoTypeDef,
     BatchGetAssetPropertyValueHistoryEntryTypeDef,
     BatchGetAssetPropertyValueHistoryErrorEntryTypeDef,
     BatchGetAssetPropertyValueHistoryErrorInfoTypeDef,
     ConfigurationErrorDetailsTypeDef,
-    CreateAccessPolicyResponseTypeDef,
     CreateAssetRequestRequestTypeDef,
     ErrorReportLocationTypeDef,
     FileTypeDef,
-    CreateBulkImportJobResponseTypeDef,
     CreateDashboardRequestRequestTypeDef,
-    CreateDashboardResponseTypeDef,
-    CreateGatewayResponseTypeDef,
     ImageFileTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
     CsvOutputTypeDef,
     CsvTypeDef,
-    CustomerManagedS3StorageOutputTypeDef,
     CustomerManagedS3StorageTypeDef,
     DashboardSummaryTypeDef,
     DeleteAccessPolicyRequestRequestTypeDef,
     DeleteAssetModelRequestRequestTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeleteDashboardRequestRequestTypeDef,
     DeleteGatewayRequestRequestTypeDef,
@@ -530,204 +520,182 @@
     DeleteTimeSeriesRequestRequestTypeDef,
     DescribeAccessPolicyRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeAssetModelRequestRequestTypeDef,
     DescribeAssetPropertyRequestRequestTypeDef,
     DescribeAssetRequestRequestTypeDef,
     DescribeBulkImportJobRequestRequestTypeDef,
-    ErrorReportLocationOutputTypeDef,
-    FileOutputTypeDef,
     DescribeDashboardRequestRequestTypeDef,
-    DescribeDashboardResponseTypeDef,
     DescribeGatewayCapabilityConfigurationRequestRequestTypeDef,
-    DescribeGatewayCapabilityConfigurationResponseTypeDef,
     DescribeGatewayRequestRequestTypeDef,
     GatewayCapabilitySummaryTypeDef,
-    LoggingOptionsOutputTypeDef,
+    LoggingOptionsTypeDef,
     DescribePortalRequestRequestTypeDef,
     ImageLocationTypeDef,
     DescribeProjectRequestRequestTypeDef,
-    DescribeProjectResponseTypeDef,
-    RetentionPeriodOutputTypeDef,
+    RetentionPeriodTypeDef,
     DescribeTimeSeriesRequestRequestTypeDef,
-    DescribeTimeSeriesResponseTypeDef,
     DetailedErrorTypeDef,
     DisassociateAssetsRequestRequestTypeDef,
     DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    VariableValueOutputTypeDef,
     VariableValueTypeDef,
-    ForwardingConfigOutputTypeDef,
     ForwardingConfigTypeDef,
-    GreengrassOutputTypeDef,
-    GreengrassV2OutputTypeDef,
     GreengrassTypeDef,
     GreengrassV2TypeDef,
-    GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetAssetPropertyAggregatesRequestRequestTypeDef,
-    GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef,
     GetAssetPropertyValueHistoryRequestRequestTypeDef,
     GetAssetPropertyValueRequestRequestTypeDef,
-    GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
     GetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
-    GroupIdentityOutputTypeDef,
     GroupIdentityTypeDef,
-    IAMRoleIdentityOutputTypeDef,
     IAMRoleIdentityTypeDef,
-    IAMUserIdentityOutputTypeDef,
     IAMUserIdentityTypeDef,
-    UserIdentityOutputTypeDef,
     UserIdentityTypeDef,
     JobSummaryTypeDef,
-    ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef,
     ListAccessPoliciesRequestRequestTypeDef,
-    ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
     ListAssetModelPropertiesRequestRequestTypeDef,
-    ListAssetModelsRequestListAssetModelsPaginateTypeDef,
     ListAssetModelsRequestRequestTypeDef,
-    ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
     ListAssetPropertiesRequestRequestTypeDef,
-    ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
     ListAssetRelationshipsRequestRequestTypeDef,
-    ListAssetsRequestListAssetsPaginateTypeDef,
     ListAssetsRequestRequestTypeDef,
-    ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
     ListAssociatedAssetsRequestRequestTypeDef,
-    ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef,
     ListBulkImportJobsRequestRequestTypeDef,
-    ListDashboardsRequestListDashboardsPaginateTypeDef,
     ListDashboardsRequestRequestTypeDef,
-    ListGatewaysRequestListGatewaysPaginateTypeDef,
     ListGatewaysRequestRequestTypeDef,
-    ListPortalsRequestListPortalsPaginateTypeDef,
     ListPortalsRequestRequestTypeDef,
-    ListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
     ListProjectAssetsRequestRequestTypeDef,
-    ListProjectAssetsResponseTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTimeSeriesRequestListTimeSeriesPaginateTypeDef,
     ListTimeSeriesRequestRequestTypeDef,
     TimeSeriesSummaryTypeDef,
-    LoggingOptionsTypeDef,
-    MetricProcessingConfigOutputTypeDef,
     MetricProcessingConfigTypeDef,
-    TumblingWindowOutputTypeDef,
     TumblingWindowTypeDef,
     MonitorErrorDetailsTypeDef,
-    PaginatorConfigTypeDef,
-    PortalResourceOutputTypeDef,
     PortalResourceTypeDef,
-    ProjectResourceOutputTypeDef,
     ProjectResourceTypeDef,
     PutDefaultEncryptionConfigurationRequestRequestTypeDef,
-    RetentionPeriodTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssetPropertyRequestRequestTypeDef,
     UpdateAssetRequestRequestTypeDef,
     UpdateDashboardRequestRequestTypeDef,
     UpdateGatewayCapabilityConfigurationRequestRequestTypeDef,
-    UpdateGatewayCapabilityConfigurationResponseTypeDef,
     UpdateGatewayRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     AggregatedValueTypeDef,
-    BatchAssociateProjectAssetsResponseTypeDef,
-    BatchDisassociateProjectAssetsResponseTypeDef,
     AssetRelationshipSummaryTypeDef,
     AssetPropertySummaryTypeDef,
     AssetPropertyTypeDef,
     BatchPutAssetPropertyErrorTypeDef,
-    AssetPropertyValueOutputTypeDef,
-    InterpolatedAssetPropertyValueTypeDef,
     AssetPropertyValueTypeDef,
+    InterpolatedAssetPropertyValueTypeDef,
+    BatchAssociateProjectAssetsResponseTypeDef,
+    BatchDisassociateProjectAssetsResponseTypeDef,
+    CreateAccessPolicyResponseTypeDef,
+    CreateBulkImportJobResponseTypeDef,
+    CreateDashboardResponseTypeDef,
+    CreateGatewayResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    DescribeDashboardResponseTypeDef,
+    DescribeGatewayCapabilityConfigurationResponseTypeDef,
+    DescribeProjectResponseTypeDef,
+    DescribeTimeSeriesResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListProjectAssetsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateGatewayCapabilityConfigurationResponseTypeDef,
     BatchGetAssetPropertyAggregatesRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesSkippedEntryTypeDef,
     BatchGetAssetPropertyValueRequestRequestTypeDef,
     BatchGetAssetPropertyValueSkippedEntryTypeDef,
     BatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
     BatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
     ConfigurationStatusTypeDef,
     CreatePortalRequestRequestTypeDef,
     ImageTypeDef,
     FileFormatOutputTypeDef,
     FileFormatTypeDef,
-    MultiLayerStorageOutputTypeDef,
     MultiLayerStorageTypeDef,
     ListDashboardsResponseTypeDef,
     DescribeAssetModelRequestAssetModelActiveWaitTypeDef,
     DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef,
     DescribeAssetRequestAssetActiveWaitTypeDef,
     DescribeAssetRequestAssetNotExistsWaitTypeDef,
     DescribePortalRequestPortalActiveWaitTypeDef,
     DescribePortalRequestPortalNotExistsWaitTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
+    PutLoggingOptionsRequestRequestTypeDef,
     ErrorDetailsTypeDef,
-    ExpressionVariableOutputTypeDef,
     ExpressionVariableTypeDef,
-    MeasurementProcessingConfigOutputTypeDef,
-    TransformProcessingConfigOutputTypeDef,
     MeasurementProcessingConfigTypeDef,
     TransformProcessingConfigTypeDef,
-    GatewayPlatformOutputTypeDef,
     GatewayPlatformTypeDef,
-    IdentityOutputTypeDef,
+    GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
+    GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef,
+    GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
+    ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef,
+    ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
+    ListAssetModelsRequestListAssetModelsPaginateTypeDef,
+    ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
+    ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
+    ListAssetsRequestListAssetsPaginateTypeDef,
+    ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
+    ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef,
+    ListDashboardsRequestListDashboardsPaginateTypeDef,
+    ListGatewaysRequestListGatewaysPaginateTypeDef,
+    ListPortalsRequestListPortalsPaginateTypeDef,
+    ListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListTimeSeriesRequestListTimeSeriesPaginateTypeDef,
     IdentityTypeDef,
     ListBulkImportJobsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTimeSeriesResponseTypeDef,
-    PutLoggingOptionsRequestRequestTypeDef,
-    MetricWindowOutputTypeDef,
     MetricWindowTypeDef,
     PortalStatusTypeDef,
-    ResourceOutputTypeDef,
     ResourceTypeDef,
     BatchGetAssetPropertyAggregatesSuccessEntryTypeDef,
     GetAssetPropertyAggregatesResponseTypeDef,
     ListAssetRelationshipsResponseTypeDef,
     ListAssetPropertiesResponseTypeDef,
     AssetCompositeModelTypeDef,
     BatchPutAssetPropertyErrorEntryTypeDef,
     BatchGetAssetPropertyValueHistorySuccessEntryTypeDef,
     BatchGetAssetPropertyValueSuccessEntryTypeDef,
     GetAssetPropertyValueHistoryResponseTypeDef,
     GetAssetPropertyValueResponseTypeDef,
-    GetInterpolatedAssetPropertyValuesResponseTypeDef,
     PutAssetPropertyValueEntryTypeDef,
+    GetInterpolatedAssetPropertyValuesResponseTypeDef,
     DescribeDefaultEncryptionConfigurationResponseTypeDef,
     PutDefaultEncryptionConfigurationResponseTypeDef,
     UpdatePortalRequestRequestTypeDef,
     JobConfigurationOutputTypeDef,
     JobConfigurationTypeDef,
     DescribeStorageConfigurationResponseTypeDef,
-    PutStorageConfigurationResponseTypeDef,
     PutStorageConfigurationRequestRequestTypeDef,
+    PutStorageConfigurationResponseTypeDef,
     AssetModelStatusTypeDef,
     AssetStatusTypeDef,
-    MeasurementOutputTypeDef,
-    TransformOutputTypeDef,
     MeasurementTypeDef,
+    TransformOutputTypeDef,
     TransformTypeDef,
+    CreateGatewayRequestRequestTypeDef,
     DescribeGatewayResponseTypeDef,
     GatewaySummaryTypeDef,
-    CreateGatewayRequestRequestTypeDef,
     MetricOutputTypeDef,
     MetricTypeDef,
     CreatePortalResponseTypeDef,
     DeletePortalResponseTypeDef,
     DescribePortalResponseTypeDef,
     PortalSummaryTypeDef,
     UpdatePortalResponseTypeDef,
     AccessPolicySummaryTypeDef,
-    DescribeAccessPolicyResponseTypeDef,
     CreateAccessPolicyRequestRequestTypeDef,
+    DescribeAccessPolicyResponseTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesResponseTypeDef,
     BatchPutAssetPropertyValueResponseTypeDef,
     BatchGetAssetPropertyValueHistoryResponseTypeDef,
     BatchGetAssetPropertyValueResponseTypeDef,
     BatchPutAssetPropertyValueRequestRequestTypeDef,
     DescribeBulkImportJobResponseTypeDef,
```

### Comparing `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/SOURCES.txt` & `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.12/setup.py` & `mypy-boto3-iotsitewise-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotsitewise",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iotsitewise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTSiteWise 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.IoTSiteWise 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

