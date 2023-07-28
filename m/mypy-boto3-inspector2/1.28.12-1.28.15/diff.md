# Comparing `tmp/mypy-boto3-inspector2-1.28.12.tar.gz` & `tmp/mypy-boto3-inspector2-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-inspector2-1.28.12.tar", last modified: Thu Jul 27 05:34:47 2023, max compression
+gzip compressed data, was "mypy-boto3-inspector2-1.28.15.tar", last modified: Fri Jul 28 20:42:56 2023, max compression
```

## Comparing `mypy-boto3-inspector2-1.28.12.tar` & `mypy-boto3-inspector2-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.068491 mypy-boto3-inspector2-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23597 2023-07-27 05:34:47.068491 mypy-boto3-inspector2-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22098 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.068491 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35728 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35666 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17650 2023-07-27 05:23:37.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-07-27 05:23:37.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-07-27 05:23:37.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-07-27 05:23:37.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    79197 2023-07-27 05:23:38.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79108 2023-07-27 05:23:38.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.068491 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23597 2023-07-27 05:34:46.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:46.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:46.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:46.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:47.068491 mypy-boto3-inspector2-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.377214 mypy-boto3-inspector2-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23307 2023-07-28 20:42:56.377214 mypy-boto3-inspector2-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.365214 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35728 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35666 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17650 2023-07-28 20:27:47.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-07-28 20:27:47.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    75649 2023-07-28 20:27:50.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75568 2023-07-28 20:27:48.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.377214 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23307 2023-07-28 20:42:56.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:56.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:56.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:56.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:56.377214 mypy-boto3-inspector2-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/setup.py
```

### Comparing `mypy-boto3-inspector2-1.28.12/LICENSE` & `mypy-boto3-inspector2-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.12/PKG-INFO` & `mypy-boto3-inspector2-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.28.12
-Summary: Type annotations for boto3.Inspector2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Inspector2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector2)](https://pepy.tech/project/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
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
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -426,123 +426,95 @@
     SeverityCountsTypeDef,
     AccountAggregationTypeDef,
     StateTypeDef,
     ResourceStatusTypeDef,
     FindingTypeAggregationTypeDef,
     StringFilterTypeDef,
     AssociateMemberRequestRequestTypeDef,
-    AssociateMemberResponseTypeDef,
+    ResponseMetadataTypeDef,
     AtigDataTypeDef,
-    AutoEnableOutputTypeDef,
     AutoEnableTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     LambdaVpcConfigTypeDef,
     BatchGetAccountStatusRequestRequestTypeDef,
     BatchGetCodeSnippetRequestRequestTypeDef,
     CodeSnippetErrorTypeDef,
     BatchGetFreeTrialInfoRequestRequestTypeDef,
     FreeTrialInfoErrorTypeDef,
     BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     FailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
     CancelFindingsReportRequestRequestTypeDef,
-    CancelFindingsReportResponseTypeDef,
     CancelSbomExportRequestRequestTypeDef,
-    CancelSbomExportResponseTypeDef,
     CisaDataTypeDef,
     CodeFilePathTypeDef,
     CodeLineTypeDef,
     SuggestedFixTypeDef,
     CountsTypeDef,
     CoverageDateFilterTypeDef,
     CoverageMapFilterTypeDef,
     CoverageStringFilterTypeDef,
     ScanStatusTypeDef,
-    CreateFilterResponseTypeDef,
     DestinationTypeDef,
-    CreateFindingsReportResponseTypeDef,
-    CreateSbomExportResponseTypeDef,
     Cvss2TypeDef,
     Cvss3TypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DateFilterOutputTypeDef,
     DateFilterTypeDef,
     DelegatedAdminAccountTypeDef,
     DelegatedAdminTypeDef,
     DeleteFilterRequestRequestTypeDef,
-    DeleteFilterResponseTypeDef,
-    DestinationOutputTypeDef,
     DisableDelegatedAdminAccountRequestRequestTypeDef,
-    DisableDelegatedAdminAccountResponseTypeDef,
     DisableRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
-    DisassociateMemberResponseTypeDef,
     MapFilterTypeDef,
     Ec2MetadataTypeDef,
     EcrRescanDurationStateTypeDef,
     EcrConfigurationTypeDef,
     EcrContainerImageMetadataTypeDef,
     EcrRepositoryMetadataTypeDef,
     EnableDelegatedAdminAccountRequestRequestTypeDef,
-    EnableDelegatedAdminAccountResponseTypeDef,
     EnableRequestRequestTypeDef,
     EpssDetailsTypeDef,
     EpssTypeDef,
     ExploitObservedTypeDef,
     ExploitabilityDetailsTypeDef,
-    MapFilterOutputTypeDef,
-    NumberFilterOutputTypeDef,
-    PortRangeFilterOutputTypeDef,
-    StringFilterOutputTypeDef,
     NumberFilterTypeDef,
     PortRangeFilterTypeDef,
     FreeTrialInfoTypeDef,
-    GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyRequestRequestTypeDef,
-    GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusRequestRequestTypeDef,
     GetMemberRequestRequestTypeDef,
     MemberTypeDef,
     GetSbomExportRequestRequestTypeDef,
     LambdaFunctionMetadataTypeDef,
-    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
-    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
     ListDelegatedAdminAccountsRequestRequestTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
     SortCriteriaTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListUsageTotalsRequestRequestTypeDef,
     StepTypeDef,
     PortRangeTypeDef,
     VulnerablePackageTypeDef,
-    PaginatorConfigTypeDef,
     RecommendationTypeDef,
     ResetEncryptionKeyRequestRequestTypeDef,
-    ResourceMapFilterOutputTypeDef,
-    ResourceStringFilterOutputTypeDef,
     ResourceMapFilterTypeDef,
     ResourceStringFilterTypeDef,
-    ResponseMetadataTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef,
-    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateEncryptionKeyRequestRequestTypeDef,
-    UpdateFilterResponseTypeDef,
     UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef,
     UsageTypeDef,
     AccountAggregationResponseTypeDef,
     AmiAggregationResponseTypeDef,
     AwsEcrContainerAggregationResponseTypeDef,
     Ec2InstanceAggregationResponseTypeDef,
     FindingTypeAggregationResponseTypeDef,
@@ -558,17 +530,32 @@
     AmiAggregationTypeDef,
     AwsEcrContainerAggregationTypeDef,
     ImageLayerAggregationTypeDef,
     LambdaLayerAggregationTypeDef,
     PackageAggregationTypeDef,
     RepositoryAggregationTypeDef,
     TitleAggregationTypeDef,
+    AssociateMemberResponseTypeDef,
+    CancelFindingsReportResponseTypeDef,
+    CancelSbomExportResponseTypeDef,
+    CreateFilterResponseTypeDef,
+    CreateFindingsReportResponseTypeDef,
+    CreateSbomExportResponseTypeDef,
+    DeleteFilterResponseTypeDef,
+    DisableDelegatedAdminAccountResponseTypeDef,
+    DisassociateMemberResponseTypeDef,
+    EnableDelegatedAdminAccountResponseTypeDef,
+    GetEc2DeepInspectionConfigurationResponseTypeDef,
+    GetEncryptionKeyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
+    UpdateFilterResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
-    UpdateOrganizationConfigurationResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
+    UpdateOrganizationConfigurationResponseTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     CodeVulnerabilityDetailsTypeDef,
     CodeSnippetResultTypeDef,
     ListCoverageStatisticsResponseTypeDef,
@@ -577,20 +564,24 @@
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     VulnerabilityTypeDef,
-    PackageFilterOutputTypeDef,
     PackageFilterTypeDef,
     FreeTrialAccountInfoTypeDef,
     GetMemberResponseTypeDef,
     ListMembersResponseTypeDef,
     ResourceScanMetadataTypeDef,
+    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
+    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListAccountPermissionsResponseTypeDef,
     NetworkPathTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     ResourceFilterCriteriaOutputTypeDef,
     ResourceFilterCriteriaTypeDef,
     SearchVulnerabilitiesRequestRequestTypeDef,
```

### Comparing `mypy-boto3-inspector2-1.28.12/README.md` & `mypy-boto3-inspector2-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector2)](https://pepy.tech/project/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
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
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -394,123 +394,95 @@
     SeverityCountsTypeDef,
     AccountAggregationTypeDef,
     StateTypeDef,
     ResourceStatusTypeDef,
     FindingTypeAggregationTypeDef,
     StringFilterTypeDef,
     AssociateMemberRequestRequestTypeDef,
-    AssociateMemberResponseTypeDef,
+    ResponseMetadataTypeDef,
     AtigDataTypeDef,
-    AutoEnableOutputTypeDef,
     AutoEnableTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     LambdaVpcConfigTypeDef,
     BatchGetAccountStatusRequestRequestTypeDef,
     BatchGetCodeSnippetRequestRequestTypeDef,
     CodeSnippetErrorTypeDef,
     BatchGetFreeTrialInfoRequestRequestTypeDef,
     FreeTrialInfoErrorTypeDef,
     BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     FailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
     CancelFindingsReportRequestRequestTypeDef,
-    CancelFindingsReportResponseTypeDef,
     CancelSbomExportRequestRequestTypeDef,
-    CancelSbomExportResponseTypeDef,
     CisaDataTypeDef,
     CodeFilePathTypeDef,
     CodeLineTypeDef,
     SuggestedFixTypeDef,
     CountsTypeDef,
     CoverageDateFilterTypeDef,
     CoverageMapFilterTypeDef,
     CoverageStringFilterTypeDef,
     ScanStatusTypeDef,
-    CreateFilterResponseTypeDef,
     DestinationTypeDef,
-    CreateFindingsReportResponseTypeDef,
-    CreateSbomExportResponseTypeDef,
     Cvss2TypeDef,
     Cvss3TypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DateFilterOutputTypeDef,
     DateFilterTypeDef,
     DelegatedAdminAccountTypeDef,
     DelegatedAdminTypeDef,
     DeleteFilterRequestRequestTypeDef,
-    DeleteFilterResponseTypeDef,
-    DestinationOutputTypeDef,
     DisableDelegatedAdminAccountRequestRequestTypeDef,
-    DisableDelegatedAdminAccountResponseTypeDef,
     DisableRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
-    DisassociateMemberResponseTypeDef,
     MapFilterTypeDef,
     Ec2MetadataTypeDef,
     EcrRescanDurationStateTypeDef,
     EcrConfigurationTypeDef,
     EcrContainerImageMetadataTypeDef,
     EcrRepositoryMetadataTypeDef,
     EnableDelegatedAdminAccountRequestRequestTypeDef,
-    EnableDelegatedAdminAccountResponseTypeDef,
     EnableRequestRequestTypeDef,
     EpssDetailsTypeDef,
     EpssTypeDef,
     ExploitObservedTypeDef,
     ExploitabilityDetailsTypeDef,
-    MapFilterOutputTypeDef,
-    NumberFilterOutputTypeDef,
-    PortRangeFilterOutputTypeDef,
-    StringFilterOutputTypeDef,
     NumberFilterTypeDef,
     PortRangeFilterTypeDef,
     FreeTrialInfoTypeDef,
-    GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyRequestRequestTypeDef,
-    GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusRequestRequestTypeDef,
     GetMemberRequestRequestTypeDef,
     MemberTypeDef,
     GetSbomExportRequestRequestTypeDef,
     LambdaFunctionMetadataTypeDef,
-    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
-    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
     ListDelegatedAdminAccountsRequestRequestTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
     SortCriteriaTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListUsageTotalsRequestRequestTypeDef,
     StepTypeDef,
     PortRangeTypeDef,
     VulnerablePackageTypeDef,
-    PaginatorConfigTypeDef,
     RecommendationTypeDef,
     ResetEncryptionKeyRequestRequestTypeDef,
-    ResourceMapFilterOutputTypeDef,
-    ResourceStringFilterOutputTypeDef,
     ResourceMapFilterTypeDef,
     ResourceStringFilterTypeDef,
-    ResponseMetadataTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef,
-    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateEncryptionKeyRequestRequestTypeDef,
-    UpdateFilterResponseTypeDef,
     UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef,
     UsageTypeDef,
     AccountAggregationResponseTypeDef,
     AmiAggregationResponseTypeDef,
     AwsEcrContainerAggregationResponseTypeDef,
     Ec2InstanceAggregationResponseTypeDef,
     FindingTypeAggregationResponseTypeDef,
@@ -526,17 +498,32 @@
     AmiAggregationTypeDef,
     AwsEcrContainerAggregationTypeDef,
     ImageLayerAggregationTypeDef,
     LambdaLayerAggregationTypeDef,
     PackageAggregationTypeDef,
     RepositoryAggregationTypeDef,
     TitleAggregationTypeDef,
+    AssociateMemberResponseTypeDef,
+    CancelFindingsReportResponseTypeDef,
+    CancelSbomExportResponseTypeDef,
+    CreateFilterResponseTypeDef,
+    CreateFindingsReportResponseTypeDef,
+    CreateSbomExportResponseTypeDef,
+    DeleteFilterResponseTypeDef,
+    DisableDelegatedAdminAccountResponseTypeDef,
+    DisassociateMemberResponseTypeDef,
+    EnableDelegatedAdminAccountResponseTypeDef,
+    GetEc2DeepInspectionConfigurationResponseTypeDef,
+    GetEncryptionKeyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
+    UpdateFilterResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
-    UpdateOrganizationConfigurationResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
+    UpdateOrganizationConfigurationResponseTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     CodeVulnerabilityDetailsTypeDef,
     CodeSnippetResultTypeDef,
     ListCoverageStatisticsResponseTypeDef,
@@ -545,20 +532,24 @@
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     VulnerabilityTypeDef,
-    PackageFilterOutputTypeDef,
     PackageFilterTypeDef,
     FreeTrialAccountInfoTypeDef,
     GetMemberResponseTypeDef,
     ListMembersResponseTypeDef,
     ResourceScanMetadataTypeDef,
+    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
+    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListAccountPermissionsResponseTypeDef,
     NetworkPathTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     ResourceFilterCriteriaOutputTypeDef,
     ResourceFilterCriteriaTypeDef,
     SearchVulnerabilitiesRequestRequestTypeDef,
```

### Comparing `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/__init__.py` & `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/__init__.pyi` & `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/__main__.py` & `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Inspector2 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Inspector2 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2\nOther"
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

### Comparing `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/client.py` & `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/client.pyi` & `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/literals.py` & `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/literals.pyi` & `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/paginator.py` & `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 class ListAccountPermissionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListAccountPermissions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listaccountpermissionspaginator)
     """
 
     def paginate(
-        self, *, service: ServiceType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, service: ServiceType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListAccountPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listaccountpermissionspaginator)
         """
 
 
@@ -107,15 +107,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listcoveragepaginator)
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCoverageResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverage.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listcoveragepaginator)
         """
 
 
@@ -126,30 +126,30 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         groupBy: GroupKeyType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCoverageStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverageStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listcoveragestatisticspaginator)
         """
 
 
 class ListDelegatedAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListDelegatedAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listdelegatedadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDelegatedAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListDelegatedAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listdelegatedadminaccountspaginator)
         """
 
 
@@ -160,15 +160,15 @@
     """
 
     def paginate(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfilterspaginator)
         """
 
 
@@ -180,15 +180,15 @@
 
     def paginate(
         self,
         *,
         aggregationType: AggregationTypeType,
         accountIds: Sequence[StringFilterTypeDef] = ...,
         aggregationRequest: AggregationRequestTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingAggregationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindingAggregations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingaggregationspaginator)
         """
 
 
