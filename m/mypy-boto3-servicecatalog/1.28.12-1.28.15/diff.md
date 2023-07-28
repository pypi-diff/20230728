# Comparing `tmp/mypy-boto3-servicecatalog-1.28.12.tar.gz` & `tmp/mypy-boto3-servicecatalog-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-servicecatalog-1.28.12.tar", last modified: Thu Jul 27 11:49:38 2023, max compression
+gzip compressed data, was "mypy-boto3-servicecatalog-1.28.15.tar", last modified: Fri Jul 28 20:43:44 2023, max compression
```

## Comparing `mypy-boto3-servicecatalog-1.28.12.tar` & `mypy-boto3-servicecatalog-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.589291 mypy-boto3-servicecatalog-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27839 2023-07-27 11:49:38.585291 mypy-boto3-servicecatalog-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26324 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.585291 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76162 2023-07-27 11:46:41.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    76049 2023-07-27 11:46:41.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-07-27 11:46:42.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-07-27 11:46:41.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21847 2023-07-27 11:46:41.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21828 2023-07-27 11:46:41.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   103851 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   103706 2023-07-27 11:46:45.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.585291 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27839 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.589291 mypy-boto3-servicecatalog-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.285872 mypy-boto3-servicecatalog-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:12.000000 mypy-boto3-servicecatalog-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27654 2023-07-28 20:43:44.281872 mypy-boto3-servicecatalog-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26139 2023-07-28 20:39:12.000000 mypy-boto3-servicecatalog-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.265871 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-28 20:39:12.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-28 20:39:12.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:39:12.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76162 2023-07-28 20:39:13.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76049 2023-07-28 20:39:13.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-07-28 20:39:14.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-07-28 20:39:13.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21847 2023-07-28 20:39:13.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21828 2023-07-28 20:39:13.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:12.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   102689 2023-07-28 20:39:16.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102544 2023-07-28 20:39:15.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:12.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.281872 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27654 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:44.285872 mypy-boto3-servicecatalog-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:39:12.000000 mypy-boto3-servicecatalog-1.28.15/setup.py
```

### Comparing `mypy-boto3-servicecatalog-1.28.12/LICENSE` & `mypy-boto3-servicecatalog-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.12/PKG-INFO` & `mypy-boto3-servicecatalog-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog
-Version: 1.28.12
-Summary: Type annotations for boto3.ServiceCatalog 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ServiceCatalog 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicecatalog)](https://pepy.tech/project/mypy-boto3-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceCatalog 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[boto3.ServiceCatalog 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [mypy-boto3-servicecatalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -442,23 +442,21 @@
     AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     AssociateTagOptionWithResourceInputRequestTypeDef,
     ServiceActionAssociationTypeDef,
     FailedServiceActionAssociationTypeDef,
     ResponseMetadataTypeDef,
     BudgetDetailTypeDef,
     CloudWatchDashboardTypeDef,
-    CodeStarParametersOutputTypeDef,
     CodeStarParametersTypeDef,
     ConstraintDetailTypeDef,
     ConstraintSummaryTypeDef,
     CopyProductInputRequestTypeDef,
     CreateConstraintInputRequestTypeDef,
     TagTypeDef,
     PortfolioDetailTypeDef,
-    TagOutputTypeDef,
     OrganizationNodeTypeDef,
     ProvisioningArtifactPropertiesTypeDef,
     ProvisioningArtifactDetailTypeDef,
     UpdateProvisioningParameterTypeDef,
     CreateServiceActionInputRequestTypeDef,
     CreateTagOptionInputRequestTypeDef,
     TagOptionDetailTypeDef,
@@ -510,15 +508,14 @@
     LastSyncTypeDef,
     PaginatorConfigTypeDef,
     ListAcceptedPortfolioSharesInputRequestTypeDef,
     ListBudgetsForResourceInputRequestTypeDef,
     ListConstraintsForPortfolioInputRequestTypeDef,
     ListLaunchPathsInputRequestTypeDef,
     ListOrganizationPortfolioAccessInputRequestTypeDef,
-    OrganizationNodeOutputTypeDef,
     ListPortfolioAccessInputRequestTypeDef,
     ListPortfoliosForProductInputRequestTypeDef,
     ListPortfoliosInputRequestTypeDef,
     ListPrincipalsForPortfolioInputRequestTypeDef,
     PrincipalTypeDef,
     ProvisionedProductPlanSummaryTypeDef,
     ListProvisioningArtifactsForServiceActionInputRequestTypeDef,
@@ -533,15 +530,14 @@
     StackInstanceTypeDef,
     ListTagOptionsFiltersTypeDef,
     NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     ParameterConstraintsTypeDef,
     ProductViewAggregationValueTypeDef,
     ProvisioningParameterTypeDef,
     ProvisioningPreferencesTypeDef,
-    UpdateProvisioningParameterOutputTypeDef,
     RecordErrorTypeDef,
     RecordTagTypeDef,
     RejectPortfolioShareInputRequestTypeDef,
     ResourceTargetDefinitionTypeDef,
     SearchProductsAsAdminInputRequestTypeDef,
     SearchProductsInputRequestTypeDef,
     ShareErrorTypeDef,
@@ -565,37 +561,38 @@
     DeletePortfolioShareOutputTypeDef,
     DescribeCopyProductStatusOutputTypeDef,
     GetAWSOrganizationsAccessStatusOutputTypeDef,
     ListPortfolioAccessOutputTypeDef,
     UpdatePortfolioShareOutputTypeDef,
     UpdateProvisionedProductPropertiesOutputTypeDef,
     ListBudgetsForResourceOutputTypeDef,
-    SourceConnectionParametersOutputTypeDef,
     SourceConnectionParametersTypeDef,
     CreateConstraintOutputTypeDef,
     DescribeConstraintOutputTypeDef,
     ListConstraintsForPortfolioOutputTypeDef,
     UpdateConstraintOutputTypeDef,
     CreatePortfolioInputRequestTypeDef,
+    LaunchPathSummaryTypeDef,
+    ProvisionedProductAttributeTypeDef,
     UpdatePortfolioInputRequestTypeDef,
+    CreatePortfolioOutputTypeDef,
     ListAcceptedPortfolioSharesOutputTypeDef,
     ListPortfoliosForProductOutputTypeDef,
     ListPortfoliosOutputTypeDef,
-    CreatePortfolioOutputTypeDef,
-    LaunchPathSummaryTypeDef,
-    ProvisionedProductAttributeTypeDef,
     UpdatePortfolioOutputTypeDef,
     CreatePortfolioShareInputRequestTypeDef,
     DeletePortfolioShareInputRequestTypeDef,
+    ListOrganizationPortfolioAccessOutputTypeDef,
     UpdatePortfolioShareInputRequestTypeDef,
     CreateProvisioningArtifactInputRequestTypeDef,
     CreateProvisioningArtifactOutputTypeDef,
     ListProvisioningArtifactsOutputTypeDef,
     UpdateProvisioningArtifactOutputTypeDef,
     CreateProvisionedProductPlanInputRequestTypeDef,
+    ProvisionedProductPlanDetailsTypeDef,
     CreateTagOptionOutputTypeDef,
     DescribePortfolioOutputTypeDef,
     DescribeTagOptionOutputTypeDef,
     ListTagOptionsOutputTypeDef,
     UpdateTagOptionOutputTypeDef,
     DescribePortfolioSharesOutputTypeDef,
     DescribeProductOutputTypeDef,
@@ -617,30 +614,28 @@
     ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef,
     ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
     ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
     ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
     ListServiceActionsInputListServiceActionsPaginateTypeDef,
     ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef,
     SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef,
-    ListOrganizationPortfolioAccessOutputTypeDef,
     ListPrincipalsForPortfolioOutputTypeDef,
     ListProvisionedProductPlansOutputTypeDef,
     ListRecordHistoryInputListRecordHistoryPaginateTypeDef,
     ListRecordHistoryInputRequestTypeDef,
     ListResourcesForTagOptionOutputTypeDef,
     ListServiceActionsForProvisioningArtifactOutputTypeDef,
     ListServiceActionsOutputTypeDef,
     ServiceActionDetailTypeDef,
     ListStackInstancesForProvisionedProductOutputTypeDef,
     ListTagOptionsInputListTagOptionsPaginateTypeDef,
     ListTagOptionsInputRequestTypeDef,
     ProvisioningArtifactParameterTypeDef,
     SearchProductsOutputTypeDef,
     ProvisionProductInputRequestTypeDef,
-    ProvisionedProductPlanDetailsTypeDef,
     RecordDetailTypeDef,
     ResourceChangeDetailTypeDef,
     ShareDetailsTypeDef,
     UpdateProvisionedProductInputRequestTypeDef,
     SourceConnectionDetailTypeDef,
     SourceConnectionTypeDef,
     ListLaunchPathsOutputTypeDef,
```

### Comparing `mypy-boto3-servicecatalog-1.28.12/README.md` & `mypy-boto3-servicecatalog-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicecatalog)](https://pepy.tech/project/mypy-boto3-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceCatalog 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[boto3.ServiceCatalog 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [mypy-boto3-servicecatalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -410,23 +410,21 @@
     AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     AssociateTagOptionWithResourceInputRequestTypeDef,
     ServiceActionAssociationTypeDef,
     FailedServiceActionAssociationTypeDef,
     ResponseMetadataTypeDef,
     BudgetDetailTypeDef,
     CloudWatchDashboardTypeDef,
-    CodeStarParametersOutputTypeDef,
     CodeStarParametersTypeDef,
     ConstraintDetailTypeDef,
     ConstraintSummaryTypeDef,
     CopyProductInputRequestTypeDef,
     CreateConstraintInputRequestTypeDef,
     TagTypeDef,
     PortfolioDetailTypeDef,
-    TagOutputTypeDef,
     OrganizationNodeTypeDef,
     ProvisioningArtifactPropertiesTypeDef,
     ProvisioningArtifactDetailTypeDef,
     UpdateProvisioningParameterTypeDef,
     CreateServiceActionInputRequestTypeDef,
     CreateTagOptionInputRequestTypeDef,
     TagOptionDetailTypeDef,
@@ -478,15 +476,14 @@
     LastSyncTypeDef,
     PaginatorConfigTypeDef,
     ListAcceptedPortfolioSharesInputRequestTypeDef,
     ListBudgetsForResourceInputRequestTypeDef,
     ListConstraintsForPortfolioInputRequestTypeDef,
     ListLaunchPathsInputRequestTypeDef,
     ListOrganizationPortfolioAccessInputRequestTypeDef,
-    OrganizationNodeOutputTypeDef,
     ListPortfolioAccessInputRequestTypeDef,
     ListPortfoliosForProductInputRequestTypeDef,
     ListPortfoliosInputRequestTypeDef,
     ListPrincipalsForPortfolioInputRequestTypeDef,
     PrincipalTypeDef,
     ProvisionedProductPlanSummaryTypeDef,
     ListProvisioningArtifactsForServiceActionInputRequestTypeDef,
@@ -501,15 +498,14 @@
     StackInstanceTypeDef,
     ListTagOptionsFiltersTypeDef,
     NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     ParameterConstraintsTypeDef,
     ProductViewAggregationValueTypeDef,
     ProvisioningParameterTypeDef,
     ProvisioningPreferencesTypeDef,
-    UpdateProvisioningParameterOutputTypeDef,
     RecordErrorTypeDef,
     RecordTagTypeDef,
     RejectPortfolioShareInputRequestTypeDef,
     ResourceTargetDefinitionTypeDef,
     SearchProductsAsAdminInputRequestTypeDef,
     SearchProductsInputRequestTypeDef,
     ShareErrorTypeDef,
@@ -533,37 +529,38 @@
     DeletePortfolioShareOutputTypeDef,
     DescribeCopyProductStatusOutputTypeDef,
     GetAWSOrganizationsAccessStatusOutputTypeDef,
     ListPortfolioAccessOutputTypeDef,
     UpdatePortfolioShareOutputTypeDef,
     UpdateProvisionedProductPropertiesOutputTypeDef,
     ListBudgetsForResourceOutputTypeDef,
-    SourceConnectionParametersOutputTypeDef,
     SourceConnectionParametersTypeDef,
     CreateConstraintOutputTypeDef,
     DescribeConstraintOutputTypeDef,
     ListConstraintsForPortfolioOutputTypeDef,
     UpdateConstraintOutputTypeDef,
     CreatePortfolioInputRequestTypeDef,
+    LaunchPathSummaryTypeDef,
+    ProvisionedProductAttributeTypeDef,
     UpdatePortfolioInputRequestTypeDef,
+    CreatePortfolioOutputTypeDef,
     ListAcceptedPortfolioSharesOutputTypeDef,
     ListPortfoliosForProductOutputTypeDef,
     ListPortfoliosOutputTypeDef,
-    CreatePortfolioOutputTypeDef,
-    LaunchPathSummaryTypeDef,
-    ProvisionedProductAttributeTypeDef,
     UpdatePortfolioOutputTypeDef,
     CreatePortfolioShareInputRequestTypeDef,
     DeletePortfolioShareInputRequestTypeDef,
+    ListOrganizationPortfolioAccessOutputTypeDef,
     UpdatePortfolioShareInputRequestTypeDef,
     CreateProvisioningArtifactInputRequestTypeDef,
     CreateProvisioningArtifactOutputTypeDef,
     ListProvisioningArtifactsOutputTypeDef,
     UpdateProvisioningArtifactOutputTypeDef,
     CreateProvisionedProductPlanInputRequestTypeDef,
+    ProvisionedProductPlanDetailsTypeDef,
     CreateTagOptionOutputTypeDef,
     DescribePortfolioOutputTypeDef,
     DescribeTagOptionOutputTypeDef,
     ListTagOptionsOutputTypeDef,
     UpdateTagOptionOutputTypeDef,
     DescribePortfolioSharesOutputTypeDef,
     DescribeProductOutputTypeDef,
@@ -585,30 +582,28 @@
     ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef,
     ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
     ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
     ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
     ListServiceActionsInputListServiceActionsPaginateTypeDef,
     ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef,
     SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef,
-    ListOrganizationPortfolioAccessOutputTypeDef,
     ListPrincipalsForPortfolioOutputTypeDef,
     ListProvisionedProductPlansOutputTypeDef,
     ListRecordHistoryInputListRecordHistoryPaginateTypeDef,
     ListRecordHistoryInputRequestTypeDef,
     ListResourcesForTagOptionOutputTypeDef,
     ListServiceActionsForProvisioningArtifactOutputTypeDef,
     ListServiceActionsOutputTypeDef,
     ServiceActionDetailTypeDef,
     ListStackInstancesForProvisionedProductOutputTypeDef,
     ListTagOptionsInputListTagOptionsPaginateTypeDef,
     ListTagOptionsInputRequestTypeDef,
     ProvisioningArtifactParameterTypeDef,
     SearchProductsOutputTypeDef,
     ProvisionProductInputRequestTypeDef,
-    ProvisionedProductPlanDetailsTypeDef,
     RecordDetailTypeDef,
     ResourceChangeDetailTypeDef,
     ShareDetailsTypeDef,
     UpdateProvisionedProductInputRequestTypeDef,
     SourceConnectionDetailTypeDef,
     SourceConnectionTypeDef,
     ListLaunchPathsOutputTypeDef,
```

### Comparing `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/__init__.py` & `mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/__init__.pyi` & `mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/__main__.py` & `mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ServiceCatalog 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ServiceCatalog 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog\nOther"
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

### Comparing `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/client.py` & `mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/client.pyi` & `mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/literals.py` & `mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/literals.pyi` & `mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/paginator.py` & `mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/paginator.pyi` & `mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/type_defs.py` & `mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,23 +67,21 @@
     "AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     "AssociateTagOptionWithResourceInputRequestTypeDef",
     "ServiceActionAssociationTypeDef",
     "FailedServiceActionAssociationTypeDef",
     "ResponseMetadataTypeDef",
     "BudgetDetailTypeDef",
     "CloudWatchDashboardTypeDef",
-    "CodeStarParametersOutputTypeDef",
     "CodeStarParametersTypeDef",
     "ConstraintDetailTypeDef",
     "ConstraintSummaryTypeDef",
     "CopyProductInputRequestTypeDef",
     "CreateConstraintInputRequestTypeDef",
     "TagTypeDef",
     "PortfolioDetailTypeDef",
-    "TagOutputTypeDef",
     "OrganizationNodeTypeDef",
     "ProvisioningArtifactPropertiesTypeDef",
     "ProvisioningArtifactDetailTypeDef",
     "UpdateProvisioningParameterTypeDef",
     "CreateServiceActionInputRequestTypeDef",
     "CreateTagOptionInputRequestTypeDef",
     "TagOptionDetailTypeDef",
@@ -135,15 +133,14 @@
     "LastSyncTypeDef",
     "PaginatorConfigTypeDef",
     "ListAcceptedPortfolioSharesInputRequestTypeDef",
     "ListBudgetsForResourceInputRequestTypeDef",
     "ListConstraintsForPortfolioInputRequestTypeDef",
     "ListLaunchPathsInputRequestTypeDef",
     "ListOrganizationPortfolioAccessInputRequestTypeDef",
-    "OrganizationNodeOutputTypeDef",
     "ListPortfolioAccessInputRequestTypeDef",
     "ListPortfoliosForProductInputRequestTypeDef",
     "ListPortfoliosInputRequestTypeDef",
     "ListPrincipalsForPortfolioInputRequestTypeDef",
     "PrincipalTypeDef",
     "ProvisionedProductPlanSummaryTypeDef",
     "ListProvisioningArtifactsForServiceActionInputRequestTypeDef",
@@ -158,15 +155,14 @@
     "StackInstanceTypeDef",
     "ListTagOptionsFiltersTypeDef",
     "NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     "ParameterConstraintsTypeDef",
     "ProductViewAggregationValueTypeDef",
     "ProvisioningParameterTypeDef",
     "ProvisioningPreferencesTypeDef",
-    "UpdateProvisioningParameterOutputTypeDef",
     "RecordErrorTypeDef",
     "RecordTagTypeDef",
     "RejectPortfolioShareInputRequestTypeDef",
     "ResourceTargetDefinitionTypeDef",
     "SearchProductsAsAdminInputRequestTypeDef",
     "SearchProductsInputRequestTypeDef",
     "ShareErrorTypeDef",
@@ -190,37 +186,38 @@
     "DeletePortfolioShareOutputTypeDef",
     "DescribeCopyProductStatusOutputTypeDef",
     "GetAWSOrganizationsAccessStatusOutputTypeDef",
     "ListPortfolioAccessOutputTypeDef",
     "UpdatePortfolioShareOutputTypeDef",
     "UpdateProvisionedProductPropertiesOutputTypeDef",
     "ListBudgetsForResourceOutputTypeDef",
-    "SourceConnectionParametersOutputTypeDef",
     "SourceConnectionParametersTypeDef",
     "CreateConstraintOutputTypeDef",
     "DescribeConstraintOutputTypeDef",
     "ListConstraintsForPortfolioOutputTypeDef",
     "UpdateConstraintOutputTypeDef",
     "CreatePortfolioInputRequestTypeDef",
+    "LaunchPathSummaryTypeDef",
+    "ProvisionedProductAttributeTypeDef",
     "UpdatePortfolioInputRequestTypeDef",
+    "CreatePortfolioOutputTypeDef",
     "ListAcceptedPortfolioSharesOutputTypeDef",
     "ListPortfoliosForProductOutputTypeDef",
     "ListPortfoliosOutputTypeDef",
-    "CreatePortfolioOutputTypeDef",
-    "LaunchPathSummaryTypeDef",
-    "ProvisionedProductAttributeTypeDef",
     "UpdatePortfolioOutputTypeDef",
     "CreatePortfolioShareInputRequestTypeDef",
     "DeletePortfolioShareInputRequestTypeDef",
+    "ListOrganizationPortfolioAccessOutputTypeDef",
     "UpdatePortfolioShareInputRequestTypeDef",
     "CreateProvisioningArtifactInputRequestTypeDef",
     "CreateProvisioningArtifactOutputTypeDef",
     "ListProvisioningArtifactsOutputTypeDef",
     "UpdateProvisioningArtifactOutputTypeDef",
     "CreateProvisionedProductPlanInputRequestTypeDef",
+    "ProvisionedProductPlanDetailsTypeDef",
     "CreateTagOptionOutputTypeDef",
     "DescribePortfolioOutputTypeDef",
     "DescribeTagOptionOutputTypeDef",
     "ListTagOptionsOutputTypeDef",
     "UpdateTagOptionOutputTypeDef",
     "DescribePortfolioSharesOutputTypeDef",
     "DescribeProductOutputTypeDef",
@@ -242,30 +239,28 @@
     "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
     "ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
     "ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
     "ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
     "ListServiceActionsInputListServiceActionsPaginateTypeDef",
     "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
     "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
-    "ListOrganizationPortfolioAccessOutputTypeDef",
     "ListPrincipalsForPortfolioOutputTypeDef",
     "ListProvisionedProductPlansOutputTypeDef",
     "ListRecordHistoryInputListRecordHistoryPaginateTypeDef",
     "ListRecordHistoryInputRequestTypeDef",
     "ListResourcesForTagOptionOutputTypeDef",
     "ListServiceActionsForProvisioningArtifactOutputTypeDef",
     "ListServiceActionsOutputTypeDef",
     "ServiceActionDetailTypeDef",
     "ListStackInstancesForProvisionedProductOutputTypeDef",
     "ListTagOptionsInputListTagOptionsPaginateTypeDef",
     "ListTagOptionsInputRequestTypeDef",
     "ProvisioningArtifactParameterTypeDef",
     "SearchProductsOutputTypeDef",
     "ProvisionProductInputRequestTypeDef",
-    "ProvisionedProductPlanDetailsTypeDef",
     "RecordDetailTypeDef",
     "ResourceChangeDetailTypeDef",
     "ShareDetailsTypeDef",
     "UpdateProvisionedProductInputRequestTypeDef",
     "SourceConnectionDetailTypeDef",
     "SourceConnectionTypeDef",
     "ListLaunchPathsOutputTypeDef",
@@ -461,24 +456,14 @@
     "CloudWatchDashboardTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-CodeStarParametersOutputTypeDef = TypedDict(
-    "CodeStarParametersOutputTypeDef",
-    {
-        "ConnectionArn": str,
-        "Repository": str,
-        "Branch": str,
-        "ArtifactPath": str,
-    },
-)
-
 CodeStarParametersTypeDef = TypedDict(
     "CodeStarParametersTypeDef",
     {
         "ConnectionArn": str,
         "Repository": str,
         "Branch": str,
         "ArtifactPath": str,
@@ -576,22 +561,14 @@
         "Description": str,
         "CreatedTime": datetime,
         "ProviderName": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 OrganizationNodeTypeDef = TypedDict(
     "OrganizationNodeTypeDef",
     {
         "Type": OrganizationNodeTypeType,
         "Value": str,
     },
     total=False,
@@ -1539,23 +1516,14 @@
 class ListOrganizationPortfolioAccessInputRequestTypeDef(
     _RequiredListOrganizationPortfolioAccessInputRequestTypeDef,
     _OptionalListOrganizationPortfolioAccessInputRequestTypeDef,
 ):
     pass
 
 
-OrganizationNodeOutputTypeDef = TypedDict(
-    "OrganizationNodeOutputTypeDef",
-    {
-        "Type": OrganizationNodeTypeType,
-        "Value": str,
-    },
-    total=False,
-)
-
 _RequiredListPortfolioAccessInputRequestTypeDef = TypedDict(
     "_RequiredListPortfolioAccessInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalListPortfolioAccessInputRequestTypeDef = TypedDict(
@@ -1903,24 +1871,14 @@
         "StackSetFailureTolerancePercentage": int,
         "StackSetMaxConcurrencyCount": int,
         "StackSetMaxConcurrencyPercentage": int,
     },
     total=False,
 )
 
-UpdateProvisioningParameterOutputTypeDef = TypedDict(
-    "UpdateProvisioningParameterOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "UsePreviousValue": bool,
-    },
-    total=False,
-)
-
 RecordErrorTypeDef = TypedDict(
     "RecordErrorTypeDef",
     {
         "Code": str,
         "Description": str,
     },
     total=False,
@@ -2351,22 +2309,14 @@
     {
         "Budgets": List[BudgetDetailTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SourceConnectionParametersOutputTypeDef = TypedDict(
-    "SourceConnectionParametersOutputTypeDef",
-    {
-        "CodeStar": CodeStarParametersOutputTypeDef,
-    },
-    total=False,
-)
-
 SourceConnectionParametersTypeDef = TypedDict(
     "SourceConnectionParametersTypeDef",
     {
         "CodeStar": CodeStarParametersTypeDef,
     },
     total=False,
 )
@@ -2431,14 +2381,51 @@
 
 class CreatePortfolioInputRequestTypeDef(
     _RequiredCreatePortfolioInputRequestTypeDef, _OptionalCreatePortfolioInputRequestTypeDef
 ):
     pass
 
 
+LaunchPathSummaryTypeDef = TypedDict(
+    "LaunchPathSummaryTypeDef",
+    {
+        "Id": str,
+        "ConstraintSummaries": List[ConstraintSummaryTypeDef],
+        "Tags": List[TagTypeDef],
+        "Name": str,
+    },
+    total=False,
+)
+
+ProvisionedProductAttributeTypeDef = TypedDict(
+    "ProvisionedProductAttributeTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "Type": str,
+        "Id": str,
+        "Status": ProvisionedProductStatusType,
+        "StatusMessage": str,
+        "CreatedTime": datetime,
+        "IdempotencyToken": str,
+        "LastRecordId": str,
+        "LastProvisioningRecordId": str,
+        "LastSuccessfulProvisioningRecordId": str,
+        "Tags": List[TagTypeDef],
+        "PhysicalId": str,
+        "ProductId": str,
+        "ProductName": str,
+        "ProvisioningArtifactId": str,
+        "ProvisioningArtifactName": str,
+        "UserArn": str,
+        "UserArnSession": str,
+    },
+    total=False,
+)
+
 _RequiredUpdatePortfolioInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePortfolioInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePortfolioInputRequestTypeDef = TypedDict(
@@ -2457,14 +2444,23 @@
 
 class UpdatePortfolioInputRequestTypeDef(
     _RequiredUpdatePortfolioInputRequestTypeDef, _OptionalUpdatePortfolioInputRequestTypeDef
 ):
     pass
 
 
+CreatePortfolioOutputTypeDef = TypedDict(
+    "CreatePortfolioOutputTypeDef",
+    {
+        "PortfolioDetail": PortfolioDetailTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAcceptedPortfolioSharesOutputTypeDef = TypedDict(
     "ListAcceptedPortfolioSharesOutputTypeDef",
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2484,65 +2480,19 @@
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreatePortfolioOutputTypeDef = TypedDict(
-    "CreatePortfolioOutputTypeDef",
-    {
-        "PortfolioDetail": PortfolioDetailTypeDef,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LaunchPathSummaryTypeDef = TypedDict(
-    "LaunchPathSummaryTypeDef",
-    {
-        "Id": str,
-        "ConstraintSummaries": List[ConstraintSummaryTypeDef],
-        "Tags": List[TagOutputTypeDef],
-        "Name": str,
-    },
-    total=False,
-)
-
-ProvisionedProductAttributeTypeDef = TypedDict(
-    "ProvisionedProductAttributeTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Type": str,
-        "Id": str,
-        "Status": ProvisionedProductStatusType,
-        "StatusMessage": str,
-        "CreatedTime": datetime,
-        "IdempotencyToken": str,
-        "LastRecordId": str,
-        "LastProvisioningRecordId": str,
-        "LastSuccessfulProvisioningRecordId": str,
-        "Tags": List[TagOutputTypeDef],
-        "PhysicalId": str,
-        "ProductId": str,
-        "ProductName": str,
-        "ProvisioningArtifactId": str,
-        "ProvisioningArtifactName": str,
-        "UserArn": str,
-        "UserArnSession": str,
-    },
-    total=False,
-)
-
 UpdatePortfolioOutputTypeDef = TypedDict(
     "UpdatePortfolioOutputTypeDef",
     {
         "PortfolioDetail": PortfolioDetailTypeDef,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePortfolioShareInputRequestTypeDef = TypedDict(
     "_RequiredCreatePortfolioShareInputRequestTypeDef",
     {
@@ -2589,14 +2539,23 @@
 class DeletePortfolioShareInputRequestTypeDef(
     _RequiredDeletePortfolioShareInputRequestTypeDef,
     _OptionalDeletePortfolioShareInputRequestTypeDef,
 ):
     pass
 
 
+ListOrganizationPortfolioAccessOutputTypeDef = TypedDict(
+    "ListOrganizationPortfolioAccessOutputTypeDef",
+    {
+        "OrganizationNodes": List[OrganizationNodeTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdatePortfolioShareInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePortfolioShareInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalUpdatePortfolioShareInputRequestTypeDef = TypedDict(
@@ -2699,27 +2658,49 @@
 class CreateProvisionedProductPlanInputRequestTypeDef(
     _RequiredCreateProvisionedProductPlanInputRequestTypeDef,
     _OptionalCreateProvisionedProductPlanInputRequestTypeDef,
 ):
     pass
 
 
+ProvisionedProductPlanDetailsTypeDef = TypedDict(
+    "ProvisionedProductPlanDetailsTypeDef",
+    {
+        "CreatedTime": datetime,
+        "PathId": str,
+        "ProductId": str,
+        "PlanName": str,
+        "PlanId": str,
+        "ProvisionProductId": str,
+        "ProvisionProductName": str,
+        "PlanType": Literal["CLOUDFORMATION"],
+        "ProvisioningArtifactId": str,
+        "Status": ProvisionedProductPlanStatusType,
+        "UpdatedTime": datetime,
+        "NotificationArns": List[str],
+        "ProvisioningParameters": List[UpdateProvisioningParameterTypeDef],
+        "Tags": List[TagTypeDef],
+        "StatusMessage": str,
+    },
+    total=False,
+)
+
 CreateTagOptionOutputTypeDef = TypedDict(
     "CreateTagOptionOutputTypeDef",
     {
         "TagOptionDetail": TagOptionDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePortfolioOutputTypeDef = TypedDict(
     "DescribePortfolioOutputTypeDef",
     {
         "PortfolioDetail": PortfolioDetailTypeDef,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "TagOptions": List[TagOptionDetailTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagOptionOutputTypeDef = TypedDict(
@@ -3100,23 +3081,14 @@
         "SortOrder": SortOrderType,
         "ProductSource": Literal["ACCOUNT"],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListOrganizationPortfolioAccessOutputTypeDef = TypedDict(
-    "ListOrganizationPortfolioAccessOutputTypeDef",
-    {
-        "OrganizationNodes": List[OrganizationNodeOutputTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListPrincipalsForPortfolioOutputTypeDef = TypedDict(
     "ListPrincipalsForPortfolioOutputTypeDef",
     {
         "Principals": List[PrincipalTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3269,36 +3241,14 @@
 
 class ProvisionProductInputRequestTypeDef(
     _RequiredProvisionProductInputRequestTypeDef, _OptionalProvisionProductInputRequestTypeDef
 ):
     pass
 
 
-ProvisionedProductPlanDetailsTypeDef = TypedDict(
-    "ProvisionedProductPlanDetailsTypeDef",
-    {
-        "CreatedTime": datetime,
-        "PathId": str,
-        "ProductId": str,
-        "PlanName": str,
-        "PlanId": str,
-        "ProvisionProductId": str,
-        "ProvisionProductName": str,
-        "PlanType": Literal["CLOUDFORMATION"],
-        "ProvisioningArtifactId": str,
-        "Status": ProvisionedProductPlanStatusType,
-        "UpdatedTime": datetime,
-        "NotificationArns": List[str],
-        "ProvisioningParameters": List[UpdateProvisioningParameterOutputTypeDef],
-        "Tags": List[TagOutputTypeDef],
-        "StatusMessage": str,
-    },
-    total=False,
-)
-
 RecordDetailTypeDef = TypedDict(
     "RecordDetailTypeDef",
     {
         "RecordId": str,
         "ProvisionedProductName": str,
         "Status": RecordStatusType,
         "CreatedTime": datetime,
@@ -3368,15 +3318,15 @@
     pass
 
 
 SourceConnectionDetailTypeDef = TypedDict(
     "SourceConnectionDetailTypeDef",
     {
         "Type": Literal["CODESTAR"],
-        "ConnectionParameters": SourceConnectionParametersOutputTypeDef,
+        "ConnectionParameters": SourceConnectionParametersTypeDef,
         "LastSync": LastSyncTypeDef,
     },
     total=False,
 )
 
 _RequiredSourceConnectionTypeDef = TypedDict(
     "_RequiredSourceConnectionTypeDef",
@@ -3680,25 +3630,25 @@
 )
 
 CreateProductOutputTypeDef = TypedDict(
     "CreateProductOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProductAsAdminOutputTypeDef = TypedDict(
     "DescribeProductAsAdminOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
         "ProvisioningArtifactSummaries": List[ProvisioningArtifactSummaryTypeDef],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "TagOptions": List[TagOptionDetailTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchProductsAsAdminOutputTypeDef = TypedDict(
@@ -3710,11 +3660,11 @@
     },
 )
 
 UpdateProductOutputTypeDef = TypedDict(
     "UpdateProductOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/type_defs.pyi` & `mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -66,23 +66,21 @@
     "AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     "AssociateTagOptionWithResourceInputRequestTypeDef",
     "ServiceActionAssociationTypeDef",
     "FailedServiceActionAssociationTypeDef",
     "ResponseMetadataTypeDef",
     "BudgetDetailTypeDef",
     "CloudWatchDashboardTypeDef",
-    "CodeStarParametersOutputTypeDef",
     "CodeStarParametersTypeDef",
     "ConstraintDetailTypeDef",
     "ConstraintSummaryTypeDef",
     "CopyProductInputRequestTypeDef",
     "CreateConstraintInputRequestTypeDef",
     "TagTypeDef",
     "PortfolioDetailTypeDef",
-    "TagOutputTypeDef",
     "OrganizationNodeTypeDef",
     "ProvisioningArtifactPropertiesTypeDef",
     "ProvisioningArtifactDetailTypeDef",
     "UpdateProvisioningParameterTypeDef",
     "CreateServiceActionInputRequestTypeDef",
     "CreateTagOptionInputRequestTypeDef",
     "TagOptionDetailTypeDef",
@@ -134,15 +132,14 @@
     "LastSyncTypeDef",
     "PaginatorConfigTypeDef",
     "ListAcceptedPortfolioSharesInputRequestTypeDef",
     "ListBudgetsForResourceInputRequestTypeDef",
     "ListConstraintsForPortfolioInputRequestTypeDef",
     "ListLaunchPathsInputRequestTypeDef",
     "ListOrganizationPortfolioAccessInputRequestTypeDef",
-    "OrganizationNodeOutputTypeDef",
     "ListPortfolioAccessInputRequestTypeDef",
     "ListPortfoliosForProductInputRequestTypeDef",
     "ListPortfoliosInputRequestTypeDef",
     "ListPrincipalsForPortfolioInputRequestTypeDef",
     "PrincipalTypeDef",
     "ProvisionedProductPlanSummaryTypeDef",
     "ListProvisioningArtifactsForServiceActionInputRequestTypeDef",
@@ -157,15 +154,14 @@
     "StackInstanceTypeDef",
     "ListTagOptionsFiltersTypeDef",
     "NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     "ParameterConstraintsTypeDef",
     "ProductViewAggregationValueTypeDef",
     "ProvisioningParameterTypeDef",
     "ProvisioningPreferencesTypeDef",
-    "UpdateProvisioningParameterOutputTypeDef",
     "RecordErrorTypeDef",
     "RecordTagTypeDef",
     "RejectPortfolioShareInputRequestTypeDef",
     "ResourceTargetDefinitionTypeDef",
     "SearchProductsAsAdminInputRequestTypeDef",
     "SearchProductsInputRequestTypeDef",
     "ShareErrorTypeDef",
@@ -189,37 +185,38 @@
     "DeletePortfolioShareOutputTypeDef",
     "DescribeCopyProductStatusOutputTypeDef",
     "GetAWSOrganizationsAccessStatusOutputTypeDef",
     "ListPortfolioAccessOutputTypeDef",
     "UpdatePortfolioShareOutputTypeDef",
     "UpdateProvisionedProductPropertiesOutputTypeDef",
     "ListBudgetsForResourceOutputTypeDef",
-    "SourceConnectionParametersOutputTypeDef",
     "SourceConnectionParametersTypeDef",
     "CreateConstraintOutputTypeDef",
     "DescribeConstraintOutputTypeDef",
     "ListConstraintsForPortfolioOutputTypeDef",
     "UpdateConstraintOutputTypeDef",
     "CreatePortfolioInputRequestTypeDef",
+    "LaunchPathSummaryTypeDef",
+    "ProvisionedProductAttributeTypeDef",
     "UpdatePortfolioInputRequestTypeDef",
+    "CreatePortfolioOutputTypeDef",
     "ListAcceptedPortfolioSharesOutputTypeDef",
     "ListPortfoliosForProductOutputTypeDef",
     "ListPortfoliosOutputTypeDef",
-    "CreatePortfolioOutputTypeDef",
-    "LaunchPathSummaryTypeDef",
-    "ProvisionedProductAttributeTypeDef",
     "UpdatePortfolioOutputTypeDef",
     "CreatePortfolioShareInputRequestTypeDef",
     "DeletePortfolioShareInputRequestTypeDef",
+    "ListOrganizationPortfolioAccessOutputTypeDef",
     "UpdatePortfolioShareInputRequestTypeDef",
     "CreateProvisioningArtifactInputRequestTypeDef",
     "CreateProvisioningArtifactOutputTypeDef",
     "ListProvisioningArtifactsOutputTypeDef",
     "UpdateProvisioningArtifactOutputTypeDef",
     "CreateProvisionedProductPlanInputRequestTypeDef",
+    "ProvisionedProductPlanDetailsTypeDef",
     "CreateTagOptionOutputTypeDef",
     "DescribePortfolioOutputTypeDef",
     "DescribeTagOptionOutputTypeDef",
     "ListTagOptionsOutputTypeDef",
     "UpdateTagOptionOutputTypeDef",
     "DescribePortfolioSharesOutputTypeDef",
     "DescribeProductOutputTypeDef",
@@ -241,30 +238,28 @@
     "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
     "ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
     "ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
     "ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
     "ListServiceActionsInputListServiceActionsPaginateTypeDef",
     "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
     "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
-    "ListOrganizationPortfolioAccessOutputTypeDef",
     "ListPrincipalsForPortfolioOutputTypeDef",
     "ListProvisionedProductPlansOutputTypeDef",
     "ListRecordHistoryInputListRecordHistoryPaginateTypeDef",
     "ListRecordHistoryInputRequestTypeDef",
     "ListResourcesForTagOptionOutputTypeDef",
     "ListServiceActionsForProvisioningArtifactOutputTypeDef",
     "ListServiceActionsOutputTypeDef",
     "ServiceActionDetailTypeDef",
     "ListStackInstancesForProvisionedProductOutputTypeDef",
     "ListTagOptionsInputListTagOptionsPaginateTypeDef",
     "ListTagOptionsInputRequestTypeDef",
     "ProvisioningArtifactParameterTypeDef",
     "SearchProductsOutputTypeDef",
     "ProvisionProductInputRequestTypeDef",
-    "ProvisionedProductPlanDetailsTypeDef",
     "RecordDetailTypeDef",
     "ResourceChangeDetailTypeDef",
     "ShareDetailsTypeDef",
     "UpdateProvisionedProductInputRequestTypeDef",
     "SourceConnectionDetailTypeDef",
     "SourceConnectionTypeDef",
     "ListLaunchPathsOutputTypeDef",
@@ -452,24 +447,14 @@
     "CloudWatchDashboardTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-CodeStarParametersOutputTypeDef = TypedDict(
-    "CodeStarParametersOutputTypeDef",
-    {
-        "ConnectionArn": str,
-        "Repository": str,
-        "Branch": str,
-        "ArtifactPath": str,
-    },
-)
-
 CodeStarParametersTypeDef = TypedDict(
     "CodeStarParametersTypeDef",
     {
         "ConnectionArn": str,
         "Repository": str,
         "Branch": str,
         "ArtifactPath": str,
@@ -563,22 +548,14 @@
         "Description": str,
         "CreatedTime": datetime,
         "ProviderName": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 OrganizationNodeTypeDef = TypedDict(
     "OrganizationNodeTypeDef",
     {
         "Type": OrganizationNodeTypeType,
         "Value": str,
     },
     total=False,
@@ -1474,23 +1451,14 @@
 
 class ListOrganizationPortfolioAccessInputRequestTypeDef(
     _RequiredListOrganizationPortfolioAccessInputRequestTypeDef,
     _OptionalListOrganizationPortfolioAccessInputRequestTypeDef,
 ):
     pass
 
-OrganizationNodeOutputTypeDef = TypedDict(
-    "OrganizationNodeOutputTypeDef",
-    {
-        "Type": OrganizationNodeTypeType,
-        "Value": str,
-    },
-    total=False,
-)
-
 _RequiredListPortfolioAccessInputRequestTypeDef = TypedDict(
     "_RequiredListPortfolioAccessInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalListPortfolioAccessInputRequestTypeDef = TypedDict(
@@ -1820,24 +1788,14 @@
         "StackSetFailureTolerancePercentage": int,
         "StackSetMaxConcurrencyCount": int,
         "StackSetMaxConcurrencyPercentage": int,
     },
     total=False,
 )
 
-UpdateProvisioningParameterOutputTypeDef = TypedDict(
-    "UpdateProvisioningParameterOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "UsePreviousValue": bool,
-    },
-    total=False,
-)
-
 RecordErrorTypeDef = TypedDict(
     "RecordErrorTypeDef",
     {
         "Code": str,
         "Description": str,
     },
     total=False,
@@ -2250,22 +2208,14 @@
     {
         "Budgets": List[BudgetDetailTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SourceConnectionParametersOutputTypeDef = TypedDict(
-    "SourceConnectionParametersOutputTypeDef",
-    {
-        "CodeStar": CodeStarParametersOutputTypeDef,
-    },
-    total=False,
-)
-
 SourceConnectionParametersTypeDef = TypedDict(
     "SourceConnectionParametersTypeDef",
     {
         "CodeStar": CodeStarParametersTypeDef,
     },
     total=False,
 )
@@ -2328,14 +2278,51 @@
 )
 
 class CreatePortfolioInputRequestTypeDef(
     _RequiredCreatePortfolioInputRequestTypeDef, _OptionalCreatePortfolioInputRequestTypeDef
 ):
     pass
 
+LaunchPathSummaryTypeDef = TypedDict(
+    "LaunchPathSummaryTypeDef",
+    {
+        "Id": str,
+        "ConstraintSummaries": List[ConstraintSummaryTypeDef],
+        "Tags": List[TagTypeDef],
+        "Name": str,
+    },
+    total=False,
+)
+
+ProvisionedProductAttributeTypeDef = TypedDict(
+    "ProvisionedProductAttributeTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "Type": str,
+        "Id": str,
+        "Status": ProvisionedProductStatusType,
+        "StatusMessage": str,
+        "CreatedTime": datetime,
+        "IdempotencyToken": str,
+        "LastRecordId": str,
+        "LastProvisioningRecordId": str,
+        "LastSuccessfulProvisioningRecordId": str,
+        "Tags": List[TagTypeDef],
+        "PhysicalId": str,
+        "ProductId": str,
+        "ProductName": str,
+        "ProvisioningArtifactId": str,
+        "ProvisioningArtifactName": str,
+        "UserArn": str,
+        "UserArnSession": str,
+    },
+    total=False,
+)
+
 _RequiredUpdatePortfolioInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePortfolioInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePortfolioInputRequestTypeDef = TypedDict(
@@ -2352,14 +2339,23 @@
 )
 
 class UpdatePortfolioInputRequestTypeDef(
     _RequiredUpdatePortfolioInputRequestTypeDef, _OptionalUpdatePortfolioInputRequestTypeDef
 ):
     pass
 
+CreatePortfolioOutputTypeDef = TypedDict(
+    "CreatePortfolioOutputTypeDef",
+    {
+        "PortfolioDetail": PortfolioDetailTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAcceptedPortfolioSharesOutputTypeDef = TypedDict(
     "ListAcceptedPortfolioSharesOutputTypeDef",
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2379,65 +2375,19 @@
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreatePortfolioOutputTypeDef = TypedDict(
-    "CreatePortfolioOutputTypeDef",
-    {
-        "PortfolioDetail": PortfolioDetailTypeDef,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LaunchPathSummaryTypeDef = TypedDict(
-    "LaunchPathSummaryTypeDef",
-    {
-        "Id": str,
-        "ConstraintSummaries": List[ConstraintSummaryTypeDef],
-        "Tags": List[TagOutputTypeDef],
-        "Name": str,
-    },
-    total=False,
-)
-
-ProvisionedProductAttributeTypeDef = TypedDict(
-    "ProvisionedProductAttributeTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Type": str,
-        "Id": str,
-        "Status": ProvisionedProductStatusType,
-        "StatusMessage": str,
-        "CreatedTime": datetime,
-        "IdempotencyToken": str,
-        "LastRecordId": str,
-        "LastProvisioningRecordId": str,
-        "LastSuccessfulProvisioningRecordId": str,
-        "Tags": List[TagOutputTypeDef],
-        "PhysicalId": str,
-        "ProductId": str,
-        "ProductName": str,
-        "ProvisioningArtifactId": str,
-        "ProvisioningArtifactName": str,
-        "UserArn": str,
-        "UserArnSession": str,
-    },
-    total=False,
-)
-
 UpdatePortfolioOutputTypeDef = TypedDict(
     "UpdatePortfolioOutputTypeDef",
     {
         "PortfolioDetail": PortfolioDetailTypeDef,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePortfolioShareInputRequestTypeDef = TypedDict(
     "_RequiredCreatePortfolioShareInputRequestTypeDef",
     {
@@ -2480,14 +2430,23 @@
 
 class DeletePortfolioShareInputRequestTypeDef(
     _RequiredDeletePortfolioShareInputRequestTypeDef,
     _OptionalDeletePortfolioShareInputRequestTypeDef,
 ):
     pass
 
+ListOrganizationPortfolioAccessOutputTypeDef = TypedDict(
+    "ListOrganizationPortfolioAccessOutputTypeDef",
+    {
+        "OrganizationNodes": List[OrganizationNodeTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdatePortfolioShareInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePortfolioShareInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalUpdatePortfolioShareInputRequestTypeDef = TypedDict(
@@ -2584,27 +2543,49 @@
 
 class CreateProvisionedProductPlanInputRequestTypeDef(
     _RequiredCreateProvisionedProductPlanInputRequestTypeDef,
     _OptionalCreateProvisionedProductPlanInputRequestTypeDef,
 ):
     pass
 
+ProvisionedProductPlanDetailsTypeDef = TypedDict(
+    "ProvisionedProductPlanDetailsTypeDef",
+    {
+        "CreatedTime": datetime,
+        "PathId": str,
+        "ProductId": str,
+        "PlanName": str,
+        "PlanId": str,
+        "ProvisionProductId": str,
+        "ProvisionProductName": str,
+        "PlanType": Literal["CLOUDFORMATION"],
+        "ProvisioningArtifactId": str,
+        "Status": ProvisionedProductPlanStatusType,
+        "UpdatedTime": datetime,
+        "NotificationArns": List[str],
+        "ProvisioningParameters": List[UpdateProvisioningParameterTypeDef],
+        "Tags": List[TagTypeDef],
+        "StatusMessage": str,
+    },
+    total=False,
+)
+
 CreateTagOptionOutputTypeDef = TypedDict(
     "CreateTagOptionOutputTypeDef",
     {
         "TagOptionDetail": TagOptionDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePortfolioOutputTypeDef = TypedDict(
     "DescribePortfolioOutputTypeDef",
     {
         "PortfolioDetail": PortfolioDetailTypeDef,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "TagOptions": List[TagOptionDetailTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagOptionOutputTypeDef = TypedDict(
@@ -2967,23 +2948,14 @@
         "SortOrder": SortOrderType,
         "ProductSource": Literal["ACCOUNT"],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListOrganizationPortfolioAccessOutputTypeDef = TypedDict(
-    "ListOrganizationPortfolioAccessOutputTypeDef",
-    {
-        "OrganizationNodes": List[OrganizationNodeOutputTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListPrincipalsForPortfolioOutputTypeDef = TypedDict(
     "ListPrincipalsForPortfolioOutputTypeDef",
     {
         "Principals": List[PrincipalTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3134,36 +3106,14 @@
 )
 
 class ProvisionProductInputRequestTypeDef(
     _RequiredProvisionProductInputRequestTypeDef, _OptionalProvisionProductInputRequestTypeDef
 ):
     pass
 
-ProvisionedProductPlanDetailsTypeDef = TypedDict(
-    "ProvisionedProductPlanDetailsTypeDef",
-    {
-        "CreatedTime": datetime,
-        "PathId": str,
-        "ProductId": str,
-        "PlanName": str,
-        "PlanId": str,
-        "ProvisionProductId": str,
-        "ProvisionProductName": str,
-        "PlanType": Literal["CLOUDFORMATION"],
-        "ProvisioningArtifactId": str,
-        "Status": ProvisionedProductPlanStatusType,
-        "UpdatedTime": datetime,
-        "NotificationArns": List[str],
-        "ProvisioningParameters": List[UpdateProvisioningParameterOutputTypeDef],
-        "Tags": List[TagOutputTypeDef],
-        "StatusMessage": str,
-    },
-    total=False,
-)
-
 RecordDetailTypeDef = TypedDict(
     "RecordDetailTypeDef",
     {
         "RecordId": str,
         "ProvisionedProductName": str,
         "Status": RecordStatusType,
         "CreatedTime": datetime,
@@ -3231,15 +3181,15 @@
 ):
     pass
 
 SourceConnectionDetailTypeDef = TypedDict(
     "SourceConnectionDetailTypeDef",
     {
         "Type": Literal["CODESTAR"],
-        "ConnectionParameters": SourceConnectionParametersOutputTypeDef,
+        "ConnectionParameters": SourceConnectionParametersTypeDef,
         "LastSync": LastSyncTypeDef,
     },
     total=False,
 )
 
 _RequiredSourceConnectionTypeDef = TypedDict(
     "_RequiredSourceConnectionTypeDef",
@@ -3535,25 +3485,25 @@
 )
 
 CreateProductOutputTypeDef = TypedDict(
     "CreateProductOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProductAsAdminOutputTypeDef = TypedDict(
     "DescribeProductAsAdminOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
         "ProvisioningArtifactSummaries": List[ProvisioningArtifactSummaryTypeDef],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "TagOptions": List[TagOptionDetailTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchProductsAsAdminOutputTypeDef = TypedDict(
@@ -3565,11 +3515,11 @@
     },
 )
 
 UpdateProductOutputTypeDef = TypedDict(
     "UpdateProductOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/PKG-INFO` & `mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog
-Version: 1.28.12
-Summary: Type annotations for boto3.ServiceCatalog 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ServiceCatalog 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicecatalog)](https://pepy.tech/project/mypy-boto3-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceCatalog 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[boto3.ServiceCatalog 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [mypy-boto3-servicecatalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -442,23 +442,21 @@
     AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     AssociateTagOptionWithResourceInputRequestTypeDef,
     ServiceActionAssociationTypeDef,
     FailedServiceActionAssociationTypeDef,
     ResponseMetadataTypeDef,
     BudgetDetailTypeDef,
     CloudWatchDashboardTypeDef,
-    CodeStarParametersOutputTypeDef,
     CodeStarParametersTypeDef,
     ConstraintDetailTypeDef,
     ConstraintSummaryTypeDef,
     CopyProductInputRequestTypeDef,
     CreateConstraintInputRequestTypeDef,
     TagTypeDef,
     PortfolioDetailTypeDef,
-    TagOutputTypeDef,
     OrganizationNodeTypeDef,
     ProvisioningArtifactPropertiesTypeDef,
     ProvisioningArtifactDetailTypeDef,
     UpdateProvisioningParameterTypeDef,
     CreateServiceActionInputRequestTypeDef,
     CreateTagOptionInputRequestTypeDef,
     TagOptionDetailTypeDef,
@@ -510,15 +508,14 @@
     LastSyncTypeDef,
     PaginatorConfigTypeDef,
     ListAcceptedPortfolioSharesInputRequestTypeDef,
     ListBudgetsForResourceInputRequestTypeDef,
     ListConstraintsForPortfolioInputRequestTypeDef,
     ListLaunchPathsInputRequestTypeDef,
     ListOrganizationPortfolioAccessInputRequestTypeDef,
-    OrganizationNodeOutputTypeDef,
     ListPortfolioAccessInputRequestTypeDef,
     ListPortfoliosForProductInputRequestTypeDef,
     ListPortfoliosInputRequestTypeDef,
     ListPrincipalsForPortfolioInputRequestTypeDef,
     PrincipalTypeDef,
     ProvisionedProductPlanSummaryTypeDef,
     ListProvisioningArtifactsForServiceActionInputRequestTypeDef,
@@ -533,15 +530,14 @@
     StackInstanceTypeDef,
     ListTagOptionsFiltersTypeDef,
     NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     ParameterConstraintsTypeDef,
     ProductViewAggregationValueTypeDef,
     ProvisioningParameterTypeDef,
     ProvisioningPreferencesTypeDef,
-    UpdateProvisioningParameterOutputTypeDef,
     RecordErrorTypeDef,
     RecordTagTypeDef,
     RejectPortfolioShareInputRequestTypeDef,
     ResourceTargetDefinitionTypeDef,
     SearchProductsAsAdminInputRequestTypeDef,
     SearchProductsInputRequestTypeDef,
     ShareErrorTypeDef,
@@ -565,37 +561,38 @@
     DeletePortfolioShareOutputTypeDef,
     DescribeCopyProductStatusOutputTypeDef,
     GetAWSOrganizationsAccessStatusOutputTypeDef,
     ListPortfolioAccessOutputTypeDef,
     UpdatePortfolioShareOutputTypeDef,
     UpdateProvisionedProductPropertiesOutputTypeDef,
     ListBudgetsForResourceOutputTypeDef,
-    SourceConnectionParametersOutputTypeDef,
     SourceConnectionParametersTypeDef,
     CreateConstraintOutputTypeDef,
     DescribeConstraintOutputTypeDef,
     ListConstraintsForPortfolioOutputTypeDef,
     UpdateConstraintOutputTypeDef,
     CreatePortfolioInputRequestTypeDef,
+    LaunchPathSummaryTypeDef,
+    ProvisionedProductAttributeTypeDef,
     UpdatePortfolioInputRequestTypeDef,
+    CreatePortfolioOutputTypeDef,
     ListAcceptedPortfolioSharesOutputTypeDef,
     ListPortfoliosForProductOutputTypeDef,
     ListPortfoliosOutputTypeDef,
-    CreatePortfolioOutputTypeDef,
-    LaunchPathSummaryTypeDef,
-    ProvisionedProductAttributeTypeDef,
     UpdatePortfolioOutputTypeDef,
     CreatePortfolioShareInputRequestTypeDef,
     DeletePortfolioShareInputRequestTypeDef,
+    ListOrganizationPortfolioAccessOutputTypeDef,
     UpdatePortfolioShareInputRequestTypeDef,
     CreateProvisioningArtifactInputRequestTypeDef,
     CreateProvisioningArtifactOutputTypeDef,
     ListProvisioningArtifactsOutputTypeDef,
     UpdateProvisioningArtifactOutputTypeDef,
     CreateProvisionedProductPlanInputRequestTypeDef,
+    ProvisionedProductPlanDetailsTypeDef,
     CreateTagOptionOutputTypeDef,
     DescribePortfolioOutputTypeDef,
     DescribeTagOptionOutputTypeDef,
     ListTagOptionsOutputTypeDef,
     UpdateTagOptionOutputTypeDef,
     DescribePortfolioSharesOutputTypeDef,
     DescribeProductOutputTypeDef,
@@ -617,30 +614,28 @@
     ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef,
     ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
     ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
     ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
     ListServiceActionsInputListServiceActionsPaginateTypeDef,
     ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef,
     SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef,
-    ListOrganizationPortfolioAccessOutputTypeDef,
     ListPrincipalsForPortfolioOutputTypeDef,
     ListProvisionedProductPlansOutputTypeDef,
     ListRecordHistoryInputListRecordHistoryPaginateTypeDef,
     ListRecordHistoryInputRequestTypeDef,
     ListResourcesForTagOptionOutputTypeDef,
     ListServiceActionsForProvisioningArtifactOutputTypeDef,
     ListServiceActionsOutputTypeDef,
     ServiceActionDetailTypeDef,
     ListStackInstancesForProvisionedProductOutputTypeDef,
     ListTagOptionsInputListTagOptionsPaginateTypeDef,
     ListTagOptionsInputRequestTypeDef,
     ProvisioningArtifactParameterTypeDef,
     SearchProductsOutputTypeDef,
     ProvisionProductInputRequestTypeDef,
-    ProvisionedProductPlanDetailsTypeDef,
     RecordDetailTypeDef,
     ResourceChangeDetailTypeDef,
     ShareDetailsTypeDef,
     UpdateProvisionedProductInputRequestTypeDef,
     SourceConnectionDetailTypeDef,
     SourceConnectionTypeDef,
     ListLaunchPathsOutputTypeDef,
```

### Comparing `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/SOURCES.txt` & `mypy-boto3-servicecatalog-1.28.15/mypy_boto3_servicecatalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.12/setup.py` & `mypy-boto3-servicecatalog-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-servicecatalog",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_servicecatalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServiceCatalog 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ServiceCatalog 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