@@ -199,45 +199,45 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: FilterCriteriaTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
         """
 
 
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, onlyAssociated: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, onlyAssociated: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listmemberspaginator)
         """
 
 
 class ListUsageTotalsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListUsageTotals)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listusagetotalspaginator)
     """
 
     def paginate(
-        self, *, accountIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accountIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsageTotalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListUsageTotals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listusagetotalspaginator)
         """
 
 
@@ -247,13 +247,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#searchvulnerabilitiespaginator)
     """
 
     def paginate(
         self,
         *,
         filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchVulnerabilitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.SearchVulnerabilities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#searchvulnerabilitiespaginator)
         """
```

### Comparing `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/paginator.pyi` & `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 class ListAccountPermissionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListAccountPermissions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listaccountpermissionspaginator)
     """
 
     def paginate(
-        self, *, service: ServiceType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, service: ServiceType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListAccountPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listaccountpermissionspaginator)
         """
 
 class ListCoveragePaginator(Paginator):
@@ -103,15 +103,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listcoveragepaginator)
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCoverageResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverage.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listcoveragepaginator)
         """
 
 class ListCoverageStatisticsPaginator(Paginator):
@@ -121,29 +121,29 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         groupBy: GroupKeyType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCoverageStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverageStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listcoveragestatisticspaginator)
         """
 
 class ListDelegatedAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListDelegatedAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listdelegatedadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDelegatedAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListDelegatedAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listdelegatedadminaccountspaginator)
         """
 
 class ListFiltersPaginator(Paginator):
@@ -153,15 +153,15 @@
     """
 
     def paginate(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfilterspaginator)
         """
 
 class ListFindingAggregationsPaginator(Paginator):
@@ -172,15 +172,15 @@
 
     def paginate(
         self,
         *,
         aggregationType: AggregationTypeType,
         accountIds: Sequence[StringFilterTypeDef] = ...,
         aggregationRequest: AggregationRequestTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingAggregationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindingAggregations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingaggregationspaginator)
         """
 
 class ListFindingsPaginator(Paginator):
@@ -190,43 +190,43 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: FilterCriteriaTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
         """
 
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, onlyAssociated: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, onlyAssociated: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listmemberspaginator)
         """
 
 class ListUsageTotalsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListUsageTotals)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listusagetotalspaginator)
     """
 
     def paginate(
-        self, *, accountIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accountIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsageTotalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListUsageTotals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listusagetotalspaginator)
         """
 
 class SearchVulnerabilitiesPaginator(Paginator):
@@ -235,13 +235,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#searchvulnerabilitiespaginator)
     """
 
     def paginate(
         self,
         *,
         filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchVulnerabilitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.SearchVulnerabilities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#searchvulnerabilitiespaginator)
         """
```

### Comparing `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/type_defs.py` & `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,123 +89,95 @@
     "SeverityCountsTypeDef",
     "AccountAggregationTypeDef",
     "StateTypeDef",
     "ResourceStatusTypeDef",
     "FindingTypeAggregationTypeDef",
     "StringFilterTypeDef",
     "AssociateMemberRequestRequestTypeDef",
-    "AssociateMemberResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AtigDataTypeDef",
-    "AutoEnableOutputTypeDef",
     "AutoEnableTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "LambdaVpcConfigTypeDef",
     "BatchGetAccountStatusRequestRequestTypeDef",
     "BatchGetCodeSnippetRequestRequestTypeDef",
     "CodeSnippetErrorTypeDef",
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     "FreeTrialInfoErrorTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "FailedMemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusTypeDef",
     "CancelFindingsReportRequestRequestTypeDef",
-    "CancelFindingsReportResponseTypeDef",
     "CancelSbomExportRequestRequestTypeDef",
-    "CancelSbomExportResponseTypeDef",
     "CisaDataTypeDef",
     "CodeFilePathTypeDef",
     "CodeLineTypeDef",
     "SuggestedFixTypeDef",
     "CountsTypeDef",
     "CoverageDateFilterTypeDef",
     "CoverageMapFilterTypeDef",
     "CoverageStringFilterTypeDef",
     "ScanStatusTypeDef",
-    "CreateFilterResponseTypeDef",
     "DestinationTypeDef",
-    "CreateFindingsReportResponseTypeDef",
-    "CreateSbomExportResponseTypeDef",
     "Cvss2TypeDef",
     "Cvss3TypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DateFilterOutputTypeDef",
     "DateFilterTypeDef",
     "DelegatedAdminAccountTypeDef",
     "DelegatedAdminTypeDef",
     "DeleteFilterRequestRequestTypeDef",
-    "DeleteFilterResponseTypeDef",
-    "DestinationOutputTypeDef",
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
-    "DisableDelegatedAdminAccountResponseTypeDef",
     "DisableRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
-    "DisassociateMemberResponseTypeDef",
     "MapFilterTypeDef",
     "Ec2MetadataTypeDef",
     "EcrRescanDurationStateTypeDef",
     "EcrConfigurationTypeDef",
     "EcrContainerImageMetadataTypeDef",
     "EcrRepositoryMetadataTypeDef",
     "EnableDelegatedAdminAccountRequestRequestTypeDef",
-    "EnableDelegatedAdminAccountResponseTypeDef",
     "EnableRequestRequestTypeDef",
     "EpssDetailsTypeDef",
     "EpssTypeDef",
     "ExploitObservedTypeDef",
     "ExploitabilityDetailsTypeDef",
-    "MapFilterOutputTypeDef",
-    "NumberFilterOutputTypeDef",
-    "PortRangeFilterOutputTypeDef",
-    "StringFilterOutputTypeDef",
     "NumberFilterTypeDef",
     "PortRangeFilterTypeDef",
     "FreeTrialInfoTypeDef",
-    "GetEc2DeepInspectionConfigurationResponseTypeDef",
     "GetEncryptionKeyRequestRequestTypeDef",
-    "GetEncryptionKeyResponseTypeDef",
     "GetFindingsReportStatusRequestRequestTypeDef",
     "GetMemberRequestRequestTypeDef",
     "MemberTypeDef",
     "GetSbomExportRequestRequestTypeDef",
     "LambdaFunctionMetadataTypeDef",
-    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
-    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
     "ListDelegatedAdminAccountsRequestRequestTypeDef",
-    "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
     "SortCriteriaTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
     "ListUsageTotalsRequestRequestTypeDef",
     "StepTypeDef",
     "PortRangeTypeDef",
     "VulnerablePackageTypeDef",
-    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
     "ResetEncryptionKeyRequestRequestTypeDef",
-    "ResourceMapFilterOutputTypeDef",
-    "ResourceStringFilterOutputTypeDef",
     "ResourceMapFilterTypeDef",
     "ResourceStringFilterTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchVulnerabilitiesFilterCriteriaTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef",
-    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
     "UpdateEncryptionKeyRequestRequestTypeDef",
-    "UpdateFilterResponseTypeDef",
     "UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef",
     "UsageTypeDef",
     "AccountAggregationResponseTypeDef",
     "AmiAggregationResponseTypeDef",
     "AwsEcrContainerAggregationResponseTypeDef",
     "Ec2InstanceAggregationResponseTypeDef",
     "FindingTypeAggregationResponseTypeDef",
@@ -221,17 +193,32 @@
     "AmiAggregationTypeDef",
     "AwsEcrContainerAggregationTypeDef",
     "ImageLayerAggregationTypeDef",
     "LambdaLayerAggregationTypeDef",
     "PackageAggregationTypeDef",
     "RepositoryAggregationTypeDef",
     "TitleAggregationTypeDef",
+    "AssociateMemberResponseTypeDef",
+    "CancelFindingsReportResponseTypeDef",
+    "CancelSbomExportResponseTypeDef",
+    "CreateFilterResponseTypeDef",
+    "CreateFindingsReportResponseTypeDef",
+    "CreateSbomExportResponseTypeDef",
+    "DeleteFilterResponseTypeDef",
+    "DisableDelegatedAdminAccountResponseTypeDef",
+    "DisassociateMemberResponseTypeDef",
+    "EnableDelegatedAdminAccountResponseTypeDef",
+    "GetEc2DeepInspectionConfigurationResponseTypeDef",
+    "GetEncryptionKeyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
+    "UpdateFilterResponseTypeDef",
     "DescribeOrganizationConfigurationResponseTypeDef",
-    "UpdateOrganizationConfigurationResponseTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
+    "UpdateOrganizationConfigurationResponseTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "CodeVulnerabilityDetailsTypeDef",
     "CodeSnippetResultTypeDef",
     "ListCoverageStatisticsResponseTypeDef",
@@ -240,20 +227,24 @@
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "VulnerabilityTypeDef",
-    "PackageFilterOutputTypeDef",
     "PackageFilterTypeDef",
     "FreeTrialAccountInfoTypeDef",
     "GetMemberResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ResourceScanMetadataTypeDef",
+    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
+    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
     "ListAccountPermissionsResponseTypeDef",
     "NetworkPathTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
     "ResourceFilterCriteriaOutputTypeDef",
     "ResourceFilterCriteriaTypeDef",
     "SearchVulnerabilitiesRequestRequestTypeDef",
@@ -373,54 +364,36 @@
 AssociateMemberRequestRequestTypeDef = TypedDict(
     "AssociateMemberRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
-AssociateMemberResponseTypeDef = TypedDict(
-    "AssociateMemberResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "accountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AtigDataTypeDef = TypedDict(
     "AtigDataTypeDef",
     {
         "firstSeen": datetime,
         "lastSeen": datetime,
         "targets": List[str],
         "ttps": List[str],
     },
     total=False,
 )
 
-_RequiredAutoEnableOutputTypeDef = TypedDict(
-    "_RequiredAutoEnableOutputTypeDef",
-    {
-        "ec2": bool,
-        "ecr": bool,
-    },
-)
-_OptionalAutoEnableOutputTypeDef = TypedDict(
-    "_OptionalAutoEnableOutputTypeDef",
-    {
-        "lambda": bool,
-        "lambdaCode": bool,
-    },
-    total=False,
-)
-
-
-class AutoEnableOutputTypeDef(_RequiredAutoEnableOutputTypeDef, _OptionalAutoEnableOutputTypeDef):
-    pass
-
-
 _RequiredAutoEnableTypeDef = TypedDict(
     "_RequiredAutoEnableTypeDef",
     {
         "ec2": bool,
         "ecr": bool,
     },
 )
@@ -597,37 +570,21 @@
 CancelFindingsReportRequestRequestTypeDef = TypedDict(
     "CancelFindingsReportRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
-CancelFindingsReportResponseTypeDef = TypedDict(
-    "CancelFindingsReportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CancelSbomExportRequestRequestTypeDef = TypedDict(
     "CancelSbomExportRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
-CancelSbomExportResponseTypeDef = TypedDict(
-    "CancelSbomExportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CisaDataTypeDef = TypedDict(
     "CisaDataTypeDef",
     {
         "action": str,
         "dateAdded": datetime,
         "dateDue": datetime,
     },
@@ -713,22 +670,14 @@
     "ScanStatusTypeDef",
     {
         "reason": ScanStatusReasonType,
         "statusCode": ScanStatusCodeType,
     },
 )
 
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "bucketName": str,
         "kmsKeyArn": str,
     },
 )
@@ -741,30 +690,14 @@
 )
 
 
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
 
-CreateFindingsReportResponseTypeDef = TypedDict(
-    "CreateFindingsReportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSbomExportResponseTypeDef = TypedDict(
-    "CreateSbomExportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 Cvss2TypeDef = TypedDict(
     "Cvss2TypeDef",
     {
         "baseScore": float,
         "scoringVector": str,
     },
     total=False,
@@ -836,59 +769,21 @@
 DeleteFilterRequestRequestTypeDef = TypedDict(
     "DeleteFilterRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-DeleteFilterResponseTypeDef = TypedDict(
-    "DeleteFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDestinationOutputTypeDef = TypedDict(
-    "_RequiredDestinationOutputTypeDef",
-    {
-        "bucketName": str,
-        "kmsKeyArn": str,
-    },
-)
-_OptionalDestinationOutputTypeDef = TypedDict(
-    "_OptionalDestinationOutputTypeDef",
-    {
-        "keyPrefix": str,
-    },
-    total=False,
-)
-
-
-class DestinationOutputTypeDef(
-    _RequiredDestinationOutputTypeDef, _OptionalDestinationOutputTypeDef
-):
-    pass
-
-
 DisableDelegatedAdminAccountRequestRequestTypeDef = TypedDict(
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     {
         "delegatedAdminAccountId": str,
     },
 )
 
-DisableDelegatedAdminAccountResponseTypeDef = TypedDict(
-    "DisableDelegatedAdminAccountResponseTypeDef",
-    {
-        "delegatedAdminAccountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisableRequestRequestTypeDef = TypedDict(
     "DisableRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "resourceTypes": Sequence[ResourceScanTypeType],
     },
     total=False,
@@ -897,22 +792,14 @@
 DisassociateMemberRequestRequestTypeDef = TypedDict(
     "DisassociateMemberRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
-DisassociateMemberResponseTypeDef = TypedDict(
-    "DisassociateMemberResponseTypeDef",
-    {
-        "accountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMapFilterTypeDef = TypedDict(
     "_RequiredMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -991,22 +878,14 @@
 class EnableDelegatedAdminAccountRequestRequestTypeDef(
     _RequiredEnableDelegatedAdminAccountRequestRequestTypeDef,
     _OptionalEnableDelegatedAdminAccountRequestRequestTypeDef,
 ):
     pass
 
 
-EnableDelegatedAdminAccountResponseTypeDef = TypedDict(
-    "EnableDelegatedAdminAccountResponseTypeDef",
-    {
-        "delegatedAdminAccountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEnableRequestRequestTypeDef = TypedDict(
     "_RequiredEnableRequestRequestTypeDef",
     {
         "resourceTypes": Sequence[ResourceScanTypeType],
     },
 )
 _OptionalEnableRequestRequestTypeDef = TypedDict(
@@ -1054,60 +933,14 @@
     "ExploitabilityDetailsTypeDef",
     {
         "lastKnownExploitAt": datetime,
     },
     total=False,
 )
 
-_RequiredMapFilterOutputTypeDef = TypedDict(
-    "_RequiredMapFilterOutputTypeDef",
-    {
-        "comparison": Literal["EQUALS"],
-        "key": str,
-    },
-)
-_OptionalMapFilterOutputTypeDef = TypedDict(
-    "_OptionalMapFilterOutputTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-
-class MapFilterOutputTypeDef(_RequiredMapFilterOutputTypeDef, _OptionalMapFilterOutputTypeDef):
-    pass
-
-
-NumberFilterOutputTypeDef = TypedDict(
-    "NumberFilterOutputTypeDef",
-    {
-        "lowerInclusive": float,
-        "upperInclusive": float,
-    },
-    total=False,
-)
-
-PortRangeFilterOutputTypeDef = TypedDict(
-    "PortRangeFilterOutputTypeDef",
-    {
-        "beginInclusive": int,
-        "endInclusive": int,
-    },
-    total=False,
-)
-
-StringFilterOutputTypeDef = TypedDict(
-    "StringFilterOutputTypeDef",
-    {
-        "comparison": StringComparisonType,
-        "value": str,
-    },
-)
-
 NumberFilterTypeDef = TypedDict(
     "NumberFilterTypeDef",
     {
         "lowerInclusive": float,
         "upperInclusive": float,
     },
     total=False,
@@ -1128,41 +961,22 @@
         "end": datetime,
         "start": datetime,
         "status": FreeTrialStatusType,
         "type": FreeTrialTypeType,
     },
 )
 
-GetEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
-    "GetEc2DeepInspectionConfigurationResponseTypeDef",
-    {
-        "errorMessage": str,
-        "orgPackagePaths": List[str],
-        "packagePaths": List[str],
-        "status": Ec2DeepInspectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEncryptionKeyRequestRequestTypeDef = TypedDict(
     "GetEncryptionKeyRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "scanType": ScanTypeType,
     },
 )
 
-GetEncryptionKeyResponseTypeDef = TypedDict(
-    "GetEncryptionKeyResponseTypeDef",
-    {
-        "kmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFindingsReportStatusRequestRequestTypeDef = TypedDict(
     "GetFindingsReportStatusRequestRequestTypeDef",
     {
         "reportId": str,
     },
     total=False,
 )
@@ -1199,19 +1013,20 @@
         "functionTags": Dict[str, str],
         "layers": List[str],
         "runtime": RuntimeType,
     },
     total=False,
 )
 
-ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef = TypedDict(
-    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "service": ServiceType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAccountPermissionsRequestRequestTypeDef = TypedDict(
     "ListAccountPermissionsRequestRequestTypeDef",
     {
@@ -1226,41 +1041,23 @@
     "PermissionTypeDef",
     {
         "operation": OperationType,
         "service": ServiceType,
     },
 )
 
-ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef = TypedDict(
-    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDelegatedAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListDelegatedAdminAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "ListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "action": FilterActionType,
-        "arns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFiltersRequestRequestTypeDef = TypedDict(
     "ListFiltersRequestRequestTypeDef",
     {
         "action": FilterActionType,
         "arns": Sequence[str],
         "maxResults": int,
         "nextToken": str,
@@ -1272,23 +1069,14 @@
     "SortCriteriaTypeDef",
     {
         "field": SortFieldType,
         "sortOrder": SortOrderType,
     },
 )
 
-ListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "ListMembersRequestListMembersPaginateTypeDef",
-    {
-        "onlyAssociated": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMembersRequestRequestTypeDef = TypedDict(
     "ListMembersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "onlyAssociated": bool,
     },
@@ -1298,31 +1086,14 @@
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
-ListUsageTotalsRequestListUsageTotalsPaginateTypeDef = TypedDict(
-    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
-    {
-        "accountIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListUsageTotalsRequestRequestTypeDef = TypedDict(
     "ListUsageTotalsRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -1371,24 +1142,14 @@
 
 class VulnerablePackageTypeDef(
     _RequiredVulnerablePackageTypeDef, _OptionalVulnerablePackageTypeDef
 ):
     pass
 
 
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
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Url": str,
         "text": str,
     },
     total=False,
@@ -1398,44 +1159,14 @@
     "ResetEncryptionKeyRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "scanType": ScanTypeType,
     },
 )
 
-_RequiredResourceMapFilterOutputTypeDef = TypedDict(
-    "_RequiredResourceMapFilterOutputTypeDef",
-    {
-        "comparison": Literal["EQUALS"],
-        "key": str,
-    },
-)
-_OptionalResourceMapFilterOutputTypeDef = TypedDict(
-    "_OptionalResourceMapFilterOutputTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-
-class ResourceMapFilterOutputTypeDef(
-    _RequiredResourceMapFilterOutputTypeDef, _OptionalResourceMapFilterOutputTypeDef
-):
-    pass
-
-
-ResourceStringFilterOutputTypeDef = TypedDict(
-    "ResourceStringFilterOutputTypeDef",
-    {
-        "comparison": ResourceStringComparisonType,
-        "value": str,
-    },
-)
-
 _RequiredResourceMapFilterTypeDef = TypedDict(
     "_RequiredResourceMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -1458,25 +1189,14 @@
     "ResourceStringFilterTypeDef",
     {
         "comparison": ResourceStringComparisonType,
         "value": str,
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
 SearchVulnerabilitiesFilterCriteriaTypeDef = TypedDict(
     "SearchVulnerabilitiesFilterCriteriaTypeDef",
     {
         "vulnerabilityIds": Sequence[str],
     },
 )
 
@@ -1501,42 +1221,23 @@
     {
         "activateDeepInspection": bool,
         "packagePaths": Sequence[str],
     },
     total=False,
 )
 
-UpdateEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
-    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
-    {
-        "errorMessage": str,
-        "orgPackagePaths": List[str],
-        "packagePaths": List[str],
-        "status": Ec2DeepInspectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateEncryptionKeyRequestRequestTypeDef = TypedDict(
     "UpdateEncryptionKeyRequestRequestTypeDef",
     {
         "kmsKeyId": str,
         "resourceType": ResourceTypeType,
         "scanType": ScanTypeType,
     },
 )
 
-UpdateFilterResponseTypeDef = TypedDict(
-    "UpdateFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef",
     {
         "orgPackagePaths": Sequence[str],
     },
 )
 
@@ -1917,35 +1618,161 @@
         "sortOrder": SortOrderType,
         "titles": Sequence[StringFilterTypeDef],
         "vulnerabilityIds": Sequence[StringFilterTypeDef],
     },
     total=False,
 )
 
+AssociateMemberResponseTypeDef = TypedDict(
+    "AssociateMemberResponseTypeDef",
+    {
+        "accountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelFindingsReportResponseTypeDef = TypedDict(
+    "CancelFindingsReportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelSbomExportResponseTypeDef = TypedDict(
+    "CancelSbomExportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFindingsReportResponseTypeDef = TypedDict(
+    "CreateFindingsReportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSbomExportResponseTypeDef = TypedDict(
+    "CreateSbomExportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFilterResponseTypeDef = TypedDict(
+    "DeleteFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableDelegatedAdminAccountResponseTypeDef = TypedDict(
+    "DisableDelegatedAdminAccountResponseTypeDef",
+    {
+        "delegatedAdminAccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateMemberResponseTypeDef = TypedDict(
+    "DisassociateMemberResponseTypeDef",
+    {
+        "accountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnableDelegatedAdminAccountResponseTypeDef = TypedDict(
+    "EnableDelegatedAdminAccountResponseTypeDef",
+    {
+        "delegatedAdminAccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
+    "GetEc2DeepInspectionConfigurationResponseTypeDef",
+    {
+        "errorMessage": str,
+        "orgPackagePaths": List[str],
+        "packagePaths": List[str],
+        "status": Ec2DeepInspectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEncryptionKeyResponseTypeDef = TypedDict(
+    "GetEncryptionKeyResponseTypeDef",
+    {
+        "kmsKeyId": str,
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
+UpdateEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
+    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
+    {
+        "errorMessage": str,
+        "orgPackagePaths": List[str],
+        "packagePaths": List[str],
+        "status": Ec2DeepInspectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFilterResponseTypeDef = TypedDict(
+    "UpdateFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
-        "autoEnable": AutoEnableOutputTypeDef,
+        "autoEnable": AutoEnableTypeDef,
         "maxAccountLimitReached": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateOrganizationConfigurationResponseTypeDef = TypedDict(
-    "UpdateOrganizationConfigurationResponseTypeDef",
+UpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateOrganizationConfigurationRequestRequestTypeDef",
     {
-        "autoEnable": AutoEnableOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "autoEnable": AutoEnableTypeDef,
     },
 )
 
-UpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateOrganizationConfigurationRequestRequestTypeDef",
+UpdateOrganizationConfigurationResponseTypeDef = TypedDict(
+    "UpdateOrganizationConfigurationResponseTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAwsLambdaFunctionDetailsTypeDef = TypedDict(
     "_RequiredAwsLambdaFunctionDetailsTypeDef",
     {
         "codeSha256": str,
@@ -1975,24 +1802,24 @@
 
 
 BatchGetMemberEc2DeepInspectionStatusResponseTypeDef = TypedDict(
     "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
     {
         "accountIds": List[MemberAccountEc2DeepInspectionStatusStateTypeDef],
         "failedAccountIds": List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef = TypedDict(
     "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
     {
         "accountIds": List[MemberAccountEc2DeepInspectionStatusStateTypeDef],
         "failedAccountIds": List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef = TypedDict(
     "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     {
         "accountIds": Sequence[MemberAccountEc2DeepInspectionStatusTypeDef],
@@ -2040,15 +1867,15 @@
 
 ListCoverageStatisticsResponseTypeDef = TypedDict(
     "ListCoverageStatisticsResponseTypeDef",
     {
         "countsByGroup": List[CountsTypeDef],
         "nextToken": str,
         "totalCounts": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CoverageFilterCriteriaTypeDef = TypedDict(
     "CoverageFilterCriteriaTypeDef",
     {
         "accountId": Sequence[CoverageStringFilterTypeDef],
@@ -2092,23 +1919,23 @@
 
 
 ListDelegatedAdminAccountsResponseTypeDef = TypedDict(
     "ListDelegatedAdminAccountsResponseTypeDef",
     {
         "delegatedAdminAccounts": List[DelegatedAdminAccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDelegatedAdminAccountResponseTypeDef = TypedDict(
     "GetDelegatedAdminAccountResponseTypeDef",
     {
         "delegatedAdmin": DelegatedAdminTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 Ec2InstanceAggregationTypeDef = TypedDict(
     "Ec2InstanceAggregationTypeDef",
     {
         "amis": Sequence[StringFilterTypeDef],
@@ -2179,28 +2006,14 @@
 )
 
 
 class VulnerabilityTypeDef(_RequiredVulnerabilityTypeDef, _OptionalVulnerabilityTypeDef):
     pass
 
 
-PackageFilterOutputTypeDef = TypedDict(
-    "PackageFilterOutputTypeDef",
-    {
-        "architecture": StringFilterOutputTypeDef,
-        "epoch": NumberFilterOutputTypeDef,
-        "name": StringFilterOutputTypeDef,
-        "release": StringFilterOutputTypeDef,
-        "sourceLambdaLayerArn": StringFilterOutputTypeDef,
-        "sourceLayerHash": StringFilterOutputTypeDef,
-        "version": StringFilterOutputTypeDef,
-    },
-    total=False,
-)
-
 PackageFilterTypeDef = TypedDict(
     "PackageFilterTypeDef",
     {
         "architecture": StringFilterTypeDef,
         "epoch": NumberFilterTypeDef,
         "name": StringFilterTypeDef,
         "release": StringFilterTypeDef,
@@ -2219,44 +2032,89 @@
     },
 )
 
 GetMemberResponseTypeDef = TypedDict(
     "GetMemberResponseTypeDef",
     {
         "member": MemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "members": List[MemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceScanMetadataTypeDef = TypedDict(
     "ResourceScanMetadataTypeDef",
     {
         "ec2": Ec2MetadataTypeDef,
         "ecrImage": EcrContainerImageMetadataTypeDef,
         "ecrRepository": EcrRepositoryMetadataTypeDef,
         "lambdaFunction": LambdaFunctionMetadataTypeDef,
     },
     total=False,
 )
 
+ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef = TypedDict(
+    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+    {
+        "service": ServiceType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef = TypedDict(
+    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "action": FilterActionType,
+        "arns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "ListMembersRequestListMembersPaginateTypeDef",
+    {
+        "onlyAssociated": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListUsageTotalsRequestListUsageTotalsPaginateTypeDef = TypedDict(
+    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
+    {
+        "accountIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListAccountPermissionsResponseTypeDef = TypedDict(
     "ListAccountPermissionsResponseTypeDef",
     {
         "nextToken": str,
         "permissions": List[PermissionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkPathTypeDef = TypedDict(
     "NetworkPathTypeDef",
     {
         "steps": List[StepTypeDef],
@@ -2300,22 +2158,22 @@
     },
     total=False,
 )
 
 ResourceFilterCriteriaOutputTypeDef = TypedDict(
     "ResourceFilterCriteriaOutputTypeDef",
     {
-        "accountId": List[ResourceStringFilterOutputTypeDef],
-        "ec2InstanceTags": List[ResourceMapFilterOutputTypeDef],
-        "ecrImageTags": List[ResourceStringFilterOutputTypeDef],
-        "ecrRepositoryName": List[ResourceStringFilterOutputTypeDef],
-        "lambdaFunctionName": List[ResourceStringFilterOutputTypeDef],
-        "lambdaFunctionTags": List[ResourceMapFilterOutputTypeDef],
-        "resourceId": List[ResourceStringFilterOutputTypeDef],
-        "resourceType": List[ResourceStringFilterOutputTypeDef],
+        "accountId": List[ResourceStringFilterTypeDef],
+        "ec2InstanceTags": List[ResourceMapFilterTypeDef],
+        "ecrImageTags": List[ResourceStringFilterTypeDef],
+        "ecrRepositoryName": List[ResourceStringFilterTypeDef],
+        "lambdaFunctionName": List[ResourceStringFilterTypeDef],
+        "lambdaFunctionTags": List[ResourceMapFilterTypeDef],
+        "resourceId": List[ResourceStringFilterTypeDef],
+        "resourceType": List[ResourceStringFilterTypeDef],
     },
     total=False,
 )
 
 ResourceFilterCriteriaTypeDef = TypedDict(
     "ResourceFilterCriteriaTypeDef",
     {
@@ -2358,15 +2216,15 @@
     {
         "filterCriteria": SearchVulnerabilitiesFilterCriteriaTypeDef,
     },
 )
 _OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef = TypedDict(
     "_OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef(
     _RequiredSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
@@ -2412,24 +2270,24 @@
 )
 
 DisableResponseTypeDef = TypedDict(
     "DisableResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnableResponseTypeDef = TypedDict(
     "EnableResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "awsEc2Instance": AwsEc2InstanceDetailsTypeDef,
@@ -2440,23 +2298,23 @@
 )
 
 BatchGetCodeSnippetResponseTypeDef = TypedDict(
     "BatchGetCodeSnippetResponseTypeDef",
     {
         "codeSnippetResults": List[CodeSnippetResultTypeDef],
         "errors": List[CodeSnippetErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
     "ListCoverageRequestListCoveragePaginateTypeDef",
     {
         "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListCoverageRequestRequestTypeDef = TypedDict(
     "ListCoverageRequestRequestTypeDef",
     {
@@ -2468,15 +2326,15 @@
 )
 
 ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef = TypedDict(
     "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
     {
         "filterCriteria": CoverageFilterCriteriaTypeDef,
         "groupBy": GroupKeyType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListCoverageStatisticsRequestRequestTypeDef = TypedDict(
     "ListCoverageStatisticsRequestRequestTypeDef",
     {
@@ -2513,72 +2371,72 @@
     total=False,
 )
 
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
         "ecrConfiguration": EcrConfigurationStateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchVulnerabilitiesResponseTypeDef = TypedDict(
     "SearchVulnerabilitiesResponseTypeDef",
     {
         "nextToken": str,
         "vulnerabilities": List[VulnerabilityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FilterCriteriaOutputTypeDef = TypedDict(
     "FilterCriteriaOutputTypeDef",
     {
-        "awsAccountId": List[StringFilterOutputTypeDef],
-        "codeVulnerabilityDetectorName": List[StringFilterOutputTypeDef],
-        "codeVulnerabilityDetectorTags": List[StringFilterOutputTypeDef],
-        "codeVulnerabilityFilePath": List[StringFilterOutputTypeDef],
-        "componentId": List[StringFilterOutputTypeDef],
-        "componentType": List[StringFilterOutputTypeDef],
-        "ec2InstanceImageId": List[StringFilterOutputTypeDef],
-        "ec2InstanceSubnetId": List[StringFilterOutputTypeDef],
-        "ec2InstanceVpcId": List[StringFilterOutputTypeDef],
-        "ecrImageArchitecture": List[StringFilterOutputTypeDef],
-        "ecrImageHash": List[StringFilterOutputTypeDef],
+        "awsAccountId": List[StringFilterTypeDef],
+        "codeVulnerabilityDetectorName": List[StringFilterTypeDef],
+        "codeVulnerabilityDetectorTags": List[StringFilterTypeDef],
+        "codeVulnerabilityFilePath": List[StringFilterTypeDef],
+        "componentId": List[StringFilterTypeDef],
+        "componentType": List[StringFilterTypeDef],
+        "ec2InstanceImageId": List[StringFilterTypeDef],
+        "ec2InstanceSubnetId": List[StringFilterTypeDef],
+        "ec2InstanceVpcId": List[StringFilterTypeDef],
+        "ecrImageArchitecture": List[StringFilterTypeDef],
+        "ecrImageHash": List[StringFilterTypeDef],
         "ecrImagePushedAt": List[DateFilterOutputTypeDef],
-        "ecrImageRegistry": List[StringFilterOutputTypeDef],
-        "ecrImageRepositoryName": List[StringFilterOutputTypeDef],
-        "ecrImageTags": List[StringFilterOutputTypeDef],
-        "epssScore": List[NumberFilterOutputTypeDef],
-        "exploitAvailable": List[StringFilterOutputTypeDef],
-        "findingArn": List[StringFilterOutputTypeDef],
-        "findingStatus": List[StringFilterOutputTypeDef],
-        "findingType": List[StringFilterOutputTypeDef],
+        "ecrImageRegistry": List[StringFilterTypeDef],
+        "ecrImageRepositoryName": List[StringFilterTypeDef],
+        "ecrImageTags": List[StringFilterTypeDef],
+        "epssScore": List[NumberFilterTypeDef],
+        "exploitAvailable": List[StringFilterTypeDef],
+        "findingArn": List[StringFilterTypeDef],
+        "findingStatus": List[StringFilterTypeDef],
+        "findingType": List[StringFilterTypeDef],
         "firstObservedAt": List[DateFilterOutputTypeDef],
-        "fixAvailable": List[StringFilterOutputTypeDef],
-        "inspectorScore": List[NumberFilterOutputTypeDef],
-        "lambdaFunctionExecutionRoleArn": List[StringFilterOutputTypeDef],
+        "fixAvailable": List[StringFilterTypeDef],
+        "inspectorScore": List[NumberFilterTypeDef],
+        "lambdaFunctionExecutionRoleArn": List[StringFilterTypeDef],
         "lambdaFunctionLastModifiedAt": List[DateFilterOutputTypeDef],
-        "lambdaFunctionLayers": List[StringFilterOutputTypeDef],
-        "lambdaFunctionName": List[StringFilterOutputTypeDef],
-        "lambdaFunctionRuntime": List[StringFilterOutputTypeDef],
+        "lambdaFunctionLayers": List[StringFilterTypeDef],
+        "lambdaFunctionName": List[StringFilterTypeDef],
+        "lambdaFunctionRuntime": List[StringFilterTypeDef],
         "lastObservedAt": List[DateFilterOutputTypeDef],
-        "networkProtocol": List[StringFilterOutputTypeDef],
-        "portRange": List[PortRangeFilterOutputTypeDef],
-        "relatedVulnerabilities": List[StringFilterOutputTypeDef],
-        "resourceId": List[StringFilterOutputTypeDef],
-        "resourceTags": List[MapFilterOutputTypeDef],
-        "resourceType": List[StringFilterOutputTypeDef],
-        "severity": List[StringFilterOutputTypeDef],
-        "title": List[StringFilterOutputTypeDef],
+        "networkProtocol": List[StringFilterTypeDef],
+        "portRange": List[PortRangeFilterTypeDef],
+        "relatedVulnerabilities": List[StringFilterTypeDef],
+        "resourceId": List[StringFilterTypeDef],
+        "resourceTags": List[MapFilterTypeDef],
+        "resourceType": List[StringFilterTypeDef],
+        "severity": List[StringFilterTypeDef],
+        "title": List[StringFilterTypeDef],
         "updatedAt": List[DateFilterOutputTypeDef],
-        "vendorSeverity": List[StringFilterOutputTypeDef],
-        "vulnerabilityId": List[StringFilterOutputTypeDef],
-        "vulnerabilitySource": List[StringFilterOutputTypeDef],
-        "vulnerablePackages": List[PackageFilterOutputTypeDef],
+        "vendorSeverity": List[StringFilterTypeDef],
+        "vulnerabilityId": List[StringFilterTypeDef],
+        "vulnerabilitySource": List[StringFilterTypeDef],
+        "vulnerablePackages": List[PackageFilterTypeDef],
     },
     total=False,
 )
 
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
@@ -2629,15 +2487,15 @@
 )
 
 BatchGetFreeTrialInfoResponseTypeDef = TypedDict(
     "BatchGetFreeTrialInfoResponseTypeDef",
     {
         "accounts": List[FreeTrialAccountInfoTypeDef],
         "failedAccounts": List[FreeTrialInfoErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCoveredResourceTypeDef = TypedDict(
     "_RequiredCoveredResourceTypeDef",
     {
         "accountId": str,
@@ -2674,17 +2532,17 @@
     "GetSbomExportResponseTypeDef",
     {
         "errorCode": ReportingErrorCodeType,
         "errorMessage": str,
         "filterCriteria": ResourceFilterCriteriaOutputTypeDef,
         "format": SbomReportFormatType,
         "reportId": str,
-        "s3Destination": DestinationOutputTypeDef,
+        "s3Destination": DestinationTypeDef,
         "status": ExternalReportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSbomExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSbomExportRequestRequestTypeDef",
     {
         "reportFormat": SbomReportFormatType,
@@ -2707,34 +2565,34 @@
 
 
 ListUsageTotalsResponseTypeDef = TypedDict(
     "ListUsageTotalsResponseTypeDef",
     {
         "nextToken": str,
         "totals": List[UsageTotalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingAggregationsResponseTypeDef = TypedDict(
     "ListFindingAggregationsResponseTypeDef",
     {
         "aggregationType": AggregationTypeType,
         "nextToken": str,
         "responses": List[AggregationResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetAccountStatusResponseTypeDef = TypedDict(
     "BatchGetAccountStatusResponseTypeDef",
     {
         "accounts": List[AccountStateTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "id": str,
@@ -2764,15 +2622,15 @@
     },
 )
 _OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef = TypedDict(
     "_OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     {
         "accountIds": Sequence[StringFilterTypeDef],
         "aggregationRequest": AggregationRequestTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef(
     _RequiredListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
@@ -2832,21 +2690,21 @@
 class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
     pass
 
 
 GetFindingsReportStatusResponseTypeDef = TypedDict(
     "GetFindingsReportStatusResponseTypeDef",
     {
-        "destination": DestinationOutputTypeDef,
+        "destination": DestinationTypeDef,
         "errorCode": ReportingErrorCodeType,
         "errorMessage": str,
         "filterCriteria": FilterCriteriaOutputTypeDef,
         "reportId": str,
         "status": ExternalReportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "action": FilterActionType,
@@ -2895,15 +2753,15 @@
 
 
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "filterCriteria": FilterCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
@@ -2941,15 +2799,15 @@
 
 
 ListCoverageResponseTypeDef = TypedDict(
     "ListCoverageResponseTypeDef",
     {
         "coveredResources": List[CoveredResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "awsAccountId": str,
@@ -2988,19 +2846,19 @@
 
 
 ListFiltersResponseTypeDef = TypedDict(
     "ListFiltersResponseTypeDef",
     {
         "filters": List[FilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingsResponseTypeDef = TypedDict(
     "ListFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/type_defs.pyi` & `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -88,123 +88,95 @@
     "SeverityCountsTypeDef",
     "AccountAggregationTypeDef",
     "StateTypeDef",
     "ResourceStatusTypeDef",
     "FindingTypeAggregationTypeDef",
     "StringFilterTypeDef",
     "AssociateMemberRequestRequestTypeDef",
-    "AssociateMemberResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AtigDataTypeDef",
-    "AutoEnableOutputTypeDef",
     "AutoEnableTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "LambdaVpcConfigTypeDef",
     "BatchGetAccountStatusRequestRequestTypeDef",
     "BatchGetCodeSnippetRequestRequestTypeDef",
     "CodeSnippetErrorTypeDef",
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     "FreeTrialInfoErrorTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "FailedMemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusTypeDef",
     "CancelFindingsReportRequestRequestTypeDef",
-    "CancelFindingsReportResponseTypeDef",
     "CancelSbomExportRequestRequestTypeDef",
-    "CancelSbomExportResponseTypeDef",
     "CisaDataTypeDef",
     "CodeFilePathTypeDef",
     "CodeLineTypeDef",
     "SuggestedFixTypeDef",
     "CountsTypeDef",
     "CoverageDateFilterTypeDef",
     "CoverageMapFilterTypeDef",
     "CoverageStringFilterTypeDef",
     "ScanStatusTypeDef",
-    "CreateFilterResponseTypeDef",
     "DestinationTypeDef",
-    "CreateFindingsReportResponseTypeDef",
-    "CreateSbomExportResponseTypeDef",
     "Cvss2TypeDef",
     "Cvss3TypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DateFilterOutputTypeDef",
     "DateFilterTypeDef",
     "DelegatedAdminAccountTypeDef",
     "DelegatedAdminTypeDef",
     "DeleteFilterRequestRequestTypeDef",
-    "DeleteFilterResponseTypeDef",
-    "DestinationOutputTypeDef",
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
-    "DisableDelegatedAdminAccountResponseTypeDef",
     "DisableRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
-    "DisassociateMemberResponseTypeDef",
     "MapFilterTypeDef",
     "Ec2MetadataTypeDef",
     "EcrRescanDurationStateTypeDef",
     "EcrConfigurationTypeDef",
     "EcrContainerImageMetadataTypeDef",
     "EcrRepositoryMetadataTypeDef",
     "EnableDelegatedAdminAccountRequestRequestTypeDef",
-    "EnableDelegatedAdminAccountResponseTypeDef",
     "EnableRequestRequestTypeDef",
     "EpssDetailsTypeDef",
     "EpssTypeDef",
     "ExploitObservedTypeDef",
     "ExploitabilityDetailsTypeDef",
-    "MapFilterOutputTypeDef",
-    "NumberFilterOutputTypeDef",
-    "PortRangeFilterOutputTypeDef",
-    "StringFilterOutputTypeDef",
     "NumberFilterTypeDef",
     "PortRangeFilterTypeDef",
     "FreeTrialInfoTypeDef",
-    "GetEc2DeepInspectionConfigurationResponseTypeDef",
     "GetEncryptionKeyRequestRequestTypeDef",
-    "GetEncryptionKeyResponseTypeDef",
     "GetFindingsReportStatusRequestRequestTypeDef",
     "GetMemberRequestRequestTypeDef",
     "MemberTypeDef",
     "GetSbomExportRequestRequestTypeDef",
     "LambdaFunctionMetadataTypeDef",
-    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
-    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
     "ListDelegatedAdminAccountsRequestRequestTypeDef",
-    "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
     "SortCriteriaTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
     "ListUsageTotalsRequestRequestTypeDef",
     "StepTypeDef",
     "PortRangeTypeDef",
     "VulnerablePackageTypeDef",
-    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
     "ResetEncryptionKeyRequestRequestTypeDef",
-    "ResourceMapFilterOutputTypeDef",
-    "ResourceStringFilterOutputTypeDef",
     "ResourceMapFilterTypeDef",
     "ResourceStringFilterTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchVulnerabilitiesFilterCriteriaTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef",
-    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
     "UpdateEncryptionKeyRequestRequestTypeDef",
-    "UpdateFilterResponseTypeDef",
     "UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef",
     "UsageTypeDef",
     "AccountAggregationResponseTypeDef",
     "AmiAggregationResponseTypeDef",
     "AwsEcrContainerAggregationResponseTypeDef",
     "Ec2InstanceAggregationResponseTypeDef",
     "FindingTypeAggregationResponseTypeDef",
@@ -220,17 +192,32 @@
     "AmiAggregationTypeDef",
     "AwsEcrContainerAggregationTypeDef",
     "ImageLayerAggregationTypeDef",
     "LambdaLayerAggregationTypeDef",
     "PackageAggregationTypeDef",
     "RepositoryAggregationTypeDef",
     "TitleAggregationTypeDef",
+    "AssociateMemberResponseTypeDef",
+    "CancelFindingsReportResponseTypeDef",
+    "CancelSbomExportResponseTypeDef",
+    "CreateFilterResponseTypeDef",
+    "CreateFindingsReportResponseTypeDef",
+    "CreateSbomExportResponseTypeDef",
+    "DeleteFilterResponseTypeDef",
+    "DisableDelegatedAdminAccountResponseTypeDef",
+    "DisassociateMemberResponseTypeDef",
+    "EnableDelegatedAdminAccountResponseTypeDef",
+    "GetEc2DeepInspectionConfigurationResponseTypeDef",
+    "GetEncryptionKeyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
+    "UpdateFilterResponseTypeDef",
     "DescribeOrganizationConfigurationResponseTypeDef",
-    "UpdateOrganizationConfigurationResponseTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
+    "UpdateOrganizationConfigurationResponseTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "CodeVulnerabilityDetailsTypeDef",
     "CodeSnippetResultTypeDef",
     "ListCoverageStatisticsResponseTypeDef",
@@ -239,20 +226,24 @@
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "VulnerabilityTypeDef",
-    "PackageFilterOutputTypeDef",
     "PackageFilterTypeDef",
     "FreeTrialAccountInfoTypeDef",
     "GetMemberResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ResourceScanMetadataTypeDef",
+    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
+    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
     "ListAccountPermissionsResponseTypeDef",
     "NetworkPathTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
     "ResourceFilterCriteriaOutputTypeDef",
     "ResourceFilterCriteriaTypeDef",
     "SearchVulnerabilitiesRequestRequestTypeDef",
@@ -370,52 +361,36 @@
 AssociateMemberRequestRequestTypeDef = TypedDict(
     "AssociateMemberRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
-AssociateMemberResponseTypeDef = TypedDict(
-    "AssociateMemberResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "accountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AtigDataTypeDef = TypedDict(
     "AtigDataTypeDef",
     {
         "firstSeen": datetime,
         "lastSeen": datetime,
         "targets": List[str],
         "ttps": List[str],
     },
     total=False,
 )
 
-_RequiredAutoEnableOutputTypeDef = TypedDict(
-    "_RequiredAutoEnableOutputTypeDef",
-    {
-        "ec2": bool,
-        "ecr": bool,
-    },
-)
-_OptionalAutoEnableOutputTypeDef = TypedDict(
-    "_OptionalAutoEnableOutputTypeDef",
-    {
-        "lambda": bool,
-        "lambdaCode": bool,
-    },
-    total=False,
-)
-
-class AutoEnableOutputTypeDef(_RequiredAutoEnableOutputTypeDef, _OptionalAutoEnableOutputTypeDef):
-    pass
-
 _RequiredAutoEnableTypeDef = TypedDict(
     "_RequiredAutoEnableTypeDef",
     {
         "ec2": bool,
         "ecr": bool,
     },
 )
@@ -584,37 +559,21 @@
 CancelFindingsReportRequestRequestTypeDef = TypedDict(
     "CancelFindingsReportRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
-CancelFindingsReportResponseTypeDef = TypedDict(
-    "CancelFindingsReportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CancelSbomExportRequestRequestTypeDef = TypedDict(
     "CancelSbomExportRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
-CancelSbomExportResponseTypeDef = TypedDict(
-    "CancelSbomExportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CisaDataTypeDef = TypedDict(
     "CisaDataTypeDef",
     {
         "action": str,
         "dateAdded": datetime,
         "dateDue": datetime,
     },
@@ -698,22 +657,14 @@
     "ScanStatusTypeDef",
     {
         "reason": ScanStatusReasonType,
         "statusCode": ScanStatusCodeType,
     },
 )
 
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "bucketName": str,
         "kmsKeyArn": str,
     },
 )
@@ -724,30 +675,14 @@
     },
     total=False,
 )
 
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
-CreateFindingsReportResponseTypeDef = TypedDict(
-    "CreateFindingsReportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSbomExportResponseTypeDef = TypedDict(
-    "CreateSbomExportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 Cvss2TypeDef = TypedDict(
     "Cvss2TypeDef",
     {
         "baseScore": float,
         "scoringVector": str,
     },
     total=False,
@@ -819,57 +754,21 @@
 DeleteFilterRequestRequestTypeDef = TypedDict(
     "DeleteFilterRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-DeleteFilterResponseTypeDef = TypedDict(
-    "DeleteFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDestinationOutputTypeDef = TypedDict(
-    "_RequiredDestinationOutputTypeDef",
-    {
-        "bucketName": str,
-        "kmsKeyArn": str,
-    },
-)
-_OptionalDestinationOutputTypeDef = TypedDict(
-    "_OptionalDestinationOutputTypeDef",
-    {
-        "keyPrefix": str,
-    },
-    total=False,
-)
-
-class DestinationOutputTypeDef(
-    _RequiredDestinationOutputTypeDef, _OptionalDestinationOutputTypeDef
-):
-    pass
-
 DisableDelegatedAdminAccountRequestRequestTypeDef = TypedDict(
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     {
         "delegatedAdminAccountId": str,
     },
 )
 
-DisableDelegatedAdminAccountResponseTypeDef = TypedDict(
-    "DisableDelegatedAdminAccountResponseTypeDef",
-    {
-        "delegatedAdminAccountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisableRequestRequestTypeDef = TypedDict(
     "DisableRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "resourceTypes": Sequence[ResourceScanTypeType],
     },
     total=False,
@@ -878,22 +777,14 @@
 DisassociateMemberRequestRequestTypeDef = TypedDict(
     "DisassociateMemberRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
-DisassociateMemberResponseTypeDef = TypedDict(
-    "DisassociateMemberResponseTypeDef",
-    {
-        "accountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMapFilterTypeDef = TypedDict(
     "_RequiredMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -968,22 +859,14 @@
 
 class EnableDelegatedAdminAccountRequestRequestTypeDef(
     _RequiredEnableDelegatedAdminAccountRequestRequestTypeDef,
     _OptionalEnableDelegatedAdminAccountRequestRequestTypeDef,
 ):
     pass
 
-EnableDelegatedAdminAccountResponseTypeDef = TypedDict(
-    "EnableDelegatedAdminAccountResponseTypeDef",
-    {
-        "delegatedAdminAccountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEnableRequestRequestTypeDef = TypedDict(
     "_RequiredEnableRequestRequestTypeDef",
     {
         "resourceTypes": Sequence[ResourceScanTypeType],
     },
 )
 _OptionalEnableRequestRequestTypeDef = TypedDict(
@@ -1029,58 +912,14 @@
     "ExploitabilityDetailsTypeDef",
     {
         "lastKnownExploitAt": datetime,
     },
     total=False,
 )
 
-_RequiredMapFilterOutputTypeDef = TypedDict(
-    "_RequiredMapFilterOutputTypeDef",
-    {
-        "comparison": Literal["EQUALS"],
-        "key": str,
-    },
-)
-_OptionalMapFilterOutputTypeDef = TypedDict(
-    "_OptionalMapFilterOutputTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-class MapFilterOutputTypeDef(_RequiredMapFilterOutputTypeDef, _OptionalMapFilterOutputTypeDef):
-    pass
-
-NumberFilterOutputTypeDef = TypedDict(
-    "NumberFilterOutputTypeDef",
-    {
-        "lowerInclusive": float,
-        "upperInclusive": float,
-    },
-    total=False,
-)
-
-PortRangeFilterOutputTypeDef = TypedDict(
-    "PortRangeFilterOutputTypeDef",
-    {
-        "beginInclusive": int,
-        "endInclusive": int,
-    },
-    total=False,
-)
-
-StringFilterOutputTypeDef = TypedDict(
-    "StringFilterOutputTypeDef",
-    {
-        "comparison": StringComparisonType,
-        "value": str,
-    },
-)
-
 NumberFilterTypeDef = TypedDict(
     "NumberFilterTypeDef",
     {
         "lowerInclusive": float,
         "upperInclusive": float,
     },
     total=False,
@@ -1101,41 +940,22 @@
         "end": datetime,
         "start": datetime,
         "status": FreeTrialStatusType,
         "type": FreeTrialTypeType,
     },
 )
 
-GetEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
-    "GetEc2DeepInspectionConfigurationResponseTypeDef",
-    {
-        "errorMessage": str,
-        "orgPackagePaths": List[str],
-        "packagePaths": List[str],
-        "status": Ec2DeepInspectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEncryptionKeyRequestRequestTypeDef = TypedDict(
     "GetEncryptionKeyRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "scanType": ScanTypeType,
     },
 )
 
-GetEncryptionKeyResponseTypeDef = TypedDict(
-    "GetEncryptionKeyResponseTypeDef",
-    {
-        "kmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFindingsReportStatusRequestRequestTypeDef = TypedDict(
     "GetFindingsReportStatusRequestRequestTypeDef",
     {
         "reportId": str,
     },
     total=False,
 )
@@ -1172,19 +992,20 @@
         "functionTags": Dict[str, str],
         "layers": List[str],
         "runtime": RuntimeType,
     },
     total=False,
 )
 
-ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef = TypedDict(
-    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "service": ServiceType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAccountPermissionsRequestRequestTypeDef = TypedDict(
     "ListAccountPermissionsRequestRequestTypeDef",
     {
@@ -1199,41 +1020,23 @@
     "PermissionTypeDef",
     {
         "operation": OperationType,
         "service": ServiceType,
     },
 )
 
-ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef = TypedDict(
-    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDelegatedAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListDelegatedAdminAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "ListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "action": FilterActionType,
-        "arns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFiltersRequestRequestTypeDef = TypedDict(
     "ListFiltersRequestRequestTypeDef",
     {
         "action": FilterActionType,
         "arns": Sequence[str],
         "maxResults": int,
         "nextToken": str,
@@ -1245,23 +1048,14 @@
     "SortCriteriaTypeDef",
     {
         "field": SortFieldType,
         "sortOrder": SortOrderType,
     },
 )
 
-ListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "ListMembersRequestListMembersPaginateTypeDef",
-    {
-        "onlyAssociated": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMembersRequestRequestTypeDef = TypedDict(
     "ListMembersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "onlyAssociated": bool,
     },
@@ -1271,31 +1065,14 @@
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
-ListUsageTotalsRequestListUsageTotalsPaginateTypeDef = TypedDict(
-    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
-    {
-        "accountIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListUsageTotalsRequestRequestTypeDef = TypedDict(
     "ListUsageTotalsRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -1342,24 +1119,14 @@
 )
 
 class VulnerablePackageTypeDef(
     _RequiredVulnerablePackageTypeDef, _OptionalVulnerablePackageTypeDef
 ):
     pass
 
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
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Url": str,
         "text": str,
     },
     total=False,
@@ -1369,42 +1136,14 @@
     "ResetEncryptionKeyRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "scanType": ScanTypeType,
     },
 )
 
-_RequiredResourceMapFilterOutputTypeDef = TypedDict(
-    "_RequiredResourceMapFilterOutputTypeDef",
-    {
-        "comparison": Literal["EQUALS"],
-        "key": str,
-    },
-)
-_OptionalResourceMapFilterOutputTypeDef = TypedDict(
-    "_OptionalResourceMapFilterOutputTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-class ResourceMapFilterOutputTypeDef(
-    _RequiredResourceMapFilterOutputTypeDef, _OptionalResourceMapFilterOutputTypeDef
-):
-    pass
-
-ResourceStringFilterOutputTypeDef = TypedDict(
-    "ResourceStringFilterOutputTypeDef",
-    {
-        "comparison": ResourceStringComparisonType,
-        "value": str,
-    },
-)
-
 _RequiredResourceMapFilterTypeDef = TypedDict(
     "_RequiredResourceMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -1425,25 +1164,14 @@
     "ResourceStringFilterTypeDef",
     {
         "comparison": ResourceStringComparisonType,
         "value": str,
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
 SearchVulnerabilitiesFilterCriteriaTypeDef = TypedDict(
     "SearchVulnerabilitiesFilterCriteriaTypeDef",
     {
         "vulnerabilityIds": Sequence[str],
     },
 )
 
@@ -1468,42 +1196,23 @@
     {
         "activateDeepInspection": bool,
         "packagePaths": Sequence[str],
     },
     total=False,
 )
 
-UpdateEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
-    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
-    {
-        "errorMessage": str,
-        "orgPackagePaths": List[str],
-        "packagePaths": List[str],
-        "status": Ec2DeepInspectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateEncryptionKeyRequestRequestTypeDef = TypedDict(
     "UpdateEncryptionKeyRequestRequestTypeDef",
     {
         "kmsKeyId": str,
         "resourceType": ResourceTypeType,
         "scanType": ScanTypeType,
     },
 )
 
-UpdateFilterResponseTypeDef = TypedDict(
-    "UpdateFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef",
     {
         "orgPackagePaths": Sequence[str],
     },
 )
 
@@ -1862,35 +1571,161 @@
         "sortOrder": SortOrderType,
         "titles": Sequence[StringFilterTypeDef],
         "vulnerabilityIds": Sequence[StringFilterTypeDef],
     },
     total=False,
 )
 
+AssociateMemberResponseTypeDef = TypedDict(
+    "AssociateMemberResponseTypeDef",
+    {
+        "accountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelFindingsReportResponseTypeDef = TypedDict(
+    "CancelFindingsReportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelSbomExportResponseTypeDef = TypedDict(
+    "CancelSbomExportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFindingsReportResponseTypeDef = TypedDict(
+    "CreateFindingsReportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSbomExportResponseTypeDef = TypedDict(
+    "CreateSbomExportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFilterResponseTypeDef = TypedDict(
+    "DeleteFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableDelegatedAdminAccountResponseTypeDef = TypedDict(
+    "DisableDelegatedAdminAccountResponseTypeDef",
+    {
+        "delegatedAdminAccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateMemberResponseTypeDef = TypedDict(
+    "DisassociateMemberResponseTypeDef",
+    {
+        "accountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnableDelegatedAdminAccountResponseTypeDef = TypedDict(
+    "EnableDelegatedAdminAccountResponseTypeDef",
+    {
+        "delegatedAdminAccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
+    "GetEc2DeepInspectionConfigurationResponseTypeDef",
+    {
+        "errorMessage": str,
+        "orgPackagePaths": List[str],
+        "packagePaths": List[str],
+        "status": Ec2DeepInspectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEncryptionKeyResponseTypeDef = TypedDict(
+    "GetEncryptionKeyResponseTypeDef",
+    {
+        "kmsKeyId": str,
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
+UpdateEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
+    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
+    {
+        "errorMessage": str,
+        "orgPackagePaths": List[str],
+        "packagePaths": List[str],
+        "status": Ec2DeepInspectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFilterResponseTypeDef = TypedDict(
+    "UpdateFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
-        "autoEnable": AutoEnableOutputTypeDef,
+        "autoEnable": AutoEnableTypeDef,
         "maxAccountLimitReached": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateOrganizationConfigurationResponseTypeDef = TypedDict(
-    "UpdateOrganizationConfigurationResponseTypeDef",
+UpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateOrganizationConfigurationRequestRequestTypeDef",
     {
-        "autoEnable": AutoEnableOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "autoEnable": AutoEnableTypeDef,
     },
 )
 
-UpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateOrganizationConfigurationRequestRequestTypeDef",
+UpdateOrganizationConfigurationResponseTypeDef = TypedDict(
+    "UpdateOrganizationConfigurationResponseTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAwsLambdaFunctionDetailsTypeDef = TypedDict(
     "_RequiredAwsLambdaFunctionDetailsTypeDef",
     {
         "codeSha256": str,
@@ -1918,24 +1753,24 @@
     pass
 
 BatchGetMemberEc2DeepInspectionStatusResponseTypeDef = TypedDict(
     "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
     {
         "accountIds": List[MemberAccountEc2DeepInspectionStatusStateTypeDef],
         "failedAccountIds": List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef = TypedDict(
     "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
     {
         "accountIds": List[MemberAccountEc2DeepInspectionStatusStateTypeDef],
         "failedAccountIds": List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef = TypedDict(
     "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     {
         "accountIds": Sequence[MemberAccountEc2DeepInspectionStatusTypeDef],
@@ -1981,15 +1816,15 @@
 
 ListCoverageStatisticsResponseTypeDef = TypedDict(
     "ListCoverageStatisticsResponseTypeDef",
     {
         "countsByGroup": List[CountsTypeDef],
         "nextToken": str,
         "totalCounts": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CoverageFilterCriteriaTypeDef = TypedDict(
     "CoverageFilterCriteriaTypeDef",
     {
         "accountId": Sequence[CoverageStringFilterTypeDef],
@@ -2031,23 +1866,23 @@
     pass
 
 ListDelegatedAdminAccountsResponseTypeDef = TypedDict(
     "ListDelegatedAdminAccountsResponseTypeDef",
     {
         "delegatedAdminAccounts": List[DelegatedAdminAccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDelegatedAdminAccountResponseTypeDef = TypedDict(
     "GetDelegatedAdminAccountResponseTypeDef",
     {
         "delegatedAdmin": DelegatedAdminTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 Ec2InstanceAggregationTypeDef = TypedDict(
     "Ec2InstanceAggregationTypeDef",
     {
         "amis": Sequence[StringFilterTypeDef],
@@ -2116,28 +1951,14 @@
     },
     total=False,
 )
 
 class VulnerabilityTypeDef(_RequiredVulnerabilityTypeDef, _OptionalVulnerabilityTypeDef):
     pass
 
-PackageFilterOutputTypeDef = TypedDict(
-    "PackageFilterOutputTypeDef",
-    {
-        "architecture": StringFilterOutputTypeDef,
-        "epoch": NumberFilterOutputTypeDef,
-        "name": StringFilterOutputTypeDef,
-        "release": StringFilterOutputTypeDef,
-        "sourceLambdaLayerArn": StringFilterOutputTypeDef,
-        "sourceLayerHash": StringFilterOutputTypeDef,
-        "version": StringFilterOutputTypeDef,
-    },
-    total=False,
-)
-
 PackageFilterTypeDef = TypedDict(
     "PackageFilterTypeDef",
     {
         "architecture": StringFilterTypeDef,
         "epoch": NumberFilterTypeDef,
         "name": StringFilterTypeDef,
         "release": StringFilterTypeDef,
@@ -2156,44 +1977,89 @@
     },
 )
 
 GetMemberResponseTypeDef = TypedDict(
     "GetMemberResponseTypeDef",
     {
         "member": MemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "members": List[MemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceScanMetadataTypeDef = TypedDict(
     "ResourceScanMetadataTypeDef",
     {
         "ec2": Ec2MetadataTypeDef,
         "ecrImage": EcrContainerImageMetadataTypeDef,
         "ecrRepository": EcrRepositoryMetadataTypeDef,
         "lambdaFunction": LambdaFunctionMetadataTypeDef,
     },
     total=False,
 )
 
+ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef = TypedDict(
+    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+    {
+        "service": ServiceType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef = TypedDict(
+    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "action": FilterActionType,
+        "arns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "ListMembersRequestListMembersPaginateTypeDef",
+    {
+        "onlyAssociated": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListUsageTotalsRequestListUsageTotalsPaginateTypeDef = TypedDict(
+    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
+    {
+        "accountIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListAccountPermissionsResponseTypeDef = TypedDict(
     "ListAccountPermissionsResponseTypeDef",
     {
         "nextToken": str,
         "permissions": List[PermissionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkPathTypeDef = TypedDict(
     "NetworkPathTypeDef",
     {
         "steps": List[StepTypeDef],
@@ -2235,22 +2101,22 @@
     },
     total=False,
 )
 
 ResourceFilterCriteriaOutputTypeDef = TypedDict(
     "ResourceFilterCriteriaOutputTypeDef",
     {
-        "accountId": List[ResourceStringFilterOutputTypeDef],
-        "ec2InstanceTags": List[ResourceMapFilterOutputTypeDef],
-        "ecrImageTags": List[ResourceStringFilterOutputTypeDef],
-        "ecrRepositoryName": List[ResourceStringFilterOutputTypeDef],
-        "lambdaFunctionName": List[ResourceStringFilterOutputTypeDef],
-        "lambdaFunctionTags": List[ResourceMapFilterOutputTypeDef],
-        "resourceId": List[ResourceStringFilterOutputTypeDef],
-        "resourceType": List[ResourceStringFilterOutputTypeDef],
+        "accountId": List[ResourceStringFilterTypeDef],
+        "ec2InstanceTags": List[ResourceMapFilterTypeDef],
+        "ecrImageTags": List[ResourceStringFilterTypeDef],
+        "ecrRepositoryName": List[ResourceStringFilterTypeDef],
+        "lambdaFunctionName": List[ResourceStringFilterTypeDef],
+        "lambdaFunctionTags": List[ResourceMapFilterTypeDef],
+        "resourceId": List[ResourceStringFilterTypeDef],
+        "resourceType": List[ResourceStringFilterTypeDef],
     },
     total=False,
 )
 
 ResourceFilterCriteriaTypeDef = TypedDict(
     "ResourceFilterCriteriaTypeDef",
     {
@@ -2291,15 +2157,15 @@
     {
         "filterCriteria": SearchVulnerabilitiesFilterCriteriaTypeDef,
     },
 )
 _OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef = TypedDict(
     "_OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef(
     _RequiredSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
     _OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
@@ -2343,24 +2209,24 @@
 )
 
 DisableResponseTypeDef = TypedDict(
     "DisableResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnableResponseTypeDef = TypedDict(
     "EnableResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "awsEc2Instance": AwsEc2InstanceDetailsTypeDef,
@@ -2371,23 +2237,23 @@
 )
 
 BatchGetCodeSnippetResponseTypeDef = TypedDict(
     "BatchGetCodeSnippetResponseTypeDef",
     {
         "codeSnippetResults": List[CodeSnippetResultTypeDef],
         "errors": List[CodeSnippetErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
     "ListCoverageRequestListCoveragePaginateTypeDef",
     {
         "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListCoverageRequestRequestTypeDef = TypedDict(
     "ListCoverageRequestRequestTypeDef",
     {
@@ -2399,15 +2265,15 @@
 )
 
 ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef = TypedDict(
     "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
     {
         "filterCriteria": CoverageFilterCriteriaTypeDef,
         "groupBy": GroupKeyType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListCoverageStatisticsRequestRequestTypeDef = TypedDict(
     "ListCoverageStatisticsRequestRequestTypeDef",
     {
@@ -2444,72 +2310,72 @@
     total=False,
 )
 
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
         "ecrConfiguration": EcrConfigurationStateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchVulnerabilitiesResponseTypeDef = TypedDict(
     "SearchVulnerabilitiesResponseTypeDef",
     {
         "nextToken": str,
         "vulnerabilities": List[VulnerabilityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FilterCriteriaOutputTypeDef = TypedDict(
     "FilterCriteriaOutputTypeDef",
     {
-        "awsAccountId": List[StringFilterOutputTypeDef],
-        "codeVulnerabilityDetectorName": List[StringFilterOutputTypeDef],
-        "codeVulnerabilityDetectorTags": List[StringFilterOutputTypeDef],
-        "codeVulnerabilityFilePath": List[StringFilterOutputTypeDef],
-        "componentId": List[StringFilterOutputTypeDef],
-        "componentType": List[StringFilterOutputTypeDef],
-        "ec2InstanceImageId": List[StringFilterOutputTypeDef],
-        "ec2InstanceSubnetId": List[StringFilterOutputTypeDef],
-        "ec2InstanceVpcId": List[StringFilterOutputTypeDef],
-        "ecrImageArchitecture": List[StringFilterOutputTypeDef],
-        "ecrImageHash": List[StringFilterOutputTypeDef],
+        "awsAccountId": List[StringFilterTypeDef],
+        "codeVulnerabilityDetectorName": List[StringFilterTypeDef],
+        "codeVulnerabilityDetectorTags": List[StringFilterTypeDef],
+        "codeVulnerabilityFilePath": List[StringFilterTypeDef],
+        "componentId": List[StringFilterTypeDef],
+        "componentType": List[StringFilterTypeDef],
+        "ec2InstanceImageId": List[StringFilterTypeDef],
+        "ec2InstanceSubnetId": List[StringFilterTypeDef],
+        "ec2InstanceVpcId": List[StringFilterTypeDef],
+        "ecrImageArchitecture": List[StringFilterTypeDef],
+        "ecrImageHash": List[StringFilterTypeDef],
         "ecrImagePushedAt": List[DateFilterOutputTypeDef],
-        "ecrImageRegistry": List[StringFilterOutputTypeDef],
-        "ecrImageRepositoryName": List[StringFilterOutputTypeDef],
-        "ecrImageTags": List[StringFilterOutputTypeDef],
-        "epssScore": List[NumberFilterOutputTypeDef],
-        "exploitAvailable": List[StringFilterOutputTypeDef],
-        "findingArn": List[StringFilterOutputTypeDef],
-        "findingStatus": List[StringFilterOutputTypeDef],
-        "findingType": List[StringFilterOutputTypeDef],
+        "ecrImageRegistry": List[StringFilterTypeDef],
+        "ecrImageRepositoryName": List[StringFilterTypeDef],
+        "ecrImageTags": List[StringFilterTypeDef],
+        "epssScore": List[NumberFilterTypeDef],
+        "exploitAvailable": List[StringFilterTypeDef],
+        "findingArn": List[StringFilterTypeDef],
+        "findingStatus": List[StringFilterTypeDef],
+        "findingType": List[StringFilterTypeDef],
         "firstObservedAt": List[DateFilterOutputTypeDef],
-        "fixAvailable": List[StringFilterOutputTypeDef],
-        "inspectorScore": List[NumberFilterOutputTypeDef],
-        "lambdaFunctionExecutionRoleArn": List[StringFilterOutputTypeDef],
+        "fixAvailable": List[StringFilterTypeDef],
+        "inspectorScore": List[NumberFilterTypeDef],
+        "lambdaFunctionExecutionRoleArn": List[StringFilterTypeDef],
         "lambdaFunctionLastModifiedAt": List[DateFilterOutputTypeDef],
-        "lambdaFunctionLayers": List[StringFilterOutputTypeDef],
-        "lambdaFunctionName": List[StringFilterOutputTypeDef],
-        "lambdaFunctionRuntime": List[StringFilterOutputTypeDef],
+        "lambdaFunctionLayers": List[StringFilterTypeDef],
+        "lambdaFunctionName": List[StringFilterTypeDef],
+        "lambdaFunctionRuntime": List[StringFilterTypeDef],
         "lastObservedAt": List[DateFilterOutputTypeDef],
-        "networkProtocol": List[StringFilterOutputTypeDef],
-        "portRange": List[PortRangeFilterOutputTypeDef],
-        "relatedVulnerabilities": List[StringFilterOutputTypeDef],
-        "resourceId": List[StringFilterOutputTypeDef],
-        "resourceTags": List[MapFilterOutputTypeDef],
-        "resourceType": List[StringFilterOutputTypeDef],
-        "severity": List[StringFilterOutputTypeDef],
-        "title": List[StringFilterOutputTypeDef],
+        "networkProtocol": List[StringFilterTypeDef],
+        "portRange": List[PortRangeFilterTypeDef],
+        "relatedVulnerabilities": List[StringFilterTypeDef],
+        "resourceId": List[StringFilterTypeDef],
+        "resourceTags": List[MapFilterTypeDef],
+        "resourceType": List[StringFilterTypeDef],
+        "severity": List[StringFilterTypeDef],
+        "title": List[StringFilterTypeDef],
         "updatedAt": List[DateFilterOutputTypeDef],
-        "vendorSeverity": List[StringFilterOutputTypeDef],
-        "vulnerabilityId": List[StringFilterOutputTypeDef],
-        "vulnerabilitySource": List[StringFilterOutputTypeDef],
-        "vulnerablePackages": List[PackageFilterOutputTypeDef],
+        "vendorSeverity": List[StringFilterTypeDef],
+        "vulnerabilityId": List[StringFilterTypeDef],
+        "vulnerabilitySource": List[StringFilterTypeDef],
+        "vulnerablePackages": List[PackageFilterTypeDef],
     },
     total=False,
 )
 
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
@@ -2560,15 +2426,15 @@
 )
 
 BatchGetFreeTrialInfoResponseTypeDef = TypedDict(
     "BatchGetFreeTrialInfoResponseTypeDef",
     {
         "accounts": List[FreeTrialAccountInfoTypeDef],
         "failedAccounts": List[FreeTrialInfoErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCoveredResourceTypeDef = TypedDict(
     "_RequiredCoveredResourceTypeDef",
     {
         "accountId": str,
@@ -2603,17 +2469,17 @@
     "GetSbomExportResponseTypeDef",
     {
         "errorCode": ReportingErrorCodeType,
         "errorMessage": str,
         "filterCriteria": ResourceFilterCriteriaOutputTypeDef,
         "format": SbomReportFormatType,
         "reportId": str,
-        "s3Destination": DestinationOutputTypeDef,
+        "s3Destination": DestinationTypeDef,
         "status": ExternalReportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSbomExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSbomExportRequestRequestTypeDef",
     {
         "reportFormat": SbomReportFormatType,
@@ -2634,34 +2500,34 @@
     pass
 
 ListUsageTotalsResponseTypeDef = TypedDict(
     "ListUsageTotalsResponseTypeDef",
     {
         "nextToken": str,
         "totals": List[UsageTotalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingAggregationsResponseTypeDef = TypedDict(
     "ListFindingAggregationsResponseTypeDef",
     {
         "aggregationType": AggregationTypeType,
         "nextToken": str,
         "responses": List[AggregationResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetAccountStatusResponseTypeDef = TypedDict(
     "BatchGetAccountStatusResponseTypeDef",
     {
         "accounts": List[AccountStateTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "id": str,
@@ -2689,15 +2555,15 @@
     },
 )
 _OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef = TypedDict(
     "_OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     {
         "accountIds": Sequence[StringFilterTypeDef],
         "aggregationRequest": AggregationRequestTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef(
     _RequiredListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
     _OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
@@ -2751,21 +2617,21 @@
 
 class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
     pass
 
 GetFindingsReportStatusResponseTypeDef = TypedDict(
     "GetFindingsReportStatusResponseTypeDef",
     {
-        "destination": DestinationOutputTypeDef,
+        "destination": DestinationTypeDef,
         "errorCode": ReportingErrorCodeType,
         "errorMessage": str,
         "filterCriteria": FilterCriteriaOutputTypeDef,
         "reportId": str,
         "status": ExternalReportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "action": FilterActionType,
@@ -2810,15 +2676,15 @@
     pass
 
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "filterCriteria": FilterCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
@@ -2854,15 +2720,15 @@
     pass
 
 ListCoverageResponseTypeDef = TypedDict(
     "ListCoverageResponseTypeDef",
     {
         "coveredResources": List[CoveredResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "awsAccountId": str,
@@ -2899,19 +2765,19 @@
     pass
 
 ListFiltersResponseTypeDef = TypedDict(
     "ListFiltersResponseTypeDef",
     {
         "filters": List[FilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingsResponseTypeDef = TypedDict(
     "ListFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/PKG-INFO` & `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.28.12
-Summary: Type annotations for boto3.Inspector2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Inspector2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector2)](https://pepy.tech/project/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
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
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -426,123 +426,95 @@
     SeverityCountsTypeDef,
     AccountAggregationTypeDef,
     StateTypeDef,
     ResourceStatusTypeDef,
     FindingTypeAggregationTypeDef,
     StringFilterTypeDef,
     AssociateMemberRequestRequestTypeDef,
-    AssociateMemberResponseTypeDef,
+    ResponseMetadataTypeDef,
     AtigDataTypeDef,
-    AutoEnableOutputTypeDef,
     AutoEnableTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     LambdaVpcConfigTypeDef,
     BatchGetAccountStatusRequestRequestTypeDef,
     BatchGetCodeSnippetRequestRequestTypeDef,
     CodeSnippetErrorTypeDef,
     BatchGetFreeTrialInfoRequestRequestTypeDef,
     FreeTrialInfoErrorTypeDef,
     BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     FailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
     CancelFindingsReportRequestRequestTypeDef,
-    CancelFindingsReportResponseTypeDef,
     CancelSbomExportRequestRequestTypeDef,
-    CancelSbomExportResponseTypeDef,
     CisaDataTypeDef,
     CodeFilePathTypeDef,
     CodeLineTypeDef,
     SuggestedFixTypeDef,
     CountsTypeDef,
     CoverageDateFilterTypeDef,
     CoverageMapFilterTypeDef,
     CoverageStringFilterTypeDef,
     ScanStatusTypeDef,
-    CreateFilterResponseTypeDef,
     DestinationTypeDef,
-    CreateFindingsReportResponseTypeDef,
-    CreateSbomExportResponseTypeDef,
     Cvss2TypeDef,
     Cvss3TypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DateFilterOutputTypeDef,
     DateFilterTypeDef,
     DelegatedAdminAccountTypeDef,
     DelegatedAdminTypeDef,
     DeleteFilterRequestRequestTypeDef,
-    DeleteFilterResponseTypeDef,
-    DestinationOutputTypeDef,
     DisableDelegatedAdminAccountRequestRequestTypeDef,
-    DisableDelegatedAdminAccountResponseTypeDef,
     DisableRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
-    DisassociateMemberResponseTypeDef,
     MapFilterTypeDef,
     Ec2MetadataTypeDef,
     EcrRescanDurationStateTypeDef,
     EcrConfigurationTypeDef,
     EcrContainerImageMetadataTypeDef,
     EcrRepositoryMetadataTypeDef,
     EnableDelegatedAdminAccountRequestRequestTypeDef,
-    EnableDelegatedAdminAccountResponseTypeDef,
     EnableRequestRequestTypeDef,
     EpssDetailsTypeDef,
     EpssTypeDef,
     ExploitObservedTypeDef,
     ExploitabilityDetailsTypeDef,
-    MapFilterOutputTypeDef,
-    NumberFilterOutputTypeDef,
-    PortRangeFilterOutputTypeDef,
-    StringFilterOutputTypeDef,
     NumberFilterTypeDef,
     PortRangeFilterTypeDef,
     FreeTrialInfoTypeDef,
-    GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyRequestRequestTypeDef,
-    GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusRequestRequestTypeDef,
     GetMemberRequestRequestTypeDef,
     MemberTypeDef,
     GetSbomExportRequestRequestTypeDef,
     LambdaFunctionMetadataTypeDef,
-    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
-    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
     ListDelegatedAdminAccountsRequestRequestTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
     SortCriteriaTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListUsageTotalsRequestRequestTypeDef,
     StepTypeDef,
     PortRangeTypeDef,
     VulnerablePackageTypeDef,
-    PaginatorConfigTypeDef,
     RecommendationTypeDef,
     ResetEncryptionKeyRequestRequestTypeDef,
-    ResourceMapFilterOutputTypeDef,
-    ResourceStringFilterOutputTypeDef,
     ResourceMapFilterTypeDef,
     ResourceStringFilterTypeDef,
-    ResponseMetadataTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef,
-    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateEncryptionKeyRequestRequestTypeDef,
-    UpdateFilterResponseTypeDef,
     UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef,
     UsageTypeDef,
     AccountAggregationResponseTypeDef,
     AmiAggregationResponseTypeDef,
     AwsEcrContainerAggregationResponseTypeDef,
     Ec2InstanceAggregationResponseTypeDef,
     FindingTypeAggregationResponseTypeDef,
@@ -558,17 +530,32 @@
     AmiAggregationTypeDef,
     AwsEcrContainerAggregationTypeDef,
     ImageLayerAggregationTypeDef,
     LambdaLayerAggregationTypeDef,
     PackageAggregationTypeDef,
     RepositoryAggregationTypeDef,
     TitleAggregationTypeDef,
+    AssociateMemberResponseTypeDef,
+    CancelFindingsReportResponseTypeDef,
+    CancelSbomExportResponseTypeDef,
+    CreateFilterResponseTypeDef,
+    CreateFindingsReportResponseTypeDef,
+    CreateSbomExportResponseTypeDef,
+    DeleteFilterResponseTypeDef,
+    DisableDelegatedAdminAccountResponseTypeDef,
+    DisassociateMemberResponseTypeDef,
+    EnableDelegatedAdminAccountResponseTypeDef,
+    GetEc2DeepInspectionConfigurationResponseTypeDef,
+    GetEncryptionKeyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
+    UpdateFilterResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
-    UpdateOrganizationConfigurationResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
+    UpdateOrganizationConfigurationResponseTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     CodeVulnerabilityDetailsTypeDef,
     CodeSnippetResultTypeDef,
     ListCoverageStatisticsResponseTypeDef,
@@ -577,20 +564,24 @@
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     VulnerabilityTypeDef,
-    PackageFilterOutputTypeDef,
     PackageFilterTypeDef,
     FreeTrialAccountInfoTypeDef,
     GetMemberResponseTypeDef,
     ListMembersResponseTypeDef,
     ResourceScanMetadataTypeDef,
+    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
+    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListAccountPermissionsResponseTypeDef,
     NetworkPathTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     ResourceFilterCriteriaOutputTypeDef,
     ResourceFilterCriteriaTypeDef,
     SearchVulnerabilitiesRequestRequestTypeDef,
```

### Comparing `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/SOURCES.txt` & `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.12/setup.py` & `mypy-boto3-inspector2-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-inspector2",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_inspector2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Inspector2 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Inspector2 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

